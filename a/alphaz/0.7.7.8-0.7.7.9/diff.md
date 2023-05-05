# Comparing `tmp/alphaz-0.7.7.8.tar.gz` & `tmp/alphaz-0.7.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alphaz-0.7.7.8.tar", last modified: Thu May  4 16:17:49 2023, max compression
+gzip compressed data, was "dist/alphaz-0.7.7.9.tar", last modified: Fri May  5 17:01:32 2023, max compression
```

## Comparing `alphaz-0.7.7.8.tar` & `alphaz-0.7.7.9.tar`

### file list

```diff
@@ -1,398 +1,398 @@
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.651455 alphaz-0.7.7.8/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1085 2019-07-02 13:36:12.000000 alphaz-0.7.7.8/LICENSE
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11211 2023-05-04 16:17:47.000000 alphaz-0.7.7.8/MANIFEST.in
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      600 2023-05-04 16:17:49.651455 alphaz-0.7.7.8/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.7.8/README.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.587455 alphaz-0.7.7.8/alphaz/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        9 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/README.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      498 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/alphaz.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/alphaz.code-workspace
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/alphaz.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/api.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      713 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/api.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/api.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.591455 alphaz-0.7.7.8/alphaz/apis/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/log.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/mails.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.591455 alphaz-0.7.7.8/alphaz/apis/routes/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1601 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/admin.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3039 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/basic_tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3253 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/git.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7272 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/logs.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/mails.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6384 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1548 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.591455 alphaz-0.7.7.8/alphaz/apis/routes/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2479 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/user_management/application_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2243 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/user_management/permission_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4104 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/user_management/role_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/user_management/user_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3493 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/routes/users.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.591455 alphaz-0.7.7.8/alphaz/apis/users/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/users/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/users/ldap.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11859 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/apis/users/users.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.591455 alphaz-0.7.7.8/alphaz/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/config/config.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/config/config.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/config/main_configuration.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/config/page.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/config/source.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/core.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.595455 alphaz-0.7.7.8/alphaz/documentations/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.595455 alphaz-0.7.7.8/alphaz/documentations/docs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/alpha_admin.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1408 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/alpha_core.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/alpha_screens.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2222 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/alpha_setup.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.595455 alphaz-0.7.7.8/alphaz/documentations/docs/api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1527 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/api/authorizations.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/api/cache.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2931 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/api/configuration.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       24 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/api/issues.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      705 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/api/main.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      559 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/api/methods.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1728 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/api/parameters.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1197 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/api/routes.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      486 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/api/sqlalchemy.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1129 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/api_database.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/configuration.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.595455 alphaz-0.7.7.8/alphaz/documentations/docs/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2187 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/database/init.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      442 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/database/instantiate.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      113 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/database/main.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1806 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/database/model.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      373 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/database/relations.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/database/schema.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      615 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/database/update.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/documentation.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3526 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/docs/index.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1090 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/documentations/mkdocs.yml
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13156 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/404.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/alpha_admin/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14222 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/alpha_admin/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/alpha_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22752 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/alpha_core/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/alpha_screens/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21873 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/alpha_screens/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/alpha_setup/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24071 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/alpha_setup/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.579455 alphaz-0.7.7.8/alphaz/documentations/site/api/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/api/authorizations/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17905 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/api/authorizations/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/api/cache/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14918 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/api/cache/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/api/configuration/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    27645 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/api/configuration/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/api/issues/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    16365 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/api/issues/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/api/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17987 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/api/main/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/api/methods/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17722 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/api/methods/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/api/parameters/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20075 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/api/parameters/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/api/routes/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    19333 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/api/routes/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/api/sqlalchemy/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17109 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/api/sqlalchemy/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/api_database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22959 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/api_database/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.579455 alphaz-0.7.7.8/alphaz/documentations/site/assets/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/assets/images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/images/favicon.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.599455 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.603455 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.603455 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/workers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.607455 alphaz-0.7.7.8/alphaz/documentations/site/assets/stylesheets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.607455 alphaz-0.7.7.8/alphaz/documentations/site/configuration/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    28465 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/configuration/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.583455 alphaz-0.7.7.8/alphaz/documentations/site/database/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.607455 alphaz-0.7.7.8/alphaz/documentations/site/database/init/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23029 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/database/init/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.607455 alphaz-0.7.7.8/alphaz/documentations/site/database/instantiate/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17445 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/database/instantiate/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.607455 alphaz-0.7.7.8/alphaz/documentations/site/database/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14939 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/database/main/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.607455 alphaz-0.7.7.8/alphaz/documentations/site/database/model/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24758 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/database/model/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.607455 alphaz-0.7.7.8/alphaz/documentations/site/database/relations/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    16511 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/database/relations/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.607455 alphaz-0.7.7.8/alphaz/documentations/site/database/schema/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18704 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/database/schema/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.607455 alphaz-0.7.7.8/alphaz/documentations/site/database/update/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20308 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/database/update/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.607455 alphaz-0.7.7.8/alphaz/documentations/site/documentation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17065 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/documentation/index.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    29467 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.607455 alphaz-0.7.7.8/alphaz/documentations/site/search/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    54135 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/search/search_index.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2809 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/sitemap.xml
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      209 2023-04-27 20:33:29.000000 alphaz-0.7.7.8/alphaz/documentations/site/sitemap.xml.gz
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/git.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/help.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.611455 alphaz-0.7.7.8/alphaz/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/libs/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5807 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/api_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/libs/barcode_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13989 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/config_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/converter_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9474 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/database_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/date_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6381 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/dict_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.611455 alphaz-0.7.7.8/alphaz/libs/emulation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/emulation/vt102_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/libs/events.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/files_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1184 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/flask_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/libs/ftp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/img_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6207 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/io_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3233 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/json_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1151 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/logs_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13008 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/mail_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/libs/nav_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/notifications_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/libs/number_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/libs/os_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/libs/process_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14220 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/py_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      886 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/scp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/search_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6362 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/secure_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2929 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/soap_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/libs/sql_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18623 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/ssh_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9896 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/string_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5556 2023-05-04 16:17:45.000000 alphaz-0.7.7.8/alphaz/libs/test_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/libs/time_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4492 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/libs/transactions_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6565 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/libs/user_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.611455 alphaz-0.7.7.8/alphaz/libs/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/libs/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1336 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/libs/user_management/application_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1597 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/libs/user_management/permission_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3376 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/libs/user_management/role_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/libs/user_management/user_management_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.615455 alphaz-0.7.7.8/alphaz/mails/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.615455 alphaz-0.7.7.8/alphaz/mails/Images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/mails/Images/Background.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/mails/Images/Facebook_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/mails/Images/Twitter_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/mails/Images/Web_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/mails/Images/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/mails/Mail.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/mails/Webmail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/mails/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/mails/debug.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/mails/mail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/mails/password_reset.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/mails/stay_in_touch.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/mails/template.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.615455 alphaz-0.7.7.8/alphaz/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      107 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.619455 alphaz-0.7.7.8/alphaz/models/api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/api/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      926 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/api/_answer.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/api/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/api/_methods.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14340 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/api/_parameter.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14445 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/api/_reloader.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3717 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/api/_reloaders.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2402 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/api/_requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18840 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/api/_route.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20460 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/api/_structures.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/api/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.619455 alphaz-0.7.7.8/alphaz/models/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/models/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    26517 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/config/_config.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12350 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/config/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.619455 alphaz-0.7.7.8/alphaz/models/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/database/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/database/main_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9992 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/database/models.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/database/operators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/database/requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/models/database/row.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    56021 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/database/structure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/database/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4797 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/database/users_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9301 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/database/utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/database/views.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/models/excel.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6683 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/ftp.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/img.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.619455 alphaz-0.7.7.8/alphaz/models/json/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/models/json/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/json/_converters.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.619455 alphaz-0.7.7.8/alphaz/models/logger/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/logger/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/logger/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14322 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/logger/_logger.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/models/logger/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.623455 alphaz-0.7.7.8/alphaz/models/logs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.7.8/alphaz/models/logs/main.log
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.7.8/alphaz/models/logs/main.log.2021-11-07
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.623455 alphaz-0.7.7.8/alphaz/models/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      354 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/main/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    31214 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/main/_base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.623455 alphaz-0.7.7.8/alphaz/models/main/_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/models/main/_core/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    16001 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/main/_core/_core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/models/main/_core/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      335 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/main/_enum.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2001 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/main/_exception.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/models/main/_file.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/models/main/_process.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/models/main/_request.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/models/main/_singleton.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2218 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/request.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.623455 alphaz-0.7.7.8/alphaz/models/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      167 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8070 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/tests/_category.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3446 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/tests/_group.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      163 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/tests/_levels.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4125 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/tests/_method.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4578 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/tests/_save.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14950 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/tests/_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7505 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/tests/_wrappers.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2910 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/models/user.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/models/watcher.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.623455 alphaz-0.7.7.8/alphaz/pocs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/pocs/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/reload_gitignore.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/req.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/requirements.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/run.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.623455 alphaz-0.7.7.8/alphaz/src/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/src/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/src/alpha.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.623455 alphaz-0.7.7.8/alphaz/src/configs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/src/configs/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/src/configs/loggers.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/src/configs/loggers_colors.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.623455 alphaz-0.7.7.8/alphaz/src/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/src/database/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.623455 alphaz-0.7.7.8/alphaz/stitch/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/stitch/Core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/stitch/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.627455 alphaz-0.7.7.8/alphaz/stitch/imports/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/stitch/imports/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.627455 alphaz-0.7.7.8/alphaz/stitch/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/stitch/models/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/stitch/models/element.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/stitch/run.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/stitch/stitch.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.635455 alphaz-0.7.7.8/alphaz/stitch/web-drivers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/stitch/web-drivers/chromedriver.exe
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/stitch/web-drivers/geckodriver
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.583455 alphaz-0.7.7.8/alphaz/stitch/websites/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.643455 alphaz-0.7.7.8/alphaz/stitch/websites/Test/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/stitch/websites/Test/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.643455 alphaz-0.7.7.8/alphaz/stitch/websites/stiki/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/stitch/websites/stiki/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.643455 alphaz-0.7.7.8/alphaz/templates/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.643455 alphaz-0.7.7.8/alphaz/templates/assets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/assets/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.643455 alphaz-0.7.7.8/alphaz/templates/assets/css/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/assets/css/home.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/assets/css/logs.css
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.643455 alphaz-0.7.7.8/alphaz/templates/assets/images/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.647455 alphaz-0.7.7.8/alphaz/templates/assets/images/icons/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/assets/images/icons/admin.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/assets/images/icons/alpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/assets/images/icons/save.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/assets/images/icons/start-icon.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/assets/images/icons/user.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/assets/images/icons/wsalpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/assets/images/loading.gif
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.647455 alphaz-0.7.7.8/alphaz/templates/assets/js/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.647455 alphaz-0.7.7.8/alphaz/templates/assets/js/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/assets/js/libs/ansi_up.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/assets/js/libs/jquery.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/assets/js/logs.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/templates/hello.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/home.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/templates/logs.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/test.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.647455 alphaz-0.7.7.8/alphaz/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14409 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/tests/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5646 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/tests/basic_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/tests/configurations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    25295 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/tests/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/tests/processes.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/tests/utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.647455 alphaz-0.7.7.8/alphaz/utils/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       57 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11705 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/api.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.647455 alphaz-0.7.7.8/alphaz/utils/apm/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/apm/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1671 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/apm/ora.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/clean.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/configuration.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.651455 alphaz-0.7.7.8/alphaz/utils/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11444 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/database/init.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/database_to_dataclass.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/decorators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.7.8/alphaz/utils/ensure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1801 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/init_database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/mep.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/screens.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23624 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/selectionMenu.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/tasks.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/time.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3849 2023-05-04 16:17:46.000000 alphaz-0.7.7.8/alphaz/utils/transactions.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:49.587455 alphaz-0.7.7.8/alphaz.egg-info/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      600 2023-05-04 16:17:48.000000 alphaz-0.7.7.8/alphaz.egg-info/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11373 2023-05-04 16:17:49.000000 alphaz-0.7.7.8/alphaz.egg-info/SOURCES.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-05-04 16:17:48.000000 alphaz-0.7.7.8/alphaz.egg-info/dependency_links.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      458 2023-05-04 16:17:49.000000 alphaz-0.7.7.8/alphaz.egg-info/requires.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-05-04 16:17:49.000000 alphaz-0.7.7.8/alphaz.egg-info/top_level.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-05-04 16:17:49.651455 alphaz-0.7.7.8/setup.cfg
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3094 2023-05-04 15:59:16.000000 alphaz-0.7.7.8/setup.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.250320 alphaz-0.7.7.9/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1085 2019-07-02 13:36:12.000000 alphaz-0.7.7.9/LICENSE
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11211 2023-05-05 17:01:30.000000 alphaz-0.7.7.9/MANIFEST.in
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      600 2023-05-05 17:01:32.250320 alphaz-0.7.7.9/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.7.9/README.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.190321 alphaz-0.7.7.9/alphaz/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        9 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/README.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      498 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/alphaz.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/alphaz.code-workspace
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/alphaz.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/api.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      713 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/api.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/api.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.194321 alphaz-0.7.7.9/alphaz/apis/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/log.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/mails.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.194321 alphaz-0.7.7.9/alphaz/apis/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1601 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/admin.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3039 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/basic_tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3253 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/git.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7272 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/logs.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/mails.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6384 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1594 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/apis/routes/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.194321 alphaz-0.7.7.9/alphaz/apis/routes/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2479 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/user_management/application_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2243 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/user_management/permission_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4104 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/user_management/role_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/user_management/user_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3493 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/users.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.194321 alphaz-0.7.7.9/alphaz/apis/users/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/users/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/users/ldap.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11859 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/users/users.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.194321 alphaz-0.7.7.9/alphaz/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/config/config.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/config/config.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/config/main_configuration.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/config/page.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/config/source.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/core.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.194321 alphaz-0.7.7.9/alphaz/documentations/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.198320 alphaz-0.7.7.9/alphaz/documentations/docs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/alpha_admin.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1408 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/alpha_core.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/alpha_screens.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2222 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/alpha_setup.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.198320 alphaz-0.7.7.9/alphaz/documentations/docs/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1527 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/authorizations.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/cache.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2931 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/configuration.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       24 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/issues.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      705 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/main.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      559 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/methods.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1728 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/parameters.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1197 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/routes.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      486 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/sqlalchemy.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1129 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api_database.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/configuration.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.198320 alphaz-0.7.7.9/alphaz/documentations/docs/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2187 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/database/init.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      442 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/database/instantiate.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      113 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/database/main.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1806 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/database/model.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      373 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/database/relations.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/database/schema.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      615 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/database/update.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/documentation.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3526 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/index.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1090 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/mkdocs.yml
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.198320 alphaz-0.7.7.9/alphaz/documentations/site/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13156 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/404.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.198320 alphaz-0.7.7.9/alphaz/documentations/site/alpha_admin/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14222 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/alpha_admin/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.198320 alphaz-0.7.7.9/alphaz/documentations/site/alpha_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22752 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/alpha_core/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/alpha_screens/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21873 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/alpha_screens/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/alpha_setup/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24071 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/alpha_setup/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.186320 alphaz-0.7.7.9/alphaz/documentations/site/api/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/authorizations/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17905 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/authorizations/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/cache/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14918 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/cache/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    27645 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/issues/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16365 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/issues/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17987 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/main/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/methods/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17722 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/methods/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/parameters/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20075 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/parameters/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19333 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/routes/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/sqlalchemy/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17109 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/sqlalchemy/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api_database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22959 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api_database/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.186320 alphaz-0.7.7.9/alphaz/documentations/site/assets/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/assets/images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/images/favicon.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.206320 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.206320 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/workers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.206320 alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.206320 alphaz-0.7.7.9/alphaz/documentations/site/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    28465 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.186320 alphaz-0.7.7.9/alphaz/documentations/site/database/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.206320 alphaz-0.7.7.9/alphaz/documentations/site/database/init/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23029 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/database/init/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.206320 alphaz-0.7.7.9/alphaz/documentations/site/database/instantiate/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17445 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/database/instantiate/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.206320 alphaz-0.7.7.9/alphaz/documentations/site/database/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14939 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/database/main/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.210320 alphaz-0.7.7.9/alphaz/documentations/site/database/model/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24758 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/database/model/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.210320 alphaz-0.7.7.9/alphaz/documentations/site/database/relations/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16511 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/database/relations/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.210320 alphaz-0.7.7.9/alphaz/documentations/site/database/schema/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18704 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/database/schema/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.210320 alphaz-0.7.7.9/alphaz/documentations/site/database/update/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20308 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/database/update/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.210320 alphaz-0.7.7.9/alphaz/documentations/site/documentation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17065 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/documentation/index.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    29467 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.210320 alphaz-0.7.7.9/alphaz/documentations/site/search/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    54135 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/search/search_index.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2809 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/sitemap.xml
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      209 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/sitemap.xml.gz
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/git.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/help.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.214321 alphaz-0.7.7.9/alphaz/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5807 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/api_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/barcode_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13989 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/config_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/converter_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9474 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/database_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/date_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6381 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/dict_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.214321 alphaz-0.7.7.9/alphaz/libs/emulation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/emulation/vt102_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/events.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/files_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1184 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/flask_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/ftp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/img_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6207 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/io_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3783 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/libs/json_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1151 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/logs_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13008 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/mail_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/nav_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/notifications_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/number_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/os_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/process_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14220 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/py_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      886 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/scp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/search_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6362 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/secure_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2929 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/soap_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/sql_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18623 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/ssh_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9896 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/string_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5691 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/libs/test_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/time_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4492 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/transactions_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6565 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/user_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.214321 alphaz-0.7.7.9/alphaz/libs/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1336 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/user_management/application_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1597 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/user_management/permission_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3376 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/user_management/role_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/user_management/user_management_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.214321 alphaz-0.7.7.9/alphaz/mails/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.218320 alphaz-0.7.7.9/alphaz/mails/Images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/mails/Images/Background.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/mails/Images/Facebook_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/mails/Images/Twitter_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/mails/Images/Web_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/mails/Images/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/mails/Mail.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/mails/Webmail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/mails/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/mails/debug.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/mails/mail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/mails/password_reset.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/mails/stay_in_touch.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/mails/template.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.218320 alphaz-0.7.7.9/alphaz/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      107 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.218320 alphaz-0.7.7.9/alphaz/models/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      926 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_answer.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_methods.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14340 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_parameter.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14445 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_reloader.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3717 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_reloaders.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2402 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20365 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/models/api/_route.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20460 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_structures.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.218320 alphaz-0.7.7.9/alphaz/models/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    26517 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/config/_config.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12350 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/config/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.222320 alphaz-0.7.7.9/alphaz/models/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/main_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9992 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/models.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/operators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/database/row.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    56078 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/models/database/structure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4797 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/users_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9301 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/views.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/excel.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6683 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/ftp.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/img.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.222320 alphaz-0.7.7.9/alphaz/models/json/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/json/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/json/_converters.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.222320 alphaz-0.7.7.9/alphaz/models/logger/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/logger/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/logger/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14322 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/logger/_logger.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/logger/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.222320 alphaz-0.7.7.9/alphaz/models/logs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.7.9/alphaz/models/logs/main.log
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.7.9/alphaz/models/logs/main.log.2021-11-07
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.222320 alphaz-0.7.7.9/alphaz/models/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      354 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/main/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    31204 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/models/main/_base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/models/main/_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/main/_core/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16001 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/main/_core/_core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/main/_core/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      335 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/main/_enum.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2001 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/main/_exception.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/main/_file.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/main/_process.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/main/_request.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/main/_singleton.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2218 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/request.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/models/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      167 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8399 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/models/tests/_category.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3670 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/models/tests/_group.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      163 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/tests/_levels.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4224 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/models/tests/_method.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4578 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/tests/_save.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14974 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/models/tests/_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7505 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/tests/_wrappers.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2910 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/user.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/watcher.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/pocs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/pocs/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/reload_gitignore.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/req.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/requirements.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/run.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/src/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/src/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/src/alpha.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/src/configs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/src/configs/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/src/configs/loggers.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/src/configs/loggers_colors.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/src/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/src/database/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/stitch/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/Core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/stitch/imports/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/imports/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/stitch/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/stitch/models/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/models/element.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/run.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/stitch.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.234320 alphaz-0.7.7.9/alphaz/stitch/web-drivers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/web-drivers/chromedriver.exe
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/stitch/web-drivers/geckodriver
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.186320 alphaz-0.7.7.9/alphaz/stitch/websites/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.242320 alphaz-0.7.7.9/alphaz/stitch/websites/Test/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/websites/Test/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.242320 alphaz-0.7.7.9/alphaz/stitch/websites/stiki/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/stitch/websites/stiki/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.242320 alphaz-0.7.7.9/alphaz/templates/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.242320 alphaz-0.7.7.9/alphaz/templates/assets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.246320 alphaz-0.7.7.9/alphaz/templates/assets/css/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/css/home.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/css/logs.css
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.246320 alphaz-0.7.7.9/alphaz/templates/assets/images/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.246320 alphaz-0.7.7.9/alphaz/templates/assets/images/icons/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/images/icons/admin.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/images/icons/alpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/images/icons/save.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/images/icons/start-icon.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/images/icons/user.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/images/icons/wsalpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/images/loading.gif
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.246320 alphaz-0.7.7.9/alphaz/templates/assets/js/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.246320 alphaz-0.7.7.9/alphaz/templates/assets/js/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/js/libs/ansi_up.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/js/libs/jquery.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/js/logs.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/templates/hello.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/home.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/logs.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/test.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.246320 alphaz-0.7.7.9/alphaz/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14409 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/tests/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5646 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/tests/basic_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/tests/configurations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    25295 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/tests/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/tests/processes.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/tests/utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.250320 alphaz-0.7.7.9/alphaz/utils/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       57 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11705 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/api.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.250320 alphaz-0.7.7.9/alphaz/utils/apm/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/apm/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1671 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/apm/ora.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/clean.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/configuration.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.250320 alphaz-0.7.7.9/alphaz/utils/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11444 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/database/init.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/database_to_dataclass.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/decorators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/utils/ensure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1801 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/init_database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/mep.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/screens.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23624 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/selectionMenu.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/tasks.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/time.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3849 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/transactions.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.194321 alphaz-0.7.7.9/alphaz.egg-info/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      600 2023-05-05 17:01:31.000000 alphaz-0.7.7.9/alphaz.egg-info/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11373 2023-05-05 17:01:32.000000 alphaz-0.7.7.9/alphaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-05-05 17:01:31.000000 alphaz-0.7.7.9/alphaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      458 2023-05-05 17:01:31.000000 alphaz-0.7.7.9/alphaz.egg-info/requires.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-05-05 17:01:31.000000 alphaz-0.7.7.9/alphaz.egg-info/top_level.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-05-05 17:01:32.250320 alphaz-0.7.7.9/setup.cfg
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3094 2023-05-05 17:00:51.000000 alphaz-0.7.7.9/setup.py
```

### Comparing `alphaz-0.7.7.8/LICENSE` & `alphaz-0.7.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/MANIFEST.in` & `alphaz-0.7.7.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/PKG-INFO` & `alphaz-0.7.7.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz
-Version: 0.7.7.8
+Version: 0.7.7.9
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.7.8.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.7.9.tar.gz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `alphaz-0.7.7.8/README.md` & `alphaz-0.7.7.9/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/api.json` & `alphaz-0.7.7.9/alphaz/api.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/api.py` & `alphaz-0.7.7.9/alphaz/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/mails.py` & `alphaz-0.7.7.9/alphaz/apis/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/routes/admin.py` & `alphaz-0.7.7.9/alphaz/apis/routes/admin.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/routes/api.py` & `alphaz-0.7.7.9/alphaz/apis/routes/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/routes/basic_tests.py` & `alphaz-0.7.7.9/alphaz/apis/routes/basic_tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/routes/database.py` & `alphaz-0.7.7.9/alphaz/apis/routes/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/routes/logs.py` & `alphaz-0.7.7.9/alphaz/apis/routes/logs.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/routes/mails.py` & `alphaz-0.7.7.9/alphaz/apis/routes/mails.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/routes/main.py` & `alphaz-0.7.7.9/alphaz/apis/routes/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/routes/tests.py` & `alphaz-0.7.7.9/alphaz/apis/routes/tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         Parameter("file_path", ptype=str),
         Parameter("coverage", ptype=str),
         Parameter("load_from_db", ptype=bool),
         Parameter("stop", ptype=bool),
         Parameter("report", ptype=str),
         Parameter("coverage", ptype=str),
         Parameter("levels", ptype=list[Levels], default=[]),
+        Parameter("failed_only", ptype=bool),
     ],
 )
 def get_tests():
     return test_lib.get_tests_auto(**API.gets())
 
 
 @route("/tests/coverage", parameters=[Parameter("file", required=True)])
```

