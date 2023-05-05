# Comparing `tmp/lti-consumer-xblock-9.2.1.tar.gz` & `tmp/lti-consumer-xblock-9.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lti-consumer-xblock-9.2.1.tar", last modified: Wed May  3 13:40:02 2023, max compression
+gzip compressed data, was "lti-consumer-xblock-9.3.0.tar", last modified: Fri May  5 16:45:45 2023, max compression
```

## Comparing `lti-consumer-xblock-9.2.1.tar` & `lti-consumer-xblock-9.3.0.tar`

### file list

```diff
@@ -1,245 +1,245 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.978803 lti-consumer-xblock-9.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-05-03 13:40:02.978803 lti-consumer-xblock-9.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13412 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.942803 lti-consumer-xblock-9.2.1/lti_consumer/
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      672 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5921 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.946803 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15317 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.946803 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/contrib/django.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.946803 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/contrib/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/contrib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/contrib/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.946803 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14154 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/tests/test_oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.946803 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/ags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    33300 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.950803 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.950803 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      388 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      554 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3298 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10557 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/nprs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.950803 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.950803 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.954803 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     9039 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/test_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    40315 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/test_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/test_key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/test_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    72133 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/lti_xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.954803 lti-consumer-xblock-9.2.1/lti_consumer/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0002_ltiagslineitem.py
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0003_ltiagsscore.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0005_migrate_keyset_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0007_ltidlcontentitem.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0008_fix_uuid_backfill.py
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0013_auto_20210712_1352.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0014_adds_external_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0015_add_additional_1p3_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/outcomes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.958803 lti-consumer-xblock-9.2.1/lti_consumer/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11681 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/plugin/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    35176 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.930803 lti-consumer-xblock-9.2.1/lti_consumer/public/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.930803 lti-consumer-xblock-9.2.1/lti_consumer/public/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.934803 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.958803 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/ar/
--rw-r--r--   0 runner    (1001) docker     (122)    22730 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/ar/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.958803 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/en/
--rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/en/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.958803 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/es_419/
--rw-r--r--   0 runner    (1001) docker     (122)    23422 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/es_419/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.958803 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/fr/
--rw-r--r--   0 runner    (1001) docker     (122)    21751 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/fr/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.958803 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/he/
--rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/he/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.958803 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/hi/
--rw-r--r--   0 runner    (1001) docker     (122)     3735 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/hi/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.958803 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/it/
--rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/it/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.958803 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/ja/
--rw-r--r--   0 runner    (1001) docker     (122)    17362 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/ja/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.958803 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/ko/
--rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/ko/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.958803 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/pt_BR/
--rw-r--r--   0 runner    (1001) docker     (122)     4601 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/pt_BR/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.958803 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/pt_PT/
--rw-r--r--   0 runner    (1001) docker     (122)    13621 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/pt_PT/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.958803 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/ru/
--rw-r--r--   0 runner    (1001) docker     (122)     3772 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/ru/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.958803 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/zh_CN/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.962803 lti-consumer-xblock-9.2.1/lti_consumer/signals/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.934803 lti-consumer-xblock-9.2.1/lti_consumer/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.962803 lti-consumer-xblock-9.2.1/lti_consumer/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/static/css/student.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.962803 lti-consumer-xblock-9.2.1/lti_consumer/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)    12186 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/static/js/xblock_lti_consumer.js
--rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/static/js/xblock_studio_view.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.962803 lti-consumer-xblock-9.2.1/lti_consumer/static/sass/
--rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/static/sass/student.scss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.934803 lti-consumer-xblock-9.2.1/lti_consumer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.962803 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.966803 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti-dl/
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti-dl/dl_response_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti-dl/dl_response_saved.html
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti-dl/render_dl_content.html
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti-dl/render_html.html
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti-dl/render_image.html
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti-dl/render_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti_1p3_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti_1p3_permission_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti_1p3_studio.html
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti_iframe.html
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti_launch_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti_proctoring_start_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/html/student.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.966803 lti-consumer-xblock-9.2.1/lti_consumer/templates/xml/
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templates/xml/outcome_service_response.xml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.966803 lti-consumer-xblock-9.2.1/lti_consumer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templatetags/get_dl_lti_launch_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/templatetags/lti_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.966803 lti-consumer-xblock-9.2.1/lti_consumer/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.966803 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.970803 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11288 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/plugin/test_proctoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/plugin/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    84733 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/test_lti_xblock.py
--rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/test_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/track.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.970803 lti-consumer-xblock-9.2.1/lti_consumer/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.934803 lti-consumer-xblock-9.2.1/lti_consumer/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.970803 lti-consumer-xblock-9.2.1/lti_consumer/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10252 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/ar/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.934803 lti-consumer-xblock-9.2.1/lti_consumer/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.970803 lti-consumer-xblock-9.2.1/lti_consumer/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/en/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.934803 lti-consumer-xblock-9.2.1/lti_consumer/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.970803 lti-consumer-xblock-9.2.1/lti_consumer/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    20799 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26467 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.938803 lti-consumer-xblock-9.2.1/lti_consumer/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.970803 lti-consumer-xblock-9.2.1/lti_consumer/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    18761 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/fr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25340 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/fr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.938803 lti-consumer-xblock-9.2.1/lti_consumer/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.974803 lti-consumer-xblock-9.2.1/lti_consumer/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.938803 lti-consumer-xblock-9.2.1/lti_consumer/translations/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.974803 lti-consumer-xblock-9.2.1/lti_consumer/translations/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9608 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/he/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/he/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.938803 lti-consumer-xblock-9.2.1/lti_consumer/translations/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.974803 lti-consumer-xblock-9.2.1/lti_consumer/translations/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/hi/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16407 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/hi/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.938803 lti-consumer-xblock-9.2.1/lti_consumer/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.974803 lti-consumer-xblock-9.2.1/lti_consumer/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.938803 lti-consumer-xblock-9.2.1/lti_consumer/translations/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.974803 lti-consumer-xblock-9.2.1/lti_consumer/translations/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.938803 lti-consumer-xblock-9.2.1/lti_consumer/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.974803 lti-consumer-xblock-9.2.1/lti_consumer/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16884 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.938803 lti-consumer-xblock-9.2.1/lti_consumer/translations/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.974803 lti-consumer-xblock-9.2.1/lti_consumer/translations/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.938803 lti-consumer-xblock-9.2.1/lti_consumer/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.974803 lti-consumer-xblock-9.2.1/lti_consumer/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      556 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/ru/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16547 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/ru/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.938803 lti-consumer-xblock-9.2.1/lti_consumer/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.974803 lti-consumer-xblock-9.2.1/lti_consumer/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16458 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/lti_consumer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.978803 lti-consumer-xblock-9.2.1/lti_consumer_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-05-03 13:40:02.000000 lti-consumer-xblock-9.2.1/lti_consumer_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7590 2023-05-03 13:40:02.000000 lti-consumer-xblock-9.2.1/lti_consumer_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-03 13:40:02.000000 lti-consumer-xblock-9.2.1/lti_consumer_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-05-03 13:40:02.000000 lti-consumer-xblock-9.2.1/lti_consumer_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-03 13:40:02.000000 lti-consumer-xblock-9.2.1/lti_consumer_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-03 13:40:02.000000 lti-consumer-xblock-9.2.1/lti_consumer_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 13:40:02.978803 lti-consumer-xblock-9.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      343 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-03 13:40:02.978803 lti-consumer-xblock-9.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-05-03 13:39:58.000000 lti-consumer-xblock-9.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.738359 lti-consumer-xblock-9.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)    14500 2023-05-05 16:45:45.738359 lti-consumer-xblock-9.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13716 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.718359 lti-consumer-xblock-9.3.0/lti_consumer/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6551 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.722359 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15317 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.722359 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/contrib/django.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.722359 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/contrib/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/contrib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/contrib/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.722359 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14154 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/tests/test_oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.722359 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3083 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34236 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.722359 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.722359 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      388 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      554 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10557 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/nprs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.726359 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.726359 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.726359 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9875 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/test_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42504 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/test_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/test_key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/test_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    72133 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/lti_xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.726359 lti-consumer-xblock-9.3.0/lti_consumer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0002_ltiagslineitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0003_ltiagsscore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0005_migrate_keyset_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0007_ltidlcontentitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0008_fix_uuid_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0013_auto_20210712_1352.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0014_adds_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0015_add_additional_1p3_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/outcomes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.726359 lti-consumer-xblock-9.3.0/lti_consumer/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11681 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/plugin/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35381 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.714359 lti-consumer-xblock-9.3.0/lti_consumer/public/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.714359 lti-consumer-xblock-9.3.0/lti_consumer/public/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.714359 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.726359 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/ar/
+-rw-r--r--   0 runner    (1001) docker     (122)    22730 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/ar/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.726359 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/en/
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/en/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.726359 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/es_419/
+-rw-r--r--   0 runner    (1001) docker     (122)    23422 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/es_419/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.726359 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/fr/
+-rw-r--r--   0 runner    (1001) docker     (122)    21751 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/fr/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.726359 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/he/
+-rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/he/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.726359 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/hi/
+-rw-r--r--   0 runner    (1001) docker     (122)     3735 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/hi/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/it/
+-rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/it/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/ja/
+-rw-r--r--   0 runner    (1001) docker     (122)    17362 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/ja/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/ko/
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/ko/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/pt_BR/
+-rw-r--r--   0 runner    (1001) docker     (122)     4601 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/pt_BR/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/pt_PT/
+-rw-r--r--   0 runner    (1001) docker     (122)    13621 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/pt_PT/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/ru/
+-rw-r--r--   0 runner    (1001) docker     (122)     3772 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/ru/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/zh_CN/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/signals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.714359 lti-consumer-xblock-9.3.0/lti_consumer/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/static/css/student.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    12186 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/static/js/xblock_lti_consumer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/static/js/xblock_studio_view.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/static/sass/
+-rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/static/sass/student.scss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.714359 lti-consumer-xblock-9.3.0/lti_consumer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti-dl/
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti-dl/dl_response_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti-dl/dl_response_saved.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti-dl/render_dl_content.html
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti-dl/render_html.html
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti-dl/render_image.html
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti-dl/render_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti_1p3_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti_1p3_permission_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti_1p3_studio.html
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti_iframe.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti_launch_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti_proctoring_start_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/html/student.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/templates/xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templates/xml/outcome_service_response.xml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templatetags/get_dl_lti_launch_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/templatetags/lti_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.730359 lti-consumer-xblock-9.3.0/lti_consumer/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.734359 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.734359 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11288 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/plugin/test_proctoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/plugin/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    84733 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/test_lti_xblock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/test_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/track.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.734359 lti-consumer-xblock-9.3.0/lti_consumer/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.714359 lti-consumer-xblock-9.3.0/lti_consumer/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.734359 lti-consumer-xblock-9.3.0/lti_consumer/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10252 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/ar/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/ar/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.714359 lti-consumer-xblock-9.3.0/lti_consumer/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.734359 lti-consumer-xblock-9.3.0/lti_consumer/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/en/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/en/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.714359 lti-consumer-xblock-9.3.0/lti_consumer/translations/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.734359 lti-consumer-xblock-9.3.0/lti_consumer/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    20799 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26467 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/es_419/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.714359 lti-consumer-xblock-9.3.0/lti_consumer/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.734359 lti-consumer-xblock-9.3.0/lti_consumer/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    18761 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/fr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25340 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/fr/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.714359 lti-consumer-xblock-9.3.0/lti_consumer/translations/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.738359 lti-consumer-xblock-9.3.0/lti_consumer/translations/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.718359 lti-consumer-xblock-9.3.0/lti_consumer/translations/he/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.738359 lti-consumer-xblock-9.3.0/lti_consumer/translations/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9608 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/he/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/he/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.718359 lti-consumer-xblock-9.3.0/lti_consumer/translations/hi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.738359 lti-consumer-xblock-9.3.0/lti_consumer/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/hi/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16407 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/hi/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.718359 lti-consumer-xblock-9.3.0/lti_consumer/translations/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.738359 lti-consumer-xblock-9.3.0/lti_consumer/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.718359 lti-consumer-xblock-9.3.0/lti_consumer/translations/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.738359 lti-consumer-xblock-9.3.0/lti_consumer/translations/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.718359 lti-consumer-xblock-9.3.0/lti_consumer/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.738359 lti-consumer-xblock-9.3.0/lti_consumer/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16884 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.718359 lti-consumer-xblock-9.3.0/lti_consumer/translations/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.738359 lti-consumer-xblock-9.3.0/lti_consumer/translations/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.718359 lti-consumer-xblock-9.3.0/lti_consumer/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.738359 lti-consumer-xblock-9.3.0/lti_consumer/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/ru/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16547 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/ru/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.718359 lti-consumer-xblock-9.3.0/lti_consumer/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.738359 lti-consumer-xblock-9.3.0/lti_consumer/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16458 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/lti_consumer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.738359 lti-consumer-xblock-9.3.0/lti_consumer_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14500 2023-05-05 16:45:45.000000 lti-consumer-xblock-9.3.0/lti_consumer_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7590 2023-05-05 16:45:45.000000 lti-consumer-xblock-9.3.0/lti_consumer_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-05 16:45:45.000000 lti-consumer-xblock-9.3.0/lti_consumer_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-05-05 16:45:45.000000 lti-consumer-xblock-9.3.0/lti_consumer_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-05-05 16:45:45.000000 lti-consumer-xblock-9.3.0/lti_consumer_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-05 16:45:45.000000 lti-consumer-xblock-9.3.0/lti_consumer_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 16:45:45.738359 lti-consumer-xblock-9.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-05 16:45:45.738359 lti-consumer-xblock-9.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-05-05 16:45:41.000000 lti-consumer-xblock-9.3.0/setup.py
```

### Comparing `lti-consumer-xblock-9.2.1/LICENSE` & `lti-consumer-xblock-9.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/NOTICE` & `lti-consumer-xblock-9.3.0/NOTICE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/PKG-INFO` & `lti-consumer-xblock-9.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.2.1
+Version: 9.3.0
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
@@ -162,14 +162,21 @@
 See the `developer guide`_ for implementation details and other developer concerns.
 
 .. _developer guide: ./docs/developing.rst
 
 Testing
 *******
 
