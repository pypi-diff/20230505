# Comparing `tmp/nautobot_golden_config-1.3.1.tar.gz` & `tmp/nautobot_golden_config-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_golden_config-1.3.1.tar", max compression
+gzip compressed data, was "nautobot_golden_config-1.4.0.tar", max compression
```

## Comparing `nautobot_golden_config-1.3.1.tar` & `nautobot_golden_config-1.4.0.tar`

### file list

```diff
@@ -1,98 +1,101 @@
--rw-r--r--   0        0        0      591 2022-12-15 17:07:42.986571 nautobot_golden_config-1.3.1/LICENSE
--rw-r--r--   0        0        0     6560 2022-12-15 17:07:42.986571 nautobot_golden_config-1.3.1/README.md
--rw-r--r--   0        0        0     1304 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/__init__.py
--rw-r--r--   0        0        0       57 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/api/__init__.py
--rw-r--r--   0        0        0     5474 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/api/serializers.py
--rw-r--r--   0        0        0      935 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/api/urls.py
--rw-r--r--   0        0        0     4730 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/api/views.py
--rw-r--r--   0        0        0      358 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/choices.py
--rw-r--r--   0        0        0     9137 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/datasources.py
--rw-r--r--   0        0        0      402 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/exceptions.py
--rw-r--r--   0        0        0     9420 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/filters.py
--rw-r--r--   0        0        0    12686 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/forms.py
--rw-r--r--   0        0        0    10404 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/jobs.py
--rw-r--r--   0        0        0      906 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/management/commands/run_config_backup.py
--rw-r--r--   0        0        0      930 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/management/commands/run_config_compliance.py
--rw-r--r--   0        0        0      944 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/management/commands/run_generate_config.py
--rw-r--r--   0        0        0    12458 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0001_initial.py
--rw-r--r--   0        0        0      509 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0002_custom_data.py
--rw-r--r--   0        0        0     1815 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0003_auto_20210510_2356.py
--rw-r--r--   0        0        0     1825 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0004_auto_20210616_2234.py
--rw-r--r--   0        0        0     1515 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0005_json_compliance_rule.py
--rw-r--r--   0        0        0     1795 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py
--rw-r--r--   0        0        0     2556 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py
--rw-r--r--   0        0        0      666 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0008_multi_repo_support_final.py
--rw-r--r--   0        0        0     2559 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py
--rw-r--r--   0        0        0      930 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py
--rw-r--r--   0        0        0     1487 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py
--rw-r--r--   0        0        0      910 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py
--rw-r--r--   0        0        0      464 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0013_multiple_gc_settings_part_5.py
--rw-r--r--   0        0        0      430 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0014_convert_sotagg_queries_part1.py
--rw-r--r--   0        0        0      706 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py
--rw-r--r--   0        0        0      770 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py
--rw-r--r--   0        0        0     1646 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py
--rw-r--r--   0        0        0      328 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0018_convert_sotagg_queries_part5.py
--rw-r--r--   0        0        0      679 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py
--rw-r--r--   0        0        0     1187 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py
--rw-r--r--   0        0        0      664 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py
--rw-r--r--   0        0        0        0 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/__init__.py
--rw-r--r--   0        0        0    24587 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/models.py
--rw-r--r--   0        0        0     4331 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/navigation.py
--rw-r--r--   0        0        0     5844 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/nornir_plays/config_backup.py
--rw-r--r--   0        0        0     7183 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/nornir_plays/config_compliance.py
--rw-r--r--   0        0        0     5682 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/nornir_plays/config_intended.py
--rw-r--r--   0        0        0     1525 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/nornir_plays/processor.py
--rw-r--r--   0        0        0     4941 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.css
--rw-r--r--   0        0        0    67546 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.js
--rw-r--r--   0        0        0    16543 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/tables.py
--rw-r--r--   0        0        0     3547 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/template_content.py
--rw-r--r--   0        0        0     7459 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/compliance_device_report.html
--rw-r--r--   0        0        0     3680 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/compliance_overview_report.html
--rw-r--r--   0        0        0     1568 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/compliance_report.html
--rw-r--r--   0        0        0     3056 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/compliancefeature.html
--rw-r--r--   0        0        0     3498 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/compliancerule.html
--rw-r--r--   0        0        0     3902 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/configcompliance.html
--rw-r--r--   0        0        0     1961 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/configcompliancedetails.html
--rw-r--r--   0        0        0     1127 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/configcompliancedetails_modal.html
--rw-r--r--   0        0        0     3169 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/configremove.html
--rw-r--r--   0        0        0     3324 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/configreplace.html
--rw-r--r--   0        0        0     4142 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/content_template.html
--rw-r--r--   0        0        0      365 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/dff2html_base.html
--rw-r--r--   0        0        0     3601 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html
--rw-r--r--   0        0        0     3335 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting.html
--rw-r--r--   0        0        0     1393 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_edit.html
--rw-r--r--   0        0        0      181 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/manytomany.html
--rw-r--r--   0        0        0       52 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/__init__.py
--rw-r--r--   0        0        0    13854 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/conftest.py
--rw-r--r--   0        0        0       51 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/forms/__init__.py
--rw-r--r--   0        0        0     1939 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/forms/test_golden_config_settings.py
--rw-r--r--   0        0        0       83 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/jinja_filters.py
--rw-r--r--   0        0        0    12405 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_api.py
--rw-r--r--   0        0        0      994 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_basic.py
--rw-r--r--   0        0        0     3503 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_datasources.py
--rw-r--r--   0        0        0    12768 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_filters.py
--rw-r--r--   0        0        0    12960 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_graphql.py
--rw-r--r--   0        0        0     5464 2022-12-15 17:07:43.018571 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_helpers.py
--rw-r--r--   0        0        0    11326 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_models.py
--rw-r--r--   0        0        0       58 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_nornir_plays/__init__.py
--rw-r--r--   0        0        0     1018 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py
--rw-r--r--   0        0        0       55 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_utilities/__init__.py
--rw-r--r--   0        0        0     2899 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_utilities/test_git.py
--rw-r--r--   0        0        0     1245 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_utilities/test_graphql.py
--rw-r--r--   0        0        0    13388 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_utilities/test_helpers.py
--rw-r--r--   0        0        0     1284 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_utilities/test_utils.py
--rw-r--r--   0        0        0     1624 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_views.py
--rw-r--r--   0        0        0     7180 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/urls.py
--rw-r--r--   0        0        0       17 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/__init__.py
--rw-r--r--   0        0        0     8522 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/config_postprocessing.py
--rw-r--r--   0        0        0      627 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/constant.py
--rw-r--r--   0        0        0      607 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/db_management.py
--rw-r--r--   0        0        0     2990 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/git.py
--rw-r--r--   0        0        0     1771 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/graphql.py
--rw-r--r--   0        0        0     5337 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/helper.py
--rw-r--r--   0        0        0     3402 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/management.py
--rw-r--r--   0        0        0     1079 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/utils.py
--rw-r--r--   0        0        0    38770 2022-12-15 17:07:43.022572 nautobot_golden_config-1.3.1/nautobot_golden_config/views.py
--rw-r--r--   0        0        0     3541 2022-12-15 17:08:01.290773 nautobot_golden_config-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     7966 1970-01-01 00:00:00.000000 nautobot_golden_config-1.3.1/setup.py
--rw-r--r--   0        0        0     7989 1970-01-01 00:00:00.000000 nautobot_golden_config-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      591 2023-05-05 15:54:12.999758 nautobot_golden_config-1.4.0/LICENSE
+-rw-r--r--   0        0        0     6560 2023-05-05 15:54:12.999758 nautobot_golden_config-1.4.0/README.md
+-rw-r--r--   0        0        0     1957 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/__init__.py
+-rw-r--r--   0        0        0       57 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/api/__init__.py
+-rw-r--r--   0        0        0     5450 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/api/serializers.py
+-rw-r--r--   0        0        0      935 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/api/urls.py
+-rw-r--r--   0        0        0     4706 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/api/views.py
+-rw-r--r--   0        0        0      358 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/choices.py
+-rw-r--r--   0        0        0     9137 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/datasources.py
+-rw-r--r--   0        0        0      402 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/exceptions.py
+-rw-r--r--   0        0        0     9369 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/filters.py
+-rw-r--r--   0        0        0    12220 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/forms.py
+-rw-r--r--   0        0        0    10715 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/jobs.py
+-rw-r--r--   0        0        0      906 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/management/commands/run_config_backup.py
+-rw-r--r--   0        0        0      930 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/management/commands/run_config_compliance.py
+-rw-r--r--   0        0        0      944 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/management/commands/run_generate_config.py
+-rw-r--r--   0        0        0    12457 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0001_initial.py
+-rw-r--r--   0        0        0      508 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0002_custom_data.py
+-rw-r--r--   0        0        0     1814 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0003_auto_20210510_2356.py
+-rw-r--r--   0        0        0     1824 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0004_auto_20210616_2234.py
+-rw-r--r--   0        0        0     1514 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0005_json_compliance_rule.py
+-rw-r--r--   0        0        0     1794 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py
+-rw-r--r--   0        0        0     2555 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py
+-rw-r--r--   0        0        0      665 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0008_multi_repo_support_final.py
+-rw-r--r--   0        0        0     2558 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py
+-rw-r--r--   0        0        0      929 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py
+-rw-r--r--   0        0        0     1486 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py
+-rw-r--r--   0        0        0      909 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py
+-rw-r--r--   0        0        0      463 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0013_multiple_gc_settings_part_5.py
+-rw-r--r--   0        0        0      429 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0014_convert_sotagg_queries_part1.py
+-rw-r--r--   0        0        0      705 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py
+-rw-r--r--   0        0        0      769 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py
+-rw-r--r--   0        0        0     1645 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py
+-rw-r--r--   0        0        0      327 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0018_convert_sotagg_queries_part5.py
+-rw-r--r--   0        0        0      678 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py
+-rw-r--r--   0        0        0     1186 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py
+-rw-r--r--   0        0        0      663 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py
+-rw-r--r--   0        0        0      389 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0022_alter_configcompliance_options.py
+-rw-r--r--   0        0        0        0 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/__init__.py
+-rw-r--r--   0        0        0    25184 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/models.py
+-rw-r--r--   0        0        0     4331 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/navigation.py
+-rw-r--r--   0        0        0     5843 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/config_backup.py
+-rw-r--r--   0        0        0     7182 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/config_compliance.py
+-rw-r--r--   0        0        0     5641 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/config_intended.py
+-rw-r--r--   0        0        0     1525 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/processor.py
+-rwxr-xr-x   0        0        0      719 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/signals.py
+-rw-r--r--   0        0        0     4941 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.css
+-rw-r--r--   0        0        0    67546 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.js
+-rw-r--r--   0        0        0    16129 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tables.py
+-rw-r--r--   0        0        0     4714 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/template_content.py
+-rw-r--r--   0        0        0     7593 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliance_device_report.html
+-rw-r--r--   0        0        0     3680 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliance_overview_report.html
+-rw-r--r--   0        0        0     1568 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliance_report.html
+-rw-r--r--   0        0        0     1123 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliancefeature_retrieve.html
+-rw-r--r--   0        0        0     1100 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliancerule_retrieve.html
+-rw-r--r--   0        0        0     3902 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configcompliance.html
+-rw-r--r--   0        0        0     1961 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_details.html
+-rw-r--r--   0        0        0     1127 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_detailsmodal.html
+-rw-r--r--   0        0        0      950 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configremove_retrieve.html
+-rw-r--r--   0        0        0      951 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configreplace_retrieve.html
+-rw-r--r--   0        0        0     4142 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/content_template.html
+-rw-r--r--   0        0        0      365 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/dff2html_base.html
+-rw-r--r--   0        0        0     3616 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html
+-rw-r--r--   0        0        0     3487 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_retrieve.html
+-rw-r--r--   0        0        0     1393 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_update.html
+-rw-r--r--   0        0        0      181 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/manytomany.html
+-rw-r--r--   0        0        0       35 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templatetags/__init__.py
+-rw-r--r--   0        0        0      451 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/templatetags/json_helpers.py
+-rw-r--r--   0        0        0       52 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/__init__.py
+-rw-r--r--   0        0        0    14003 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/conftest.py
+-rw-r--r--   0        0        0       51 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/forms/__init__.py
+-rw-r--r--   0        0        0     3228 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/forms/test_golden_config_settings.py
+-rw-r--r--   0        0        0       83 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/jinja_filters.py
+-rw-r--r--   0        0        0    12405 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_api.py
+-rw-r--r--   0        0        0      995 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_basic.py
+-rw-r--r--   0        0        0     3503 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_datasources.py
+-rw-r--r--   0        0        0    12768 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_filters.py
+-rw-r--r--   0        0        0    12960 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_graphql.py
+-rw-r--r--   0        0        0     5464 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_helpers.py
+-rw-r--r--   0        0        0    12194 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_models.py
+-rw-r--r--   0        0        0       58 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_nornir_plays/__init__.py
+-rw-r--r--   0        0        0     1018 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py
+-rw-r--r--   0        0        0       55 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/__init__.py
+-rw-r--r--   0        0        0     2899 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_git.py
+-rw-r--r--   0        0        0     1247 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_graphql.py
+-rw-r--r--   0        0        0    15214 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_helpers.py
+-rw-r--r--   0        0        0     1284 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_utils.py
+-rw-r--r--   0        0        0    12883 2023-05-05 15:54:13.027758 nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_views.py
+-rw-r--r--   0        0        0     1963 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/urls.py
+-rw-r--r--   0        0        0       17 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/__init__.py
+-rw-r--r--   0        0        0     8758 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/config_postprocessing.py
+-rw-r--r--   0        0        0      627 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/constant.py
+-rw-r--r--   0        0        0      607 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/db_management.py
+-rw-r--r--   0        0        0     2990 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/git.py
+-rw-r--r--   0        0        0     1771 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/graphql.py
+-rw-r--r--   0        0        0     5407 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/helper.py
+-rw-r--r--   0        0        0     3401 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/management.py
+-rw-r--r--   0        0        0     1079 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/utils.py
+-rw-r--r--   0        0        0    33739 2023-05-05 15:54:13.031758 nautobot_golden_config-1.4.0/nautobot_golden_config/views.py
+-rw-r--r--   0        0        0     3753 2023-05-05 15:54:23.583909 nautobot_golden_config-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7982 1970-01-01 00:00:00.000000 nautobot_golden_config-1.4.0/PKG-INFO
```

### Comparing `nautobot_golden_config-1.3.1/LICENSE` & `nautobot_golden_config-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/README.md` & `nautobot_golden_config-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/__init__.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,28 +4,29 @@
     from importlib import metadata
 except ImportError:
     # Python version < 3.8
     import importlib_metadata as metadata
 
 __version__ = metadata.version(__name__)
 
+from django.db.models.signals import post_migrate
 from nautobot.extras.plugins import PluginConfig
 
 
 class GoldenConfig(PluginConfig):
     """Plugin configuration for the nautobot_golden_config plugin."""
 
     name = "nautobot_golden_config"
     verbose_name = "Golden Configuration"
     version = __version__
     author = "Network to Code, LLC"
     author_email = "opensource@networktocode.com"
-    description = "A plugin for managing Golden Configurations."
+    description = "Nautobot Apps that embraces NetDevOps and automates configuration backups, performs configuration compliance, and generates intended configurations. Includes native Git integration and gives users the flexibility to mix and match the supported features."
     base_url = "golden-config"
-    min_version = "1.4.0"
+    min_version = "1.5.3"
     max_version = "1.99"
     default_settings = {
         "enable_backup": True,
         "enable_compliance": True,
         "enable_intended": True,
         "enable_sotagg": True,
         "enable_postprocessing": False,
@@ -33,9 +34,18 @@
         "postprocessing_subscribed": [],
         "per_feature_bar_width": 0.3,
         "per_feature_width": 13,
         "per_feature_height": 4,
         "get_custom_compliance": None,
     }
 
+    def ready(self):
+        """Register custom signals."""
+        from nautobot_golden_config.models import ConfigCompliance  # pylint: disable=import-outside-toplevel
+
+        from .signals import config_compliance_platform_cleanup  # pylint: disable=import-outside-toplevel
+
+        super().ready()
+        post_migrate.connect(config_compliance_platform_cleanup, sender=ConfigCompliance)
+
 
 config = GoldenConfig  # pylint:disable=invalid-name
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/api/serializers.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/api/serializers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,76 +1,77 @@
 """REST API serializer capabilities for graphql plugin."""
 # pylint: disable=too-many-ancestors
 from rest_framework import serializers
 
-from nautobot.extras.api.customfields import CustomFieldModelSerializer
 from nautobot.extras.api.serializers import TaggedObjectSerializer
 from nautobot.extras.api.nested_serializers import NestedDynamicGroupSerializer
 from nautobot.dcim.api.serializers import DeviceSerializer
 from nautobot.dcim.models import Device
+from nautobot.extras.api.serializers import NautobotModelSerializer
+
 
 from nautobot_golden_config import models
 from nautobot_golden_config.utilities.config_postprocessing import get_config_postprocessing
 
 
 class GraphQLSerializer(serializers.Serializer):  # pylint: disable=abstract-method
     """Serializer for a GraphQL object."""
 
     data = serializers.JSONField()
 
 
-class ComplianceFeatureSerializer(TaggedObjectSerializer, CustomFieldModelSerializer):
+class ComplianceFeatureSerializer(NautobotModelSerializer, TaggedObjectSerializer):
     """Serializer for ComplianceFeature object."""
 
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:nautobot_golden_config-api:compliancefeature-detail"
     )
 
     class Meta:
         """Set Meta Data for ComplianceFeature, will serialize all fields."""
 
         model = models.ComplianceFeature
         fields = "__all__"
 
 
-class ComplianceRuleSerializer(TaggedObjectSerializer, CustomFieldModelSerializer):
+class ComplianceRuleSerializer(NautobotModelSerializer, TaggedObjectSerializer):
     """Serializer for ComplianceRule object."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_golden_config-api:compliancerule-detail")
 
     class Meta:
         """Set Meta Data for ComplianceRule, will serialize all fields."""
 
         model = models.ComplianceRule
         fields = "__all__"
 
 
-class ConfigComplianceSerializer(TaggedObjectSerializer, CustomFieldModelSerializer):
+class ConfigComplianceSerializer(NautobotModelSerializer, TaggedObjectSerializer):
     """Serializer for ConfigCompliance object."""
 
     class Meta:
         """Set Meta Data for ConfigCompliance, will serialize fields."""
 
         model = models.ConfigCompliance
         fields = "__all__"
 
 
-class GoldenConfigSerializer(TaggedObjectSerializer, CustomFieldModelSerializer):
+class GoldenConfigSerializer(NautobotModelSerializer, TaggedObjectSerializer):
     """Serializer for GoldenConfig object."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_golden_config-api:goldenconfig-detail")
 
     class Meta:
         """Set Meta Data for GoldenConfig, will serialize all fields."""
 
         model = models.GoldenConfig
         fields = "__all__"
 
 