### Comparing `alphaz-0.7.7.8/alphaz/apis/routes/user_management/application_management.py` & `alphaz-0.7.7.9/alphaz/apis/routes/user_management/application_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/routes/user_management/permission_management.py` & `alphaz-0.7.7.9/alphaz/apis/routes/user_management/permission_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/routes/user_management/role_management.py` & `alphaz-0.7.7.9/alphaz/apis/routes/user_management/role_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/routes/user_management/user_management.py` & `alphaz-0.7.7.9/alphaz/apis/routes/user_management/user_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/routes/users.py` & `alphaz-0.7.7.9/alphaz/apis/routes/users.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/tests.py` & `alphaz-0.7.7.9/alphaz/apis/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/users/ldap.py` & `alphaz-0.7.7.9/alphaz/apis/users/ldap.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/apis/users/users.py` & `alphaz-0.7.7.9/alphaz/apis/users/users.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/config/config.css` & `alphaz-0.7.7.9/alphaz/config/config.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/config/config.html` & `alphaz-0.7.7.9/alphaz/config/config.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/config/main_configuration.py` & `alphaz-0.7.7.9/alphaz/config/main_configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/config/page.py` & `alphaz-0.7.7.9/alphaz/config/page.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/config/source.html` & `alphaz-0.7.7.9/alphaz/config/source.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/config.json` & `alphaz-0.7.7.9/alphaz/config.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/alpha_core.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/alpha_core.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/alpha_screens.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/alpha_screens.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/alpha_setup.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/alpha_setup.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/api/authorizations.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/api/authorizations.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/api/configuration.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/api/configuration.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/api/main.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/api/main.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/api/methods.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/api/methods.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/api/parameters.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/api/parameters.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/api/routes.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/api/routes.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/api_database.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/api_database.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/configuration.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/database/init.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/database/init.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/database/model.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/database/model.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/database/schema.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/database/schema.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/database/update.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/database/update.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/docs/index.md` & `alphaz-0.7.7.9/alphaz/documentations/docs/index.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/mkdocs.yml` & `alphaz-0.7.7.9/alphaz/documentations/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/404.html` & `alphaz-0.7.7.9/alphaz/documentations/site/404.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/alpha_admin/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/alpha_admin/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/alpha_core/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/alpha_core/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/alpha_screens/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/alpha_screens/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/alpha_setup/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/alpha_setup/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/api/authorizations/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/api/authorizations/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/api/cache/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/api/cache/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/api/configuration/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/api/configuration/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/api/issues/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/api/issues/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/api/main/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/api/main/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/api/methods/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/api/methods/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/api/parameters/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/api/parameters/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/api/routes/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/api/routes/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/api/sqlalchemy/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/api/sqlalchemy/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/api_database/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/api_database/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/images/favicon.png` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map` & `alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/configuration/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/configuration/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/database/init/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/database/init/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/database/instantiate/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/database/instantiate/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/database/main/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/database/main/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/database/model/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/database/model/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/database/relations/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/database/relations/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/database/schema/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/database/schema/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/database/update/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/database/update/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/documentation/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/documentation/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/index.html` & `alphaz-0.7.7.9/alphaz/documentations/site/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/search/search_index.json` & `alphaz-0.7.7.9/alphaz/documentations/site/search/search_index.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/documentations/site/sitemap.xml` & `alphaz-0.7.7.9/alphaz/documentations/site/sitemap.xml`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/index.html` & `alphaz-0.7.7.9/alphaz/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/api_lib.py` & `alphaz-0.7.7.9/alphaz/libs/api_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/barcode_lib.py` & `alphaz-0.7.7.9/alphaz/libs/barcode_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/config_lib.py` & `alphaz-0.7.7.9/alphaz/libs/config_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/converter_lib.py` & `alphaz-0.7.7.9/alphaz/libs/converter_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/database_lib.py` & `alphaz-0.7.7.9/alphaz/libs/database_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/date_lib.py` & `alphaz-0.7.7.9/alphaz/libs/date_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/dict_lib.py` & `alphaz-0.7.7.9/alphaz/libs/dict_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/emulation/vt102_lib.py` & `alphaz-0.7.7.9/alphaz/libs/emulation/vt102_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/events.py` & `alphaz-0.7.7.9/alphaz/libs/events.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/files_lib.py` & `alphaz-0.7.7.9/alphaz/libs/files_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/flask_lib.py` & `alphaz-0.7.7.9/alphaz/libs/flask_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/img_lib.py` & `alphaz-0.7.7.9/alphaz/libs/img_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/io_lib.py` & `alphaz-0.7.7.9/alphaz/libs/io_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/json_lib.py` & `alphaz-0.7.7.9/alphaz/libs/json_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-import json, dataclasses
+import dataclasses
+
+try:
+    import ujson as json
+except:
+    import json
+
+    print("Cannot import ujson")
+
+
 from flask_sqlalchemy.model import DefaultMeta
 from sqlalchemy.orm.attributes import instance_state
 from sqlalchemy import null
 
 from ..libs.time_lib import timer
 
 from ..models.database.row import Row