+Unit Testing
+============
+
+* To run all of the unit tests at once, run `make test`
+* To run tests on individual files in development, run `python ./test.py -k=[name of test file without .py]`
+* For example, if you want to run the tests in test_permissions.py, run `python ./test.py -k=test_permissions`
+
 Testing Against an LTI Provider
 ===============================
 
 LTI 1.1
 -------
 
 http://lti.tools/saltire/ provides a "Test Tool Provider" service that allows
```

### Comparing `lti-consumer-xblock-9.2.1/README.rst` & `lti-consumer-xblock-9.3.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -141,14 +141,21 @@
 See the `developer guide`_ for implementation details and other developer concerns.
 
 .. _developer guide: ./docs/developing.rst
 
 Testing
 *******
 
+Unit Testing
+============
+
+* To run all of the unit tests at once, run `make test`
+* To run tests on individual files in development, run `python ./test.py -k=[name of test file without .py]`
+* For example, if you want to run the tests in test_permissions.py, run `python ./test.py -k=test_permissions`
+
 Testing Against an LTI Provider
 ===============================
 
 LTI 1.1
 -------
 
 http://lti.tools/saltire/ provides a "Test Tool Provider" service that allows
```

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/admin.py` & `lti-consumer-xblock-9.3.0/lti_consumer/admin.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/api.py` & `lti-consumer-xblock-9.3.0/lti_consumer/api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/apps.py` & `lti-consumer-xblock-9.3.0/lti_consumer/apps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/data.py` & `lti-consumer-xblock-9.3.0/lti_consumer/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 This modules provides public data structures to represent LTI 1.3 launch data that can be used within this library and
 by users of this library.
 """
 
 from attrs import define, field, validators
 
+from lti_consumer.lti_1p3.constants import LTI_PROCTORING_ASSESSMENT_CONTROL_ACTIONS
+
 
 @define
 class Lti1p3ProctoringLaunchData:
     """
     The Lti1p3ProctoringLaunchData class contains data necessary and related to an LTI 1.3 proctoring launch.
     It is a mechanism to share launch data between apps. Applications using this library should use the
     Lti1p3ProctoringLaunchData class to supply contextually defined or stored launch data to the LTI 1.3 proctoring
@@ -20,17 +22,27 @@
     * attempt_number (required): The number of the user's attempt in the assessment. The attempt number
         should be an integer that starts with 1 and that is incremented by 1 for each of user's subsequent attempts at
         the assessment.
     * start_assessment_url (conditionally required): The Platform URL that the Tool will send the start
         assessment message to after it has completed the proctoring setup and verification. This attribute is required
         if the message_type attribute of the Lti1p3LaunchData instance is "LtiStartProctoring". It is optional and
         unused otherwise.
+    * assessment_control_url (optional): The Platform URL that the Tool will send assessment control messages to.
+    * assessment_control_actions (optional): A list of assessment control actions supported by the platform.
     """
     attempt_number = field()
     start_assessment_url = field(default=None)
+    assessment_control_url = field(default=None)
+    assessment_control_actions = field(
+        default=[],
+        validator=[validators.deep_iterable(
+            member_validator=validators.in_(LTI_PROCTORING_ASSESSMENT_CONTROL_ACTIONS),
+            iterable_validator=validators.instance_of(list),
+        )],
+    )
 
 
 @define
 class Lti1p3LaunchData:
     """
     The Lti1p3LaunchData class contains data necessary and related to an LTI 1.3 launch. It is a mechanism to share
     launch data between apps. Applications using this library should use the Lti1p3LaunchData class to supply
```

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/filters.py` & `lti-consumer-xblock-9.3.0/lti_consumer/filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/forms.py` & `lti-consumer-xblock-9.3.0/lti_consumer/forms.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/consumer.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/contrib/django.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/contrib/django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/contrib/tests/test_django.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/contrib/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/oauth.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/tests/test_consumer.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p1/tests/test_oauth.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p1/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/ags.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/constants.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,17 @@
     'https://purl.imsglobal.org/spec/lti-ags/scope/lineitem.readonly',
     'https://purl.imsglobal.org/spec/lti-ags/scope/lineitem',
     'https://purl.imsglobal.org/spec/lti-ags/scope/result.readonly',
     'https://purl.imsglobal.org/spec/lti-ags/scope/score',
 
     # LTI-NRPS Scopes
     'https://purl.imsglobal.org/spec/lti-nrps/scope/contextmembership.readonly',