-class GoldenConfigSettingSerializer(TaggedObjectSerializer, CustomFieldModelSerializer):
+class GoldenConfigSettingSerializer(NautobotModelSerializer, TaggedObjectSerializer):
     """Serializer for GoldenConfigSetting object."""
 
     url = serializers.HyperlinkedIdentityField(
         view_name="plugins-api:nautobot_golden_config-api:goldenconfigsetting-detail"
     )
     scope = serializers.JSONField(required=False)
     dynamic_group = NestedDynamicGroupSerializer(required=False)
@@ -103,27 +104,27 @@
         setting.scope = scope
 
         # Using .save() over .validated_save() as validation is done prior to .create() being called
         setting.save()
         return setting
 
 
-class ConfigRemoveSerializer(TaggedObjectSerializer, CustomFieldModelSerializer):
+class ConfigRemoveSerializer(NautobotModelSerializer, TaggedObjectSerializer):
     """Serializer for ConfigRemove object."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_golden_config-api:configremove-detail")
 
     class Meta:
         """Set Meta Data for ConfigRemove, will serialize all fields."""
 
         model = models.ConfigRemove
         fields = "__all__"
 
 
-class ConfigReplaceSerializer(TaggedObjectSerializer, CustomFieldModelSerializer):
+class ConfigReplaceSerializer(NautobotModelSerializer, TaggedObjectSerializer):
     """Serializer for ConfigReplace object."""
 
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nautobot_golden_config-api:configreplace-detail")
 
     class Meta:
         """Set Meta Data for ConfigReplace, will serialize all fields."""
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/api/urls.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/api/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/api/views.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/api/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from rest_framework.views import APIView
 from rest_framework.response import Response
 from rest_framework.routers import APIRootView
 from rest_framework.permissions import AllowAny, IsAuthenticated, BasePermission
 from rest_framework import mixins, viewsets
 
-from nautobot.extras.api.views import CustomFieldModelViewSet
+from nautobot.extras.api.views import NautobotModelViewSet
 from nautobot.dcim.models import Device
 
 
 from nautobot_golden_config.api import serializers
 from nautobot_golden_config import models
 from nautobot_golden_config import filters
 from nautobot_golden_config.utilities.graphql import graph_ql_query
@@ -36,63 +36,63 @@
         device = Device.objects.get(pk=kwargs["pk"])
         settings = get_device_to_settings_map(queryset=Device.objects.filter(pk=device.pk))[device.id]
         status_code, data = graph_ql_query(request, device, settings.sot_agg_query.query)
         data = json.loads(json.dumps(data))
         return Response(serializers.GraphQLSerializer(data=data).initial_data, status=status_code)
 
 
-class ComplianceRuleViewSet(CustomFieldModelViewSet):  # pylint:disable=too-many-ancestors
+class ComplianceRuleViewSet(NautobotModelViewSet):  # pylint:disable=too-many-ancestors
     """API viewset for interacting with ComplianceRule objects."""
 
     queryset = models.ComplianceRule.objects.all()
     serializer_class = serializers.ComplianceRuleSerializer
     filterset_class = filters.ComplianceRuleFilterSet
 
 
-class ComplianceFeatureViewSet(CustomFieldModelViewSet):  # pylint:disable=too-many-ancestors
+class ComplianceFeatureViewSet(NautobotModelViewSet):  # pylint:disable=too-many-ancestors
     """API viewset for interacting with ComplianceFeature objects."""
 
     queryset = models.ComplianceFeature.objects.all()
     serializer_class = serializers.ComplianceFeatureSerializer
     filterset_class = filters.ComplianceFeatureFilterSet
 
 
-class ConfigComplianceViewSet(CustomFieldModelViewSet):  # pylint:disable=too-many-ancestors
+class ConfigComplianceViewSet(NautobotModelViewSet):  # pylint:disable=too-many-ancestors
     """API viewset for interacting with ConfigCompliance objects."""
 
     queryset = models.ConfigCompliance.objects.all()
     serializer_class = serializers.ConfigComplianceSerializer
     filterset_class = filters.ConfigComplianceFilterSet
 
 
-class GoldenConfigViewSet(CustomFieldModelViewSet):  # pylint:disable=too-many-ancestors
+class GoldenConfigViewSet(NautobotModelViewSet):  # pylint:disable=too-many-ancestors
     """API viewset for interacting with GoldenConfig objects."""
 
     queryset = models.GoldenConfig.objects.all()
     serializer_class = serializers.GoldenConfigSerializer
     filterset_class = filters.GoldenConfigFilterSet
 
 
-class GoldenConfigSettingViewSet(CustomFieldModelViewSet):  # pylint:disable=too-many-ancestors
+class GoldenConfigSettingViewSet(NautobotModelViewSet):  # pylint:disable=too-many-ancestors
     """API viewset for interacting with GoldenConfigSetting objects."""
 
     queryset = models.GoldenConfigSetting.objects.all()
     serializer_class = serializers.GoldenConfigSettingSerializer
     filterset_class = filters.GoldenConfigSettingFilterSet
 
 
-class ConfigRemoveViewSet(CustomFieldModelViewSet):  # pylint:disable=too-many-ancestors
+class ConfigRemoveViewSet(NautobotModelViewSet):  # pylint:disable=too-many-ancestors
     """API viewset for interacting with ConfigRemove objects."""
 
     queryset = models.ConfigRemove.objects.all()
     serializer_class = serializers.ConfigRemoveSerializer
     filterset_class = filters.ConfigRemoveFilterSet
 
 
-class ConfigReplaceViewSet(CustomFieldModelViewSet):  # pylint:disable=too-many-ancestors
+class ConfigReplaceViewSet(NautobotModelViewSet):  # pylint:disable=too-many-ancestors
     """API viewset for interacting with ConfigReplace objects."""
 
     queryset = models.ConfigReplace.objects.all()
     serializer_class = serializers.ConfigReplaceSerializer
     filterset_class = filters.ConfigReplaceFilterSet
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/datasources.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/datasources.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/filters.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 """Filters for UI and API Views."""
 
 import django_filters
-
 from django.db.models import Q
-
-from nautobot.dcim.models import Device, Platform, Region, Site, DeviceRole, DeviceType, Manufacturer, Rack, RackGroup
+from nautobot.dcim.models import Device, DeviceRole, DeviceType, Manufacturer, Platform, Rack, RackGroup, Region, Site
+from nautobot.extras.filters import CustomFieldModelFilterSet, StatusFilter
 from nautobot.extras.models import Status
-from nautobot.extras.filters import StatusFilter, CustomFieldModelFilterSet
 from nautobot.tenancy.models import Tenant, TenantGroup
-from nautobot.utilities.filters import TreeNodeMultipleChoiceFilter, BaseFilterSet, NameSlugSearchFilterSet
-
+from nautobot.utilities.filters import BaseFilterSet, NameSlugSearchFilterSet, TreeNodeMultipleChoiceFilter
 from nautobot_golden_config import models
 
 
 class GenericPlatformFilterSet(CustomFieldModelFilterSet):
     """Generic method to reuse common FilterSet."""
 
     platform_id = django_filters.ModelMultipleChoiceFilter(
@@ -80,18 +77,17 @@
         label="Site name (slug)",
     )
     rack_group_id = TreeNodeMultipleChoiceFilter(
         queryset=RackGroup.objects.all(),
         field_name="device__rack__group",
         label="Rack group (ID)",
     )
-    rack_group = django_filters.ModelMultipleChoiceFilter(
-        field_name="device__rack__group__slug",
+    rack_group = TreeNodeMultipleChoiceFilter(
+        field_name="device__rack__group",
         queryset=RackGroup.objects.all(),
-        to_field_name="slug",
         label="Rack group (slug)",
     )
     rack_id = django_filters.ModelMultipleChoiceFilter(
         field_name="device__rack",
         queryset=Rack.objects.all(),
         label="Rack (ID)",
     )
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/forms.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Forms for Device Configuration Backup."""
+# pylint: disable=too-many-ancestors
 
 from django import forms
 
 import nautobot.extras.forms as extras_forms
 import nautobot.utilities.forms as utilities_forms
 from nautobot.dcim.models import Device, Platform, Region, Site, DeviceRole, DeviceType, Manufacturer, Rack, RackGroup
 from nautobot.extras.models import Status, GitRepository, DynamicGroup
 from nautobot.tenancy.models import Tenant, TenantGroup
 from nautobot.utilities.forms import SlugField
+from nautobot.extras.forms import NautobotFilterForm, NautobotBulkEditForm, NautobotModelForm
 
 
 from nautobot_golden_config import models
 
 # ConfigCompliance
 
 
-class ConfigComplianceFilterForm(utilities_forms.BootstrapMixin, extras_forms.CustomFieldModelFilterFormMixin):
+class ConfigComplianceFilterForm(NautobotFilterForm):
     """Filter Form for ConfigCompliance instances."""
 
     model = models.ConfigCompliance
     # Set field order to be explicit
     field_order = [
         "q",
         "tenant_group",
@@ -100,17 +102,15 @@
         )
         self.order_fields(self.field_order)  # Reorder fields again
 
 
 # ComplianceRule
 
 
-class ComplianceRuleForm(
-    utilities_forms.BootstrapMixin, extras_forms.CustomFieldModelFormMixin, extras_forms.RelationshipModelFormMixin
-):
+class ComplianceRuleForm(NautobotModelForm):
     """Filter Form for ComplianceRule instances."""
 
     platform = utilities_forms.DynamicModelChoiceField(queryset=Platform.objects.all())
 
     class Meta:
         """Boilerplate form Meta data for compliance rule."""
 
@@ -121,32 +121,30 @@
             "description",
             "config_ordered",
             "match_config",
             "config_type",
         )
 
 
-class ComplianceRuleFilterForm(utilities_forms.BootstrapMixin, extras_forms.CustomFieldModelFilterFormMixin):
+class ComplianceRuleFilterForm(NautobotFilterForm):
     """Form for ComplianceRule instances."""
 
     model = models.ComplianceRule
 
     q = forms.CharField(required=False, label="Search")
     platform = utilities_forms.DynamicModelMultipleChoiceField(
         queryset=Platform.objects.all(), to_field_name="slug", required=False, null_option="None"
     )
 
     feature = utilities_forms.DynamicModelMultipleChoiceField(
         queryset=models.ComplianceFeature.objects.all(), required=False
     )
 
 
-class ComplianceRuleBulkEditForm(
-    utilities_forms.BootstrapMixin, extras_forms.TagsBulkEditFormMixin, extras_forms.CustomFieldModelBulkEditFormMixin
-):
+class ComplianceRuleBulkEditForm(NautobotBulkEditForm):
     """BulkEdit form for ComplianceRule instances."""
 
     pk = forms.ModelMultipleChoiceField(queryset=models.ComplianceRule.objects.all(), widget=forms.MultipleHiddenInput)
 
     class Meta:
         """Boilerplate form Meta data for ComplianceRule."""
 
@@ -162,39 +160,35 @@
         model = models.ComplianceRule
         fields = models.ComplianceRule.csv_headers
 
 
 # ComplianceFeature
 
 
-class ComplianceFeatureForm(
-    utilities_forms.BootstrapMixin, extras_forms.CustomFieldModelFormMixin, extras_forms.RelationshipModelFormMixin
-):
+class ComplianceFeatureForm(NautobotModelForm):
     """Filter Form for ComplianceFeature instances."""
 
     slug = SlugField()
 
     class Meta:
         """Boilerplate form Meta data for compliance feature."""
 
         model = models.ComplianceFeature
         fields = ("name", "slug", "description")
 
 
-class ComplianceFeatureFilterForm(utilities_forms.BootstrapMixin, extras_forms.CustomFieldModelFilterFormMixin):
+class ComplianceFeatureFilterForm(NautobotFilterForm):
     """Form for ComplianceFeature instances."""
 
     model = models.ComplianceFeature
     q = forms.CharField(required=False, label="Search")
     name = utilities_forms.DynamicModelChoiceField(queryset=models.ComplianceFeature.objects.all(), required=False)
 
 
-class ComplianceFeatureBulkEditForm(
-    utilities_forms.BootstrapMixin, extras_forms.TagsBulkEditFormMixin, extras_forms.CustomFieldModelBulkEditFormMixin
-):
+class ComplianceFeatureBulkEditForm(NautobotBulkEditForm):
     """BulkEdit form for ComplianceFeature instances."""
 
     pk = forms.ModelMultipleChoiceField(
         queryset=models.ComplianceFeature.objects.all(), widget=forms.MultipleHiddenInput
     )
 
     class Meta:
@@ -212,17 +206,15 @@
         model = models.ComplianceFeature
         fields = models.ComplianceFeature.csv_headers
 
 
 # ConfigRemove
 
 
-class ConfigRemoveForm(
-    utilities_forms.BootstrapMixin, extras_forms.CustomFieldModelFormMixin, extras_forms.RelationshipModelFormMixin
-):
+class ConfigRemoveForm(NautobotModelForm):
     """Filter Form for Line Removal instances."""
 
     platform = utilities_forms.DynamicModelChoiceField(queryset=Platform.objects.all())
 
     class Meta:
         """Boilerplate form Meta data for removal feature."""
 
@@ -231,29 +223,27 @@
             "platform",
             "name",
             "description",
             "regex",
         )
 
 
-class ConfigRemoveFeatureFilterForm(utilities_forms.BootstrapMixin, extras_forms.CustomFieldModelFilterFormMixin):
+class ConfigRemoveFilterForm(NautobotFilterForm):
     """Filter Form for Line Removal."""
 
     model = models.ConfigRemove
     platform = utilities_forms.DynamicModelMultipleChoiceField(
         queryset=Platform.objects.all(), to_field_name="slug", required=False, null_option="None"
     )
     name = utilities_forms.DynamicModelChoiceField(
         queryset=models.ConfigRemove.objects.all(), to_field_name="name", required=False
     )
 
 
-class ConfigRemoveBulkEditForm(
-    utilities_forms.BootstrapMixin, extras_forms.TagsBulkEditFormMixin, extras_forms.CustomFieldModelBulkEditFormMixin
-):
+class ConfigRemoveBulkEditForm(NautobotBulkEditForm):
     """BulkEdit form for ConfigRemove instances."""
 
     pk = forms.ModelMultipleChoiceField(queryset=models.ConfigRemove.objects.all(), widget=forms.MultipleHiddenInput)
 
     class Meta:
         """Boilerplate form Meta data for ConfigRemove."""
 
@@ -269,17 +259,15 @@
         model = models.ConfigRemove
         fields = models.ConfigRemove.csv_headers
 
 
 # ConfigReplace
 
 
-class ConfigReplaceForm(
-    utilities_forms.BootstrapMixin, extras_forms.CustomFieldModelFormMixin, extras_forms.RelationshipModelFormMixin
-):
+class ConfigReplaceForm(NautobotModelForm):
     """Filter Form for Line Removal instances."""
 
     platform = utilities_forms.DynamicModelChoiceField(queryset=Platform.objects.all())
 
     class Meta:
         """Boilerplate form Meta data for removal feature."""
 
@@ -289,15 +277,15 @@
             "name",
             "description",
             "regex",
             "replace",
         )
 
 
-class ConfigReplaceFeatureFilterForm(utilities_forms.BootstrapMixin, extras_forms.CustomFieldModelFilterFormMixin):
+class ConfigReplaceFilterForm(NautobotFilterForm):
     """Filter Form for Line Replacement."""
 
     model = models.ConfigReplace
 
     platform = utilities_forms.DynamicModelMultipleChoiceField(
         queryset=Platform.objects.all(), to_field_name="slug", required=False, null_option="None"
     )
@@ -312,40 +300,36 @@
     class Meta:
         """Boilerplate form Meta data for ConfigReplace."""
 
         model = models.ConfigReplace
         fields = models.ConfigReplace.csv_headers
 
 
-class ConfigReplaceBulkEditForm(
-    utilities_forms.BootstrapMixin, extras_forms.TagsBulkEditFormMixin, extras_forms.CustomFieldModelBulkEditFormMixin
-):
+class ConfigReplaceBulkEditForm(NautobotBulkEditForm):
     """BulkEdit form for ConfigReplace instances."""
 
     pk = forms.ModelMultipleChoiceField(queryset=models.ConfigReplace.objects.all(), widget=forms.MultipleHiddenInput)
 
     class Meta:
         """Boilerplate form Meta data for ConfigReplace."""
 
         nullable_fields = []
 
 
 # GoldenConfigSetting
 
 
-class GoldenConfigSettingFeatureForm(
-    utilities_forms.BootstrapMixin, extras_forms.CustomFieldModelFormMixin, extras_forms.RelationshipModelFormMixin
-):
-    """Filter Form for GoldenConfigSettingFeatureForm instances."""
+class GoldenConfigSettingForm(NautobotModelForm):
+    """Filter Form for GoldenConfigSettingForm instances."""
 
     slug = SlugField()
     dynamic_group = utilities_forms.DynamicModelChoiceField(queryset=DynamicGroup.objects.all(), required=False)
 
     class Meta:
-        """Filter Form Meta Data for GoldenConfigSettingFeatureForm instances."""
+        """Filter Form Meta Data for GoldenConfigSettingForm instances."""
 
         model = models.GoldenConfigSetting
         fields = (
             "name",
             "slug",
             "weight",
             "description",
@@ -358,15 +342,15 @@
             "backup_test_connectivity",
             "dynamic_group",
             "sot_agg_query",
             "tags",
         )
 
 
-class GoldenConfigSettingFilterForm(utilities_forms.BootstrapMixin, extras_forms.CustomFieldModelFilterFormMixin):
+class GoldenConfigSettingFilterForm(NautobotFilterForm):
     """Form for GoldenConfigSetting instances."""
 
     model = models.GoldenConfigSetting
 
     q = forms.CharField(required=False, label="Search")
     name = forms.CharField(required=False)
     weight = forms.IntegerField(required=False)
@@ -378,7 +362,30 @@
         queryset=GitRepository.objects.filter(provided_contents__contains="nautobot_golden_config.intendedconfigs"),
         required=False,
     )
     jinja_repository = forms.ModelChoiceField(
         queryset=GitRepository.objects.filter(provided_contents__contains="nautobot_golden_config.jinjatemplate"),
         required=False,
     )
+
+
+class GoldenConfigSettingCSVForm(extras_forms.CustomFieldModelCSVForm):
+    """CSV Form for GoldenConfigSetting instances."""
+
+    class Meta:
+        """Boilerplate form Meta data for GoldenConfigSetting."""
+
+        model = models.GoldenConfigSetting
+        fields = models.GoldenConfigSetting.csv_headers
+
+
+class GoldenConfigSettingBulkEditForm(NautobotBulkEditForm):
+    """BulkEdit form for GoldenConfigSetting instances."""
+
+    pk = forms.ModelMultipleChoiceField(
+        queryset=models.GoldenConfigSetting.objects.all(), widget=forms.MultipleHiddenInput
+    )
+
+    class Meta:
+        """Boilerplate form Meta data for GoldenConfigSetting."""
+
+        nullable_fields = []
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/jobs.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """Jobs to run backups, intended config, and compliance."""
 # pylint: disable=too-many-function-args
 
 from datetime import datetime
 