@@ -42,14 +51,28 @@
         try:
             results_json = json.dumps(model.__dict__)
         except:
             results_json = str(model)
     return results_json
 
 
+def is_standard(data) -> bool:
+    if type(data) == Row:
+        return False
+    elif hasattr(data, "schema") or hasattr(data, "get_schema"):
+        return False
+    elif hasattr(data, "_fields"):
+        return False
+    elif hasattr(data, "to_json"):
+        return False
+    elif dataclasses.is_dataclass(data):
+        return False
+    return True
+
+
 def jsonify_data(data, string_output: bool = False):
     """Convert any data to a json structure
 
     Args:
         data ([type]): data to convert
 
     Returns:
@@ -63,30 +86,31 @@
     if type(data) == str:
         return data
     if type(data) == tuple:
         result = (jsonify_data(x) for x in data)
     elif type(data) == list:
         result = [jsonify_data(x) for x in data]
     elif type(data) == dict:
-        result = {jsonify_data(x): jsonify_data(y) for x, y in data.items()}
+        if len(data) and not is_standard(list(data.keys())[0]):
+            result = {jsonify_data(x): jsonify_data(y) for x, y in data.items()}
+        else:
+            result = {x: jsonify_data(y) for x, y in data.items()}
     elif type(data) == Row:
         result = dict(data)
     else:
         result = data
 
         if hasattr(data, "schema") or hasattr(data, "get_schema"):
             result = jsonify_database_models(data)
         elif hasattr(data, "_fields"):
             result = {x: data[i] for i, x in enumerate(data._fields)}
         elif hasattr(data, "to_json"):
             result = data.to_json()
         elif dataclasses.is_dataclass(data):
             result = dataclasses.asdict(data)
-        else:
-            result = data
     if string_output:
         result = json.dumps(result)
     return result
 
 
 def load_json(string: str):
     if string is None:
```

### Comparing `alphaz-0.7.7.8/alphaz/libs/logs_lib.py` & `alphaz-0.7.7.9/alphaz/libs/logs_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/mail_lib.py` & `alphaz-0.7.7.9/alphaz/libs/mail_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/notifications_lib.py` & `alphaz-0.7.7.9/alphaz/libs/notifications_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/number_lib.py` & `alphaz-0.7.7.9/alphaz/libs/number_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/process_lib.py` & `alphaz-0.7.7.9/alphaz/libs/process_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/py_lib.py` & `alphaz-0.7.7.9/alphaz/libs/py_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/scp_lib.py` & `alphaz-0.7.7.9/alphaz/libs/scp_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/search_lib.py` & `alphaz-0.7.7.9/alphaz/libs/search_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/secure_lib.py` & `alphaz-0.7.7.9/alphaz/libs/secure_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/soap_lib.py` & `alphaz-0.7.7.9/alphaz/libs/soap_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/ssh_lib.py` & `alphaz-0.7.7.9/alphaz/libs/ssh_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/string_lib.py` & `alphaz-0.7.7.9/alphaz/libs/string_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/test_lib.py` & `alphaz-0.7.7.9/alphaz/libs/test_lib.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     groups: list[str] = [],
     names: list[str] = [],
     levels: list[Levels] = [],
     run: bool = False,
     coverage: str | None = None,
     load_from_db: bool = True,
     stop: bool = True,
+    failed_only: bool = False,
 ):
     subclasses = AlphaTest.__subclasses__()
     subclasses_by_module = defaultdict(list)
     for subclass in subclasses:
         module_name = subclass.__module__.split(".")[0]
         subclasses_by_module[module_name].append(subclass)
 
@@ -70,18 +71,18 @@
                 continue
 
             if LOG is not None:
                 LOG.debug(f"Found function group <{test_group.name}>")
 
             test_categories.add_test_group(test_group)
 
-    if load_from_db:
+    if load_from_db or failed_only:
         test_categories.get_from_database()
     if run:
-        test_categories.test_all(names, levels, stop=stop)
+        test_categories.test_all(names, levels, stop=stop, failed_only=failed_only)
 
     return test_categories
 
 
 def get_tests_auto(
     name: str | None = None,
     names: list[str] = [],
@@ -92,14 +93,15 @@
     file_path: str | None = None,
     run: bool = False,
     load_from_db: bool = False,
     report: str | None = None,
     coverage: str | None = None,
     levels: list[Levels] = [],
     stop: bool = False,
+    failed_only: bool = False,
 ) -> TestCategories:
     """Get the TestCategories class, containings all required tests.
 
     Args:
         tests_modules (list[str]): list of test modules path
         tests_modules (list[str]): list of test modules path
         name (str, optional): the name of the test to select. Defaults to None.