+
+    # ACS Scope
+    'https://purl.imsglobal.org/spec/lti-ap/scope/control.all',
 ]
 
 
 LTI_DEEP_LINKING_ACCEPTED_TYPES = [
     'ltiResourceLink',
     'link',
     'html',
@@ -81,8 +84,23 @@
     """ LTI 1.3 Context Claim Types """
     group = 'http://purl.imsglobal.org/vocab/lis/v2/course#CourseGroup'
     course_offering = 'http://purl.imsglobal.org/vocab/lis/v2/course#CourseOffering'
     course_section = 'http://purl.imsglobal.org/vocab/lis/v2/course#CourseSection'
     course_template = 'http://purl.imsglobal.org/vocab/lis/v2/course#CourseTemplate'
 
 
-LTI_PROCTORING_DATA_KEYS = ['attempt_number', 'resource_link_id', 'session_data', 'start_assessment_url']
+LTI_PROCTORING_DATA_KEYS = [
+    'attempt_number',
+    'resource_link_id',
+    'session_data',
+    'start_assessment_url',
+    'assessment_control_url',
+    'assessment_control_actions'
+]
+
+LTI_PROCTORING_ASSESSMENT_CONTROL_ACTIONS = [
+    'pauseRequest',
+    'resumeRequest',
+    'terminateRequest',
+    'update',
+    'flagRequest',
+]
```

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/consumer.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,15 +452,14 @@
         )
 
         # Check scopes and only return valid and supported ones
         valid_scopes = []
         requested_scopes = token_request_data['scope'].split(' ')
 
         for scope in requested_scopes:
-            # TODO: Add additional checks for permitted scopes
             # Currently there are no scopes, because there is no use for
             # these access tokens until a tool needs to access the LMS.
             # LTI Advantage extensions make use of this.
             if scope in LTI_1P3_ACCESS_TOKEN_SCOPES:
                 valid_scopes.append(scope)
 
         # Scopes are space separated as described in
@@ -818,14 +817,25 @@
             "https://purl.imsglobal.org/spec/lti/claim/message_type": "LtiStartProctoring",
             "https://purl.imsglobal.org/spec/lti-ap/claim/start_assessment_url":
                 self.proctoring_data.get("start_assessment_url"),
         })
 
         return proctoring_claims
 
+    def get_assessment_control_claim(self):
+        """
+        Returns LTI Proctoring Services ACS Claim to be injected in the LTI launch message.
+        """
+        return {
+            "https://purl.imsglobal.org/spec/lti-ap/claim/acs": {
+                "assessment_control_url": self.proctoring_data.get("assessment_control_url"),
+                "actions": self.proctoring_data.get("assessment_control_actions"),
+            }
+        }
+
     def get_end_assessment_claims(self):
         """
         Returns claims specific to LTI Proctoring Services LtiEndAssessment LTI launch message,
         to be injected into the LTI launch message.
         """
         proctoring_claims = self._get_base_claims()
         proctoring_claims.update({
@@ -845,21 +855,30 @@
         the set_extra_claim method to include these additional claims in the LTI launch message.
         """
         lti_message_hint = preflight_response.get('lti_message_hint')
         launch_data = get_data_from_cache(lti_message_hint)
 
         if launch_data.message_type == "LtiStartProctoring":
             proctoring_claims = self.get_start_proctoring_claims()
+
+            # Enable ACS if assessment_control_url is present on the launch data.
+            # Normally we would enable this using a field on the LtiConfiguration model like other
+            # Advantage services, but this isn't actually optional or configurable for Open edX.
+            if self.proctoring_data.get("assessment_control_url"):
+                self.set_extra_claim(self.get_assessment_control_claim())
         elif launch_data.message_type == "LtiEndAssessment":
             proctoring_claims = self.get_end_assessment_claims()
         else:
             raise ValueError('lti_message_hint must \"LtiStartProctoring\" or \"LtiEndAssessment\".')
 
         self.set_extra_claim(proctoring_claims)
 
+        if self.proctoring_data.get("assessment_control_url"):
+            self.set_extra_claim(self.get_assessment_control_claim())
+
         return super().generate_launch_request(preflight_response)
 
     def check_and_decode_token(self, token):
         """
         Decodes a Tool JWT token and validates OAuth and LTI Proctoring Services specificatin related claims. Returns a
         dictionary representation of key proctoring claims in the Tool JWT token.
```

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/deep_linking.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/exceptions.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/exceptions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py`

 * *Files 11% similar despite different names*

```diff
@@ -95,7 +95,28 @@
 
         if view.action == 'list':
             scopes = [
                 'https://purl.imsglobal.org/spec/lti-nrps/scope/contextmembership.readonly'
             ]
 
         return scopes
+
+
+class LtiProctoringAcsPermissions(LTIBasePermissions):
+    """
+    LTI ACS Permissions.
+
+    This checks if the token included in the request
+    has the allowed scopes to perform ACS actions
+    (insert action examples here)
+
+    Link to relevant docs: (ims global docs url here)
+    """
+
+    def get_permission_scopes(self, request, view):
+        """
+        Return the LTI ACS scope.
+        There is only one: http://www.imsglobal.org/spec/proctoring/v1p0#h.ckrfa92a27mw
+        """
+        return [
+            'https://purl.imsglobal.org/spec/lti-ap/scope/control.all',
+        ]
```

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/extensions/rest_framework/utils.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/extensions/rest_framework/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/key_handlers.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/nprs.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/nprs.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from django.test.testcases import TestCase
 
 from lti_consumer.lti_1p3.consumer import LtiConsumer1p3
 from lti_consumer.models import LtiConfiguration
 from lti_consumer.lti_1p3.extensions.rest_framework.permissions import (
     LtiAgsPermissions,
     LtiNrpsContextMembershipsPermissions,
+    LtiProctoringAcsPermissions,
 )
 
 
 # Variables required for testing and verification
 ISS = "http://test-platform.example/"
 OIDC_URL = "http://test-platform/oidc"
 LAUNCH_URL = "http://test-platform/launch"
@@ -264,14 +265,40 @@
 
         mock_view = MagicMock()
 
         # Make token and include it in the mock request
         token = self._make_token(token_scopes)
         self.mock_request.headers = {
             "Authorization": "Bearer {}".format(token)
+        }
+
+        # Test scores view
+        mock_view.action = 'list'
+        self.assertEqual(
+            perm_class.has_permission(self.mock_request, mock_view),
+            is_allowed,
+        )
+
+    @ddt.data(
+        (["https://purl.imsglobal.org/spec/lti-ap/scope/control.all"], True),
+        ([], False),
+    )
+    @ddt.unpack
+    def test_proctoring_acs_permissions(self, token_scopes, is_allowed):
+        """
+        Test if LTI Proctoring ACS Permissions endpoint is availabe for correct token.
+        """
+        perm_class = LtiProctoringAcsPermissions()
+
+        mock_view = MagicMock()
+
+        # Make token and include it in the mock request
+        token = self._make_token(token_scopes)
+        self.mock_request.headers = {
+            "Authorization": "Bearer {}".format(token)
         }
 
         # Test scores view
         mock_view.action = 'list'
         self.assertEqual(
             perm_class.has_permission(self.mock_request, mock_view),
             is_allowed,
```

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/test_ags.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/test_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/test_consumer.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/test_consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1005,14 +1005,35 @@
             "https://purl.imsglobal.org/spec/lti-ap/claim/attempt_number": "attempt_number",
             "https://purl.imsglobal.org/spec/lti-ap/claim/session_data": "session_data",
             "https://purl.imsglobal.org/spec/lti/claim/message_type": "LtiEndAssessment",
         }
 
         self.assertEqual(expected_get_end_assessment_claims, actual_get_end_assessment_claims)
 
