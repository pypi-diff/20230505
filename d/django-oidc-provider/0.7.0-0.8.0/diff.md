# Comparing `tmp/django-oidc-provider-0.7.0.tar.gz` & `tmp/django-oidc-provider-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-oidc-provider-0.7.0.tar", last modified: Wed Oct 17 22:09:22 2018, max compression
+gzip compressed data, was "django-oidc-provider-0.8.0.tar", last modified: Fri May  5 20:08:25 2023, max compression
```

## Comparing `django-oidc-provider-0.7.0.tar` & `django-oidc-provider-0.8.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     1095 2018-08-03 14:55:10.000000 django-oidc-provider-0.7.0/LICENSE
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)       38 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/setup.cfg
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      210 2018-03-22 15:48:30.000000 django-oidc-provider-0.7.0/MANIFEST.in
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      147 2018-03-22 15:47:44.000000 django-oidc-provider-0.7.0/oidc_provider/apps.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     8937 2018-09-14 19:34:52.000000 django-oidc-provider-0.7.0/oidc_provider/models.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)       62 2018-03-22 15:47:44.000000 django-oidc-provider-0.7.0/oidc_provider/__init__.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     1029 2018-07-10 14:18:27.000000 django-oidc-provider-0.7.0/oidc_provider/urls.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      869 2018-03-22 15:49:03.000000 django-oidc-provider-0.7.0/oidc_provider/middleware.py
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/static/
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/static/oidc_provider/
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/static/oidc_provider/js/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     3989 2018-03-22 15:48:30.000000 django-oidc-provider-0.7.0/oidc_provider/static/oidc_provider/js/sha256.min.js
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      487 2018-03-22 15:48:06.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0012_auto_20160405_2041.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     7082 2018-04-13 19:43:28.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0016_userconsent_and_verbosenames.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-03-08 13:55:41.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/__init__.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      464 2018-03-22 15:48:06.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0010_code_is_authentication.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      515 2018-03-22 15:48:30.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0019_auto_20161005_1552.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     1365 2018-04-13 19:43:28.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0007_auto_20160111_1844.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      630 2018-03-22 15:47:44.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0009_auto_20160202_1945.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     2694 2018-04-13 19:43:28.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0015_change_client_code.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      386 2018-03-22 15:47:44.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0006_unique_user_client.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      797 2018-04-13 19:43:28.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0011_client_client_type.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     2625 2018-04-13 19:43:28.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0017_auto_20160811_1954.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      646 2018-03-22 15:48:06.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0013_auto_20160407_1912.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      633 2018-04-13 19:43:28.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0020_client__post_logout_redirect_uris.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      801 2018-04-13 19:43:28.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0025_user_field_codetoken.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      469 2018-03-22 15:47:44.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0005_token_refresh_token.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      738 2018-04-13 19:43:28.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0023_client_owner.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     2324 2018-04-13 19:43:28.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0018_hybridflow_and_clientattrs.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     5120 2018-04-13 19:43:28.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0001_initial.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      620 2018-04-13 19:43:28.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0014_client_jwt_alg.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      992 2018-03-22 15:49:03.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0002_userconsent.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      422 2018-03-08 13:55:41.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0003_code_nonce.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     1062 2018-04-13 19:43:28.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0022_auto_20170331_1626.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     2354 2018-09-14 19:34:52.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0026_client_multiple_response_types.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      568 2018-03-22 15:48:30.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0021_refresh_token_not_unique.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      414 2018-04-13 19:43:28.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0004_remove_userinfo.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      587 2018-04-13 19:43:28.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0024_auto_20180327_1959.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      567 2018-03-22 15:47:44.000000 django-oidc-provider-0.7.0/oidc_provider/migrations/0008_rsakey.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)    14192 2018-10-17 22:03:52.000000 django-oidc-provider-0.7.0/oidc_provider/views.py
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/lib/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     5665 2018-09-14 19:34:52.000000 django-oidc-provider-0.7.0/oidc_provider/lib/claims.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-03-08 13:55:41.000000 django-oidc-provider-0.7.0/oidc_provider/lib/__init__.py
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/lib/utils/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      696 2018-10-17 22:03:52.000000 django-oidc-provider-0.7.0/oidc_provider/lib/utils/authorize.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     3033 2018-08-03 14:55:10.000000 django-oidc-provider-0.7.0/oidc_provider/lib/utils/oauth2.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-03-08 13:55:41.000000 django-oidc-provider-0.7.0/oidc_provider/lib/utils/__init__.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     4600 2018-10-17 22:03:52.000000 django-oidc-provider-0.7.0/oidc_provider/lib/utils/token.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     5472 2018-07-10 14:18:27.000000 django-oidc-provider-0.7.0/oidc_provider/lib/utils/common.py
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/lib/endpoints/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)    11734 2018-09-14 19:34:52.000000 django-oidc-provider-0.7.0/oidc_provider/lib/endpoints/authorize.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-03-08 13:55:41.000000 django-oidc-provider-0.7.0/oidc_provider/lib/endpoints/__init__.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     4123 2018-08-03 14:55:10.000000 django-oidc-provider-0.7.0/oidc_provider/lib/endpoints/introspection.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)    10012 2018-07-10 14:18:27.000000 django-oidc-provider-0.7.0/oidc_provider/lib/endpoints/token.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     6554 2018-07-10 14:18:27.000000 django-oidc-provider-0.7.0/oidc_provider/lib/errors.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)       22 2018-10-17 22:05:01.000000 django-oidc-provider-0.7.0/oidc_provider/version.py
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/management/
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/management/commands/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-03-08 13:55:41.000000 django-oidc-provider-0.7.0/oidc_provider/management/commands/__init__.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      608 2018-10-17 22:03:52.000000 django-oidc-provider-0.7.0/oidc_provider/management/commands/creatersakey.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-03-08 13:55:41.000000 django-oidc-provider-0.7.0/oidc_provider/management/__init__.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     2739 2018-09-14 19:34:52.000000 django-oidc-provider-0.7.0/oidc_provider/admin.py
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/tests/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-03-22 14:36:32.000000 django-oidc-provider-0.7.0/oidc_provider/tests/__init__.py
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/tests/app/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-03-08 13:55:41.000000 django-oidc-provider-0.7.0/oidc_provider/tests/app/__init__.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      703 2018-09-14 19:34:52.000000 django-oidc-provider-0.7.0/oidc_provider/tests/app/urls.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     4776 2018-09-14 19:34:52.000000 django-oidc-provider-0.7.0/oidc_provider/tests/app/utils.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     1825 2018-03-22 15:49:03.000000 django-oidc-provider-0.7.0/oidc_provider/tests/settings.py
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/tests/templates/
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/tests/templates/accounts/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      239 2018-03-08 13:55:41.000000 django-oidc-provider-0.7.0/oidc_provider/tests/templates/accounts/login.html
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)       83 2018-03-08 13:55:41.000000 django-oidc-provider-0.7.0/oidc_provider/tests/templates/accounts/logout.html
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     6318 2018-07-10 14:18:27.000000 django-oidc-provider-0.7.0/oidc_provider/settings.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      208 2018-03-22 15:48:30.000000 django-oidc-provider-0.7.0/oidc_provider/signals.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      136 2018-03-22 15:49:03.000000 django-oidc-provider-0.7.0/oidc_provider/compat.py
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/locale/
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/locale/pl/
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/locale/pl/LC_MESSAGES/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     3765 2018-03-22 15:48:06.000000 django-oidc-provider-0.7.0/oidc_provider/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     2465 2018-03-22 15:48:06.000000 django-oidc-provider-0.7.0/oidc_provider/locale/pl/LC_MESSAGES/django.mo
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/locale/fr/
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/locale/fr/LC_MESSAGES/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     3852 2018-03-22 15:48:06.000000 django-oidc-provider-0.7.0/oidc_provider/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     2962 2018-03-22 15:48:30.000000 django-oidc-provider-0.7.0/oidc_provider/locale/fr/LC_MESSAGES/django.mo
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/locale/es/
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/locale/es/LC_MESSAGES/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     2915 2018-03-22 15:48:06.000000 django-oidc-provider-0.7.0/oidc_provider/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      421 2018-03-22 15:48:06.000000 django-oidc-provider-0.7.0/oidc_provider/locale/es/LC_MESSAGES/django.mo
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/templates/
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/oidc_provider/templates/oidc_provider/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)       45 2018-03-08 13:55:41.000000 django-oidc-provider-0.7.0/oidc_provider/templates/oidc_provider/error.html
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      732 2018-03-22 15:48:06.000000 django-oidc-provider-0.7.0/oidc_provider/templates/oidc_provider/hidden_inputs.html
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)      519 2018-03-22 15:48:06.000000 django-oidc-provider-0.7.0/oidc_provider/templates/oidc_provider/authorize.html
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     1919 2018-04-13 19:43:28.000000 django-oidc-provider-0.7.0/oidc_provider/templates/oidc_provider/check_session_iframe.html
-drwxr-xr-x   0 jfiorentino  (1000) jfiorentino  (1000)        0 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/django_oidc_provider.egg-info/
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)       16 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/django_oidc_provider.egg-info/requires.txt
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     3337 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/django_oidc_provider.egg-info/SOURCES.txt
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)        1 2018-07-31 17:17:30.000000 django-oidc-provider-0.7.0/django_oidc_provider.egg-info/not-zip-safe
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)        1 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/django_oidc_provider.egg-info/dependency_links.txt
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)       14 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/django_oidc_provider.egg-info/top_level.txt
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     1022 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/django_oidc_provider.egg-info/PKG-INFO
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     1599 2018-10-17 22:03:52.000000 django-oidc-provider-0.7.0/setup.py
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     1484 2018-07-10 14:18:27.000000 django-oidc-provider-0.7.0/README.md
--rw-r--r--   0 jfiorentino  (1000) jfiorentino  (1000)     1022 2018-10-17 22:09:22.000000 django-oidc-provider-0.7.0/PKG-INFO
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.134045 django-oidc-provider-0.8.0/
+-rw-r--r--   0 juanifioren   (501) staff       (20)     1095 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/LICENSE
+-rw-r--r--   0 juanifioren   (501) staff       (20)      210 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/MANIFEST.in
+-rw-r--r--   0 juanifioren   (501) staff       (20)     1018 2023-05-05 20:08:25.130929 django-oidc-provider-0.8.0/PKG-INFO
+-rw-r--r--   0 juanifioren   (501) staff       (20)     1342 2023-05-04 16:40:52.000000 django-oidc-provider-0.8.0/README.md
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.068241 django-oidc-provider-0.8.0/django_oidc_provider.egg-info/
+-rw-r--r--   0 juanifioren   (501) staff       (20)     1018 2023-05-05 20:08:25.000000 django-oidc-provider-0.8.0/django_oidc_provider.egg-info/PKG-INFO
+-rw-r--r--   0 juanifioren   (501) staff       (20)     3337 2023-05-05 20:08:25.000000 django-oidc-provider-0.8.0/django_oidc_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 juanifioren   (501) staff       (20)        1 2023-05-05 20:08:25.000000 django-oidc-provider-0.8.0/django_oidc_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 juanifioren   (501) staff       (20)        1 2023-05-04 14:57:54.000000 django-oidc-provider-0.8.0/django_oidc_provider.egg-info/not-zip-safe
+-rw-r--r--   0 juanifioren   (501) staff       (20)       16 2023-05-05 20:08:25.000000 django-oidc-provider-0.8.0/django_oidc_provider.egg-info/requires.txt
+-rw-r--r--   0 juanifioren   (501) staff       (20)       14 2023-05-05 20:08:25.000000 django-oidc-provider-0.8.0/django_oidc_provider.egg-info/top_level.txt
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.075322 django-oidc-provider-0.8.0/oidc_provider/
+-rw-r--r--   0 juanifioren   (501) staff       (20)       62 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/__init__.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     2798 2023-05-04 14:52:10.000000 django-oidc-provider-0.8.0/oidc_provider/admin.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      147 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/apps.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      136 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/compat.py
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.076470 django-oidc-provider-0.8.0/oidc_provider/lib/
+-rw-r--r--   0 juanifioren   (501) staff       (20)        0 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/lib/__init__.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     5664 2023-05-04 14:52:10.000000 django-oidc-provider-0.8.0/oidc_provider/lib/claims.py
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.078808 django-oidc-provider-0.8.0/oidc_provider/lib/endpoints/
+-rw-r--r--   0 juanifioren   (501) staff       (20)        0 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/lib/endpoints/__init__.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)    11734 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/lib/endpoints/authorize.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     4254 2023-05-04 14:52:10.000000 django-oidc-provider-0.8.0/oidc_provider/lib/endpoints/introspection.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)    11127 2023-05-04 14:52:10.000000 django-oidc-provider-0.8.0/oidc_provider/lib/endpoints/token.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     6554 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/lib/errors.py
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.082095 django-oidc-provider-0.8.0/oidc_provider/lib/utils/
+-rw-r--r--   0 juanifioren   (501) staff       (20)        0 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/lib/utils/__init__.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      696 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/lib/utils/authorize.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     5472 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/lib/utils/common.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     3035 2023-05-04 14:52:10.000000 django-oidc-provider-0.8.0/oidc_provider/lib/utils/oauth2.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     4597 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/lib/utils/token.py
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.059616 django-oidc-provider-0.8.0/oidc_provider/locale/
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.059197 django-oidc-provider-0.8.0/oidc_provider/locale/es/
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.083271 django-oidc-provider-0.8.0/oidc_provider/locale/es/LC_MESSAGES/
+-rw-r--r--   0 juanifioren   (501) staff       (20)      421 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 juanifioren   (501) staff       (20)     2915 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.059461 django-oidc-provider-0.8.0/oidc_provider/locale/fr/
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.084793 django-oidc-provider-0.8.0/oidc_provider/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 juanifioren   (501) staff       (20)     2962 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 juanifioren   (501) staff       (20)     3852 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.059717 django-oidc-provider-0.8.0/oidc_provider/locale/pl/
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.086230 django-oidc-provider-0.8.0/oidc_provider/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 juanifioren   (501) staff       (20)     2465 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 juanifioren   (501) staff       (20)     3765 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.086945 django-oidc-provider-0.8.0/oidc_provider/management/
+-rw-r--r--   0 juanifioren   (501) staff       (20)        0 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/management/__init__.py
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.087933 django-oidc-provider-0.8.0/oidc_provider/management/commands/
+-rw-r--r--   0 juanifioren   (501) staff       (20)        0 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/management/commands/__init__.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      608 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/management/commands/creatersakey.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      869 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/middleware.py
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.117044 django-oidc-provider-0.8.0/oidc_provider/migrations/
+-rw-r--r--   0 juanifioren   (501) staff       (20)     5120 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0001_initial.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      992 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0002_userconsent.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      422 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0003_code_nonce.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      414 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0004_remove_userinfo.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      469 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0005_token_refresh_token.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      386 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0006_unique_user_client.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     1365 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0007_auto_20160111_1844.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      567 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0008_rsakey.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      630 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0009_auto_20160202_1945.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      464 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0010_code_is_authentication.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      797 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0011_client_client_type.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      487 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0012_auto_20160405_2041.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      646 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0013_auto_20160407_1912.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      620 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0014_client_jwt_alg.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     2694 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0015_change_client_code.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     7082 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0016_userconsent_and_verbosenames.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     2625 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0017_auto_20160811_1954.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     2324 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0018_hybridflow_and_clientattrs.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      515 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0019_auto_20161005_1552.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      633 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0020_client__post_logout_redirect_uris.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      568 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0021_refresh_token_not_unique.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     1062 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0022_auto_20170331_1626.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      738 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0023_client_owner.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      587 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0024_auto_20180327_1959.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      801 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0025_user_field_codetoken.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     2354 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/0026_client_multiple_response_types.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)        0 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/migrations/__init__.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     8912 2023-05-04 14:52:10.000000 django-oidc-provider-0.8.0/oidc_provider/models.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     6532 2023-05-04 14:52:10.000000 django-oidc-provider-0.8.0/oidc_provider/settings.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      124 2023-05-04 15:16:49.000000 django-oidc-provider-0.8.0/oidc_provider/signals.py
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.060551 django-oidc-provider-0.8.0/oidc_provider/static/
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.060670 django-oidc-provider-0.8.0/oidc_provider/static/oidc_provider/
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.117603 django-oidc-provider-0.8.0/oidc_provider/static/oidc_provider/js/
+-rw-r--r--   0 juanifioren   (501) staff       (20)     3989 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/static/oidc_provider/js/sha256.min.js
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.061087 django-oidc-provider-0.8.0/oidc_provider/templates/
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.121149 django-oidc-provider-0.8.0/oidc_provider/templates/oidc_provider/
+-rw-r--r--   0 juanifioren   (501) staff       (20)      519 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/templates/oidc_provider/authorize.html
+-rw-r--r--   0 juanifioren   (501) staff       (20)     1914 2023-05-04 14:52:10.000000 django-oidc-provider-0.8.0/oidc_provider/templates/oidc_provider/check_session_iframe.html
+-rw-r--r--   0 juanifioren   (501) staff       (20)       45 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/templates/oidc_provider/error.html
+-rw-r--r--   0 juanifioren   (501) staff       (20)      732 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/templates/oidc_provider/hidden_inputs.html
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.124158 django-oidc-provider-0.8.0/oidc_provider/tests/
+-rw-r--r--   0 juanifioren   (501) staff       (20)        0 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/tests/__init__.py
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.127575 django-oidc-provider-0.8.0/oidc_provider/tests/app/
+-rw-r--r--   0 juanifioren   (501) staff       (20)        0 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/tests/app/__init__.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)      803 2023-05-04 14:52:10.000000 django-oidc-provider-0.8.0/oidc_provider/tests/app/urls.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     4814 2023-05-04 14:52:10.000000 django-oidc-provider-0.8.0/oidc_provider/tests/app/utils.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)     1825 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/tests/settings.py
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.062041 django-oidc-provider-0.8.0/oidc_provider/tests/templates/
+drwxr-xr-x   0 juanifioren   (501) staff       (20)        0 2023-05-05 20:08:25.129970 django-oidc-provider-0.8.0/oidc_provider/tests/templates/accounts/
+-rw-r--r--   0 juanifioren   (501) staff       (20)      239 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/tests/templates/accounts/login.html
+-rw-r--r--   0 juanifioren   (501) staff       (20)       83 2023-05-04 14:44:46.000000 django-oidc-provider-0.8.0/oidc_provider/tests/templates/accounts/logout.html
+-rw-r--r--   0 juanifioren   (501) staff       (20)     1126 2023-05-04 14:52:10.000000 django-oidc-provider-0.8.0/oidc_provider/urls.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)       22 2023-05-05 19:57:36.000000 django-oidc-provider-0.8.0/oidc_provider/version.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)    14406 2023-05-04 14:52:10.000000 django-oidc-provider-0.8.0/oidc_provider/views.py
+-rw-r--r--   0 juanifioren   (501) staff       (20)       38 2023-05-05 20:08:25.134307 django-oidc-provider-0.8.0/setup.cfg
+-rw-r--r--   0 juanifioren   (501) staff       (20)     1603 2023-05-04 16:39:52.000000 django-oidc-provider-0.8.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-oidc-provider-0.7.0/LICENSE` & `django-oidc-provider-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/models.py` & `django-oidc-provider-0.8.0/oidc_provider/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# -*- coding: utf-8 -*-
 import base64
 import binascii
 from hashlib import md5, sha256
 import json
 
 from django.db import models
 from django.utils import timezone
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.conf import settings
 
 
 CLIENT_TYPE_CHOICES = [
     ('confidential', 'Confidential'),
     ('public', 'Public'),
 ]