-from nautobot.extras.jobs import Job, MultiObjectVar, ObjectVar, BooleanVar
-from nautobot.extras.models import Tag, DynamicGroup, GitRepository
+from nautobot.dcim.models import Device, DeviceRole, DeviceType, Manufacturer, Platform, Rack, RackGroup, Region, Site
 from nautobot.extras.datasources.git import ensure_git_repository
-from nautobot.dcim.models import Device, DeviceRole, DeviceType, Manufacturer, Site, Platform, Region, Rack, RackGroup
+from nautobot.extras.jobs import BooleanVar, Job, MultiObjectVar, ObjectVar
+from nautobot.extras.models import DynamicGroup, GitRepository, Status, Tag
 from nautobot.tenancy.models import Tenant, TenantGroup
-
-from nautobot_golden_config.nornir_plays.config_intended import config_intended
 from nautobot_golden_config.nornir_plays.config_backup import config_backup
 from nautobot_golden_config.nornir_plays.config_compliance import config_compliance
+from nautobot_golden_config.nornir_plays.config_intended import config_intended
 from nautobot_golden_config.utilities.constant import ENABLE_BACKUP, ENABLE_COMPLIANCE, ENABLE_INTENDED
 from nautobot_golden_config.utilities.git import GitRepo
 from nautobot_golden_config.utilities.helper import get_job_filter
 
-
 name = "Golden Configuration"  # pylint: disable=invalid-name
 
 
 def get_refreshed_repos(job_obj, repo_type, data=None):
     """Small wrapper to pull latest branch, and return a GitRepo plugin specific object."""
     devices = get_job_filter(data)
     dynamic_groups = DynamicGroup.objects.exclude(golden_config_setting__isnull=True)
@@ -65,16 +63,22 @@
     rack = MultiObjectVar(model=Rack, required=False)
     role = MultiObjectVar(model=DeviceRole, required=False)
     manufacturer = MultiObjectVar(model=Manufacturer, required=False)
     platform = MultiObjectVar(model=Platform, required=False)
     device_type = MultiObjectVar(model=DeviceType, required=False, display_field="display_name")
     device = MultiObjectVar(model=Device, required=False)
     tag = MultiObjectVar(model=Tag, required=False)
+    status = MultiObjectVar(
+        model=Status,
+        required=False,
+        query_params={"content_types": Device._meta.label_lower},
+        display_field="label",
+        label="Device Status",
+    )
     debug = BooleanVar(description="Enable for more verbose debug logging")
-    # TODO: Add status
 
 
 class ComplianceJob(Job, FormEntry):
     """Job to to run the compliance engine."""
 
     tenant_group = FormEntry.tenant_group
     tenant = FormEntry.tenant
@@ -84,14 +88,15 @@
     rack = FormEntry.rack
     role = FormEntry.role
     manufacturer = FormEntry.manufacturer
     platform = FormEntry.platform
     device_type = FormEntry.device_type
     device = FormEntry.device
     tag = FormEntry.tag
+    status = FormEntry.status
     debug = FormEntry.debug
 
     class Meta:
         """Meta object boilerplate for compliance."""
 
         name = "Perform Configuration Compliance"
         description = "Run configuration compliance on your network infrastructure."
@@ -122,14 +127,15 @@
     rack = FormEntry.rack
     role = FormEntry.role
     manufacturer = FormEntry.manufacturer
     platform = FormEntry.platform
     device_type = FormEntry.device_type
     device = FormEntry.device
     tag = FormEntry.tag
+    status = FormEntry.status
     debug = FormEntry.debug
 
     class Meta:
         """Meta object boilerplate for intended."""
 
         name = "Generate Intended Configurations"
         description = "Generate the configuration for your intended state."
@@ -169,27 +175,27 @@
     rack = FormEntry.rack
     role = FormEntry.role
     manufacturer = FormEntry.manufacturer
     platform = FormEntry.platform
     device_type = FormEntry.device_type
     device = FormEntry.device
     tag = FormEntry.tag
+    status = FormEntry.status
     debug = FormEntry.debug
 
     class Meta:
         """Meta object boilerplate for backup configurations."""
 
         name = "Backup Configurations"
         description = "Backup the configurations of your network devices."
 
     @commit_check
     def run(self, data, commit):
         """Run config backup process."""
         self.log_debug("Starting backup job.")
-
         now = datetime.now()
         self.log_debug("Pull Backup config repo.")
 
         # Instantiate a GitRepo object for each GitRepository in GoldenConfigSettings.
         backup_repos = get_refreshed_repos(job_obj=self, repo_type="backup_repository", data=data)
 
         self.log_debug(f"Starting backup jobs to the following repos: {backup_repos}")
@@ -238,14 +244,15 @@
     rack = FormEntry.rack
     role = FormEntry.role
     manufacturer = FormEntry.manufacturer
     platform = FormEntry.platform
     device_type = FormEntry.device_type
     device = FormEntry.device
     tag = FormEntry.tag