+    def test_assessment_control_claims(self):
+        """
+        Ensure the correct claims are returned for the assessment control service.
+        """
+        self.lti_consumer.set_proctoring_data(
+            attempt_number="attempt_number",
+            session_data="session_data",
+            start_assessment_url="start_assessment_url",
+            assessment_control_url="assessment_control_url",
+            assessment_control_actions=["flagRequest", "terminateRequest"],
+        )
+        proctoring_acs_claims = self.lti_consumer.get_assessment_control_claim()
+
+        expected_acs_claims = {
+            "https://purl.imsglobal.org/spec/lti-ap/claim/acs": {
+                "assessment_control_url": "assessment_control_url",
+                "actions": ["flagRequest", "terminateRequest"],
+            },
+        }
+        self.assertDictEqual(proctoring_acs_claims, expected_acs_claims)
+
     @ddt.data("LtiStartProctoring", "LtiEndAssessment")
     @patch('lti_consumer.lti_1p3.consumer.get_data_from_cache')
     def test_generate_launch_request(self, message_type, mock_get_data_from_cache):
         """
         Ensures that the correct claims are included in LTI launch messages for the LtiStartProctoring and
         LtiEndAssessment launch message types.
         """
@@ -1042,14 +1063,44 @@
             expected_claims = self.lti_consumer.get_end_assessment_claims()
 
         decoded_token_claims = decoded_token.items()
         for claim in expected_claims.items():
             self.assertIn(claim, decoded_token_claims)
 
     @patch('lti_consumer.lti_1p3.consumer.get_data_from_cache')