```

### Comparing `django-oidc-provider-0.7.0/oidc_provider/urls.py` & `django-oidc-provider-0.8.0/oidc_provider/urls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 try:
-    from django.urls import url
+    from django.urls import include, re_path
 except ImportError:
-    from django.conf.urls import url
+    from django.conf.urls import include
+    from django.conf.urls import url as re_path
 from django.views.decorators.csrf import csrf_exempt
 
 from oidc_provider import (
     settings,
     views,
 )
 
 app_name = 'oidc_provider'
 urlpatterns = [
-    url(r'^authorize/?$', views.AuthorizeView.as_view(), name='authorize'),
-    url(r'^token/?$', csrf_exempt(views.TokenView.as_view()), name='token'),
-    url(r'^userinfo/?$', csrf_exempt(views.userinfo), name='userinfo'),
-    url(r'^end-session/?$', views.EndSessionView.as_view(), name='end-session'),
-    url(r'^\.well-known/openid-configuration/?$', views.ProviderInfoView.as_view(),
+    re_path(r'^authorize/?$', views.AuthorizeView.as_view(), name='authorize'),
+    re_path(r'^token/?$', csrf_exempt(views.TokenView.as_view()), name='token'),
+    re_path(r'^userinfo/?$', csrf_exempt(views.userinfo), name='userinfo'),
+    re_path(r'^end-session/?$', views.EndSessionView.as_view(), name='end-session'),
+    re_path(r'^\.well-known/openid-configuration/?$', views.ProviderInfoView.as_view(),
         name='provider-info'),
-    url(r'^introspect/?$', views.TokenIntrospectionView.as_view(), name='token-introspection'),
-    url(r'^jwks/?$', views.JwksView.as_view(), name='jwks'),
+    re_path(r'^introspect/?$', views.TokenIntrospectionView.as_view(), name='token-introspection'),
+    re_path(r'^jwks/?$', views.JwksView.as_view(), name='jwks'),
 ]
 
 if settings.get('OIDC_SESSION_MANAGEMENT_ENABLE'):
     urlpatterns += [
-        url(r'^check-session-iframe/?$', views.CheckSessionIframeView.as_view(),
+        re_path(r'^check-session-iframe/?$', views.CheckSessionIframeView.as_view(),
             name='check-session-iframe'),
     ]
```

### Comparing `django-oidc-provider-0.7.0/oidc_provider/middleware.py` & `django-oidc-provider-0.8.0/oidc_provider/middleware.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/static/oidc_provider/js/sha256.min.js` & `django-oidc-provider-0.8.0/oidc_provider/static/oidc_provider/js/sha256.min.js`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0016_userconsent_and_verbosenames.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0016_userconsent_and_verbosenames.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0019_auto_20161005_1552.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0019_auto_20161005_1552.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0007_auto_20160111_1844.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0007_auto_20160111_1844.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0009_auto_20160202_1945.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0009_auto_20160202_1945.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0015_change_client_code.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0015_change_client_code.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0011_client_client_type.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0011_client_client_type.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0017_auto_20160811_1954.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0017_auto_20160811_1954.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0013_auto_20160407_1912.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0013_auto_20160407_1912.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0020_client__post_logout_redirect_uris.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0020_client__post_logout_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0025_user_field_codetoken.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0025_user_field_codetoken.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0023_client_owner.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0023_client_owner.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0018_hybridflow_and_clientattrs.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0018_hybridflow_and_clientattrs.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0001_initial.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0014_client_jwt_alg.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0014_client_jwt_alg.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0002_userconsent.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0002_userconsent.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0022_auto_20170331_1626.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0022_auto_20170331_1626.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0026_client_multiple_response_types.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0026_client_multiple_response_types.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0021_refresh_token_not_unique.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0021_refresh_token_not_unique.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0024_auto_20180327_1959.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0024_auto_20180327_1959.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/migrations/0008_rsakey.py` & `django-oidc-provider-0.8.0/oidc_provider/migrations/0008_rsakey.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/views.py` & `django-oidc-provider-0.8.0/oidc_provider/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             uri = error.create_uri(
                 authorize.params['redirect_uri'],
                 authorize.params['state'])
 
             return redirect(uri)
 
     def post(self, request, *args, **kwargs):
-        authorize = AuthorizeEndpoint(request)
+        authorize = self.authorize_endpoint_class(request)
 
         try:
             authorize.validate_params()
 
             if not request.POST.get('allow'):
                 signals.user_decline_consent.send(
                     self.__class__, user=request.user,
@@ -199,28 +199,30 @@
                 authorize.params['redirect_uri'],
                 authorize.params['state'])
 
             return redirect(uri)
 
 
 class TokenView(View):
+    token_endpoint_class = TokenEndpoint
+
     def post(self, request, *args, **kwargs):
-        token = TokenEndpoint(request)
+        token = self.token_endpoint_class(request)
 
         try:
             token.validate_params()
 
             dic = token.create_response_dic()
 
-            return TokenEndpoint.response(dic)
+            return self.token_endpoint_class.response(dic)
 
         except TokenError as error:
-            return TokenEndpoint.response(error.create_dict(), status=400)
+            return self.token_endpoint_class.response(error.create_dict(), status=400)
         except UserAuthError as error:
-            return TokenEndpoint.response(error.create_dict(), status=403)
+            return self.token_endpoint_class.response(error.create_dict(), status=403)
 
 
 @require_http_methods(['GET', 'POST', 'OPTIONS'])
 @protected_resource_view(['openid'])
 def userinfo(request, *args, **kwargs):
     """
     Create a dictionary with all the requested claims about the End-User.
@@ -358,20 +360,22 @@
         return super(CheckSessionIframeView, self).dispatch(request, *args, **kwargs)
 
     def get(self, request, *args, **kwargs):
         return render(request, 'oidc_provider/check_session_iframe.html', kwargs)
 
 
 class TokenIntrospectionView(View):
+    token_instrospection_endpoint_class = TokenIntrospectionEndpoint
+
     @method_decorator(csrf_exempt)
     def dispatch(self, request, *args, **kwargs):
         return super(TokenIntrospectionView, self).dispatch(request, *args, **kwargs)
 
     def post(self, request, *args, **kwargs):
-        introspection = TokenIntrospectionEndpoint(request)
+        introspection = self.token_instrospection_endpoint_class(request)
 
         try:
             introspection.validate_params()
             dic = introspection.create_response_dic()
-            return TokenIntrospectionEndpoint.response(dic)
+            return self.token_instrospection_endpoint_class.response(dic)
         except TokenIntrospectionError:
-            return TokenIntrospectionEndpoint.response({'active': False})
+            return self.token_instrospection_endpoint_class.response({'active': False})
```

### Comparing `django-oidc-provider-0.7.0/oidc_provider/lib/claims.py` & `django-oidc-provider-0.8.0/oidc_provider/lib/claims.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from oidc_provider import settings
 
 
 STANDARD_CLAIMS = {
     'name': '',
     'given_name': '',
```

### Comparing `django-oidc-provider-0.7.0/oidc_provider/lib/utils/authorize.py` & `django-oidc-provider-0.8.0/oidc_provider/lib/utils/authorize.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/lib/utils/oauth2.py` & `django-oidc-provider-0.8.0/oidc_provider/lib/utils/oauth2.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     Or try getting via GET.
     See: http://tools.ietf.org/html/rfc6750#section-2.1
 
     Return a string.
     """
     auth_header = request.META.get('HTTP_AUTHORIZATION', '')
 
-    if re.compile('^[Bb]earer\s{1}.+$').match(auth_header):
+    if re.compile(r'^[Bb]earer\s{1}.+$').match(auth_header):
         access_token = auth_header.split()[1]
     else:
         access_token = request.GET.get('access_token', '')
 
     return access_token
 
 
@@ -35,15 +35,15 @@
     Or try getting parameters via POST.
     See: http://tools.ietf.org/html/rfc6750#section-2.1
 
     Return a tuple `(client_id, client_secret)`.
     """
     auth_header = request.META.get('HTTP_AUTHORIZATION', '')
 
-    if re.compile('^Basic\s{1}.+$').match(auth_header):
+    if re.compile(r'^Basic\s{1}.+$').match(auth_header):
         b64_user_pass = auth_header.split()[1]
         try:
             user_pass = b64decode(b64_user_pass).decode('utf-8').split(':')
             client_id, client_secret = tuple(user_pass)
         except Exception:
             client_id = client_secret = ''
     else:
```

### Comparing `django-oidc-provider-0.7.0/oidc_provider/lib/utils/token.py` & `django-oidc-provider-0.8.0/oidc_provider/lib/utils/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,19 +51,20 @@
         dic['nonce'] = str(nonce)
 
     if at_hash:
         dic['at_hash'] = at_hash
 
     # Inlude (or not) user standard claims in the id_token.
     if settings.get('OIDC_IDTOKEN_INCLUDE_CLAIMS'):
-        standard_claims = StandardScopeClaims(token)
-        dic.update(standard_claims.create_response_dic())
         if settings.get('OIDC_EXTRA_SCOPE_CLAIMS'):
             custom_claims = settings.get('OIDC_EXTRA_SCOPE_CLAIMS', import_str=True)(token)
-            dic.update(custom_claims.create_response_dic())
+            claims = custom_claims.create_response_dic()
+        else:
+            claims = StandardScopeClaims(token).create_response_dic()
+        dic.update(claims)
 
     dic = run_processing_hook(
         dic, 'OIDC_IDTOKEN_PROCESSING_HOOK',
         user=user, token=token, request=request)
 
     return dic
```

### Comparing `django-oidc-provider-0.7.0/oidc_provider/lib/utils/common.py` & `django-oidc-provider-0.8.0/oidc_provider/lib/utils/common.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/lib/endpoints/authorize.py` & `django-oidc-provider-0.8.0/oidc_provider/lib/endpoints/authorize.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/lib/endpoints/introspection.py` & `django-oidc-provider-0.8.0/oidc_provider/lib/endpoints/introspection.py`

 * *Files 15% similar despite different names*

```diff
@@ -81,15 +81,16 @@
     def create_response_dic(self):
         response_dic = {}
         if self.id_token:
             for k in ('aud', 'sub', 'exp', 'iat', 'iss'):
                 response_dic[k] = self.id_token[k]
         response_dic['active'] = True
         response_dic['client_id'] = self.token.client.client_id
-
+        if settings.get('OIDC_INTROSPECTION_RESPONSE_SCOPE_ENABLE'):
+            response_dic['scope'] = ' '.join(self.token.scope)
         response_dic = run_processing_hook(response_dic,
                                            'OIDC_INTROSPECTION_PROCESSING_HOOK',
                                            client=self.client,
                                            id_token=self.id_token)
 
         return response_dic
```

### Comparing `django-oidc-provider-0.7.0/oidc_provider/lib/endpoints/token.py` & `django-oidc-provider-0.8.0/oidc_provider/lib/endpoints/token.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import inspect
-from base64 import urlsafe_b64encode
 import hashlib
+import inspect
 import logging
-from django.contrib.auth import authenticate
+from base64 import urlsafe_b64encode
 
+from django.contrib.auth import authenticate
 from django.http import JsonResponse
 
+from oidc_provider import settings
 from oidc_provider.lib.errors import (
     TokenError,
     UserAuthError,
 )
 from oidc_provider.lib.utils.oauth2 import extract_client_auth
 from oidc_provider.lib.utils.token import (
     create_id_token,
@@ -17,15 +18,14 @@
     encode_id_token,
 )
 from oidc_provider.models import (
     Client,
     Code,
     Token,
 )
-from oidc_provider import settings
 
 logger = logging.getLogger(__name__)
 
 
 class TokenEndpoint(object):
 
     def __init__(self, request):
@@ -72,24 +72,24 @@
             try:
                 self.code = Code.objects.get(code=self.params['code'])
             except Code.DoesNotExist:
                 logger.debug('[Token] Code does not exist: %s', self.params['code'])
                 raise TokenError('invalid_grant')
 
             if not (self.code.client == self.client) \
-               or self.code.has_expired():
+                    or self.code.has_expired():
                 logger.debug('[Token] Invalid code: invalid client or code has expired')
                 raise TokenError('invalid_grant')
 
             # Validate PKCE parameters.
             if self.params['code_verifier']:
                 if self.code.code_challenge_method == 'S256':
                     new_code_challenge = urlsafe_b64encode(
-                            hashlib.sha256(self.params['code_verifier'].encode('ascii')).digest()
-                        ).decode('utf-8').replace('=', '')
+                        hashlib.sha256(self.params['code_verifier'].encode('ascii')).digest()
+                    ).decode('utf-8').replace('=', '')
                 else:
                     new_code_challenge = self.params['code_verifier']
 
                 # TODO: We should explain the error.
                 if not (new_code_challenge == self.code.code_challenge):
                     raise TokenError('invalid_grant')
 
@@ -131,14 +131,35 @@
             if not self.client._scope:
                 logger.debug('[Token] Client using client credentials with empty scope')
                 raise TokenError('invalid_scope')
         else:
             logger.debug('[Token] Invalid grant type: %s', self.params['grant_type'])
             raise TokenError('unsupported_grant_type')
 
+    def validate_requested_scopes(self):
+        """
+        Handling validation of requested scope for grant_type=[password|client_credentials]
+        """
+        token_scopes = []
+        if self.params['scope']:
+            # See https://tools.ietf.org/html/rfc6749#section-3.3
+            # The value of the scope parameter is expressed
+            # as a list of space-delimited, case-sensitive strings
+            for scope_requested in self.params['scope'].split(' '):
+                if scope_requested in self.client.scope:
+                    token_scopes.append(scope_requested)
+                else:
+                    logger.debug('[Token] The request scope %s is not supported by client %s',
+                                 scope_requested, self.client.client_id)
+                    raise TokenError('invalid_scope')
+        # if no scopes requested assign client's scopes
+        else:
+            token_scopes.extend(self.client.scope)
+        return token_scopes
+
     def create_response_dic(self):
         if self.params['grant_type'] == 'authorization_code':
             return self.create_code_response_dic()
         elif self.params['grant_type'] == 'refresh_token':
             return self.create_refresh_response_dic()
         elif self.params['grant_type'] == 'password':
             return self.create_access_token_response_dic()
@@ -226,19 +247,19 @@
             'id_token': encode_id_token(id_token_dic, self.token.client),
         }
 
         return dic
 
     def create_access_token_response_dic(self):
         # See https://tools.ietf.org/html/rfc6749#section-4.3
-
+        token_scopes = self.validate_requested_scopes()
         token = create_token(
             self.user,
             self.client,
-            self.params['scope'].split(' '))
+            token_scopes)
 
         id_token_dic = create_id_token(
             token=token,
             user=self.user,
             aud=self.client.client_id,
             nonce='self.code.nonce',
             at_hash=token.at_hash,
@@ -251,31 +272,33 @@
 
         return {
             'access_token': token.access_token,
             'refresh_token': token.refresh_token,
             'expires_in': settings.get('OIDC_TOKEN_EXPIRE'),
             'token_type': 'bearer',
             'id_token': encode_id_token(id_token_dic, token.client),
+            'scope': ' '.join(token.scope)
         }
 
     def create_client_credentials_response_dic(self):
         # See https://tools.ietf.org/html/rfc6749#section-4.4.3
+        token_scopes = self.validate_requested_scopes()
 
         token = create_token(
             user=None,
             client=self.client,
-            scope=self.client.scope)
+            scope=token_scopes)
 
         token.save()
 
         return {
             'access_token': token.access_token,
             'expires_in': settings.get('OIDC_TOKEN_EXPIRE'),
             'token_type': 'bearer',
-            'scope': self.client._scope,
+            'scope': ' '.join(token.scope),
         }
 
     @classmethod
     def response(cls, dic, status=200):
         """
         Create and return a response object.
         """