+    status = FormEntry.status
     debug = FormEntry.debug
 
     class Meta:
         """Meta object boilerplate for all jobs to run against multiple devices."""
 
         name = "Execute All Golden Configuration Jobs - Multiple Device"
         description = "Process to run all Golden Configuration jobs configured against multiple devices."
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/management/commands/run_config_backup.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/management/commands/run_config_backup.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/management/commands/run_config_compliance.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/management/commands/run_config_compliance.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/management/commands/run_generate_config.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/management/commands/run_generate_config.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0001_initial.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from django.db import migrations, models
 import django.db.models.deletion
 import taggit.managers
 import uuid
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("extras", "0004_populate_default_status_records"),
         ("dcim", "0004_initial_part_4"),
     ]
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0003_auto_20210510_2356.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0003_auto_20210510_2356.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.1.8 on 2021-05-10 23:56
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("extras", "0004_populate_default_status_records"),
         ("nautobot_golden_config", "0002_custom_data"),
     ]
 
     operations = [
         migrations.AlterField(
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0004_auto_20210616_2234.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0004_auto_20210616_2234.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.1.8 on 2021-06-16 22:34
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("extras", "0004_populate_default_status_records"),
         ("nautobot_golden_config", "0003_auto_20210510_2356"),
     ]
 
     operations = [
         migrations.AlterField(
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0005_json_compliance_rule.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0005_json_compliance_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
             value = getattr(i, attr)
             if value:
                 setattr(i, attr, json.dumps(value))
         i.save()
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("nautobot_golden_config", "0004_auto_20210616_2234"),
     ]
 
     operations = [
         migrations.RunPython(code=jsonify),
         migrations.AlterField(
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     if settings_obj.backup_repository:
         settings_obj.backup_repositories.add(settings_obj.backup_repository)
     if settings_obj.intended_repository:
         settings_obj.intended_repositories.add(settings_obj.intended_repository)
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("extras", "0013_default_fallback_value_computedfield"),
         ("nautobot_golden_config", "0005_json_compliance_rule"),
     ]
 
     operations = [
         migrations.AddField(
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py`

 * *Files identical despite different names*

```diff
@@ -17,15 +17,14 @@
         [
             settings_obj.intended_repository.add(intended_repo)
             for intended_repo in settings_obj.intended_repositories.all()
         ]
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("extras", "0013_default_fallback_value_computedfield"),
         ("nautobot_golden_config", "0006_multi_repo_support_temp_field"),
     ]
 
     operations = [
         migrations.AddField(
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0008_multi_repo_support_final.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0008_multi_repo_support_final.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.1.13 on 2021-12-07 19:33
 
 from django.db import migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("nautobot_golden_config", "0007_multi_repo_support_convert_many"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
             name="goldenconfigsetting",
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("extras", "0018_joblog_data_migration"),
         ("nautobot_golden_config", "0008_multi_repo_support_final"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
     if settings_obj.intended_repository:
         settings_obj.intended_repository_tmp = settings_obj.intended_repository.first()
         settings_obj.save()
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("nautobot_golden_config", "0009_multiple_gc_settings_part_1"),
     ]
 
     operations = [
         migrations.RunPython(convert_many_repos_part1),
     ]
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("nautobot_golden_config", "0010_multiple_gc_settings_part_2"),
     ]
 
     operations = [
         migrations.RemoveField(
             model_name="goldenconfigsetting",
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
     if settings_obj.intended_repository_tmp:
         settings_obj.intended_repository = settings_obj.intended_repository_tmp
         settings_obj.save()
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("nautobot_golden_config", "0011_multiple_gc_settings_part_3"),
     ]
 
     operations = [
         migrations.RunPython(convert_many_repos_part2),
     ]
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     for gc_setting_obj in GoldenConfigSetting.objects.all():
         if gc_setting_obj.sot_agg_query:
             gc_setting_obj.sot_agg_query_tmp = gc_setting_obj.sot_agg_query
             gc_setting_obj.save()
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("nautobot_golden_config", "0014_convert_sotagg_queries_part1"),
     ]
 
     operations = [
         migrations.RunPython(save_existing_sotagg_queries),
     ]
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from datetime import date
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("nautobot_golden_config", "0015_convert_sotagg_queries_part2"),
     ]
 
     operations = [
         migrations.RemoveField(
             model_name="goldenconfigsetting",
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
             gc_setting_obj.sot_agg_query = gqlsq_obj
             gc_setting_obj.save()
             msg = f"Migrated SoTAgg query for Golden Config Setting '{gcsetting_name}'"
             logger.info(msg)
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("nautobot_golden_config", "0016_convert_sotagg_queries_part3"),
     ]
 
     operations = [
         migrations.RunPython(create_and_link_gql_queries),
     ]
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.14 on 2022-07-11 14:18
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("nautobot_golden_config", "0018_convert_sotagg_queries_part5"),
     ]
 
     operations = [
         migrations.AddField(
             model_name="goldenconfigsetting",
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
             description="Automatically generated for nautobot_golden_config version 1.2.0.",
         )
         i.dynamic_group = d_group
         i.save()
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("nautobot_golden_config", "0019_convert_dynamicgroup_part_1"),
     ]
 
     operations = [
         migrations.RunPython(code=create_dynamic_groups),
     ]
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Generated by Django 3.2.14 on 2022-07-11 16:33
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("nautobot_golden_config", "0020_convert_dynamicgroup_part_2"),
     ]
 
     operations = [
         migrations.RemoveField(
             model_name="goldenconfigsetting",
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/models.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """Django Models for tracking the configuration compliance per feature and device."""
 
-import logging
 import json
+import logging
+
 from deepdiff import DeepDiff
-from django.db import models
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ValidationError
+from django.db import models
 from django.shortcuts import reverse
 from django.utils.module_loading import import_string
 from django.utils.text import slugify
-
-from nautobot.extras.models import ObjectChange, DynamicGroup
+from nautobot.core.models.generics import PrimaryModel
+from nautobot.extras.models import DynamicGroup, ObjectChange
 from nautobot.extras.utils import extras_features
 from nautobot.utilities.utils import serialize_object, serialize_object_v2
-from nautobot.core.models.generics import PrimaryModel
 from netutils.config.compliance import feature_compliance
-
 from nautobot_golden_config.choices import ComplianceRuleTypeChoice
+from nautobot_golden_config.utilities.constant import ENABLE_SOTAGG, PLUGIN_CFG
 from nautobot_golden_config.utilities.utils import get_platform
-from nautobot_golden_config.utilities.constant import PLUGIN_CFG
 
 
 LOGGER = logging.getLogger(__name__)
 GRAPHQL_STR_START = "query ($device_id: ID!)"
 
 ERROR_MSG = (
     "There was an issue with the data that was returned by your get_custom_compliance function. "
@@ -131,15 +130,15 @@
 
 
 # The below maps the provided compliance types
 FUNC_MAPPER = {
     ComplianceRuleTypeChoice.TYPE_CLI: _get_cli_compliance,
     ComplianceRuleTypeChoice.TYPE_JSON: _get_json_compliance,
 }
-# The below conditionally add the cusom provided compliance type
+# The below conditionally add the custom provided compliance type
 if PLUGIN_CFG.get("get_custom_compliance"):
     try:
         FUNC_MAPPER[ComplianceRuleTypeChoice.TYPE_CUSTOM] = import_string(PLUGIN_CFG["get_custom_compliance"])
     except Exception as error:  # pylint: disable=broad-except
         msg = (
             "There was an issue attempting to import the get_custom_compliance function of"
             f"{PLUGIN_CFG['get_custom_compliance']}, this is expected with a local configuration issue "
@@ -291,15 +290,17 @@
         """Return absolute URL for instance."""
         return reverse("plugins:nautobot_golden_config:configcompliance", args=[self.pk])
 
     def to_csv(self):
         """Indicates model fields to return as csv."""
         return (self.device.name, self.rule.feature.name, self.compliance)
 
-    def to_objectchange(self, action, related_object=None, object_data_extra=None, object_data_exclude=None):
+    def to_objectchange(
+        self, action, *, related_object=None, object_data_extra=None, object_data_exclude=None
+    ):  # pylint: disable=arguments-differ
         """Remove actual and intended configuration from changelog."""
         if not object_data_exclude:
             object_data_exclude = ["actual", "intended"]
         return ObjectChange(
             changed_object=self,
             object_repr=str(self),
             action=action,
@@ -307,15 +308,15 @@
             object_data_v2=serialize_object_v2(self),
             related_object=related_object,
         )
 
     class Meta:
         """Set unique together fields for model."""
 
-        ordering = ["device"]
+        ordering = ["device", "rule"]
         unique_together = ("device", "rule")
 
     def __str__(self):
         """String representation of a the compliance."""
         return f"{self.device} -> {self.rule} -> {self.compliance}"
 
     def save(self, *args, **kwargs):
@@ -388,15 +389,17 @@
             self.backup_last_success_date,
             self.intended_last_attempt_date,
             self.intended_last_success_date,
             self.compliance_last_attempt_date,
             self.compliance_last_success_date,
         )
 
-    def to_objectchange(self, action, related_object=None, object_data_extra=None, object_data_exclude=None):
+    def to_objectchange(
+        self, action, *, related_object=None, object_data_extra=None, object_data_exclude=None
+    ):  # pylint: disable=arguments-differ
         """Remove actual and intended configuration from changelog."""
         if not object_data_exclude:
             object_data_exclude = ["backup_config", "intended_config", "compliance_config"]
         return ObjectChange(
             changed_object=self,
             object_repr=str(self),
             action=action,
@@ -415,15 +418,15 @@
         return f"{self.device}"
 
 
 @extras_features(
     "graphql",
 )
 class GoldenConfigSetting(PrimaryModel):  # pylint: disable=too-many-ancestors
-    """GoldenConfigSetting Model defintion. This provides global configs instead of via configs.py."""
+    """GoldenConfigSetting Model definition. This provides global configs instead of via configs.py."""
 
     name = models.CharField(max_length=100, unique=True, blank=False)
     slug = models.SlugField(max_length=100, unique=True, blank=False)
     weight = models.PositiveSmallIntegerField(default=1000, blank=False)
     description = models.CharField(
         max_length=200,
         blank=True,
@@ -488,17 +491,33 @@
     )
     dynamic_group = models.OneToOneField(
         to="extras.DynamicGroup",
         on_delete=models.PROTECT,
         related_name="golden_config_setting",
     )
 
+    csv_headers = [
+        "name",
+        "slug",
+        "weight",
+        "description",
+    ]
+
+    def to_csv(self):
+        """Indicates model fields to return as csv."""
+        return (
+            self.name,
+            self.slug,
+            self.weight,
+            self.description,
+        )
+
     def get_absolute_url(self):  # pylint: disable=no-self-use
         """Return absolute URL for instance."""
-        return reverse("plugins:nautobot_golden_config:goldenconfigsetting", args=[self.slug])
+        return reverse("plugins:nautobot_golden_config:goldenconfigsetting", args=[self.pk])
 
     def __str__(self):
         """Return a simple string if model is called."""
         return f"Golden Config Setting - {self.name}"
 
     @property
     def scope(self):
@@ -537,17 +556,20 @@
         verbose_name = "Golden Config Setting"
         ordering = ["-weight", "name"]  # Refer to weight comment in class docstring.
 
     def clean(self):
         """Validate the scope and GraphQL query."""
         super().clean()
 
+        if ENABLE_SOTAGG and not self.sot_agg_query:
+            raise ValidationError("A GraphQL query must be defined when `ENABLE_SOTAGG` is True")
+
         if self.sot_agg_query:
             LOGGER.debug("GraphQL - test  query start with: `%s`", GRAPHQL_STR_START)
-            if not str(self.sot_agg_query.query).startswith(GRAPHQL_STR_START):
+            if not str(self.sot_agg_query.query.lstrip()).startswith(GRAPHQL_STR_START):
                 raise ValidationError(f"The GraphQL query must start with exactly `{GRAPHQL_STR_START}`")
 
     def get_queryset(self):
         """Generate a Device QuerySet from the filter."""
         return self.dynamic_group.members
 
     def device_count(self):
@@ -565,15 +587,15 @@
     "custom_validators",
     "export_templates",
     "graphql",
     "relationships",
     "webhooks",
 )
 class ConfigRemove(PrimaryModel):  # pylint: disable=too-many-ancestors
-    """ConfigRemove for Regex Line Removals from Backup Configuration Model defintion."""
+    """ConfigRemove for Regex Line Removals from Backup Configuration Model definition."""
 
     name = models.CharField(max_length=255, null=False, blank=False)
     platform = models.ForeignKey(
         to="dcim.Platform",
         on_delete=models.CASCADE,
         related_name="backup_line_remove",
         null=False,
@@ -617,15 +639,15 @@
     "custom_validators",
     "export_templates",
     "graphql",
     "relationships",
     "webhooks",
 )
 class ConfigReplace(PrimaryModel):  # pylint: disable=too-many-ancestors
-    """ConfigReplace for Regex Line Replacements from Backup Configuration Model defintion."""
+    """ConfigReplace for Regex Line Replacements from Backup Configuration Model definition."""
 
     name = models.CharField(max_length=255, null=False, blank=False)
     platform = models.ForeignKey(
         to="dcim.Platform",
         on_delete=models.CASCADE,
         related_name="backup_line_replace",
         null=False,
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/navigation.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/navigation.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/nornir_plays/config_backup.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/config_backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,14 @@
                     "credentials_class": NORNIR_SETTINGS.get("credentials"),
                     "params": NORNIR_SETTINGS.get("inventory_params"),
                     "queryset": qs,
                     "defaults": {"now": now},
                 },
             },
         ) as nornir_obj:
-
             nr_with_processors = nornir_obj.with_processors([ProcessGoldenConfig(logger)])
 
             logger.log_debug("Run nornir backup tasks.")
             nr_with_processors.run(
                 task=run_backup,
                 name="BACKUP CONFIG",
                 logger=logger,
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/nornir_plays/config_compliance.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/config_compliance.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,14 @@
                     "credentials_class": NORNIR_SETTINGS.get("credentials"),
                     "params": NORNIR_SETTINGS.get("inventory_params"),
                     "queryset": qs,
                     "defaults": {"now": now},
                 },
             },
         ) as nornir_obj:
-
             nr_with_processors = nornir_obj.with_processors([ProcessGoldenConfig(logger)])
 
             logger.log_debug("Run nornir compliance tasks.")
             nr_with_processors.run(
                 task=run_compliance,
                 name="RENDER COMPLIANCE TASK GROUP",
                 logger=logger,
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/nornir_plays/config_intended.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/config_intended.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 
 from datetime import datetime
 from nornir import InitNornir
 from nornir.core.plugins.inventory import InventoryPluginRegister
 from nornir.core.task import Result, Task
 
-from django_jinja.backend import Jinja2
+from django.template import engines
 
 from nornir_nautobot.exceptions import NornirNautobotException
 from nornir_nautobot.plugins.tasks.dispatcher import dispatcher
 from nornir_nautobot.utils.logger import NornirLogger
 
 from nautobot_plugin_nornir.plugins.inventory.nautobot_orm import NautobotORMInventory
 from nautobot_plugin_nornir.constants import NORNIR_SETTINGS
@@ -28,16 +28,15 @@
 )
 from nautobot_golden_config.utilities.graphql import graph_ql_query
 from nautobot_golden_config.nornir_plays.processor import ProcessGoldenConfig
 
 InventoryPluginRegister.register("nautobot-inventory", NautobotORMInventory)
 LOGGER = logging.getLogger(__name__)
 
-jinja_settings = Jinja2.get_default()
-jinja_env = jinja_settings.env
+jinja_env = engines["jinja"].env
 
 
 @close_threaded_db_connections
 def run_template(  # pylint: disable=too-many-arguments
     task: Task, logger, device_to_settings_map, nautobot_job
 ) -> Result:
     """Render Jinja Template.
@@ -127,15 +126,14 @@
                     "credentials_class": NORNIR_SETTINGS.get("credentials"),
                     "params": NORNIR_SETTINGS.get("inventory_params"),
                     "queryset": qs,
                     "defaults": {"now": now},
                 },
             },
         ) as nornir_obj:
-
             nr_with_processors = nornir_obj.with_processors([ProcessGoldenConfig(logger)])
 
             logger.log_debug("Run nornir render config tasks.")
             # Run the Nornir Tasks
             nr_with_processors.run(
                 task=run_template,
                 name="RENDER CONFIG",
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/nornir_plays/processor.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/nornir_plays/processor.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.css` & `nautobot_golden_config-1.4.0/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.css`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.js` & `nautobot_golden_config-1.4.0/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.13/diff2html.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/tables.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Django Tables2 classes for golden_config plugin."""
 import copy
 
 from django.utils.html import format_html
 from django_tables2 import Column, LinkColumn, TemplateColumn
 from django_tables2.utils import A
 
-from nautobot.dcim.models import Device
 from nautobot.utilities.tables import (
     BaseTable,
     ToggleColumn,
 )
 from nautobot_golden_config import models
 from nautobot_golden_config.utilities.constant import (
     ENABLE_BACKUP,
@@ -128,14 +127,15 @@
             return format_html('<span class="mdi mdi-minus"></span>')
 
 
 #
 # Tables
 #
 
+
 # ConfigCompliance
 class ConfigComplianceTable(BaseTable):
     """Table for rendering a listing of Device entries and their associated ConfigCompliance record status."""
 
     pk = ToggleColumn(accessor=A("device"))
     device = TemplateColumn(
         template_code="""<a href="{% url 'plugins:nautobot_golden_config:configcompliance_devicedetail' pk=record.device  %}" <strong>{{ record.device__name }}</strong></a> """
@@ -233,22 +233,14 @@
 
 # GoldenConfig
 
 
 class GoldenConfigTable(BaseTable):
     """Table to display Config Management Status."""
 
-    def __init__(self, *args, **kwargs):
-        """Remove custom field columns from showing."""
-        super().__init__(*args, **kwargs)
-        for feature in list(self.base_columns.keys()):  # pylint: disable=no-member
-            if feature.startswith("cf_"):
-                self.base_columns.pop(feature)  # pylint: disable=no-member
-                self.sequence.remove(feature)
-
     pk = ToggleColumn()
     name = TemplateColumn(
         template_code="""<a href="{% url 'dcim:device' pk=record.pk %}">{{ record.name }}</a>""",
         verbose_name="Device",
     )
 
     if ENABLE_BACKUP:
@@ -299,15 +291,15 @@
     def render_compliance_last_success_date(self, record, column):  # pylint: disable=no-self-use
         """Pull back compliance last success per row record."""
         return self._render_last_success_date(record, column, "compliance")
 
     class Meta(BaseTable.Meta):
         """Meta for class GoldenConfigTable."""
 
-        model = Device
+        model = models.GoldenConfig
         fields = actual_fields()
 
 
 # ComplianceFeature
 
 
 class ComplianceFeatureTable(BaseTable):
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/template_content.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/template_content.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Added content to the device model view for config compliance."""
 from django.db.models import Count, Q
 from nautobot.dcim.models import Device
 from nautobot.extras.plugins import PluginTemplateExtension
-
 from nautobot_golden_config.models import ConfigCompliance, GoldenConfig
-from nautobot_golden_config.utilities.constant import ENABLE_COMPLIANCE, CONFIG_FEATURES
+from nautobot_golden_config.utilities.constant import CONFIG_FEATURES, ENABLE_COMPLIANCE
 from nautobot_golden_config.utilities.helper import get_device_to_settings_map
 
 
 class ConfigComplianceDeviceCheck(PluginTemplateExtension):  # pylint: disable=abstract-method
     """Plugin extension class for config compliance."""
 
     model = "dcim.device"
@@ -83,13 +82,44 @@
         }
         return self.render(
             "nautobot_golden_config/content_template.html",
             extra_context=extra_context,
         )
 
 
+class ConfigComplianceTenantCheck(PluginTemplateExtension):  # pylint: disable=abstract-method
+    """Plugin extension class for config compliance."""
+
+    model = "tenancy.tenant"
+
+    def get_tenant(self):
+        """Get tenant object."""
+        return self.context["object"]
+
+    def right_page(self):
+        """Content to add to the configuration compliance."""
+        comp_obj = (
+            ConfigCompliance.objects.values("rule__feature__name")
+            .filter(device__tenant=self.get_tenant().id)
+            .annotate(
+                count=Count("rule__feature__name"),
+                compliant=Count("rule__feature__name", filter=Q(compliance=True)),
+                non_compliant=Count("rule__feature__name", filter=~Q(compliance=True)),
+            )
+            .order_by("rule__feature__name")
+            .values("rule__feature__name", "compliant", "non_compliant")
+        )
+        extra_context = {"compliance": comp_obj, "template_type": "site"}
+        return self.render(
+            "nautobot_golden_config/content_template.html",
+            extra_context=extra_context,
+        )
+
+
 extensions = [ConfigDeviceDetails]
 if ENABLE_COMPLIANCE:
     extensions.append(ConfigComplianceDeviceCheck)
     extensions.append(ConfigComplianceSiteCheck)
+    extensions.append(ConfigComplianceTenantCheck)
+
 
 template_extensions = extensions
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/compliance_device_report.html` & `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliance_device_report.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 {% extends 'base.html' %}
 {% load buttons %}
 {% load helpers %}
+{% load json_helpers %}
 {% load static %}
 
 {% block content %}
 <style>
     pre {
         font-size: 10px;
         display: inline-block;
@@ -107,64 +108,64 @@
             {% endif %}
 
         </tr>
         {% if item.ordered %}
             <tr>
                 <td style="width:250px">Configuration</td>
                 <td class="config_hover">
-                    <span id="{{ item.rule|slugify }}_actual"><pre>{{ item.actual|placeholder }}</pre></span>
+                    <span id="{{ item.rule|slugify }}_actual"><pre>{{ item.actual|placeholder|condition_render_json }}</pre></span>
                     <span class="config_hover_button">
                         <button class="btn btn-inline btn-default hover_copy_button" data-clipboard-target="#{{ item.rule|slugify }}_actual">
                             <span class="mdi mdi-content-copy"></span>
                         </button>
                     </span>
                 </td>
             </tr>
         {% else %}
             <tr>
                 <td style="width:250px">Intended Configuration</td>
                 <td class="config_hover">
-                    <span id="{{ item.rule|slugify }}_intended"><pre>{{ item.intended|placeholder }}</pre></span>
+                    <span id="{{ item.rule|slugify }}_intended"><pre>{{ item.intended|placeholder|condition_render_json }}</pre></span>
                     <span class="config_hover_button">
                         <button class="btn btn-inline btn-default hover_copy_button" data-clipboard-target="#{{ item.rule|slugify }}_intended">
                             <span class="mdi mdi-content-copy"></span>
                         </button>
                     </span>
                 </td>
             </tr>
             <tr>
                 <td style="width:250px">Actual Configuration</td>
                 <td class="config_hover">
-                    <span id="{{ item.rule|slugify }}_actual"><pre>{{ item.actual|placeholder }}</pre></span>
+                    <span id="{{ item.rule|slugify }}_actual"><pre>{{ item.actual|placeholder|condition_render_json }}</pre></span>
                     <span class="config_hover_button">
                         <button class="btn btn-inline btn-default hover_copy_button" data-clipboard-target="#{{ item.rule|slugify }}_actual">
                             <span class="mdi mdi-content-copy"></span>
                         </button>
                     </span>
                 </td>
             </tr>
         {% endif %}
         {% if item.missing != "" %}
             <tr>
                 <td style="color:red;width:250px">Missing Configuration</td>
                 <td class="config_hover">
-                    <span id="{{ item.rule|slugify }}_missing"><pre>{{ item.missing }}</pre></span>
+                    <span id="{{ item.rule|slugify }}_missing"><pre>{{ item.missing|condition_render_json }}</pre></span>
                     <span class="config_hover_button">
                         <button class="btn btn-inline btn-default hover_copy_button" data-clipboard-target="#{{ item.rule|slugify }}_missing">
                             <span class="mdi mdi-content-copy"></span>
                         </button>
                     </span>
                 </td>
             </tr>
         {% endif %}
         {% if item.extra != "" %}
             <tr>
                 <td style="color:red;width:250px">Extra Configuration</td>
                 <td class="config_hover">
-                    <span id="{{ item.rule|slugify }}_extra"><pre>{{ item.extra }}</pre></span>
+                    <span id="{{ item.rule|slugify }}_extra"><pre>{{ item.extra|condition_render_json }}</pre></span>
                     <span class="config_hover_button">
                         <button class="btn btn-inline btn-default hover_copy_button" data-clipboard-target="#{{ item.rule|slugify }}_extra">
                             <span class="mdi mdi-content-copy"></span>
                         </button>
                     </span>
                 </td>
             </tr>
```

#### html2text {}

```diff
@@ -1,29 +1,30 @@
-{% extends 'base.html' %} {% load buttons %} {% load helpers %} {% load static
-%} {% block content %}
+{% extends 'base.html' %} {% load buttons %} {% load helpers %} {% load
+json_helpers %} {% load static %} {% block content %}
 ****** {% block title %}Configuration Compliance - {{ device.name }}{% endblock
 %} ******
 {% block navigation %}
 Feature Navigation Compliant Non-Compliant Clear
 {% else %} {% endif %} {{_item.rule_}}
 {% endblock %} {% for item in compliance_details %}
 {{ item.rule.feature.name|upper }}
-Status        Compliant                 Non-Compliant Compliant  Non-Compliant
+Status        Compliant                                       Non-      Compliant Non-
+                                                              Compliant           Compliant
               {
-Configuration { item.actual|placeholder
+Configuration { item.actual|placeholder|condition_render_json
               }}
 
               {
 Intended      {
-Configuration item.intended|placeholder
+Configuration item.intended|placeholder|condition_render_json
               }}
 
               {
-Actual        { item.actual|placeholder
+Actual        { item.actual|placeholder|condition_render_json
 Configuration }}
 
-Missing       {{ item.missing }}
+Missing       {{ item.missing|condition_render_json }}
 Configuration
-Extra         {{ item.extra }}
+Extra         {{ item.extra|condition_render_json }}
 Configuration
 {% endfor %} {% endblock %}  {% block javascript %}
  {% endblock %}
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/compliance_overview_report.html` & `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliance_overview_report.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/compliance_report.html` & `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/compliance_report.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/compliancerule.html` & `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configcompliance.html`

 * *Files 20% similar despite different names*

```diff
@@ -3,93 +3,108 @@
 {% load static %}
 {% load custom_links %}
 {% load helpers %}
 
 {% block title %}{{ object }}{% endblock %}
 
 {% block header %}
-    <div class="row noprint">
-        <div class="col-sm-8 col-md-9">
-            <ol class="breadcrumb">
-                <li>Compliance Rule</li>
-                <li><a href="{% url 'plugins:nautobot_golden_config:compliancerule_list' %}">Compliance Rules</a></li>
-            </ol>
-        </div>
-        <div class="col-sm-4 col-md-3">
-            <form action="{% url 'plugins:nautobot_golden_config:compliancerule_list' %}" method="get">
-                <div class="input-group">
-                    <input type="text" name="q" class="form-control" />
-                    <span class="input-group-btn">
-                        <button type="submit" class="btn btn-primary">
-                            <span class="mdi mdi-magnify" aria-hidden="true"></span>
-                        </button>
-                    </span>
-                </div>
-            </form>
-        </div>
-    </div>
-    <div class="pull-right noprint">
-        {% if perms.nautobot_golden_config.add_compliancerule %}
-            {% clone_button object %}
-        {% endif %}
-        {% if perms.nautobot_golden_config.change_compliancerule %}
-            {% edit_button object use_pk=1 %}
-        {% endif %}
-        {% if perms.nautobot_golden_config.delete_compliancerule %}
-            {% delete_button object use_pk=1 %}
-        {% endif %}
+<div class="row noprint">
+    <div class="col-sm-8 col-md-9">
+        <ol class="breadcrumb">
+            <li>Compliance Feature</li>
+            <li><a href="{% url 'plugins:nautobot_golden_config:configcompliance_list' %}">Compliance Device</a>
+            </li>
+        </ol>
     </div>
-    <h1>{{ object }}</h1>
-    {% include 'inc/created_updated.html' %}
-    <div class="pull-right noprint">
-        {% custom_links object %}
+    <div class="col-sm-4 col-md-3">
+        <form action="{% url 'plugins:nautobot_golden_config:configcompliance_list' %}" method="get">
+            <div class="input-group">
+                <input type="text" name="q" class="form-control" />
+                <span class="input-group-btn">
+                    <button type="submit" class="btn btn-primary">
+                        <span class="mdi mdi-magnify" aria-hidden="true"></span>
+                    </button>
+                </span>
+            </div>
+        </form>
     </div>
-    <ul class="nav nav-tabs">
-        <li role="presentation"{% if not active_tab %} class="active"{% endif %}>
-            <a href="{{ object.get_absolute_url }}">Compliance Rule</a>
-        </li>
-        {% if perms.extras.view_objectchange %}
-            <li role="presentation"{% if active_tab == 'changelog' %} class="active"{% endif %}>
-                <a href="{% url 'plugins:nautobot_golden_config:compliancerule_changelog' pk=object.pk %}">Change Log</a>
-            </li>
-        {% endif %}
-    </ul>
+</div>
+<div class="pull-right noprint">
+{% if perms.nautobot_golden_config.delete_compliancerule %}
+    {% delete_button object use_pk=1 %}
+{% endif %}
+</div>
+<h1>{{ object }}</h1>
+{% include 'inc/created_updated.html' %}
+<div class="pull-right noprint">
+    {% custom_links object %}
+</div>
+<ul class="nav nav-tabs">
+    <li role="presentation" {% if not active_tab %} class="active" {% endif %}>
+        <a href="{{ object.get_absolute_url }}">Config Compliance</a>
+    </li>
+    {% if perms.extras.view_objectchange %}
+    <li role="presentation">
+        <a href="{% url 'plugins:nautobot_golden_config:configcompliance_changelog' pk=object.pk %}">Change Log</a>
+    </li>
+    {% endif %}
+</ul>
 {% endblock %}
 
 {% block content %}
 <div class="row">
-	<div class="col-md-4">
+    <div class="col-md-8">
         <div class="panel panel-default">
             <div class="panel-heading">
                 <strong>Details</strong>
             </div>
             <table class="table table-hover panel-body attr-table">
                 <tr>
-                    <td>Platform</td>
-                    <td>{{ object.platform.name }}</td>
+                    <td>Device Name</td>
+                    <td>{{ object.device }}</td>
                 </tr>
                 <tr>
                     <td>Feature</td>
-                    <td>{{ object.feature.name }}</a></td>
+                    <td>{{ object.rule.feature.name }}</td>
+                </tr>
+                <tr>
+                    <td>Compliance Status</td>
+                    <td>
+                    {% if object.compliance %}
+                        <span class="text-success"><i class="mdi mdi-check-bold"></i></span>
+                    {% else %}
+                        <span class="text-danger"><i class="mdi mdi-close"></i></span>
+                    {% endif %}
+                    </td>
+                </tr>
+                <tr>
+                    <td>Actual Configuration</td>
+                    <td><pre>{{ object.actual }}</pre></td>
                 </tr>
                 <tr>
-                    <td>Description</td>
-                    <td>{{ object.description }}</a></td>
+                    <td>Intended Configuration</td>
+                    <td><pre>{{ object.intended }}</pre></td>
                 </tr>
                 <tr>
-                    <td>Config Ordered</td>
-                    <td>{{ object.config_ordered }}</a></td>
+                    <td>Extra Configuration</td>
+                    <td><pre>{{ object.extra }}</pre></td>
                 </tr>
                 <tr>
-                    <td>Match Config</td>
-                    <td><pre>{{ object.match_config }}</pre></a></td>
+                    <td>Missing Configuration</td>
+                    <td><pre>{{ object.missing }}</pre></td>
                 </tr>
                 <tr>
-                    <td>Config Type</td>
-                    <td>{{ object.config_type }}</a></td>
+                    <td>Ordered</td>
+                    <td>
+                    {% if object.ordered %}
+                        <span class="text-success"><i class="mdi mdi-check-bold"></i></span>
+                    {% else %}
+                        <span class="text-danger"><i class="mdi mdi-close"></i></span>
+                    {% endif %}
+                    </td>
                 </tr>
             </table>
         </div>
         {% include 'inc/custom_fields_panel.html' %}
         {% include 'inc/relationships_panel.html' %}
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,29 +1,28 @@
 {% extends 'base.html' %} {% load buttons %} {% load static %} {% load
 custom_links %} {% load helpers %} {% block title %}{{ object }}{% endblock %}
 {% block header %}
-   1. Compliance Rule
-   2. Compliance_Rules
+   1. Compliance Feature
+   2. Compliance_Device
 [q                   ]
-{% if perms.nautobot_golden_config.add_compliancerule %} {% clone_button object
-%} {% endif %} {% if perms.nautobot_golden_config.change_compliancerule %} {%
-edit_button object use_pk=1 %} {% endif %} {% if
-perms.nautobot_golden_config.delete_compliancerule %} {% delete_button object
-use_pk=1 %} {% endif %}
+{% if perms.nautobot_golden_config.delete_compliancerule %} {% delete_button
+object use_pk=1 %} {% endif %}
 ****** {{ object }} ******
 {% include 'inc/created_updated.html' %}
 {% custom_links object %}
-    * % if not active_tab %} class="active"{% endif %}> Compliance_Rule
+    * % if not active_tab %} class="active" {% endif %}> Config_Compliance
 {% if perms.extras.view_objectchange %}
-% if active_tab == 'changelog' %} class="active"{% endif %}> Change_Log
+Change_Log
 {% endif %}
 {% endblock %} {% block content %}
 Details
-Platform       {{ object.platform.name }}
-Feature        {{ object.feature.name }}
-Description    {{ object.description }}
-Config Ordered {{ object.config_ordered }}
-Match Config   {{ object.match_config }}
-Config Type    {{ object.config_type }}
+Device Name            {{ object.device }}
+Feature                {{ object.rule.feature.name }}
+Compliance Status      {% if object.compliance %}  {% else %}  {% endif %}
+Actual Configuration   {{ object.actual }}
+Intended Configuration {{ object.intended }}
+Extra Configuration    {{ object.extra }}
+Missing Configuration  {{ object.missing }}
+Ordered                {% if object.ordered %}  {% else %}  {% endif %}
 {% include 'inc/custom_fields_panel.html' %} {% include 'inc/
 relationships_panel.html' %}
 {% endblock %}
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/configcompliancedetails.html` & `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_details.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/configcompliancedetails_modal.html` & `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_detailsmodal.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/content_template.html` & `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/content_template.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html` & `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% extends 'base.html' %}
+{% extends 'generic/object_list.html' %}
 {% load buttons %}
 {% load static %}
 {% load helpers %}
 
 {% block content %}
 <div class="pull-right noprint">
 {% block buttons %}
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting.html` & `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_retrieve.html`

 * *Files 12% similar despite different names*

```diff
@@ -12,22 +12,27 @@
       <td>{{ object.weight }}</td>
     </tr>
     <tr>
       <td>Description</td>
       <td>{{ object.description|placeholder }}</td>
     </tr>
     <tr>
-      <td>
-        <a href="{{ object.get_url_to_filtered_device_list }}">Scope of Devices</a>
-        <br/>via <a href="{{ object.dynamic_group.get_absolute_url }}">{{ object.dynamic_group.name }}</a>
-      </td>
+      <td>Dynamic Group</td>
+      <td><a href="{{ object.dynamic_group.get_absolute_url }}">{{ object.dynamic_group.name }}</a></td>
+    </tr>
+    <tr>
+      <td>Filter Query Logic</td>
       <td>
         <pre>{{ object.scope|render_json }}</pre></a>
       </td>
     </tr>
+    <tr>
+      <td>Scope of Devices</td>
+      <td><a href="{{ object.get_url_to_filtered_device_list }}">{{ object.get_url_to_filtered_device_list | length }}</a></td>
+    </tr>
   </table>
 </div>
 {% endblock content_left_page %}
 
 {% block content_right_page %}
 <div class="panel panel-default">
   <div class="panel-heading">
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 {% extends 'generic/object_detail.html' %} {% load helpers %} {% block
 content_left_page %}
 General Settings
-Weight                              {{ object.weight }}
-Description                         {{ object.description|placeholder }}
-Scope_of_Devices                    {{ object.scope|render_json }}
-via {{_object.dynamic_group.name_}}
+Weight             {{ object.weight }}
+Description        {{ object.description|placeholder }}
+Dynamic Group      {{_object.dynamic_group.name_}}
+Filter Query Logic {{ object.scope|render_json }}
+Scope of Devices   {{_object.get_url_to_filtered_device_list_|_length_}}
 {% endblock content_left_page %} {% block content_right_page %}
 Backup Configuration
                                    {% if object.backup_repository %} {
 Backup Repository                  {_object.backup_repository_}} {% else %}
                                    None {% endif %}
 Backup Path in Jinja Template Form {{ object.backup_path_template|placeholder
                                    }}
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_edit.html` & `nautobot_golden_config-1.4.0/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_update.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/tests/conftest.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Params for testing."""
 from django.contrib.contenttypes.models import ContentType
 from django.utils.text import slugify
-
-from nautobot.dcim.models import Device, Site, Manufacturer, DeviceType, DeviceRole, Rack, RackGroup, Region, Platform
-from nautobot.tenancy.models import Tenant, TenantGroup
-from nautobot.extras.models import Status, GitRepository, GraphQLQuery, Tag
+from nautobot.dcim.models import Device, DeviceRole, DeviceType, Manufacturer, Platform, Rack, RackGroup, Region, Site
 from nautobot.extras.datasources.registry import get_datasource_contents
-
-from nautobot_golden_config.models import ConfigCompliance, ComplianceFeature, ComplianceRule
+from nautobot.extras.models import GitRepository, GraphQLQuery, Status, Tag
+from nautobot.tenancy.models import Tenant, TenantGroup
 from nautobot_golden_config.choices import ComplianceRuleTypeChoice
+from nautobot_golden_config.models import ComplianceFeature, ComplianceRule, ConfigCompliance
 
 
 def create_device_data():
     """Creates a Device and associated data."""
     manufacturers = (
         Manufacturer.objects.create(name="Manufacturer 1", slug="manufacturer-1"),
         Manufacturer.objects.create(name="Manufacturer 2", slug="manufacturer-2"),
@@ -140,16 +138,17 @@
     site, _ = Site.objects.get_or_create(name="Site 1", slug="site-1", region=child_region)
     manufacturer, _ = Manufacturer.objects.get_or_create(name="Manufacturer 1", slug="manufacturer-1")
     device_role, _ = DeviceRole.objects.get_or_create(name="Role 1", slug="role-1")
     device_type, _ = DeviceType.objects.get_or_create(
         manufacturer=manufacturer, model="Device Type 1", slug="device-type-1"
     )
     platform, _ = Platform.objects.get_or_create(manufacturer=manufacturer, name="Platform 1", slug="platform-1")
+    status, _ = Status.objects.get_or_create(name="Failed")
     device = Device.objects.create(
-        name=name, platform=platform, site=site, device_role=device_role, device_type=device_type
+        name=name, platform=platform, site=site, device_role=device_role, device_type=device_type, status=status
     )
     return device
 
 
 def create_orphan_device(name="orphan"):
     """Creates a Device to be used with tests."""
     parent_region, _ = Region.objects.get_or_create(name="Parent Region 4", slug="parent_region-4")
@@ -160,16 +159,17 @@
     device_type, _ = DeviceType.objects.get_or_create(
         manufacturer=manufacturer, model="Device Type 4", slug="device-type-4"
     )
     platform, _ = Platform.objects.get_or_create(manufacturer=manufacturer, name="Platform 4", slug="platform-4")
     content_type = ContentType.objects.get(app_label="dcim", model="device")
     tag, _ = Tag.objects.get_or_create(name="Orphaned", slug="orphaned")
     tag.content_types.add(content_type)
+    status, _ = Status.objects.get_or_create(name="Offline")
     device = Device.objects.create(
-        name=name, platform=platform, site=site, device_role=device_role, device_type=device_type
+        name=name, platform=platform, site=site, device_role=device_role, device_type=device_type, status=status
     )
     device.tags.add(tag)
     return device
 
 
 def create_feature_rule_json(device, feature="foo", rule="json"):
     """Creates a Feature/Rule Mapping and Returns the rule."""
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_api.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_basic.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_basic.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import toml
 
 
 class TestDocsPackaging(unittest.TestCase):
     """Test Version in doc requirements is the same pyproject."""
 
     def test_version(self):
-        """Verify that pyproject.toml dev dependecies have the same versions as in the docs requirements.txt."""
+        """Verify that pyproject.toml dev dependencies have the same versions as in the docs requirements.txt."""
         parent_path = os.path.dirname(os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
         poetry_details = toml.load(os.path.join(parent_path, "pyproject.toml"))["tool"]["poetry"]["dev-dependencies"]
         with open(f"{parent_path}/docs/requirements.txt", "r", encoding="utf-8") as file:
             requirements = [line for line in file.read().splitlines() if (len(line) > 0 and not line.startswith("#"))]
         for pkg in requirements:
             if len(pkg.split("==")) == 2:
                 pkg, version = pkg.split("==")
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_datasources.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_datasources.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_filters.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_graphql.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_helpers.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_models.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,19 @@
 """Unit tests for nautobot_golden_config models."""
 
-from django.test import TestCase
-from django.db.utils import IntegrityError
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ValidationError
+from django.db.utils import IntegrityError
+from django.test import TestCase
 from nautobot.dcim.models import Platform
-from nautobot.extras.models import GitRepository, GraphQLQuery, DynamicGroup
+from nautobot.extras.models import DynamicGroup, GitRepository, GraphQLQuery
+from nautobot_golden_config.models import ConfigCompliance, ConfigRemove, ConfigReplace, GoldenConfigSetting
 from nautobot_golden_config.tests.conftest import create_git_repos
 
-from nautobot_golden_config.models import (
-    ConfigCompliance,
-    GoldenConfigSetting,
-    ConfigRemove,
-    ConfigReplace,
-)
-
-from .conftest import create_device, create_feature_rule_json, create_config_compliance, create_saved_queries
+from .conftest import create_config_compliance, create_device, create_feature_rule_json, create_saved_queries
 
 
 class ConfigComplianceModelTestCase(TestCase):
     """Test CRUD operations for ConfigCompliance Model."""
 
     def setUp(self):
         """Set up base objects."""
@@ -70,14 +64,34 @@
             intended={"foo": {"bar-1": "baz"}},
         )
 
         self.assertTrue(cc_obj.compliance)
         self.assertEqual(cc_obj.missing, "")
         self.assertEqual(cc_obj.extra, "")
 
+    def test_config_compliance_signal_change_platform(self):
+        """Make sure signal is working."""
+        ConfigCompliance.objects.create(
+            device=self.device,
+            rule=self.compliance_rule_json,
+            actual={"foo": {"bar-1": "baz"}},
+            intended={"foo": {"bar-1": "baz"}},
+        )
+        self.assertEqual(ConfigCompliance.objects.filter(device=self.device).count(), 1)
+        self.device.platform = Platform.objects.create(name="Platform Change", slug="platform-change")
+        new_rule_json = create_feature_rule_json(self.device)
+
+        ConfigCompliance.objects.create(
+            device=self.device,
+            rule=new_rule_json,
+            actual={"foo": {"bar-1": "baz"}},
+            intended={"foo": {"bar-1": "baz"}},
+        )
+        self.assertEqual(ConfigCompliance.objects.filter(device=self.device).count(), 1)
+
 
 class GoldenConfigTestCase(TestCase):
     """Test GoldenConfig Model."""
 
 
 class ComplianceRuleTestCase(TestCase):
     """Test ComplianceRule Model."""
@@ -115,15 +129,15 @@
             intended_repository=GitRepository.objects.get(name="test-intended-repo-1"),
             dynamic_group=dynamic_group,
         )
 
     def test_absolute_url_success(self):
         """Verify that get_absolute_url() returns the expected URL."""
         url_string = self.global_settings.get_absolute_url()
-        self.assertEqual(url_string, f"/plugins/golden-config/setting/{self.global_settings.slug}/")
+        self.assertEqual(url_string, f"/plugins/golden-config/golden-config-setting/{self.global_settings.pk}")
 
     def test_good_graphql_query_invalid_starts_with(self):
         """Valid graphql query, however invalid in the usage with golden config plugin."""
         self.global_settings.sot_agg_query = GraphQLQuery.objects.get(name="GC-SoTAgg-Query-3")
         with self.assertRaises(ValidationError) as error:
             self.global_settings.clean()
         self.assertEqual(error.exception.message, "The GraphQL query must start with exactly `query ($device_id: ID!)`")
@@ -178,15 +192,15 @@
         self.assertTrue(self.golden_config.backup_test_connectivity)
         self.assertEqual(self.golden_config.jinja_repository, GitRepository.objects.get(name="test-jinja-repo-1"))
         self.assertEqual(self.golden_config.jinja_path_template, "{{ obj.platform.slug }}/main.j2")
         self.assertEqual(self.golden_config.backup_repository, GitRepository.objects.get(name="test-backup-repo-1"))
         self.assertEqual(self.golden_config.intended_repository, GitRepository.objects.get(name="test-intended-repo-1"))
 
     def test_removing_git_repos(self):
-        """Ensure we can remove the Git Repository obejcts from GoldenConfigSetting."""
+        """Ensure we can remove the Git Repository objects from GoldenConfigSetting."""
         GitRepository.objects.all().delete()
         gc = GoldenConfigSetting.objects.all().first()  # pylint: disable=invalid-name
         self.assertEqual(gc.intended_repository, None)
         self.assertEqual(gc.backup_repository, None)
         self.assertEqual(GoldenConfigSetting.objects.all().count(), 1)
 
     def test_clean_up(self):
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_utilities/test_git.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_git.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_utilities/test_graphql.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_graphql.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 # pylint: disable=no-self-use
 
 
 class GraphQLTest(TestCase):
     """Test for the GraphQL Queries."""
 
-    @skip("Update to accomodate uuid vs device")
+    @skip("Update to accommodate uuid vs device")
     @patch("nautobot_golden_config.utilities.graphql.graph_ql_query")
     def test_graph_ql_query(self, mock):
         """Make sure graph_ql_query is called correctly."""
         mock("request", Device.objects.get(name="ams-edge-01"), '{devices(name:"ams-edge-01"){id}}')
         mock.assert_called_with("request", Device.objects.get(name="ams-edge-01"), '{devices(name:"ams-edge-01"){id}}')
 
-    @skip("Update to accomodate uuid vs device")
+    @skip("Update to accommodate uuid vs device")
     def test_bad_graph_ql_query_syntax(self):
         """Ensure invalid GraphQL query results with Error."""
         result = graph_ql_query("request", Device.objects.get(name="ams-edge-01"), "not valid query")
         self.assertEqual(result[0], 400)
         self.assertTrue(result[1]["error"])
         self.assertRegex(result[1].get("error"), r"Syntax Error GraphQL.*")
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_utilities/test_helpers.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """Unit tests for nautobot_golden_config utilities helpers."""
 
-from unittest.mock import patch, MagicMock
+from unittest.mock import MagicMock, patch
 
-from django.test import TestCase
 from django.contrib.contenttypes.models import ContentType
-
-from nornir_nautobot.exceptions import NornirNautobotException
-from nornir_nautobot.utils.logger import NornirLogger
+from django.test import TestCase
 from jinja2 import exceptions as jinja_errors
-
 from nautobot.dcim.models import Device, Platform, Site
-from nautobot.extras.models import GitRepository, Status, DynamicGroup, Tag
+from nautobot.extras.models import DynamicGroup, GitRepository, GraphQLQuery, Status, Tag
+from nornir_nautobot.exceptions import NornirNautobotException
+from nornir_nautobot.utils.logger import NornirLogger
 from nautobot_golden_config.models import GoldenConfigSetting
-from nautobot_golden_config.tests.conftest import create_device, create_orphan_device, create_helper_repo
+from nautobot_golden_config.tests.conftest import create_device, create_helper_repo, create_orphan_device
 from nautobot_golden_config.utilities.helper import (
+    get_device_to_settings_map,
+    get_job_filter,
     null_to_empty,
     render_jinja_template,
-    get_job_filter,
-    get_device_to_settings_map,
 )
 
-
 # pylint: disable=no-self-use
 
 
 class HelpersTest(TestCase):  # pylint: disable=too-many-instance-attributes
     """Test Helper Functions."""
 
     def setUp(self):
@@ -63,47 +60,60 @@
         )
         dynamic_group3 = DynamicGroup.objects.create(
             name="test3 site site-4",
             slug="test3-site-site-4",
             content_type=self.content_type,
             filter={},
         )
+        graphql_query = GraphQLQuery.objects.create(
+            name="testing",
+            query="""
+              query ($device_id: ID!) {
+                device(id: $device_id){
+                  name
+                }
+              }
+            """,
+        )
         self.test_settings_a = GoldenConfigSetting.objects.create(
             name="test_a",
             slug="test_a",
             description="test_a",
             weight=1000,
             backup_repository=GitRepository.objects.get(name="backup-parent_region-1"),
             intended_repository=GitRepository.objects.get(name="intended-parent_region-1"),
             jinja_repository=GitRepository.objects.get(name="test-jinja-repo"),
             # Limit scope to orphaned device only
             dynamic_group=dynamic_group1,
+            sot_agg_query=graphql_query,
         )
 
         self.test_settings_b = GoldenConfigSetting.objects.create(
             name="test_b",
             slug="test_b",
             description="test_b",
             weight=2000,
             backup_repository=GitRepository.objects.get(name="backup-parent_region-2"),
             intended_repository=GitRepository.objects.get(name="intended-parent_region-2"),
             jinja_repository=GitRepository.objects.get(name="test-jinja-repo-2"),
             # Limit scope to orphaned device only
             dynamic_group=dynamic_group2,
+            sot_agg_query=graphql_query,
         )
 
         self.test_settings_c = GoldenConfigSetting.objects.create(
             name="test_c",
             slug="test_c",
             description="test_c",
             weight=1000,
             backup_repository=GitRepository.objects.get(name="backup-parent_region-3"),
             intended_repository=GitRepository.objects.get(name="intended-parent_region-3"),
             jinja_repository=GitRepository.objects.get(name="test-jinja-repo-3"),
             dynamic_group=dynamic_group3,
+            sot_agg_query=graphql_query,
         )
 
         # Device.objects.all().delete()
         create_device(name="test_device")
         create_orphan_device(name="orphan_device")
         self.job_result = MagicMock()
         self.data = MagicMock()
@@ -210,14 +220,39 @@
         self.assertEqual(result.count(), 1)
 
     def test_get_job_filter_tag_success(self):
         """Verify we get a single device returned when providing tag filter that matches on device."""
         result = get_job_filter(data={"tag": Tag.objects.filter(name="Orphaned")})
         self.assertEqual(result.count(), 1)
 
+    def test_get_job_filter_tag_success_and_logic(self):
+        """Verify we get a single device returned when providing multiple tag filter that matches on device."""
+        device = Device.objects.get(name="orphan_device")
+        device_2 = Device.objects.get(name="test_device")
+        content_type = ContentType.objects.get(app_label="dcim", model="device")
+        tag, _ = Tag.objects.get_or_create(name="second-tag", slug="second-tag")
+        tag.content_types.add(content_type)
+        device.tags.add(tag)
+        device_2.tags.add(tag)
+        # Default tag logic is an `AND` not and `OR`.
+        result = get_job_filter(data={"tag": Tag.objects.filter(name__in=["second-tag", "Orphaned"])})
+        self.assertEqual(device.tags.count(), 2)
+        self.assertEqual(device_2.tags.count(), 1)
+        self.assertEqual(result.count(), 1)
+
+    def test_get_job_filter_status_success(self):
+        """Verify we get a single device returned when providing status filter that matches on device."""
+        result = get_job_filter(data={"status": Status.objects.filter(name="Offline")})
+        self.assertEqual(result.count(), 1)
+
+    def test_get_job_filter_multiple_status_success(self):
+        """Verify we get a0 devices returned matching multiple status'."""
+        result = get_job_filter(data={"status": Status.objects.filter(name__in=["Offline", "Failed"])})
+        self.assertEqual(result.count(), 2)
+
     def test_get_job_filter_base_queryset_raise(self):
         """Verify we get raise for having a base_qs with no objects due to bad Golden Config Setting scope."""
         Platform.objects.create(name="Placeholder Platform", slug="placeholder-platform")
         for golden_settings in GoldenConfigSetting.objects.all():
             dynamic_group = DynamicGroup.objects.create(
                 name=f"{golden_settings.name} group",
                 slug=f"{golden_settings.slug}-group",
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/tests/test_utilities/test_utils.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/tests/test_utilities/test_utils.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/config_postprocessing.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/config_postprocessing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Functions related to prepare configuration with postprocessing."""
 from functools import partial
 from typing import Optional
-import jinja2
+from jinja2.sandbox import SandboxedEnvironment
 from jinja2 import exceptions as jinja_errors
 
 from django.http import HttpRequest
 from django.core.exceptions import ObjectDoesNotExist
 from django.utils.module_loading import import_string
 
 from nautobot.dcim.models import Device
@@ -23,19 +23,18 @@
 
 
 def get_secret_by_secret_group_slug(
     user: User,
     secrets_group_slug: str,
     secret_type: str,
     secret_access_type: Optional[str] = SecretsGroupAccessTypeChoices.TYPE_GENERIC,
+    **kwargs,
 ) -> Optional[str]:
     """Gets the secret from a Secret Group slug. To be used as a Jinja filter.
 
-    We assume that there is only one secret group corresponding to a model.
-
     Args:
         user (User): User object that performs API call to render push template with secrets.
         secrets_group_slug (str): Secrets Group slug. It needs to be part of the GraphQL query.
         secret_type (str): Type of secret, such as "username", "password", "token", "secret", or "key".
         secret_access_type (Optional[str], optional): Type of secret such as "Generic", "gNMI", "HTTP(S)". Defaults to "Generic".
 
     Returns:
@@ -48,14 +47,15 @@
 
     if not user.has_perm("extras.view_secretsgroup", secrets_group):
         return f"You have no permission to read this secret {secrets_group_slug}."
 
     return secrets_group.get_secret_value(
         access_type=secret_access_type,
         secret_type=secret_type,
+        **kwargs,
     )
 
 
 def _get_device_agg_data(device, request):
     """Helper method to retrieve GraphQL data from a device."""
     settings = get_device_to_settings_map(Device.objects.filter(pk=device.pk))[device.id]
     _, device_data = graph_ql_query(request, device, settings.sot_agg_query.query)
@@ -77,36 +77,38 @@
     Returns:
         str : Return a string, with the rendered intended configuration with secrets, or an error message.
 
     """
     if not config_postprocessing:
         return ""
 
-    jinja_env = jinja2.Environment(autoescape=True)
-
-    for name, func in jinja2_convenience_function().items():
-        # Only importing the encrypt helpers as complements to get_secrets filter
-        if name in ["encrypt_type5", "encrypt_type7"]:
-            jinja_env.filters[name] = func
-
-    # Wrapper for get_secret filter that includes user argument to ensure
-    # that secrets are only rendered by authorized users.
-    # To call this method, the view verifies that it's an authenticated request.
+    # Based on https://docs.nautobot.com/projects/golden-config/en/latest/dev/dev_adr/#renders-secrets
+    # the Jinja2 environment that starts with Nautobot should not be used.
+    jinja_env = SandboxedEnvironment(autoescape=True)
+
+    # This can only be done safely since the Jinja2 environment does not persist beyond this function.
+    # If the code is changed to use the Nautobot Jinja2 environment, then the request's user must be passed
+    # in via the template code.
     jinja_env.filters["get_secret_by_secret_group_slug"] = partial(get_secret_by_secret_group_slug, request.user)
 
+    netutils_filters = jinja2_convenience_function()
+    for template_name in ["encrypt_type5", "encrypt_type7"]:
+        template_filter = netutils_filters.get(template_name)
+        if template_filter is not None:
+            jinja_env.filters[template_name] = template_filter
+
     try:
         template = jinja_env.from_string(config_postprocessing)
     except jinja_errors.TemplateAssertionError as error:
         return f"Jinja encountered an TemplateAssertionError: '{error}'; check the template for correctness"
 
     device_data = _get_device_agg_data(configs.device, request)
 
     try:
         return template.render(device_data)
-
     except jinja_errors.UndefinedError as error:
         raise RenderConfigToPushError(
             f"Jinja encountered and UndefinedError: {error}, check the template for missing variable definitions.\n"
         ) from error
     except jinja_errors.TemplateSyntaxError as error:  # Also catches subclass of TemplateAssertionError
         raise RenderConfigToPushError(
             f"Jinja encountered a SyntaxError at line number {error.lineno},"
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/constant.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/constant.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/db_management.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/db_management.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/git.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/git.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/graphql.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/graphql.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/helper.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 """Helper functions."""
 # pylint: disable=raise-missing-from
-from jinja2 import exceptions as jinja_errors
-
 from django.db.models import Q
-
-from nautobot.dcim.models import Device
+from jinja2 import exceptions as jinja_errors
 from nautobot.dcim.filters import DeviceFilterSet
+from nautobot.dcim.models import Device
 from nautobot.utilities.utils import render_jinja2
-
 from nornir_nautobot.exceptions import NornirNautobotException
 
 from nautobot_golden_config import models
 
-
-FIELDS = {
+FIELDS_PK = {
     "platform",
     "tenant_group",
     "tenant",
     "region",
     "site",
     "role",
     "rack",
     "rack_group",
     "manufacturer",
     "device_type",
 }
 
+FIELDS_SLUG = {"tag", "status"}
+
 
 def get_job_filter(data=None):
     """Helper function to return a the filterable list of OS's based on platform.slug and a specific custom value."""
     if not data:
         data = {}
     query = {}
 
     # Translate instances from FIELDS set to list of primary keys
-    for field in FIELDS:
+    for field in FIELDS_PK:
         if data.get(field):
             query[f"{field}_id"] = data[field].values_list("pk", flat=True)
 
-    # Build tag query based on slug values for each instance
-    if data.get("tag"):
-        query.update({"tag": data["tag"].values_list("slug", flat=True)})
+    # Translate instances from FIELDS set to list of slugs
+    for field in FIELDS_SLUG:
+        if data.get(field):
+            query[f"{field}"] = data[field].values_list("slug", flat=True)
 
     # Handle case where object is from single device run all.
     if data.get("device") and isinstance(data["device"], Device):
         query.update({"id": [str(data["device"].pk)]})
     elif data.get("device"):
         query.update({"id": data["device"].values_list("pk", flat=True)})
 
@@ -56,15 +55,17 @@
 
     base_qs = Device.objects.filter(raw_qs)
 
     if not base_qs.exists():
         raise NornirNautobotException(
             "The base queryset didn't find any devices. Please check the Golden Config Setting scope."
         )
+
     devices_filtered = DeviceFilterSet(data=query, queryset=base_qs)
+
     if not devices_filtered.qs.exists():
         raise NornirNautobotException(
             "The provided job parameters didn't match any devices detected by the Golden Config scope. Please check the scope defined within Golden Config Settings or select the correct job parameters to correctly match devices."
         )
     devices_no_platform = devices_filtered.qs.filter(platform__isnull=True)
     if devices_no_platform.exists():
         raise NornirNautobotException(
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/management.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/management.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     # Wait on the job to finish
     while job_result.status not in JobResultStatusChoices.TERMINAL_STATE_CHOICES:
         time.sleep(1)
         job_result = JobResult.objects.get(pk=job_result.pk)
 
     # Report on success/failure
     for test_name, attrs in job_result.data.items():
-
         if test_name in ["total", "output"]:
             continue
 
         handle_class.stdout.write(
             f"\t{test_name}: {attrs['success']} success, {attrs['info']} info, {attrs['warning']} warning, {attrs['failure']} failure"
         )
```

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/utilities/utils.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-1.3.1/nautobot_golden_config/views.py` & `nautobot_golden_config-1.4.0/nautobot_golden_config/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,29 +13,31 @@
 from django.contrib import messages
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.models import Count, ExpressionWrapper, F, FloatField, Max, ProtectedError, Q
 from django.forms import ModelMultipleChoiceField, MultipleHiddenInput
 from django.shortcuts import redirect, render
 from django_pivot.pivot import pivot
 from nautobot.core.views import generic
+from nautobot.core.views.viewsets import NautobotUIViewSet
 from nautobot.dcim.filters import DeviceFilterSet
 from nautobot.dcim.forms import DeviceFilterForm
 from nautobot.dcim.models import Device
-from nautobot.extras.models import CustomField
 from nautobot.utilities.error_handlers import handle_protectederror
 from nautobot.utilities.forms import ConfirmationForm
 from nautobot.utilities.utils import csv_format
 from nautobot.utilities.views import ContentTypePermissionRequiredMixin
 
 from nautobot_golden_config import filters, forms, models, tables
+from nautobot_golden_config.api import serializers
 from nautobot_golden_config.utilities.constant import CONFIG_FEATURES, ENABLE_COMPLIANCE, PLUGIN_CFG
 from nautobot_golden_config.utilities.graphql import graph_ql_query
 from nautobot_golden_config.utilities.helper import get_device_to_settings_map
 from nautobot_golden_config.utilities.config_postprocessing import get_config_postprocessing
 
+
 LOGGER = logging.getLogger(__name__)
 
 GREEN = "#D5E8D4"
 RED = "#F8CECC"
 
 #
 # GoldenConfig
@@ -46,14 +48,15 @@
     """View for displaying the configuration management status for backup, intended, diff, and SoT Agg."""
 
     table = tables.GoldenConfigTable
     filterset = DeviceFilterSet
     filterset_form = DeviceFilterForm
     queryset = Device.objects.all()
     template_name = "nautobot_golden_config/goldenconfig_list.html"
+    action_buttons = ("export",)
 
     def extra_context(self):
         """Boilerplace code to modify data before returning."""
         return CONFIG_FEATURES
 
     def alter_queryset(self, request):
         """Build actual runtime queryset as the build time queryset provides no information."""
@@ -69,38 +72,39 @@
             intended_last_success_date=F("goldenconfig__intended_last_success_date"),
             compliance_last_success_date=F("goldenconfig__compliance_last_success_date"),
             backup_last_attempt_date=F("goldenconfig__backup_last_attempt_date"),
             intended_last_attempt_date=F("goldenconfig__intended_last_attempt_date"),
             compliance_last_attempt_date=F("goldenconfig__compliance_last_attempt_date"),
         )
 
+    @property
+    def dynamic_group_queryset(self):
+        """Return queryset of DynamicGroups associated with all GoldenConfigSettings."""
+        golden_config_device_queryset = Device.objects.none()
+        for setting in models.GoldenConfigSetting.objects.all():
+            golden_config_device_queryset = golden_config_device_queryset | setting.dynamic_group.members
+        return golden_config_device_queryset
+
     def queryset_to_csv(self):
         """Override nautobot default to account for using Device model for GoldenConfig data."""
-        csv_data = []
-        custom_fields = []
-
-        # Start with the column headers
-        headers = models.GoldenConfig.csv_headers.copy()
-
-        # Add custom field headers, if any
-        if hasattr(models.GoldenConfig, "_custom_field_data"):
-            for custom_field in CustomField.objects.get_for_model(models.GoldenConfig):
-                headers.append(custom_field.name)
-                custom_fields.append(custom_field.name)
-
-        csv_data.append(",".join(headers))
-
-        # Iterate through the queryset appending each object
-        for obj in self.alter_queryset(None):
-            data = obj.to_csv()
-
-            for custom_field in custom_fields:
-                data += (obj.cf.get(custom_field, ""),)
-
-            csv_data.append(csv_format(data))
+        golden_config_devices_in_scope = self.dynamic_group_queryset
+        csv_headers = models.GoldenConfig.csv_headers.copy()
+        # Exclude GoldenConfig entries no longer in scope
+        golden_config_entries_in_scope = models.GoldenConfig.objects.filter(device__in=golden_config_devices_in_scope)
+        golden_config_entries_as_csv = [csv_format(entry.to_csv()) for entry in golden_config_entries_in_scope]
+        # Account for devices in scope without GoldenConfig entries
+        commas = "," * (len(csv_headers) - 1)
+        devices_in_scope_without_golden_config_entries_as_csv = [
+            f"{device.name}{commas}" for device in golden_config_devices_in_scope.filter(goldenconfig__isnull=True)
+        ]
+        csv_data = (
+            [",".join(csv_headers)]
+            + golden_config_entries_as_csv
+            + devices_in_scope_without_golden_config_entries_as_csv
+        )
 
         return "\n".join(csv_data)
 
 
 class GoldenConfigBulkDeleteView(generic.BulkDeleteView):
     """Standard view for bulk deletion of data."""
 
@@ -406,15 +410,19 @@
 
         if config_type == "sotagg":
             if request.GET.get("format") in ["json", "yaml"]:
                 structure_format = request.GET.get("format")
 
             settings = get_device_to_settings_map(queryset=Device.objects.filter(pk=device.pk))
             if device.id in settings:
-                _, output = graph_ql_query(request, device, settings[device.id].sot_agg_query.query)
+                sot_agg_query_setting = settings[device.id].sot_agg_query
+                if sot_agg_query_setting is not None:
+                    _, output = graph_ql_query(request, device, sot_agg_query_setting.query)
+                else:
+                    output = {"Error": "No saved `GraphQL Query` query was configured in the `Golden Config Setting`"}
             else:
                 raise ObjectDoesNotExist(f"{device.name} does not map to a Golden Config Setting.")
 
             if structure_format == "yaml":
                 output = yaml.dump(json.loads(json.dumps(output)), default_flow_style=False)
             else:
                 output = json.dumps(output, indent=4)
@@ -480,17 +488,17 @@
                     + intended_date
                     + "\n"
                     + output[first_occurence:second_occurence]
                     + "@@"
                     + output[second_occurence + 2 :]
                 )
 
-        template_name = "nautobot_golden_config/configcompliancedetails.html"
+        template_name = "nautobot_golden_config/configcompliance_details.html"
         if request.GET.get("modal") == "true":
-            template_name = "nautobot_golden_config/configcompliancedetails_modal.html"
+            template_name = "nautobot_golden_config/configcompliance_detailsmodal.html"
 
         return render(
             request,
             template_name,
             {
                 "output": output,
                 "device_name": device.name,
@@ -711,309 +719,75 @@
             csv_data.append(
                 ",".join([f"{str(val)} %" if key == "comp_percent" else str(val) for key, val in obj.items()])
             )
 
         return "\n".join(csv_data)
 
 
-#
-# ComplianceFeature
-#
-
-
-class ComplianceFeatureListView(generic.ObjectListView):
-    """View for managing the config compliance rule definition."""
+class ComplianceFeatureUIViewSet(NautobotUIViewSet):
+    """Views for the ComplianceFeature model."""
 
-    table = tables.ComplianceFeatureTable
-    filterset = filters.ComplianceFeatureFilterSet
-    filterset_form = forms.ComplianceFeatureFilterForm
+    bulk_create_form_class = forms.ComplianceFeatureCSVForm
+    bulk_update_form_class = forms.ComplianceFeatureBulkEditForm
+    filterset_class = filters.ComplianceFeatureFilterSet
+    filterset_form_class = forms.ComplianceFeatureFilterForm
+    form_class = forms.ComplianceFeatureForm
     queryset = models.ComplianceFeature.objects.all()
-    # TODO: Get import working
-    action_buttons = ("add", "export")
-
-
-class ComplianceFeatureView(generic.ObjectView):
-    """View for single ComplianceFeature instance."""
-
-    queryset = models.ComplianceFeature.objects.all()
-
-    def get_extra_context(self, request, instance):
-        """Add extra data to detail view for Nautobot."""
-        return {}
-
-
-class ComplianceFeatureBulkImportView(generic.BulkImportView):
-    """View for bulk import of ComplianceFeature."""
-
-    queryset = models.ComplianceFeature.objects.all()
-    model_form = forms.ComplianceFeatureCSVForm
-    table = tables.ComplianceFeatureTable
-
-
-class ComplianceFeatureEditView(generic.ObjectEditView):
-    """View for managing compliance rules."""
-
-    queryset = models.ComplianceFeature.objects.all()
-    model_form = forms.ComplianceFeatureForm
-
-
-class ComplianceFeatureDeleteView(generic.ObjectDeleteView):
-    """View for deleting compliance rules."""
-
-    queryset = models.ComplianceFeature.objects.all()
-
-
-class ComplianceFeatureBulkDeleteView(generic.BulkDeleteView):
-    """View for bulk deleting compliance rules."""
-
-    queryset = models.ComplianceFeature.objects.all()
-    table = tables.ComplianceFeatureTable
-
+    serializer_class = serializers.ComplianceFeatureSerializer
+    table_class = tables.ComplianceFeatureTable
+    lookup_field = "pk"
 
-class ComplianceFeatureBulkEditView(generic.BulkEditView):
-    """View for bulk deleting ComplianceFeature instance."""
-
-    queryset = models.ComplianceFeature.objects.all()
-    filterset = filters.ComplianceFeatureFilterSet
-    table = tables.ComplianceFeatureTable
-    form = forms.ComplianceFeatureBulkEditForm
-
-
-#
-# ComplianceRule
-#
-
-
-class ComplianceRuleListView(generic.ObjectListView):
-    """View for managing the config compliance rule definition."""
-
-    table = tables.ComplianceRuleTable
-    filterset = filters.ComplianceRuleFilterSet
-    filterset_form = forms.ComplianceRuleFilterForm
-    queryset = models.ComplianceRule.objects.all()
-    # TODO: Get import working
-    action_buttons = ("add", "export")
-
-
-class ComplianceRuleView(generic.ObjectView):
-    """View for single ComplianceRule instance."""
-
-    queryset = models.ComplianceRule.objects.all()
-
-    def get_extra_context(self, request, instance):
-        """Add extra data to detail view for Nautobot."""
-        return {}
-
-
-class ComplianceRuleBulkImportView(generic.BulkImportView):
-    """View for bulk import of ComplianceRule."""
-
-    queryset = models.ComplianceRule.objects.all()
-    model_form = forms.ComplianceRuleCSVForm
-    table = tables.ComplianceRuleTable
-
-
-class ComplianceRuleEditView(generic.ObjectEditView):
-    """View for managing compliance rules."""
 
+class ComplianceRuleUIViewSet(NautobotUIViewSet):
+    """Views for the ComplianceRule model."""
+
+    bulk_create_form_class = forms.ComplianceRuleCSVForm
+    bulk_update_form_class = forms.ComplianceRuleBulkEditForm
+    filterset_class = filters.ComplianceRuleFilterSet
+    filterset_form_class = forms.ComplianceRuleFilterForm
+    form_class = forms.ComplianceRuleForm
     queryset = models.ComplianceRule.objects.all()
-    model_form = forms.ComplianceRuleForm
-
-
-class ComplianceRuleDeleteView(generic.ObjectDeleteView):
-    """View for deleting compliance rules."""
-
-    queryset = models.ComplianceRule.objects.all()
-
-
-class ComplianceRuleBulkDeleteView(generic.BulkDeleteView):
-    """View for bulk deleting compliance rules."""
-
-    queryset = models.ComplianceRule.objects.all()
-    table = tables.ComplianceRuleTable
-
-
-class ComplianceRuleBulkEditView(generic.BulkEditView):
-    """View for bulk deleting ComplianceRule instance."""
-
-    queryset = models.ComplianceRule.objects.all()
-    filterset = filters.ComplianceRuleFilterSet
-    table = tables.ComplianceRuleTable
-    form = forms.ComplianceRuleBulkEditForm
-
-
-#
-# GoldenConfigSetting
-#
-class GoldenConfigSettingView(generic.ObjectView):
-    """View for single GoldenConfigSetting instance."""
-
-    queryset = models.GoldenConfigSetting.objects.all()
-
-    # def get_extra_context(self, request, instance):
-    #     """Add extra data to detail view for Nautobot."""
-    #     return {}
-
-
-class GoldenConfigSettingCreateView(generic.ObjectEditView):
-    """Create view."""
-
-    model = models.GoldenConfigSetting
-    queryset = models.GoldenConfigSetting.objects.all()
-    model_form = forms.GoldenConfigSettingFeatureForm
-    template_name = "nautobot_golden_config/goldenconfigsetting_edit.html"
-
-
-class GoldenConfigSettingDeleteView(generic.ObjectDeleteView):
-    """Delete view."""
-
-    model = models.GoldenConfigSetting
-    queryset = models.GoldenConfigSetting.objects.all()
-
+    serializer_class = serializers.ComplianceRuleSerializer
+    table_class = tables.ComplianceRuleTable
+    lookup_field = "pk"
 
-class GoldenConfigSettingBulkDeleteView(generic.BulkDeleteView):
-    """Delete view."""
 
+class GoldenConfigSettingUIViewSet(NautobotUIViewSet):
+    """Views for the GoldenConfigSetting model."""
+
+    bulk_create_form_class = forms.GoldenConfigSettingCSVForm
+    bulk_update_form_class = forms.GoldenConfigSettingBulkEditForm
+    filterset_class = filters.GoldenConfigSettingFilterSet
+    filterset_form_class = forms.GoldenConfigSettingFilterForm
+    form_class = forms.GoldenConfigSettingForm
     queryset = models.GoldenConfigSetting.objects.all()
-    table = tables.GoldenConfigSettingTable
+    serializer_class = serializers.GoldenConfigSettingSerializer
+    table_class = tables.GoldenConfigSettingTable
+    lookup_field = "pk"
 
 
-class GoldenConfigSettingEditView(generic.ObjectEditView):
-    """Edit view."""
-
-    model = models.GoldenConfigSetting
-    queryset = models.GoldenConfigSetting.objects.all()
-    model_form = forms.GoldenConfigSettingFeatureForm
-    template_name = "nautobot_golden_config/goldenconfigsetting_edit.html"
-
-
-class GoldenConfigSettingListView(generic.ObjectListView):
-    """List view."""
-
-    queryset = models.GoldenConfigSetting.objects.all()
-    table = tables.GoldenConfigSettingTable
-    filterset = filters.GoldenConfigSettingFilterSet
-    filterset_form = forms.GoldenConfigSettingFilterForm
-    # TODO: Get import working
-    action_buttons = ("add", "export")
-
-
-#
-# ConfigRemove
-#
-
-
-class ConfigRemoveListView(generic.ObjectListView):
-    """View to display the current Line Removals."""
-
-    queryset = models.ConfigRemove.objects.all()
-    table = tables.ConfigRemoveTable
-    filterset = filters.ConfigRemoveFilterSet
-    filterset_form = forms.ConfigRemoveFeatureFilterForm
-
-
-class ConfigRemoveView(generic.ObjectView):
-    """View for single ConfigRemove instance."""
-
+class ConfigRemoveUIViewSet(NautobotUIViewSet):
+    """Views for the ConfigRemove model."""
+
+    bulk_create_form_class = forms.ConfigRemoveCSVForm
+    bulk_update_form_class = forms.ConfigRemoveBulkEditForm
+    filterset_class = filters.ConfigRemoveFilterSet
+    filterset_form_class = forms.ConfigRemoveFilterForm
+    form_class = forms.ConfigRemoveForm
     queryset = models.ConfigRemove.objects.all()
+    serializer_class = serializers.ConfigRemoveSerializer
+    table_class = tables.ConfigRemoveTable
+    lookup_field = "pk"
 
-    def get_extra_context(self, request, instance):
-        """Add extra data to detail view for Nautobot."""
-        return {}
-
-
-class ConfigRemoveBulkImportView(generic.BulkImportView):
-    """View for bulk import of ConfigRemove."""
-
-    queryset = models.ConfigRemove.objects.all()
-    model_form = forms.ConfigRemoveCSVForm
-    table = tables.ConfigRemoveTable
-
-
-class ConfigRemoveBulkEditView(generic.BulkEditView):
-    """View for bulk deleting ConfigRemove instances."""
-
-    queryset = models.ConfigRemove.objects.all()
-    filterset = filters.ConfigRemoveFilterSet
-    table = tables.ConfigRemoveTable
-    form = forms.ConfigRemoveBulkEditForm
-
-
-class ConfigRemoveEditView(generic.ObjectEditView):
-    """View for editing the current Line Removals."""
-
-    queryset = models.ConfigRemove.objects.all()
-    model_form = forms.ConfigRemoveForm
-
-
-class ConfigRemoveDeleteView(generic.ObjectDeleteView):
-    """View for deleting a ConfigRemove instance."""
-
-    queryset = models.ConfigRemove.objects.all()
-
-
-class ConfigRemoveBulkDeleteView(generic.BulkDeleteView):
-    """View for bulk deleting Line Removals."""
-
-    queryset = models.ConfigRemove.objects.all()
-    table = tables.ConfigRemoveTable
-
-
-#
-# ConfigReplace
-#
-
-
-class ConfigReplaceListView(generic.ObjectListView):
-    """View for displaying the current Line Replacements."""
-
-    queryset = models.ConfigReplace.objects.all()
-    table = tables.ConfigReplaceTable
-    filterset = filters.ConfigReplaceFilterSet
-    filterset_form = forms.ConfigReplaceFeatureFilterForm
-
-
-class ConfigReplaceView(generic.ObjectView):
-    """View for single ConfigReplace instance."""
-
-    queryset = models.ConfigReplace.objects.all()
-
-    def get_extra_context(self, request, instance):
-        """Add extra data to detail view for Nautobot."""
-        return {}
-
-
-class ConfigReplaceEditView(generic.ObjectEditView):
-    """View for editing the current Line Replacements."""
-
-    queryset = models.ConfigReplace.objects.all()
-    model_form = forms.ConfigReplaceForm
-
-
-class ConfigReplaceBulkDeleteView(generic.BulkDeleteView):
-    """View for bulk deleting Line Replacements."""
-
-    queryset = models.ConfigReplace.objects.all()
-    table = tables.ConfigReplaceTable
-
-
-class ConfigReplaceBulkImportView(generic.BulkImportView):
-    """View for bulk import of ConfigReplace."""
-
-    queryset = models.ConfigReplace.objects.all()
-    model_form = forms.ConfigReplaceCSVForm
-    table = tables.ConfigReplaceTable
-
-
-class ConfigReplaceDeleteView(generic.ObjectDeleteView):
-    """View for deleting a ConfigReplace instance."""
-
-    queryset = models.ConfigReplace.objects.all()
-
-
-class ConfigReplaceBulkEditView(generic.BulkEditView):
-    """View for bulk deleting ConfigReplace instances."""
 
+class ConfigReplaceUIViewSet(NautobotUIViewSet):
+    """Views for the ConfigReplace model."""
+
+    bulk_create_form_class = forms.ConfigReplaceCSVForm
+    bulk_update_form_class = forms.ConfigReplaceBulkEditForm
+    filterset_class = filters.ConfigReplaceFilterSet
+    filterset_form_class = forms.ConfigReplaceFilterForm
+    form_class = forms.ConfigReplaceForm
     queryset = models.ConfigReplace.objects.all()
-    filterset = filters.ConfigReplaceFilterSet
-    table = tables.ConfigReplaceTable
-    form = forms.ConfigReplaceBulkEditForm
+    serializer_class = serializers.ConfigReplaceSerializer
+    table_class = tables.ConfigReplaceTable
+    lookup_field = "pk"
```

### Comparing `nautobot_golden_config-1.3.1/pyproject.toml` & `nautobot_golden_config-1.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-golden-config"
-version = "v1.3.1"
+version = "v1.4.0"
 description = "A plugin for configuration on nautobot"
 authors = ["Network to Code, LLC", "<opensource@networktocode.com>"]
 
 license = "Apache-2.0"
 
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-plugin-golden-config"
@@ -26,37 +26,41 @@
 ]
 packages = [
     { include = "nautobot_golden_config" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-deepdiff = "^5.5.0"
+deepdiff = ">=5.5.0,>=6.2.0"
 django-pivot = "^1.8.1"
 matplotlib = "^3.3.2"
-## Setting as next to test with DynamicGroup changes
-nautobot = ">=1.4.0"
+nautobot = ">=1.5.3"
 nautobot-plugin-nornir = ">=1.0.0"
 
 [tool.poetry.dev-dependencies]
 bandit = "*"
+# Black 23.x.x configuration changes and migration files are taken into account
 black = "*"
 django-debug-toolbar = "*"
 # we need to pin flake8 because of package dependencies that cause it to downgrade and
 # therefore cause issues with linting since older versions do not take .flake8 as config
 flake8 = "^3.9.2"
 invoke = "*"
 pydocstyle = "*"
 pylint = "*"
 pylint-django = "*"
 yamllint = "*"
 Markdown = "*"
-# documentation dependencies
+# Rendering docs to HTML
 mkdocs = "1.3.1"
-mkdocs-material = "8.3.9"
+# Material for MkDocs theme
+mkdocs-material = "8.4.2"
+# Render custom markdown for version added/changed/remove notes
+mkdocs-version-annotations = "1.0.0"
+# Automatic documentation from sources, for MkDocs
 mkdocstrings = "0.19"
 mkdocstrings-python = "0.7.1"
 
 [tool.black]
 line-length = 120
 target-version = ['py37']
 include = '\.pyi?$'
```

### Comparing `nautobot_golden_config-1.3.1/setup.py` & `nautobot_golden_config-1.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,108 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nautobot-golden-config
+Version: 1.4.0
+Summary: A plugin for configuration on nautobot
+Home-page: https://github.com/nautobot/nautobot-plugin-golden-config
+License: Apache-2.0
+Keywords: nautobot,nautobot-plugin
+Author: Network to Code, LLC
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: deepdiff (>=6.2.0)
+Requires-Dist: django-pivot (>=1.8.1,<2.0.0)
+Requires-Dist: matplotlib (>=3.3.2,<4.0.0)
+Requires-Dist: nautobot (>=1.5.3)
+Requires-Dist: nautobot-plugin-nornir (>=1.0.0)
+Project-URL: Documentation, https://github.com/nautobot/nautobot-plugin-golden-config
+Project-URL: Repository, https://github.com/nautobot/nautobot-plugin-golden-config
+Description-Content-Type: text/markdown
 
-packages = \
-['nautobot_golden_config',
- 'nautobot_golden_config.api',
- 'nautobot_golden_config.management.commands',
- 'nautobot_golden_config.migrations',
- 'nautobot_golden_config.nornir_plays',
- 'nautobot_golden_config.tests',
- 'nautobot_golden_config.tests.forms',
- 'nautobot_golden_config.tests.test_nornir_plays',
- 'nautobot_golden_config.tests.test_utilities',
- 'nautobot_golden_config.utilities']
-
-package_data = \
-{'': ['*'],
- 'nautobot_golden_config': ['static/nautobot_golden_config/diff2html-3.4.13/*',
-                            'templates/nautobot_golden_config/*']}
-
-install_requires = \
-['deepdiff>=5.5.0,<6.0.0',
- 'django-pivot>=1.8.1,<2.0.0',
- 'matplotlib>=3.3.2,<4.0.0',
- 'nautobot-plugin-nornir>=1.0.0',
- 'nautobot>=1.4.0']
-
-setup_kwargs = {
-    'name': 'nautobot-golden-config',
-    'version': '1.3.1',
-    'description': 'A plugin for configuration on nautobot',
-    'long_description': '# Nautobot Golden Config\n\n<p align="center">\n  <img src="https://raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/docs/images/icon-NautobotGoldenConfig.png" class="logo" height="200px">\n  <br>\n  <a href="https://github.com/nautobot/nautobot-plugin-golden-config/actions"><img src="https://github.com/nautobot/nautobot-plugin-golden-config/actions/workflows/ci.yml/badge.svg?branch=main"></a>\n  <a href="https://docs.nautobot.com/projects/golden-config/en/latest/"><img src="https://readthedocs.org/projects/nautobot-plugin-golden-config/badge/"></a>\n  <a href="https://pypi.org/project/nautobot-golden-config/"><img src="https://img.shields.io/pypi/v/nautobot-golden-config"></a>\n  <a href="https://pypi.org/project/nautobot-golden-config/"><img src="https://img.shields.io/pypi/dm/nautobot-golden-config"></a>\n  <br>\n  An App for <a href="https://github.com/nautobot/nautobot">Nautobot</a>.\n</p>\n\n## Overview\n\nThe Golden Config plugin is a Nautobot plugin that provides a NetDevOps approach to golden configuration and configuration compliance.\n\n### Key Use Cases\n\nThis plugin enable five (5) key use cases.\n\n1. **Configuration Backups** - Is a Nornir process to connect to devices, optionally parse out lines/secrets, backup the configuration, and save to a Git repository.\n2. **Intended Configuration** - Is a Nornir process to generate configuration based on a Git repo of Jinja files to combine with a GraphQL generated data and a Git repo to store the intended configuration.\n3. **Source of Truth Aggregation** - Is a GraphQL query per device that creates a data structure used in the generation of configuration.\n4. **Configuration Compliance** - Is a process to run comparison of the actual (via backups) and intended (via Jinja file creation) CLI configurations upon saving the actual and intended configuration. This is started by either a Nornir process for cli-like configurations or calling the API for json-like configurations\n5. **Configuration Postprocessing** - (beta) This process renders a valid configuration artifact from an intended configuration, that can be pushed to devices. The current implementation renders this configuration; however, **it doesn\'t push it** to the target device.\n\n> Notice: The operators of their own Nautobot instance are welcome to use any combination of these features. Though the appearance may seem like they are tightly coupled, this isn\'t actually the case. For example, one can obtain backup configurations from their current RANCID/Oxidized process and simply provide a Git Repo of the location of the backup configurations, and the compliance process would work the same way. Also, another user may only want to generate configurations, but not want to use other features, which is perfectly fine to do so.\n\n## Screenshots\n\nThere are many features and capabilities the plugin provides into the Nautobot ecosystem. The following screenshots are intended to provide a quick visual overview of some of these features.\n\nThe golden configuration is driven by jobs that run a series of tasks and the result is captured in this overview.\n\n![Overview](https://raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/docs/images/ss_golden-overview.png)\n\nThe compliance report provides a high-level overview on the compliance of your network.\n![Compliance Report](https://raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/docs/images/ss_compliance-report.png)\n\nThe compliance overview will provide a per device and feature overview on the compliance of your network devices.\n![Compliance Overview](https://raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/docs/images/ss_compliance-overview.png)\n\nDrilling into a specific device and feature, you can get an immediate detailed understanding of your device.\n![Compliance Device](https://raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/docs/images/ss_compliance-device.png)\n\n![Compliance Rule](https://raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/docs/images/ss_compliance-rule.png)\n\n## Try it out!\n\nThis App is installed in the Nautobot Community Sandbox found over at [demo.nautobot.com](https://demo.nautobot.com/)!\n\n> For a full list of all the available always-on sandbox environments, head over to the main page on [networktocode.com](https://www.networktocode.com/nautobot/sandbox-environments/).\n\n## Documentation\n\nFull web-based HTML documentation for this app can be found over on the [Nautobot Docs](https://docs.nautobot.com/projects/golden-config/en/latest/) website:\n\n- [User Guide](https://docs.nautobot.com/projects/golden-config/en/latest/user/app_overview/) - Overview, Using the App, Getting Started, Navigating compliance (cli, json, custom), backup, app usage, intended state creation.\n- [Administrator Guide](https://docs.nautobot.com/projects/golden-config/en/latest/admin/admin_install/) - How to Install, Configure, Upgrade, or Uninstall the App.\n- [Developer Guide](https://docs.nautobot.com/projects/golden-config/en/latest/dev/dev_contributing/) - Extending the App, Code Reference, Contribution Guide.\n- [Release Notes / Changelog](https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/)\n- [Frequently Asked Questions](https://docs.nautobot.com/projects/golden-config/en/latest/user/app_faq/)\n\n### Contributing to the Docs\n\nYou can find all the Markdown source for the App documentation under the [docs](https://github.com/nautobot/nautobot-plugin-golden-config/tree/develop/docs) folder in this repository. For simple edits, a Markdown capable editor is sufficient - clone the repository and edit away.\n\nIf you need to view the fully generated documentation site, you can build it with [mkdocs](https://www.mkdocs.org/). A container hosting the docs will be started using the invoke commands (details in the [Development Environment Guide](https://docs.nautobot.com/projects/golden-config/en/latest/dev/dev_environment/#docker-development-environment)) on [http://localhost:8001](http://localhost:8001). As your changes are saved, the live docs will be automatically reloaded.\n\nAny PRs with fixes or improvements are very welcome!\n\n## Questions\n\nFor any questions or comments, please check the [FAQ](https://docs.nautobot.com/projects/golden-config/en/latest/user/app_faq/) first. Feel free to also swing by the [Network to Code Slack](https://networktocode.slack.com/) (channel `#nautobot`), sign up [here](http://slack.networktocode.com/) if you don\'t have an account.\n',
-    'author': 'Network to Code, LLC',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/nautobot/nautobot-plugin-golden-config',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+# Nautobot Golden Config
 
+<p align="center">
+  <img src="https://raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/docs/images/icon-NautobotGoldenConfig.png" class="logo" height="200px">
+  <br>
+  <a href="https://github.com/nautobot/nautobot-plugin-golden-config/actions"><img src="https://github.com/nautobot/nautobot-plugin-golden-config/actions/workflows/ci.yml/badge.svg?branch=main"></a>
+  <a href="https://docs.nautobot.com/projects/golden-config/en/latest/"><img src="https://readthedocs.org/projects/nautobot-plugin-golden-config/badge/"></a>
+  <a href="https://pypi.org/project/nautobot-golden-config/"><img src="https://img.shields.io/pypi/v/nautobot-golden-config"></a>
+  <a href="https://pypi.org/project/nautobot-golden-config/"><img src="https://img.shields.io/pypi/dm/nautobot-golden-config"></a>
+  <br>
+  An App for <a href="https://github.com/nautobot/nautobot">Nautobot</a>.
+</p>
+
+## Overview
+
+The Golden Config plugin is a Nautobot plugin that provides a NetDevOps approach to golden configuration and configuration compliance.
+
+### Key Use Cases
+
+This plugin enable five (5) key use cases.
+
+1. **Configuration Backups** - Is a Nornir process to connect to devices, optionally parse out lines/secrets, backup the configuration, and save to a Git repository.
+2. **Intended Configuration** - Is a Nornir process to generate configuration based on a Git repo of Jinja files to combine with a GraphQL generated data and a Git repo to store the intended configuration.
+3. **Source of Truth Aggregation** - Is a GraphQL query per device that creates a data structure used in the generation of configuration.
+4. **Configuration Compliance** - Is a process to run comparison of the actual (via backups) and intended (via Jinja file creation) CLI configurations upon saving the actual and intended configuration. This is started by either a Nornir process for cli-like configurations or calling the API for json-like configurations
+5. **Configuration Postprocessing** - (beta) This process renders a valid configuration artifact from an intended configuration, that can be pushed to devices. The current implementation renders this configuration; however, **it doesn't push it** to the target device.
+
+> Notice: The operators of their own Nautobot instance are welcome to use any combination of these features. Though the appearance may seem like they are tightly coupled, this isn't actually the case. For example, one can obtain backup configurations from their current RANCID/Oxidized process and simply provide a Git Repo of the location of the backup configurations, and the compliance process would work the same way. Also, another user may only want to generate configurations, but not want to use other features, which is perfectly fine to do so.
+
+## Screenshots
+
+There are many features and capabilities the plugin provides into the Nautobot ecosystem. The following screenshots are intended to provide a quick visual overview of some of these features.
+
+The golden configuration is driven by jobs that run a series of tasks and the result is captured in this overview.
+
+![Overview](https://raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/docs/images/ss_golden-overview.png)
+
+The compliance report provides a high-level overview on the compliance of your network.
+![Compliance Report](https://raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/docs/images/ss_compliance-report.png)
+
+The compliance overview will provide a per device and feature overview on the compliance of your network devices.
+![Compliance Overview](https://raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/docs/images/ss_compliance-overview.png)
+
+Drilling into a specific device and feature, you can get an immediate detailed understanding of your device.
+![Compliance Device](https://raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/docs/images/ss_compliance-device.png)
+
+![Compliance Rule](https://raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/docs/images/ss_compliance-rule.png)
+
+## Try it out!
+
+This App is installed in the Nautobot Community Sandbox found over at [demo.nautobot.com](https://demo.nautobot.com/)!
+
+> For a full list of all the available always-on sandbox environments, head over to the main page on [networktocode.com](https://www.networktocode.com/nautobot/sandbox-environments/).
+
+## Documentation
+
+Full web-based HTML documentation for this app can be found over on the [Nautobot Docs](https://docs.nautobot.com/projects/golden-config/en/latest/) website:
+
+- [User Guide](https://docs.nautobot.com/projects/golden-config/en/latest/user/app_overview/) - Overview, Using the App, Getting Started, Navigating compliance (cli, json, custom), backup, app usage, intended state creation.
+- [Administrator Guide](https://docs.nautobot.com/projects/golden-config/en/latest/admin/admin_install/) - How to Install, Configure, Upgrade, or Uninstall the App.
+- [Developer Guide](https://docs.nautobot.com/projects/golden-config/en/latest/dev/dev_contributing/) - Extending the App, Code Reference, Contribution Guide.
+- [Release Notes / Changelog](https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/)
+- [Frequently Asked Questions](https://docs.nautobot.com/projects/golden-config/en/latest/user/app_faq/)
+
+### Contributing to the Docs
+
+You can find all the Markdown source for the App documentation under the [docs](https://github.com/nautobot/nautobot-plugin-golden-config/tree/develop/docs) folder in this repository. For simple edits, a Markdown capable editor is sufficient - clone the repository and edit away.
+
+If you need to view the fully generated documentation site, you can build it with [mkdocs](https://www.mkdocs.org/). A container hosting the docs will be started using the invoke commands (details in the [Development Environment Guide](https://docs.nautobot.com/projects/golden-config/en/latest/dev/dev_environment/#docker-development-environment)) on [http://localhost:8001](http://localhost:8001). As your changes are saved, the live docs will be automatically reloaded.
+
+Any PRs with fixes or improvements are very welcome!
+
+## Questions
+
+For any questions or comments, please check the [FAQ](https://docs.nautobot.com/projects/golden-config/en/latest/user/app_faq/) first. Feel free to also swing by the [Network to Code Slack](https://networktocode.slack.com/) (channel `#nautobot`), sign up [here](http://slack.networktocode.com/) if you don't have an account.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,104 +1,102 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['nautobot_golden_config', 'nautobot_golden_config.api',
-'nautobot_golden_config.management.commands',
-'nautobot_golden_config.migrations', 'nautobot_golden_config.nornir_plays',
-'nautobot_golden_config.tests', 'nautobot_golden_config.tests.forms',
-'nautobot_golden_config.tests.test_nornir_plays',
-'nautobot_golden_config.tests.test_utilities',
-'nautobot_golden_config.utilities'] package_data = \ {'': ['*'],
-'nautobot_golden_config': ['static/nautobot_golden_config/diff2html-3.4.13/*',
-'templates/nautobot_golden_config/*']} install_requires = \
-['deepdiff>=5.5.0,<6.0.0', 'django-pivot>=1.8.1,<2.0.0',
-'matplotlib>=3.3.2,<4.0.0', 'nautobot-plugin-nornir>=1.0.0', 'nautobot>=1.4.0']
-setup_kwargs = { 'name': 'nautobot-golden-config', 'version': '1.3.1',
-'description': 'A plugin for configuration on nautobot', 'long_description': '#
-Nautobot Golden Config\n\n
- \n [https://raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/
-             develop/docs/images/icon-NautobotGoldenConfig.png]\n
-    \n [https://github.com/nautobot/nautobot-plugin-golden-config/actions/
- workflows/ci.yml/badge.svg?branch=main]\n [https://readthedocs.org/projects/
-    nautobot-plugin-golden-config/badge/]\n [https://img.shields.io/pypi/v/
-  nautobot-golden-config]\n [https://img.shields.io/pypi/dm/nautobot-golden-
-                                  config]\n
-                           \n An App for Nautobot.\n
-\n\n## Overview\n\nThe Golden Config plugin is a Nautobot plugin that provides
-a NetDevOps approach to golden configuration and configuration
-compliance.\n\n### Key Use Cases\n\nThis plugin enable five (5) key use
-cases.\n\n1. **Configuration Backups** - Is a Nornir process to connect to
-devices, optionally parse out lines/secrets, backup the configuration, and save
-to a Git repository.\n2. **Intended Configuration** - Is a Nornir process to
-generate configuration based on a Git repo of Jinja files to combine with a
-GraphQL generated data and a Git repo to store the intended configuration.\n3.
-**Source of Truth Aggregation** - Is a GraphQL query per device that creates a
-data structure used in the generation of configuration.\n4. **Configuration
-Compliance** - Is a process to run comparison of the actual (via backups) and
-intended (via Jinja file creation) CLI configurations upon saving the actual
-and intended configuration. This is started by either a Nornir process for cli-
-like configurations or calling the API for json-like configurations\n5.
+Metadata-Version: 2.1 Name: nautobot-golden-config Version: 1.4.0 Summary: A
+plugin for configuration on nautobot Home-page: https://github.com/nautobot/
+nautobot-plugin-golden-config License: Apache-2.0 Keywords: nautobot,nautobot-
+plugin Author: Network to Code, LLC Requires-Python: >=3.7,<4.0 Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Requires-Dist: deepdiff (>=6.2.0) Requires-Dist:
+django-pivot (>=1.8.1,<2.0.0) Requires-Dist: matplotlib (>=3.3.2,<4.0.0)
+Requires-Dist: nautobot (>=1.5.3) Requires-Dist: nautobot-plugin-nornir
+(>=1.0.0) Project-URL: Documentation, https://github.com/nautobot/nautobot-
+plugin-golden-config Project-URL: Repository, https://github.com/nautobot/
+nautobot-plugin-golden-config Description-Content-Type: text/markdown #
+Nautobot Golden Config
+  [https://raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/
+              develop/docs/images/icon-NautobotGoldenConfig.png]
+ [https://github.com/nautobot/nautobot-plugin-golden-config/actions/workflows/
+   ci.yml/badge.svg?branch=main] [https://readthedocs.org/projects/nautobot-
+ plugin-golden-config/badge/] [https://img.shields.io/pypi/v/nautobot-golden-
+       config] [https://img.shields.io/pypi/dm/nautobot-golden-config]
+                             An App for Nautobot.
+## Overview The Golden Config plugin is a Nautobot plugin that provides a
+NetDevOps approach to golden configuration and configuration compliance. ###
+Key Use Cases This plugin enable five (5) key use cases. 1. **Configuration
+Backups** - Is a Nornir process to connect to devices, optionally parse out
+lines/secrets, backup the configuration, and save to a Git repository. 2.
+**Intended Configuration** - Is a Nornir process to generate configuration
+based on a Git repo of Jinja files to combine with a GraphQL generated data and
+a Git repo to store the intended configuration. 3. **Source of Truth
+Aggregation** - Is a GraphQL query per device that creates a data structure
+used in the generation of configuration. 4. **Configuration Compliance** - Is a
+process to run comparison of the actual (via backups) and intended (via Jinja
+file creation) CLI configurations upon saving the actual and intended
+configuration. This is started by either a Nornir process for cli-like
+configurations or calling the API for json-like configurations 5.
 **Configuration Postprocessing** - (beta) This process renders a valid
 configuration artifact from an intended configuration, that can be pushed to
 devices. The current implementation renders this configuration; however, **it
-doesn\'t push it** to the target device.\n\n> Notice: The operators of their
-own Nautobot instance are welcome to use any combination of these features.
-Though the appearance may seem like they are tightly coupled, this isn\'t
-actually the case. For example, one can obtain backup configurations from their
-current RANCID/Oxidized process and simply provide a Git Repo of the location
-of the backup configurations, and the compliance process would work the same
-way. Also, another user may only want to generate configurations, but not want
-to use other features, which is perfectly fine to do so.\n\n##
-Screenshots\n\nThere are many features and capabilities the plugin provides
-into the Nautobot ecosystem. The following screenshots are intended to provide
-a quick visual overview of some of these features.\n\nThe golden configuration
-is driven by jobs that run a series of tasks and the result is captured in this
-overview.\n\n![Overview](https://raw.githubusercontent.com/nautobot/nautobot-
-plugin-golden-config/develop/docs/images/ss_golden-overview.png)\n\nThe
-compliance report provides a high-level overview on the compliance of your
-network.\n![Compliance Report](https://raw.githubusercontent.com/nautobot/
-nautobot-plugin-golden-config/develop/docs/images/ss_compliance-
-report.png)\n\nThe compliance overview will provide a per device and feature
-overview on the compliance of your network devices.\n![Compliance Overview]
-(https://raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/
-develop/docs/images/ss_compliance-overview.png)\n\nDrilling into a specific
-device and feature, you can get an immediate detailed understanding of your
-device.\n![Compliance Device](https://raw.githubusercontent.com/nautobot/
-nautobot-plugin-golden-config/develop/docs/images/ss_compliance-
-device.png)\n\n![Compliance Rule](https://raw.githubusercontent.com/nautobot/
-nautobot-plugin-golden-config/develop/docs/images/ss_compliance-rule.png)\n\n##
-Try it out!\n\nThis App is installed in the Nautobot Community Sandbox found
-over at [demo.nautobot.com](https://demo.nautobot.com/)!\n\n> For a full list
-of all the available always-on sandbox environments, head over to the main page
-on [networktocode.com](https://www.networktocode.com/nautobot/sandbox-
-environments/).\n\n## Documentation\n\nFull web-based HTML documentation for
-this app can be found over on the [Nautobot Docs](https://docs.nautobot.com/
-projects/golden-config/en/latest/) website:\n\n- [User Guide](https://
-docs.nautobot.com/projects/golden-config/en/latest/user/app_overview/) -
-Overview, Using the App, Getting Started, Navigating compliance (cli, json,
-custom), backup, app usage, intended state creation.\n- [Administrator Guide]
-(https://docs.nautobot.com/projects/golden-config/en/latest/admin/
-admin_install/) - How to Install, Configure, Upgrade, or Uninstall the App.\n-
-[Developer Guide](https://docs.nautobot.com/projects/golden-config/en/latest/
-dev/dev_contributing/) - Extending the App, Code Reference, Contribution
-Guide.\n- [Release Notes / Changelog](https://docs.nautobot.com/projects/
-golden-config/en/latest/admin/release_notes/)\n- [Frequently Asked Questions]
-(https://docs.nautobot.com/projects/golden-config/en/latest/user/app_faq/
-)\n\n### Contributing to the Docs\n\nYou can find all the Markdown source for
+doesn't push it** to the target device. > Notice: The operators of their own
+Nautobot instance are welcome to use any combination of these features. Though
+the appearance may seem like they are tightly coupled, this isn't actually the
+case. For example, one can obtain backup configurations from their current
+RANCID/Oxidized process and simply provide a Git Repo of the location of the
+backup configurations, and the compliance process would work the same way.
+Also, another user may only want to generate configurations, but not want to
+use other features, which is perfectly fine to do so. ## Screenshots There are
+many features and capabilities the plugin provides into the Nautobot ecosystem.
+The following screenshots are intended to provide a quick visual overview of
+some of these features. The golden configuration is driven by jobs that run a
+series of tasks and the result is captured in this overview. ![Overview](https:
+//raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/
+docs/images/ss_golden-overview.png) The compliance report provides a high-level
+overview on the compliance of your network. ![Compliance Report](https://
+raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/docs/
+images/ss_compliance-report.png) The compliance overview will provide a per
+device and feature overview on the compliance of your network devices. !
+[Compliance Overview](https://raw.githubusercontent.com/nautobot/nautobot-
+plugin-golden-config/develop/docs/images/ss_compliance-overview.png) Drilling
+into a specific device and feature, you can get an immediate detailed
+understanding of your device. ![Compliance Device](https://
+raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/docs/
+images/ss_compliance-device.png) ![Compliance Rule](https://
+raw.githubusercontent.com/nautobot/nautobot-plugin-golden-config/develop/docs/
+images/ss_compliance-rule.png) ## Try it out! This App is installed in the
+Nautobot Community Sandbox found over at [demo.nautobot.com](https://
+demo.nautobot.com/)! > For a full list of all the available always-on sandbox
+environments, head over to the main page on [networktocode.com](https://
+www.networktocode.com/nautobot/sandbox-environments/). ## Documentation Full
+web-based HTML documentation for this app can be found over on the [Nautobot
+Docs](https://docs.nautobot.com/projects/golden-config/en/latest/) website: -
+[User Guide](https://docs.nautobot.com/projects/golden-config/en/latest/user/
+app_overview/) - Overview, Using the App, Getting Started, Navigating
+compliance (cli, json, custom), backup, app usage, intended state creation. -
+[Administrator Guide](https://docs.nautobot.com/projects/golden-config/en/
+latest/admin/admin_install/) - How to Install, Configure, Upgrade, or Uninstall
+the App. - [Developer Guide](https://docs.nautobot.com/projects/golden-config/
+en/latest/dev/dev_contributing/) - Extending the App, Code Reference,
+Contribution Guide. - [Release Notes / Changelog](https://docs.nautobot.com/
+projects/golden-config/en/latest/admin/release_notes/) - [Frequently Asked
+Questions](https://docs.nautobot.com/projects/golden-config/en/latest/user/
+app_faq/) ### Contributing to the Docs You can find all the Markdown source for
 the App documentation under the [docs](https://github.com/nautobot/nautobot-
 plugin-golden-config/tree/develop/docs) folder in this repository. For simple
 edits, a Markdown capable editor is sufficient - clone the repository and edit
-away.\n\nIf you need to view the fully generated documentation site, you can
-build it with [mkdocs](https://www.mkdocs.org/). A container hosting the docs
-will be started using the invoke commands (details in the [Development
-Environment Guide](https://docs.nautobot.com/projects/golden-config/en/latest/
-dev/dev_environment/#docker-development-environment)) on [http://localhost:
-8001](http://localhost:8001). As your changes are saved, the live docs will be
-automatically reloaded.\n\nAny PRs with fixes or improvements are very
-welcome!\n\n## Questions\n\nFor any questions or comments, please check the
-[FAQ](https://docs.nautobot.com/projects/golden-config/en/latest/user/app_faq/
-) first. Feel free to also swing by the [Network to Code Slack](https://
+away. If you need to view the fully generated documentation site, you can build
+it with [mkdocs](https://www.mkdocs.org/). A container hosting the docs will be
+started using the invoke commands (details in the [Development Environment
+Guide](https://docs.nautobot.com/projects/golden-config/en/latest/dev/
+dev_environment/#docker-development-environment)) on [http://localhost:8001]
+(http://localhost:8001). As your changes are saved, the live docs will be
+automatically reloaded. Any PRs with fixes or improvements are very welcome! ##
+Questions For any questions or comments, please check the [FAQ](https://
+docs.nautobot.com/projects/golden-config/en/latest/user/app_faq/) first. Feel
+free to also swing by the [Network to Code Slack](https://
 networktocode.slack.com/) (channel `#nautobot`), sign up [here](http://
-slack.networktocode.com/) if you don\'t have an account.\n', 'author': 'Network
-to Code, LLC', 'author_email': 'None', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/nautobot/nautobot-
-plugin-golden-config', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.7,<4.0', } setup
-(**setup_kwargs)
+slack.networktocode.com/) if you don't have an account.
```