+    def test_enable_assessment_control(self, mock_get_data_from_cache):
+        """
+        Ensure that the correct claims are included in LTI launch messages with an ACS url set.
+        """
+
+        mock_launch_data = self.get_launch_data(message_type="LtiStartProctoring")
+        mock_get_data_from_cache.return_value = mock_launch_data
+        self._setup_proctoring()
+
+        self.lti_consumer.set_proctoring_data(
+            attempt_number="attempt_number",
+            session_data="session_data",
+            start_assessment_url="start_assessment_url",
+            assessment_control_url="assessment_control_url",
+            assessment_control_actions=["flagRequest", "terminateRequest"],
+        )
+
+        token = self.lti_consumer.generate_launch_request(
+            self.preflight_response,
+        )['id_token']
+
+        decoded_token = self.lti_consumer.key_handler.validate_and_decode(token)
+        expected_claims = self.lti_consumer.get_start_proctoring_claims()
+        expected_claims.update(self.lti_consumer.get_assessment_control_claim())
+
+        decoded_token_claims = decoded_token.items()
+        for claim in expected_claims.items():
+            self.assertIn(claim, decoded_token_claims)
+
+    @patch('lti_consumer.lti_1p3.consumer.get_data_from_cache')
     def test_generate_launch_request_invalid_message(self, mock_get_data_from_cache):
         """
         Ensures that a ValueError is raised if the launch_data.message_type is not LtiStartProctoring or
         LtiEndAssessment.
         """
 
         mock_launch_data = self.get_launch_data(message_type="LtiResourceLinkRequest")