```

### Comparing `django-oidc-provider-0.7.0/oidc_provider/lib/errors.py` & `django-oidc-provider-0.8.0/oidc_provider/lib/errors.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/management/commands/creatersakey.py` & `django-oidc-provider-0.8.0/oidc_provider/management/commands/creatersakey.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/admin.py` & `django-oidc-provider-0.8.0/oidc_provider/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from hashlib import sha224
 from random import randint
 from uuid import uuid4
 
 from django.forms import ModelForm
 from django.contrib import admin
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from oidc_provider.models import Client, Code, Token, RSAKey
 
 
 class ClientForm(ModelForm):
 
     class Meta:
@@ -71,21 +71,25 @@
     search_fields = ['name']
     raw_id_fields = ['owner']
 
 
 @admin.register(Code)
 class CodeAdmin(admin.ModelAdmin):
 
+    raw_id_fields = ['user']
+
     def has_add_permission(self, request):
         return False
 
 
 @admin.register(Token)
 class TokenAdmin(admin.ModelAdmin):
 
+    raw_id_fields = ['user']
+
     def has_add_permission(self, request):
         return False
 
 
 @admin.register(RSAKey)
 class RSAKeyAdmin(admin.ModelAdmin):
```

### Comparing `django-oidc-provider-0.7.0/oidc_provider/tests/app/utils.py` & `django-oidc-provider-0.8.0/oidc_provider/tests/app/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     if is_public:
         client.client_type = 'public'
         client.client_secret = ''
     else:
         client.client_secret = str(random.randint(1, 999999)).zfill(6)
     client.redirect_uris = ['http://example.com/']
     client.require_consent = require_consent
