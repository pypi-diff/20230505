# Comparing `tmp/django_twined-0.4.1.tar.gz` & `tmp/django_twined-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_twined-0.4.1.tar", max compression
+gzip compressed data, was "django_twined-0.4.2.tar", max compression
```

## Comparing `django_twined-0.4.1.tar` & `django_twined-0.4.2.tar`

### file list

```diff
@@ -1,54 +1,53 @@
--rw-r--r--   0        0        0     1088 2022-10-13 13:49:00.156745 django_twined-0.4.1/LICENSE
--rw-r--r--   0        0        0     1463 2022-10-13 13:49:00.156745 django_twined-0.4.1/README.md
--rw-r--r--   0        0        0       64 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/__init__.py
--rw-r--r--   0        0        0      257 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/admin/__init__.py
--rw-r--r--   0        0        0     6781 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/admin/admin.py
--rw-r--r--   0        0        0      402 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/admin/fieldsets.py
--rw-r--r--   0        0        0      881 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/admin/mixins.py
--rw-r--r--   0        0        0      682 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/admin/proxy.py
--rw-r--r--   0        0        0      496 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/apps.py
--rw-r--r--   0        0        0      104 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/consumers/__init__.py
--rw-r--r--   0        0        0     3765 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/consumers/analysis.py
--rw-r--r--   0        0        0     1001 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/consumers/analysis_log.py
--rw-r--r--   0        0        0     5822 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/consumers/service.py
--rw-r--r--   0        0        0      130 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/exceptions.py
--rw-r--r--   0        0        0     2357 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/fields.py
--rw-r--r--   0        0        0        0 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/management/__init__.py
--rw-r--r--   0        0        0        0 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/management/commands/__init__.py
--rw-r--r--   0        0        0     2299 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/management/commands/sync_data_stores.py
--rw-r--r--   0        0        0     2990 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/messages.py
--rw-r--r--   0        0        0     2345 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/migrations/0001_initial.py
--rw-r--r--   0        0        0      595 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/migrations/0002_slug_unique_and_not_editable.py
--rw-r--r--   0        0        0      408 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/migrations/0003_rename_slug_to_name.py
--rw-r--r--   0        0        0      670 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/migrations/0004_add_timestamps.py
--rw-r--r--   0        0        0      731 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/migrations/0005_question_date_help_text.py
--rw-r--r--   0        0        0     4710 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/migrations/0006_service_revisions_and_events.py
--rw-r--r--   0        0        0     1476 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/migrations/0007_registered_to_revision.py
--rw-r--r--   0        0        0      669 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/migrations/0008_registered_relations_to_nullable.py
--rw-r--r--   0        0        0      683 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/migrations/0009_remove_registered_services.py
--rw-r--r--   0        0        0      681 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/migrations/0010_alter_servicerevision_project_name.py
--rw-r--r--   0        0        0      362 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/migrations/0011_remove_servicerevision_topic_id.py
--rw-r--r--   0        0        0      568 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/migrations/0012_servicerevision_is_default.py
--rw-r--r--   0        0        0      639 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/migrations/0013_alter_serviceusageevent_question.py
--rw-r--r--   0        0        0        0 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/migrations/__init__.py
--rw-r--r--   0        0        0      698 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/models/__init__.py
--rw-r--r--   0        0        0    11448 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/models/datastores.py
--rw-r--r--   0        0        0       85 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/models/querysets/__init__.py
--rw-r--r--   0        0        0     9794 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/models/querysets/datastore_queryset.py
--rw-r--r--   0        0        0     6623 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/models/questions.py
--rw-r--r--   0        0        0     7824 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/models/service_revisions.py
--rw-r--r--   0        0        0     2514 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/models/service_usage_events.py
--rw-r--r--   0        0        0      290 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/routing.py
--rw-r--r--   0        0        0      479 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/signals/__init__.py
--rw-r--r--   0        0        0     3079 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/signals/receivers.py
--rw-r--r--   0        0        0      262 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/signals/senders.py
--rw-r--r--   0        0        0        0 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/static/.gitignore
--rw-r--r--   0        0        0     2666 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/tasks.py
--rw-r--r--   0        0        0     1149 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/templates/admin/question_ask_row.html
--rw-r--r--   0        0        0        0 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/templates/django_twined/.gitignore
--rw-r--r--   0        0        0      343 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/templates/django_twined/question_changeform.html
--rw-r--r--   0        0        0        0 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/templatetags/__init__.py
--rw-r--r--   0        0        0      480 2022-10-13 13:49:00.156745 django_twined-0.4.1/django_twined/templatetags/question_ask_row.py
--rw-r--r--   0        0        0     1550 2022-10-13 13:49:00.160745 django_twined-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2703 1970-01-01 00:00:00.000000 django_twined-0.4.1/setup.py
--rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 django_twined-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-05 16:50:04.055920 django_twined-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1463 2023-05-05 16:50:04.055920 django_twined-0.4.2/README.md
+-rw-r--r--   0        0        0       64 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/__init__.py
+-rw-r--r--   0        0        0      257 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/admin/__init__.py
+-rw-r--r--   0        0        0     6781 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/admin/admin.py
+-rw-r--r--   0        0        0      402 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/admin/fieldsets.py
+-rw-r--r--   0        0        0      881 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/admin/mixins.py
+-rw-r--r--   0        0        0      682 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/admin/proxy.py
+-rw-r--r--   0        0        0      496 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/apps.py
+-rw-r--r--   0        0        0      104 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/consumers/__init__.py
+-rw-r--r--   0        0        0     3765 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/consumers/analysis.py
+-rw-r--r--   0        0        0     1001 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/consumers/analysis_log.py
+-rw-r--r--   0        0        0     5822 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/consumers/service.py
+-rw-r--r--   0        0        0      130 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/exceptions.py
+-rw-r--r--   0        0        0     2357 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/fields.py
+-rw-r--r--   0        0        0        0 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/management/commands/__init__.py
+-rw-r--r--   0        0        0     2299 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/management/commands/sync_data_stores.py
+-rw-r--r--   0        0        0     2990 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/messages.py
+-rw-r--r--   0        0        0     2345 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0001_initial.py
+-rw-r--r--   0        0        0      595 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0002_slug_unique_and_not_editable.py
+-rw-r--r--   0        0        0      408 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0003_rename_slug_to_name.py
+-rw-r--r--   0        0        0      670 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0004_add_timestamps.py
+-rw-r--r--   0        0        0      731 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0005_question_date_help_text.py
+-rw-r--r--   0        0        0     4710 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0006_service_revisions_and_events.py
+-rw-r--r--   0        0        0     1476 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0007_registered_to_revision.py
+-rw-r--r--   0        0        0      669 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0008_registered_relations_to_nullable.py
+-rw-r--r--   0        0        0      683 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0009_remove_registered_services.py
+-rw-r--r--   0        0        0      681 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0010_alter_servicerevision_project_name.py
+-rw-r--r--   0        0        0      362 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0011_remove_servicerevision_topic_id.py
+-rw-r--r--   0        0        0      568 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0012_servicerevision_is_default.py
+-rw-r--r--   0        0        0      639 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/0013_alter_serviceusageevent_question.py
+-rw-r--r--   0        0        0        0 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/migrations/__init__.py
+-rw-r--r--   0        0        0      698 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/models/__init__.py
+-rw-r--r--   0        0        0    11448 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/models/datastores.py
+-rw-r--r--   0        0        0       85 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/models/querysets/__init__.py
+-rw-r--r--   0        0        0     9794 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/models/querysets/datastore_queryset.py
+-rw-r--r--   0        0        0     6623 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/models/questions.py
+-rw-r--r--   0        0        0     7824 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/models/service_revisions.py
+-rw-r--r--   0        0        0     2514 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/models/service_usage_events.py
+-rw-r--r--   0        0        0      290 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/routing.py
+-rw-r--r--   0        0        0      479 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/signals/__init__.py
+-rw-r--r--   0        0        0     3079 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/signals/receivers.py
+-rw-r--r--   0        0        0      262 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/signals/senders.py
+-rw-r--r--   0        0        0        0 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/static/.gitignore
+-rw-r--r--   0        0        0     2666 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/tasks.py
+-rw-r--r--   0        0        0     1149 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/templates/admin/question_ask_row.html
+-rw-r--r--   0        0        0        0 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/templates/django_twined/.gitignore
+-rw-r--r--   0        0        0      343 2023-05-05 16:50:04.055920 django_twined-0.4.2/django_twined/templates/django_twined/question_changeform.html
+-rw-r--r--   0        0        0        0 2023-05-05 16:50:04.059920 django_twined-0.4.2/django_twined/templatetags/__init__.py
+-rw-r--r--   0        0        0      480 2023-05-05 16:50:04.059920 django_twined-0.4.2/django_twined/templatetags/question_ask_row.py
+-rw-r--r--   0        0        0     1532 2023-05-05 16:50:04.059920 django_twined-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 django_twined-0.4.2/PKG-INFO
```

### Comparing `django_twined-0.4.1/LICENSE` & `django_twined-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/README.md` & `django_twined-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/admin/admin.py` & `django_twined-0.4.2/django_twined/admin/admin.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/admin/mixins.py` & `django_twined-0.4.2/django_twined/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/admin/proxy.py` & `django_twined-0.4.2/django_twined/admin/proxy.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/consumers/analysis.py` & `django_twined-0.4.2/django_twined/consumers/analysis.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/consumers/analysis_log.py` & `django_twined-0.4.2/django_twined/consumers/analysis_log.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/consumers/service.py` & `django_twined-0.4.2/django_twined/consumers/service.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/fields.py` & `django_twined-0.4.2/django_twined/fields.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/management/commands/sync_data_stores.py` & `django_twined-0.4.2/django_twined/management/commands/sync_data_stores.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/messages.py` & `django_twined-0.4.2/django_twined/messages.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/migrations/0001_initial.py` & `django_twined-0.4.2/django_twined/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/migrations/0002_slug_unique_and_not_editable.py` & `django_twined-0.4.2/django_twined/migrations/0002_slug_unique_and_not_editable.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/migrations/0004_add_timestamps.py` & `django_twined-0.4.2/django_twined/migrations/0004_add_timestamps.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/migrations/0005_question_date_help_text.py` & `django_twined-0.4.2/django_twined/migrations/0005_question_date_help_text.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/migrations/0006_service_revisions_and_events.py` & `django_twined-0.4.2/django_twined/migrations/0006_service_revisions_and_events.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/migrations/0007_registered_to_revision.py` & `django_twined-0.4.2/django_twined/migrations/0007_registered_to_revision.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/migrations/0008_registered_relations_to_nullable.py` & `django_twined-0.4.2/django_twined/migrations/0008_registered_relations_to_nullable.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/migrations/0009_remove_registered_services.py` & `django_twined-0.4.2/django_twined/migrations/0009_remove_registered_services.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/migrations/0010_alter_servicerevision_project_name.py` & `django_twined-0.4.2/django_twined/migrations/0010_alter_servicerevision_project_name.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/migrations/0012_servicerevision_is_default.py` & `django_twined-0.4.2/django_twined/migrations/0012_servicerevision_is_default.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/migrations/0013_alter_serviceusageevent_question.py` & `django_twined-0.4.2/django_twined/migrations/0013_alter_serviceusageevent_question.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/models/__init__.py` & `django_twined-0.4.2/django_twined/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/models/datastores.py` & `django_twined-0.4.2/django_twined/models/datastores.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/models/querysets/datastore_queryset.py` & `django_twined-0.4.2/django_twined/models/querysets/datastore_queryset.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/models/questions.py` & `django_twined-0.4.2/django_twined/models/questions.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/models/service_revisions.py` & `django_twined-0.4.2/django_twined/models/service_revisions.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/models/service_usage_events.py` & `django_twined-0.4.2/django_twined/models/service_usage_events.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/signals/receivers.py` & `django_twined-0.4.2/django_twined/signals/receivers.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/tasks.py` & `django_twined-0.4.2/django_twined/tasks.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/django_twined/templates/admin/question_ask_row.html` & `django_twined-0.4.2/django_twined/templates/admin/question_ask_row.html`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.1/pyproject.toml` & `django_twined-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-twined"
-version = "0.4.1"
+version = "0.4.2"
 description = "A django app to manage octue services"
 authors = ["Tom Clark <tom@octue.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -21,15 +21,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 django = ">=3.0,<4.0"
 channels = ">=3.0,<4.0"
 octue = "^0.39.0"
 pika = "^1.2.0"
-django-gcp = "^0.7.3"
+django-gcp = ">=0.7.3,<0.10"
 django-jsoneditor = "^0.2.2"
 django-model-utils = "^4.2.0"
 
 [tool.poetry.group.dev.dependencies]
 channels = ">=3.0,<=4.0"
 coverage = "^6.2"
 django-dramatiq = "^0.10.0"
@@ -41,15 +41,14 @@
 pylint-django = "^2.5.3"
 pytest = "^7.1.3"
 pytest-asyncio = "^0.18.1"
 pytest-django = "^4.5.2"
 pytest-sugar = "^0.9.4"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-tabs = "^3.2.0"
-sphinx-charts = "^0.1.2"
 Sphinx = "^4.4.0"
 tox = "^3.24.5"
 tox-gh-actions = "^2.9.1"
 tox-poetry = "^0.4.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `django_twined-0.4.1/PKG-INFO` & `django_twined-0.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-twined
-Version: 0.4.1
+Version: 0.4.2
 Summary: A django app to manage octue services
 Home-page: https://github.com/octue/django-twined
 License: MIT
 Keywords: django,services,octue,twined
 Author: Tom Clark
 Author-email: tom@octue.com
 Requires-Python: >=3.9,<3.11
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: channels (>=3.0,<4.0)
 Requires-Dist: django (>=3.0,<4.0)
-Requires-Dist: django-gcp (>=0.7.3,<0.8.0)
+Requires-Dist: django-gcp (>=0.7.3,<0.10)
 Requires-Dist: django-jsoneditor (>=0.2.2,<0.3.0)
 Requires-Dist: django-model-utils (>=4.2.0,<5.0.0)
 Requires-Dist: octue (>=0.39.0,<0.40.0)
 Requires-Dist: pika (>=1.2.0,<2.0.0)
 Project-URL: Repository, https://github.com/octue/django-twined
 Description-Content-Type: text/markdown
```