```

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/test_deep_linking.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/test_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/test_key_handlers.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/test_key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_1p3/tests/test_nrps.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_1p3/tests/test_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/lti_xblock.py` & `lti-consumer-xblock-9.3.0/lti_consumer/lti_xblock.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0001_initial.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0002_ltiagslineitem.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0002_ltiagslineitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0003_ltiagsscore.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0003_ltiagsscore.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0004_keyset_mgmt_to_model.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0004_keyset_mgmt_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0005_migrate_keyset_to_model.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0005_migrate_keyset_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0007_ltidlcontentitem.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0007_ltidlcontentitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0008_fix_uuid_backfill.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0008_fix_uuid_backfill.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0009_backfill-empty-string-config-id.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0009_backfill-empty-string-config-id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0013_auto_20210712_1352.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0013_auto_20210712_1352.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0014_adds_external_id.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0014_adds_external_id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0015_add_additional_1p3_fields.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0015_add_additional_1p3_fields.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py` & `lti-consumer-xblock-9.3.0/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/models.py` & `lti-consumer-xblock-9.3.0/lti_consumer/models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/outcomes.py` & `lti-consumer-xblock-9.3.0/lti_consumer/outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/plugin/compat.py` & `lti-consumer-xblock-9.3.0/lti_consumer/plugin/compat.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/plugin/urls.py` & `lti-consumer-xblock-9.3.0/lti_consumer/plugin/urls.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/plugin/views.py` & `lti-consumer-xblock-9.3.0/lti_consumer/plugin/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,17 @@
             if not session_data:
                 session_data = get_random_string(32)
                 TieredCache.set_all_tiers(session_data_key, session_data)
 
             lti_consumer.set_proctoring_data(
                 attempt_number=launch_data.proctoring_launch_data.attempt_number,
                 session_data=session_data,
-                start_assessment_url=launch_data.proctoring_launch_data.start_assessment_url
+                start_assessment_url=launch_data.proctoring_launch_data.start_assessment_url,
+                assessment_control_url=launch_data.proctoring_launch_data.assessment_control_url,
+                assessment_control_actions=launch_data.proctoring_launch_data.assessment_control_actions,
             )
         elif launch_data.message_type == 'LtiEndAssessment':
             lti_consumer.set_proctoring_data(
                 attempt_number=launch_data.proctoring_launch_data.attempt_number,
             )
 
         # Update context with LTI launch parameters
```

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/ar/text.js` & `lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/ar/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/en/text.js` & `lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/en/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/es_419/text.js` & `lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/es_419/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/fr/text.js` & `lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/fr/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/he/text.js` & `lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/he/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/hi/text.js` & `lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/hi/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/it/text.js` & `lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/it/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/ja/text.js` & `lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/ja/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/ko/text.js` & `lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/ko/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/pt_BR/text.js` & `lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/pt_BR/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/pt_PT/text.js` & `lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/pt_PT/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/ru/text.js` & `lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/ru/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/public/js/translations/zh_CN/text.js` & `lti-consumer-xblock-9.3.0/lti_consumer/public/js/translations/zh_CN/text.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/signals/signals.py` & `lti-consumer-xblock-9.3.0/lti_consumer/signals/signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/static/css/student.css` & `lti-consumer-xblock-9.3.0/lti_consumer/static/css/student.css`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/static/js/xblock_lti_consumer.js` & `lti-consumer-xblock-9.3.0/lti_consumer/static/js/xblock_lti_consumer.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/static/js/xblock_studio_view.js` & `lti-consumer-xblock-9.3.0/lti_consumer/static/js/xblock_studio_view.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/static/sass/student.scss` & `lti-consumer-xblock-9.3.0/lti_consumer/static/sass/student.scss`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti-dl/render_dl_content.html` & `lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti-dl/render_dl_content.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti-dl/render_image.html` & `lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti-dl/render_image.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti-dl/render_link.html` & `lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti-dl/render_link.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti_1p3_launch.html` & `lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti_1p3_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti_1p3_studio.html` & `lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti_1p3_studio.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/templates/html/lti_launch.html` & `lti-consumer-xblock-9.3.0/lti_consumer/templates/html/lti_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/templates/html/student.html` & `lti-consumer-xblock-9.3.0/lti_consumer/templates/html/student.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/templates/xml/outcome_service_response.xml` & `lti-consumer-xblock-9.3.0/lti_consumer/templates/xml/outcome_service_response.xml`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/templatetags/get_dl_lti_launch_url.py` & `lti-consumer-xblock-9.3.0/lti_consumer/templatetags/get_dl_lti_launch_url.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/templatetags/lti_sanitize.py` & `lti-consumer-xblock-9.3.0/lti_consumer/templatetags/lti_sanitize.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/tests/test_utils.py` & `lti-consumer-xblock-9.3.0/lti_consumer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/plugin/test_proctoring.py` & `lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/plugin/test_proctoring.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/plugin/test_views.py` & `lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/plugin/test_views.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/plugin/test_views_lti_ags.py` & `lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/plugin/test_views_lti_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py` & `lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py` & `lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/test_api.py` & `lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/test_filters.py` & `lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/test_lti_xblock.py` & `lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/test_lti_xblock.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/test_models.py` & `lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/test_outcomes.py` & `lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/test_signals.py` & `lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/test_signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/tests/unit/test_utils.py` & `lti-consumer-xblock-9.3.0/lti_consumer/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/ar/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/ar/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/ar/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/ar/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/en/LC_MESSAGES/django.po` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/en/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/en/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/es_419/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/es_419/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/es_419/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/es_419/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/fr/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/fr/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/fr/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/fr/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/he/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/he/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/he/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/he/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/hi/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/hi/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/ru/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/ru/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/ru/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/ru/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/settings.py` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/settings.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.3.0/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer/utils.py` & `lti-consumer-xblock-9.3.0/lti_consumer/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer_xblock.egg-info/PKG-INFO` & `lti-consumer-xblock-9.3.0/lti_consumer_xblock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.2.1
+Version: 9.3.0
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
@@ -162,14 +162,21 @@
 See the `developer guide`_ for implementation details and other developer concerns.
 
 .. _developer guide: ./docs/developing.rst
 
 Testing
 *******
 
+Unit Testing
+============
+
+* To run all of the unit tests at once, run `make test`
+* To run tests on individual files in development, run `python ./test.py -k=[name of test file without .py]`
+* For example, if you want to run the tests in test_permissions.py, run `python ./test.py -k=test_permissions`
+
 Testing Against an LTI Provider
 ===============================
 
 LTI 1.1
 -------
 
 http://lti.tools/saltire/ provides a "Test Tool Provider" service that allows
```

### Comparing `lti-consumer-xblock-9.2.1/lti_consumer_xblock.egg-info/SOURCES.txt` & `lti-consumer-xblock-9.3.0/lti_consumer_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.2.1/setup.py` & `lti-consumer-xblock-9.3.0/setup.py`

 * *Files identical despite different names*