-
+    client.scope = ['openid', 'email']
     client.save()
 
     # check if response_type is a string in a python 2 and 3 compatible way
     if isinstance(response_type, ("".__class__, u"".__class__)):
         response_type = (response_type,)
     for value in response_type:
         client.response_types.add(ResponseType.objects.get(value=value))
```

### Comparing `django-oidc-provider-0.7.0/oidc_provider/tests/settings.py` & `django-oidc-provider-0.8.0/oidc_provider/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/settings.py` & `django-oidc-provider-0.8.0/oidc_provider/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,21 @@
     @property
     def OIDC_TEMPLATES(self):
         return {
             'authorize': 'oidc_provider/authorize.html',
             'error': 'oidc_provider/error.html'
         }
 
+    @property
+    def OIDC_INTROSPECTION_RESPONSE_SCOPE_ENABLE(self):
+        """
+        OPTIONAL: A boolean to specify whether or not to include scope in introspection response.
+        """
+        return False
+
 
 default_settings = DefaultSettings()
 
 
 def import_from_str(value):
     """
     Attempt to import a class from a string representation.
```

### Comparing `django-oidc-provider-0.7.0/oidc_provider/locale/pl/LC_MESSAGES/django.po` & `django-oidc-provider-0.8.0/oidc_provider/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/locale/pl/LC_MESSAGES/django.mo` & `django-oidc-provider-0.8.0/oidc_provider/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/locale/fr/LC_MESSAGES/django.po` & `django-oidc-provider-0.8.0/oidc_provider/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/locale/fr/LC_MESSAGES/django.mo` & `django-oidc-provider-0.8.0/oidc_provider/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/locale/es/LC_MESSAGES/django.po` & `django-oidc-provider-0.8.0/oidc_provider/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/templates/oidc_provider/hidden_inputs.html` & `django-oidc-provider-0.8.0/oidc_provider/templates/oidc_provider/hidden_inputs.html`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/templates/oidc_provider/authorize.html` & `django-oidc-provider-0.8.0/oidc_provider/templates/oidc_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/oidc_provider/templates/oidc_provider/check_session_iframe.html` & `django-oidc-provider-0.8.0/oidc_provider/templates/oidc_provider/check_session_iframe.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% load staticfiles %}
+{% load static %}
 
 <html lang="en">
     <head>
         <meta charset="utf-8">
         <title>OP Iframe</title>
         <script src="{% static 'oidc_provider/js/sha256.min.js' %}"></script>
         <script language="JavaScript" type="text/javascript">
```

#### html2text {}

```diff
@@ -1,2 +1,2 @@
-{% load staticfiles %}
+{% load static %}
 OpenID Connect Session Management OP Iframe.
```

### Comparing `django-oidc-provider-0.7.0/django_oidc_provider.egg-info/SOURCES.txt` & `django-oidc-provider-0.8.0/django_oidc_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-oidc-provider-0.7.0/django_oidc_provider.egg-info/PKG-INFO` & `django-oidc-provider-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-oidc-provider
-Version: 0.7.0
+Version: 0.8.0
 Summary: OpenID Connect Provider implementation for Django.
 Home-page: http://github.com/juanifioren/django-oidc-provider
 Author: Juan Ignacio Fiorentino
 Author-email: juanifioren@gmail.com
 License: MIT License
-Description: http://github.com/juanifioren/django-oidc-provider
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE
+
+http://github.com/juanifioren/django-oidc-provider
```

### Comparing `django-oidc-provider-0.7.0/setup.py` & `django-oidc-provider-0.8.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,19 +27,19 @@
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
     test_suite='runtests.runtests',
     tests_require=[
         'pyjwkest>=1.3.0',
         'mock>=2.0.0',
```

### Comparing `django-oidc-provider-0.7.0/README.md` & `django-oidc-provider-0.8.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Django OpenID Connect Provider
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/django-oidc-provider.svg)](https://pypi.python.org/pypi/django-oidc-provider)
 [![PyPI Versions](https://img.shields.io/pypi/v/django-oidc-provider.svg)](https://pypi.python.org/pypi/django-oidc-provider)
 [![Documentation Status](https://readthedocs.org/projects/django-oidc-provider/badge/?version=master)](http://django-oidc-provider.readthedocs.io/)
-[![Travis](https://travis-ci.org/juanifioren/django-oidc-provider.svg?branch=master)](https://travis-ci.org/juanifioren/django-oidc-provider)
 
 ## About OpenID
 
 OpenID Connect is a simple identity layer on top of the OAuth 2.0 protocol, which allows computing clients to verify the identity of an end-user based on the authentication performed by an authorization server, as well as to obtain basic profile information about the end-user in an interoperable and REST-like manner. Like [Google](https://developers.google.com/identity/protocols/OpenIDConnect) for example.
 
 ## About the package
```

### Comparing `django-oidc-provider-0.7.0/PKG-INFO` & `django-oidc-provider-0.8.0/django_oidc_provider.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-oidc-provider
-Version: 0.7.0
+Version: 0.8.0
 Summary: OpenID Connect Provider implementation for Django.
 Home-page: http://github.com/juanifioren/django-oidc-provider
 Author: Juan Ignacio Fiorentino
 Author-email: juanifioren@gmail.com
 License: MIT License
-Description: http://github.com/juanifioren/django-oidc-provider
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE
+
+http://github.com/juanifioren/django-oidc-provider
```