@@ -127,14 +129,15 @@
         groups,
         names,
         levels,
         run,
         coverage,
         load_from_db=load_from_db,
         stop=stop,
+        failed_only=failed_only,
     )
 
     if file_path is not None:
         test_categories.to_junit(file_path)
 
     if report is not None:
         test_categories.report(report)
```

### Comparing `alphaz-0.7.7.8/alphaz/libs/time_lib.py` & `alphaz-0.7.7.9/alphaz/libs/time_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/transactions_lib.py` & `alphaz-0.7.7.9/alphaz/libs/transactions_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/user_lib.py` & `alphaz-0.7.7.9/alphaz/libs/user_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/user_management/application_management_lib.py` & `alphaz-0.7.7.9/alphaz/libs/user_management/application_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/user_management/permission_management_lib.py` & `alphaz-0.7.7.9/alphaz/libs/user_management/permission_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/user_management/role_management_lib.py` & `alphaz-0.7.7.9/alphaz/libs/user_management/role_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/libs/user_management/user_management_lib.py` & `alphaz-0.7.7.9/alphaz/libs/user_management/user_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/mails/Images/Background.png` & `alphaz-0.7.7.9/alphaz/mails/Images/Background.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/mails/Images/Facebook_logo.png` & `alphaz-0.7.7.9/alphaz/mails/Images/Facebook_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/mails/Images/Twitter_logo.png` & `alphaz-0.7.7.9/alphaz/mails/Images/Twitter_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/mails/Images/Web_logo.png` & `alphaz-0.7.7.9/alphaz/mails/Images/Web_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/mails/Mail.png` & `alphaz-0.7.7.9/alphaz/mails/Mail.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/mails/Webmail.html` & `alphaz-0.7.7.9/alphaz/mails/Webmail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/mails/debug.html` & `alphaz-0.7.7.9/alphaz/mails/debug.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/mails/mail.html` & `alphaz-0.7.7.9/alphaz/mails/mail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/mails/password_reset.html` & `alphaz-0.7.7.9/alphaz/mails/password_reset.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/mails/stay_in_touch.html` & `alphaz-0.7.7.9/alphaz/mails/stay_in_touch.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/api/_answer.py` & `alphaz-0.7.7.9/alphaz/models/api/_answer.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/api/_colorations.py` & `alphaz-0.7.7.9/alphaz/models/api/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/api/_parameter.py` & `alphaz-0.7.7.9/alphaz/models/api/_parameter.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/api/_reloader.py` & `alphaz-0.7.7.9/alphaz/models/api/_reloader.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/api/_reloaders.py` & `alphaz-0.7.7.9/alphaz/models/api/_reloaders.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/api/_requests.py` & `alphaz-0.7.7.9/alphaz/models/api/_requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/api/_route.py` & `alphaz-0.7.7.9/alphaz/models/api/_route.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,15 @@
-import datetime, os, copy, json
+import datetime, os, copy
+
+try:
+    import ujson as json
+except:
+    import json
+
+    print("Cannot import ujson")
 import time
 import traceback
 
 from flask import (
     jsonify,
     request,
     make_response,
@@ -142,14 +149,18 @@
         self.file_to_get = (None, None)
         self.file_to_set = (None, None)
 
         self.cache_dir = api.cache_dir
         self.log = api.log
         self.method = request_state.method
 
+        self.page: int = 0
+        self.total, self.total_pages, self.per_page = None, None, None
+        self._is_pagination: bool | None = None
+
         self.init_return()
 
         self.parameters: dict[Parameter] = {y.name: copy.copy(y) for y in parameters}
         for parameter in self.parameters.values():
             try:
                 parameter.set_value(
                     self.method, self.dict, self.json, self.form, self.args
@@ -370,19 +381,112 @@
 
     def is_paginated(self):
         return (
             self.parameters.get("page", None) is not None
             and self.parameters.get("per_page", None) is not None
         )
 
-    def get_return(self, forceData=False, return_status=None):
-        default_format = self.api.conf.get("default_format")
-        if default_format is None:
-            default_format = "json"
+    def is_pagination(self) -> bool:
+        if self._is_pagination is not None:
+            pagination_mode = self.api.db.config.get("pagination_mode", "raw")
+            if pagination_mode == "integrated":
+                is_pagination = self.api.db.full_count is not None
+            else:
+                is_pagination = self.page is not None and (
+                    py_lib.is_list(self.data)
+                    and len(self.data) == 2
+                    and type(self.data[0]) == list
+                    and type(self.data[1]) == int
+                )
+            self._is_pagination = is_pagination
+            return is_pagination
+        return self._is_pagination
+
+    def set_pagination(self):
+        format_ = self.get_format()
+        data = {} if self.data is None else self.data
+        self.total, self.total_pages, self.page, self.per_page = (
+            None,
+            None,
+            self.get("page", 0),
+            self.get("per_page", None),
+        )
+
+        is_pagination = self.is_pagination()
+        pagination_mode = self.api.db.config.get("pagination_mode", "raw")
+        if pagination_mode == "integrated":
+            if is_pagination and py_lib.is_iterable(data):
+                self.per_page = len(data) if self.per_page is None else self.per_page
+                self.total = (
+                    self.api.db.full_count if self.api.db.full_count is not None else 0
+                )
+                self.total_pages = (
+                    int(self.total / self.per_page)
+                    if self.per_page is not None and self.per_page != 0
+                    else 0
+                )
+        else:
+            if self.per_page is None and is_pagination:
+                self.per_page = len(data[0])
+
+            if "pagination" in format_ and is_pagination:
+                self.total, self.total_pages = (
+                    data[1] if data[1] is not None else 0,
+                    int(data[1] / self.per_page) if self.per_page is not None else 0,
+                )
+                data = data[0]
+            self.data = data
+
+    def get_headers(self):
+        format_ = self.get_format()
+        headers = {}
+        if "txt" in format_:
+            headers["Content-Type"] = "text/txt; charset=utf-8"
+        elif "xml" in format_:
+            headers["Content-Type"] = "text/xml; charset=utf-8"
+
+        headers_content = {
+            "X-token-status": self.returned.token_status,
+            "X-status": self.returned.status,
+            "X-error": self.returned.error,
+            "X-warning": self.returned.warning,
+            "X-status-description": self.returned.status_description,
+            "X-requester": self.returned.requester,
+        }
+        for key, value in headers_content.items():
+            headers[key] = value
+        headers[
+            "Access-Control-Expose-Headers"
+        ] = "*"  # ",".join(headers_content.keys())
+        # headers["Access-Control-Allow-Headers"] = "*" # ",".join(headers_content.keys())
+
+        # returned = Response(returned, status=returned["status_code"])
+        if "pagination" in format_ and self.is_pagination():
+            headers["X-pagination"] = {
+                "total": self.total,
+                "total_pages": self.total_pages,
+                "page": self.page,
+                "previous_page": self.page - 1 if self.page > 0 else 0,
+                "next_page": (
+                    self.page + 1 if self.page < self.total_pages else self.total_pages
+                )
+                if (self.total_pages is not None and self.page is not None)
+                else None,
+                "per_page": self.per_page,
+            }
+
+        return headers
+
+    def get_format(self) -> str:
+        default_format = self.api.conf.get("default_format", "json")
         format_ = self.get("format", default=default_format, enable_none=False).lower()
+        return format_
+
+    def get_return(self, forceData=False, return_status=None):
+        format_ = self.get_format()
 
         if self.mode == "html":
             if "page" in self.data:
                 return render_template(self.data["page"], **self.data["parameters"])
             else:
                 return self.data
         elif self.mode == "print":
@@ -408,52 +512,17 @@
                 self.set_error(self.data.msg, self.data.msg)
             elif hasattr(self.data, "args"):
                 self.set_error(self.data.args[0], self.data.args[0])
             self.data = {}
 
         self.returned.data = {}
 
-        data = {} if self.data is None else self.data
-        total, total_pages, page, per_page = (
-            None,
-            None,
-            self.get("page", 0),
-            self.get("per_page", None),
-        )
-
-        pagination_mode = self.api.db.config.get("pagination_mode", "raw")
-        if pagination_mode == "integrated":
-            is_pagination = self.api.db.full_count is not None
-            if is_pagination and py_lib.is_iterable(data):
-                per_page = len(data) if per_page is None else per_page
-                total = (
-                    self.api.db.full_count if self.api.db.full_count is not None else 0
-                )
-                total_pages = (
-                    int(total / per_page)
-                    if per_page is not None and per_page != 0
-                    else 0
-                )
-        else:
-            is_pagination = page is not None and (
-                py_lib.is_list(data)
-                and len(data) == 2
-                and type(data[0]) == list
-                and type(data[1]) == int
-            )
-            if per_page is None and is_pagination:
-                per_page = len(data[0])
-
-            if "pagination" in format_ and is_pagination:
-                total, total_pages = (
-                    data[1] if data[1] is not None else 0,
-                    int(data[1] / per_page) if per_page is not None else 0,
-                )
-                data = data[0]
+        self.set_pagination()
 
+        data = self.data
         if not check_format(data):
             tic = time.perf_counter()
             data = json_lib.jsonify_data(data)
             toc = time.perf_counter()
             elapsed_time = toc - tic
             if DEBUG:
                 print(f"Elapsed time: {elapsed_time:0.4f} seconds for jsonify_data")
@@ -464,90 +533,66 @@
             )
 
         self.returned.data = data
         status_code = self.returned.status_code
         if type(self.returned.status) == int:
             status_code = self.returned.status
 
-        headers = {}
-
         tic = time.perf_counter()
         if "txt" in format_:
             route_output = str(data)
             if (
                 route_output is not None
                 and len(route_output) != 0
                 and route_output[0] == '"'
             ):
                 route_output = route_output[1:-1]
         elif "xml" in format_:
             route_output = (
-                self.returned.to_json() if "raw" in format_ else jsonify(data)
+                self.returned.to_json()
+                if "raw" in format_
+                else (jsonify(data) if "make" in format_ else data)
             )
             route_output = converter_lib.dict_to_xml(
                 route_output, attr_type=not "no_type" in format_
             )
         elif "raw" in format_:
-            route_output = jsonify(data)
+            route_output = jsonify(data) if "make" in format_ else json.dumps(data)
         else:
             # returned = jsonify(self.returned)
             route_output = self.returned.to_json()
+            if not "make" in format_:
+                route_output = json.dumps(route_output)
 
         toc = time.perf_counter()
         elapsed_time = toc - tic
         if DEBUG:
             print(f"Elapsed time: {elapsed_time:0.4f} seconds for conversion")
 
-        if "txt" in format_:
-            headers["Content-Type"] = "text/txt; charset=utf-8"
-        elif "xml" in format_:
-            headers["Content-Type"] = "text/xml; charset=utf-8"
+        tic = time.perf_counter()
 
-        headers_content = {
-            "X-token-status": self.returned.token_status,
-            "X-status": self.returned.status,
-            "X-error": self.returned.error,
-            "X-warning": self.returned.warning,
-            "X-status-description": self.returned.status_description,
-            "X-requester": self.returned.requester,
-        }
-        for key, value in headers_content.items():
-            headers[key] = value
-        headers[
-            "Access-Control-Expose-Headers"
-        ] = "*"  # ",".join(headers_content.keys())
-        # headers["Access-Control-Allow-Headers"] = "*" # ",".join(headers_content.keys())
+        if "make" in format_:
+            returned = make_response(route_output, status_code)
+        else:
+            returned = make_response({}, status_code)
+            returned.set_data(route_output)
 
-        # returned = Response(returned, status=returned["status_code"])
-        tic = time.perf_counter()
-        returned = make_response(route_output, status_code)
         toc = time.perf_counter()
         elapsed_time = toc - tic
         if DEBUG:
             print(f"Elapsed time: {elapsed_time:0.4f} seconds for returned")
 
-        if "pagination" in format_ and is_pagination:
-            headers["X-pagination"] = {
-                "total": total,
-                "total_pages": total_pages,
-                "page": page,
-                "previous_page": page - 1 if page > 0 else 0,
-                "next_page": (page + 1 if page < total_pages else total_pages)
-                if (total_pages is not None and page is not None)
-                else None,
-                "per_page": per_page,
-            }
+        headers = self.get_headers()
 
         for key, value in headers.items():
             returned.headers[key] = (
                 json.dumps([str(v) for v in value.split("\n")])
                 if "\n" in str(value)
                 else value
             )
-
         return returned
 
     def log_user(self, user):
         self.returned.role = "user"
         if user.role >= 9:
             self.returned.role = "admin"
         self.returned.token = jwt.encode(
```

### Comparing `alphaz-0.7.7.8/alphaz/models/api/_structures.py` & `alphaz-0.7.7.9/alphaz/models/api/_structures.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/api/_utils.py` & `alphaz-0.7.7.9/alphaz/models/api/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/config/_config.py` & `alphaz-0.7.7.9/alphaz/models/config/_config.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/config/_utils.py` & `alphaz-0.7.7.9/alphaz/models/config/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/database/main_definitions.py` & `alphaz-0.7.7.9/alphaz/models/database/main_definitions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/database/models.py` & `alphaz-0.7.7.9/alphaz/models/database/models.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/database/operators.py` & `alphaz-0.7.7.9/alphaz/models/database/operators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/database/requests.py` & `alphaz-0.7.7.9/alphaz/models/database/requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/database/row.py` & `alphaz-0.7.7.9/alphaz/models/database/row.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/database/structure.py` & `alphaz-0.7.7.9/alphaz/models/database/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1576,14 +1576,15 @@
             tables = [x.__table__ for x in tables_models]
             if drop or create:
                 try:
                     meta = self.get_meta(bind=bind)
                 except:
                     log.error(f"Cannot find {bind=}")
                     continue
+            log.info(f"Init of {str(meta.bind.engine)}")
 
             table_names = [x.__tablename__ for x in tables_models]
             tables_names_str = ";".join(table_names)
 
             if drop:
                 if log is not None:
                     log.info(f"Drop tables from {bind=}: {tables_names_str}")
```

### Comparing `alphaz-0.7.7.8/alphaz/models/database/tests.py` & `alphaz-0.7.7.9/alphaz/models/database/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/database/users_definitions.py` & `alphaz-0.7.7.9/alphaz/models/database/users_definitions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/database/utils.py` & `alphaz-0.7.7.9/alphaz/models/database/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/database/views.py` & `alphaz-0.7.7.9/alphaz/models/database/views.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/excel.py` & `alphaz-0.7.7.9/alphaz/models/excel.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/ftp.py` & `alphaz-0.7.7.9/alphaz/models/ftp.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/json/_converters.py` & `alphaz-0.7.7.9/alphaz/models/json/_converters.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/logger/_colorations.py` & `alphaz-0.7.7.9/alphaz/models/logger/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/logger/_logger.py` & `alphaz-0.7.7.9/alphaz/models/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/logger/_utils.py` & `alphaz-0.7.7.9/alphaz/models/logger/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/logs/main.log` & `alphaz-0.7.7.9/alphaz/models/logs/main.log`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/main/_base.py` & `alphaz-0.7.7.9/alphaz/models/main/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -538,15 +538,15 @@
 def convert_value_from_field(
     field_type, value, mapping_mode: MappingMode | str | None = None
 ):
     field_type = py_lib.get_first_non_none_type(field_type)
     if value is None:
         return None
     if is_dataclass(field_type):
-        return field_type.map_from_dict(
+        return field_type.map(
             asdict(value) if is_dataclass(value) else value, mapping_mode=mapping_mode
         )
     elif isinstance(value, list) and all(isinstance(item, dict) for item in value):
         return [convert_value_from_field(field_type, item) for item in value]
     else:
         try:
             return convert_value(value, field_type)
```

### Comparing `alphaz-0.7.7.8/alphaz/models/main/_core/_core.py` & `alphaz-0.7.7.9/alphaz/models/main/_core/_core.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/main/_exception.py` & `alphaz-0.7.7.9/alphaz/models/main/_exception.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/main/_request.py` & `alphaz-0.7.7.9/alphaz/models/main/_request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/main/_singleton.py` & `alphaz-0.7.7.9/alphaz/models/main/_singleton.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/request.py` & `alphaz-0.7.7.9/alphaz/models/request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/tests/_category.py` & `alphaz-0.7.7.9/alphaz/models/tests/_category.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def get_tests_groups_names(self):
         return list(self.groups.keys())
 
     def get_test_group(self, name):
         return self.groups[name]
 
     def to_json(self):
-        return self.groups
+        return {x: y.to_json() for x, y in self.groups.items()}
 
 
 def truncate_time(number: float):
     return int(number * 100) / 100
 
 
 class TestCategories:
@@ -77,23 +77,31 @@
         self.categories = dict_lib.sort_dict(self.categories)
 
     def test_all(
         self,
         names: list[str] | None = None,
         levels: list[Levels] = [],
         stop: bool = True,
+        failed_only: bool = False,
     ) -> bool:
         stopped = False
         for category in self.categories.values():
+            if failed_only and category.status:
+                continue
             if stopped:
                 break
             for test_group in category.groups.values():
+                if failed_only and test_group.status:
+                    continue
+
                 if stopped:
                     break
-                if not test_group.test_all(names, levels, stop=stop):
+                if not test_group.test_all(
+                    names, levels, stop=stop, failed_only=failed_only
+                ):
                     self.status = False
                     if stop:
                         stopped = True
                         break
         return self.status
 
     def get_from_database(self):
@@ -193,15 +201,15 @@
         print(content)
         if file_path is not None and file_path != "print_only":
             with open(file_path, "w") as f:
                 f.write(content)
         return content
 
     def to_json(self):
-        return self.categories
+        return {x: y.to_json() for x, y in self.categories.items()}
 
     def to_junit(self, file_path):
         if not "." in file_path:
             file_path += ".xml"
         from junit_xml import TestSuite, TestCase
 
         suites = []
```

### Comparing `alphaz-0.7.7.8/alphaz/models/tests/_group.py` & `alphaz-0.7.7.9/alphaz/models/tests/_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,27 +67,35 @@
                 test.update_from_database(test_db)
 
     def test(self, name: str):
         if name in self.tests:
             self.tests[name].test(coverage=self.coverage)
 
     def test_all(
-        self, names: list[str] = None, levels: list[Levels] = [], stop: bool = True
+        self,
+        names: list[str] | None = None,
+        levels: list[Levels] = [],
+        stop: bool = True,
+        failed_only: bool = False,
     ) -> bool:
         tests = self.tests
         if names is not None and len(names) != 0:
             tests = {x: y for x, y in tests.items() if x in names}
         if levels is not None and len(levels) != 0:
             tests = {x: y for x, y in tests.items() if y.level.name in levels}
 
         if len(tests) != 0:
             classTest = self.classTest()
 
+            if failed_only and self.status:
+                return self.status
             for test in tests.values():
-                if not test.test(classTest=classTest, coverage=self.coverage):
+                if not test.test(
+                    classTest=classTest, coverage=self.coverage, failed_only=failed_only
+                ):
                     self.status = False
                     if stop:
                         break
         return self.status
 
     def save_all(self):
         for method in self.tests.values():
@@ -101,9 +109,8 @@
         for test_name, test_def in self.tests.items():
             txt += "{:60} {:4}".format(test_name, test_def.print()) + "\n"
         if output:
             print(txt)
         return txt
 
     def to_json(self):
-        tests = self.tests
-        return tests
+        return {x: y.to_json() for x, y in self.tests.items()}
```

### Comparing `alphaz-0.7.7.8/alphaz/models/tests/_method.py` & `alphaz-0.7.7.9/alphaz/models/tests/_method.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,15 +49,18 @@
         self.end_time: datetime.datetime = None
         self.elapsed: int = 0
         self.last_run_elapsed = None
         self.coverages: dict[str, object] = {}
 
         self.ex: Exception = None
 
-    def test(self, classTest=None, coverage: bool = False):
+    def test(self, classTest=None, coverage: bool = False, failed_only: bool = False):
+        if failed_only and self.status:
+            return self.status
+
         if classTest is None:
             classTest = self.classTest()
 
         self.start_time = datetime.datetime.now()
 
         log.info(
             f"Testing function <{self.name}> of <{type(self).__name__}> in category <{self.category}>"
```

### Comparing `alphaz-0.7.7.8/alphaz/models/tests/_save.py` & `alphaz-0.7.7.9/alphaz/models/tests/_save.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/tests/_test.py` & `alphaz-0.7.7.9/alphaz/models/tests/_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 # CORE
 from core import core
 
 # LIBS
 from alphaz.libs import dict_lib, database_lib
 
 # MODELS
-from alphaz.models.main import AlphaDataclass
+from alphaz.models.main import AlphaDataclass, AlphaClass
 
 LOG = core.get_logger("tests")
 
 
 @dataclass
 class TestInput(AlphaDataclass):
     value: str
     number: int
 
 
-class AlphaTest:
+class AlphaTest(AlphaClass):
     _test = True
     category = ""
     index = 0
     current_test_name = ""
 
     outputs: dict[str, bool] = {}
     coverages: dict[str, object] = {}
```

### Comparing `alphaz-0.7.7.8/alphaz/models/tests/_wrappers.py` & `alphaz-0.7.7.9/alphaz/models/tests/_wrappers.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/user.py` & `alphaz-0.7.7.9/alphaz/models/user.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/models/watcher.py` & `alphaz-0.7.7.9/alphaz/models/watcher.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/pocs/main.py` & `alphaz-0.7.7.9/alphaz/pocs/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/run.py` & `alphaz-0.7.7.9/alphaz/run.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/src/alpha.png` & `alphaz-0.7.7.9/alphaz/src/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/src/configs/loggers.json` & `alphaz-0.7.7.9/alphaz/src/configs/loggers.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/stitch/Core.py` & `alphaz-0.7.7.9/alphaz/stitch/Core.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/stitch/stitch.py` & `alphaz-0.7.7.9/alphaz/stitch/stitch.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/stitch/web-drivers/chromedriver.exe` & `alphaz-0.7.7.9/alphaz/stitch/web-drivers/chromedriver.exe`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/stitch/web-drivers/geckodriver` & `alphaz-0.7.7.9/alphaz/stitch/web-drivers/geckodriver`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/templates/assets/css/home.css` & `alphaz-0.7.7.9/alphaz/templates/assets/css/home.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/templates/assets/css/logs.css` & `alphaz-0.7.7.9/alphaz/templates/assets/css/logs.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/templates/assets/images/icons/alpha.png` & `alphaz-0.7.7.9/alphaz/templates/assets/images/icons/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/templates/assets/images/icons/start-icon.png` & `alphaz-0.7.7.9/alphaz/templates/assets/images/icons/start-icon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/templates/assets/images/icons/wsalpha.png` & `alphaz-0.7.7.9/alphaz/templates/assets/images/icons/wsalpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/templates/assets/images/loading.gif` & `alphaz-0.7.7.9/alphaz/templates/assets/images/loading.gif`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/templates/assets/js/libs/ansi_up.js` & `alphaz-0.7.7.9/alphaz/templates/assets/js/libs/ansi_up.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/templates/assets/js/libs/jquery.min.js` & `alphaz-0.7.7.9/alphaz/templates/assets/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/templates/assets/js/logs.js` & `alphaz-0.7.7.9/alphaz/templates/assets/js/logs.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/templates/home.html` & `alphaz-0.7.7.9/alphaz/templates/home.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/templates/logs.html` & `alphaz-0.7.7.9/alphaz/templates/logs.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/test.py` & `alphaz-0.7.7.9/alphaz/test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/tests/api.py` & `alphaz-0.7.7.9/alphaz/tests/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/tests/basic_test.py` & `alphaz-0.7.7.9/alphaz/tests/basic_test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/tests/configurations.py` & `alphaz-0.7.7.9/alphaz/tests/configurations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/tests/database.py` & `alphaz-0.7.7.9/alphaz/tests/database.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/tests/utils.py` & `alphaz-0.7.7.9/alphaz/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/utils/api.py` & `alphaz-0.7.7.9/alphaz/utils/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/utils/apm/ora.py` & `alphaz-0.7.7.9/alphaz/utils/apm/ora.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/utils/configuration.py` & `alphaz-0.7.7.9/alphaz/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/utils/database/init.py` & `alphaz-0.7.7.9/alphaz/utils/database/init.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/utils/database_to_dataclass.py` & `alphaz-0.7.7.9/alphaz/utils/database_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/utils/decorators.py` & `alphaz-0.7.7.9/alphaz/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/utils/ensure.py` & `alphaz-0.7.7.9/alphaz/utils/ensure.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/utils/init_database.py` & `alphaz-0.7.7.9/alphaz/utils/init_database.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/utils/mep.py` & `alphaz-0.7.7.9/alphaz/utils/mep.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/utils/screens.py` & `alphaz-0.7.7.9/alphaz/utils/screens.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/utils/selectionMenu.py` & `alphaz-0.7.7.9/alphaz/utils/selectionMenu.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/utils/tasks.py` & `alphaz-0.7.7.9/alphaz/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/utils/tests.py` & `alphaz-0.7.7.9/alphaz/utils/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/utils/time.py` & `alphaz-0.7.7.9/alphaz/utils/time.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz/utils/transactions.py` & `alphaz-0.7.7.9/alphaz/utils/transactions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/alphaz.egg-info/PKG-INFO` & `alphaz-0.7.7.9/alphaz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz
-Version: 0.7.7.8
+Version: 0.7.7.9
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.7.8.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.7.9.tar.gz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `alphaz-0.7.7.8/alphaz.egg-info/SOURCES.txt` & `alphaz-0.7.7.9/alphaz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.8/setup.py` & `alphaz-0.7.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os, glob, re
 from datetime import date
 
 today = date.today()
 
 from setuptools import setup, find_packages
 
-version = "0.7.7.8"
+version = "0.7.7.9"
 
 excludes = [".git", ".vscode"]
 
 archives = glob.glob("dist/*")
 for archive in archives:
     os.remove(archive)
```

