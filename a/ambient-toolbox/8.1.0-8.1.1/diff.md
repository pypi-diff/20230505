# Comparing `tmp/ambient-toolbox-8.1.0.tar.gz` & `tmp/ambient-toolbox-8.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient-toolbox-8.1.0.tar", last modified: Thu May  4 13:56:10 2023, max compression
+gzip compressed data, was "ambient-toolbox-8.1.1.tar", last modified: Fri May  5 09:20:32 2023, max compression
```

## Comparing `ambient-toolbox-8.1.0.tar` & `ambient-toolbox-8.1.1.tar`

### file list

```diff
@@ -1,202 +1,202 @@
--rw-r--r--   0        0        0     2799 2023-05-04 13:17:19.756427 ambient-toolbox-8.1.0/.ambient-package-update/metadata.py
--rw-r--r--   0        0        0       82 2023-05-04 13:52:31.889391 ambient-toolbox-8.1.0/.coveragerc
--rw-r--r--   0        0        0      288 2023-05-04 13:52:31.889391 ambient-toolbox-8.1.0/.editorconfig
--rw-r--r--   0        0        0     1700 2023-05-04 13:54:31.166573 ambient-toolbox-8.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3461 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/.gitignore
--rw-r--r--   0        0        0     3942 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      904 2023-05-04 13:54:31.166573 ambient-toolbox-8.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      551 2023-05-04 13:52:31.889391 ambient-toolbox-8.1.0/.readthedocs.yml
--rw-r--r--   0        0        0    18842 2023-05-04 13:54:31.166573 ambient-toolbox-8.1.0/CHANGES.md
--rw-r--r--   0        0        0      964 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/Dockerfile
--rw-r--r--   0        0        0     1107 2023-05-04 13:52:31.889391 ambient-toolbox-8.1.0/LICENSE.md
--rw-r--r--   0        0        0      134 2023-05-04 13:52:31.889391 ambient-toolbox-8.1.0/MANIFEST.in
--rw-r--r--   0        0        0     5192 2023-05-04 13:52:31.905042 ambient-toolbox-8.1.0/README.md
--rw-r--r--   0        0        0      119 2023-05-04 13:54:31.166573 ambient-toolbox-8.1.0/ambient_toolbox/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/ambient_toolbox/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/ambient_toolbox/admin/model_admins/__init__.py
--rw-r--r--   0        0        0     1644 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/ambient_toolbox/admin/model_admins/classes.py
--rw-r--r--   0        0        0      824 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/ambient_toolbox/admin/model_admins/inlines.py
--rw-r--r--   0        0        0     4623 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/ambient_toolbox/admin/model_admins/mixins.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/ambient_toolbox/admin/views/__init__.py
--rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/ambient_toolbox/admin/views/forms.py
--rw-r--r--   0        0        0     2427 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/ambient_toolbox/admin/views/mixins.py
--rw-r--r--   0        0        0      206 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/ambient_toolbox/apps.py
--rw-r--r--   0        0        0      942 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/ambient_toolbox/context_manager.py
--rw-r--r--   0        0        0      147 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/ambient_toolbox/context_processors.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/ambient_toolbox/drf/__init__.py
--rw-r--r--   0        0        0     1031 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/ambient_toolbox/drf/fields.py
--rw-r--r--   0        0        0     1143 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.0/ambient_toolbox/drf/serializers.py
--rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/drf/tests.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/gitlab/__init__.py
--rw-r--r--   0        0        0     9623 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/gitlab/coverage.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/graphql/forms/__init__.py
--rw-r--r--   0        0        0     1687 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/graphql/forms/mutations.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/graphql/schemes/__init__.py
--rw-r--r--   0        0        0     2065 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/graphql/schemes/mutations.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/graphql/sentry/__init__.py
--rw-r--r--   0        0        0      419 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/graphql/sentry/utils.py
--rw-r--r--   0        0        0     1342 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/graphql/sentry/views.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/graphql/tests/__init__.py
--rw-r--r--   0        0        0     2144 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/graphql/tests/base_test.py
--rw-r--r--   0        0        0     1360 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2177 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/mail/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/mail/backends/__init__.py
--rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/mail/backends/whitelist_smtp.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/management/commands/__init__.py
--rw-r--r--   0        0        0      303 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/management/commands/validate_test_structure.py
--rw-r--r--   0        0        0     2550 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/managers.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/middleware/__init__.py
--rw-r--r--   0        0        0     1050 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/middleware/current_user.py
--rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/mixins/__init__.py
--rw-r--r--   0        0        0     1958 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/mixins/bleacher.py
--rw-r--r--   0        0        0     1378 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/mixins/models.py
--rw-r--r--   0        0        0      246 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/mixins/validation.py
--rw-r--r--   0        0        0     2592 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/models.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/selectors/__init__.py
--rw-r--r--   0        0        0      362 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/selectors/base.py
--rw-r--r--   0        0        0     1061 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/selectors/permission.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/sentry/__init__.py
--rw-r--r--   0        0        0      668 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/sentry/helpers.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/services/__init__.py
--rw-r--r--   0        0        0     3223 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/services/custom_scrubber.py
--rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/templatetags/__init__.py
--rw-r--r--   0        0        0      244 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.0/ambient_toolbox/templatetags/ai_date_tags.py
--rw-r--r--   0        0        0      675 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.0/ambient_toolbox/templatetags/ai_email_tags.py
--rw-r--r--   0        0        0      807 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.0/ambient_toolbox/templatetags/ai_file_tags.py
--rw-r--r--   0        0        0      194 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.0/ambient_toolbox/templatetags/ai_helper_tags.py
--rw-r--r--   0        0        0     1375 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.0/ambient_toolbox/templatetags/ai_number_tags.py
--rw-r--r--   0        0        0      384 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.0/ambient_toolbox/templatetags/ai_object_tags.py
--rw-r--r--   0        0        0      654 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.0/ambient_toolbox/templatetags/ai_string_tags.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.0/ambient_toolbox/tests/__init__.py
--rw-r--r--   0        0        0       60 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.0/ambient_toolbox/tests/errors.py
--rw-r--r--   0        0        0     5145 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.0/ambient_toolbox/tests/mixins.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.0/ambient_toolbox/tests/structure_validator/__init__.py
--rw-r--r--   0        0        0      397 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.0/ambient_toolbox/tests/structure_validator/settings.py
--rw-r--r--   0        0        0     4634 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/tests/structure_validator/test_structure_validator.py
--rw-r--r--   0        0        0      261 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/utils/__init__.py
--rw-r--r--   0        0        0      127 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/utils/cache.py
--rw-r--r--   0        0        0     5971 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/utils/date.py
--rw-r--r--   0        0        0     1469 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/utils/file.py
--rw-r--r--   0        0        0      343 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/utils/log_whodid.py
--rw-r--r--   0        0        0      574 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/utils/math.py
--rw-r--r--   0        0        0      935 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/utils/model.py
--rw-r--r--   0        0        0     3970 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/utils/named_tuple.py
--rw-r--r--   0        0        0     3804 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/utils/string.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/view_layer/__init__.py
--rw-r--r--   0        0        0      750 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/view_layer/form_mixins.py
--rw-r--r--   0        0        0      485 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/view_layer/formset_mixins.py
--rw-r--r--   0        0        0     2998 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/view_layer/formset_view_mixin.py
--rw-r--r--   0        0        0     1585 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/view_layer/htmx_mixins.py
--rw-r--r--   0        0        0     2110 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/view_layer/mixins.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/view_layer/tests/__init__.py
--rw-r--r--   0        0        0     4124 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/view_layer/tests/mixins.py
--rw-r--r--   0        0        0     1882 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/ambient_toolbox/view_layer/views.py
--rw-r--r--   0        0        0      654 2023-05-04 13:52:31.920642 ambient-toolbox-8.1.0/docs/Makefile
--rw-r--r--   0        0        0     2803 2023-05-04 13:52:31.905042 ambient-toolbox-8.1.0/docs/conf.py
--rw-r--r--   0        0        0     6731 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/docs/features/admin.md
--rw-r--r--   0        0        0       35 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/docs/features/changelog.rst
--rw-r--r--   0        0        0     2313 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/docs/features/context_manager.md
--rw-r--r--   0        0        0      549 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/docs/features/context_processors.md
--rw-r--r--   0        0        0     7273 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/docs/features/database_anonymisation.md
--rw-r--r--   0        0        0     6807 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/docs/features/djangorestframework.md
--rw-r--r--   0        0        0     2554 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/docs/features/gitlab.md
--rw-r--r--   0        0        0     6567 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.0/docs/features/graphql.md
--rw-r--r--   0        0        0     1020 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/mail.md
--rw-r--r--   0        0        0     5891 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/managers.md
--rw-r--r--   0        0        0     5951 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/mixins.md
--rw-r--r--   0        0        0     1553 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/models.md
--rw-r--r--   0        0        0     4454 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/selectors.md
--rw-r--r--   0        0        0     1078 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/sentry.md
--rw-r--r--   0        0        0     4978 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/services.md
--rw-r--r--   0        0        0     1574 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/setup.md
--rw-r--r--   0        0        0     5338 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/tests.md
--rw-r--r--   0        0        0      232 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/utils.rst
--rw-r--r--   0        0        0      527 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/utils/cache.md
--rw-r--r--   0        0        0     7417 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/utils/date.md
--rw-r--r--   0        0        0      737 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/utils/math.md
--rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/utils/model.md
--rw-r--r--   0        0        0     2405 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/utils/named_tuple.md
--rw-r--r--   0        0        0     5861 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/utils/string.md
--rw-r--r--   0        0        0    15067 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/features/view-layer.md
--rw-r--r--   0        0        0     1157 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/docs/index.rst
--rwxr-xr-x   0        0        0      795 2023-05-04 13:52:31.920642 ambient-toolbox-8.1.0/docs/make.bat
--rw-r--r--   0        0        0      677 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/manage.py
--rw-r--r--   0        0        0     3892 2023-05-04 13:54:31.414401 ambient-toolbox-8.1.0/pyproject.toml
--rw-r--r--   0        0        0       56 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/pytest.ini
--rw-r--r--   0        0        0       56 2023-05-04 13:52:31.905042 ambient-toolbox-8.1.0/pytest.init
--rw-r--r--   0        0        0     1770 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/settings.py
--rw-r--r--   0        0        0       69 2023-05-04 13:52:31.905042 ambient-toolbox-8.1.0/setup.cfg
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/api/__init__.py
--rw-r--r--   0        0        0      287 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/api/serializers.py
--rw-r--r--   0        0        0      257 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/api/urls.py
--rw-r--r--   0        0        0      524 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/api/views.py
--rw-r--r--   0        0        0      219 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/forms.py
--rw-r--r--   0        0        0       97 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/managers.py
--rw-r--r--   0        0        0     6151 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/migrations/__init__.py
--rw-r--r--   0        0        0     3363 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/models.py
--rw-r--r--   0        0        0      162 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/selectors.py
--rw-r--r--   0        0        0     1449 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/templates/403.html
--rw-r--r--   0        0        0      145 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/templates/testapp/test_template.html
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/tests/missing_init/test_ok.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.0/testapp/tests/subdirectory/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/testapp/tests/subdirectory/missing_test_prefix.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/testapp/tests/subdirectory/test_ok.py
--rw-r--r--   0        0        0      382 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/testapp/urls.py
--rw-r--r--   0        0        0      505 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/testapp/views.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/admin/model_admin_mixins/__init__.py
--rw-r--r--   0        0        0     2607 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py
--rw-r--r--   0        0        0     1900 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py
--rw-r--r--   0        0        0     1683 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py
--rw-r--r--   0        0        0     1184 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py
--rw-r--r--   0        0        0     3871 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py
--rw-r--r--   0        0        0     1492 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/admin/model_admin_mixins/test_fetch_object_mixin.py
--rw-r--r--   0        0        0     1909 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/ambient_toolbox/__init__.py
--rw-r--r--   0        0        0     7503 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/ambient_toolbox/test_test_structure_validator.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/drf/__init__.py
--rw-r--r--   0        0        0     2579 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/drf/test_fields.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/mixins/__init__.py
--rw-r--r--   0        0        0      364 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/mixins/validation.py
--rw-r--r--   0        0        0      499 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/query_selectors/test_base.py
--rw-r--r--   0        0        0     1631 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/query_selectors/test_permission.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/selectors/__init__.py
--rw-r--r--   0        0        0      553 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_admin_forms.py
--rw-r--r--   0        0        0     1612 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_admin_inlines.py
--rw-r--r--   0        0        0     2651 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_admin_model_admins_classes.py
--rw-r--r--   0        0        0     2899 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_admin_view_mixins.py
--rw-r--r--   0        0        0     2218 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_context_manager.py
--rw-r--r--   0        0        0      822 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_log_whodid.py
--rw-r--r--   0        0        0     1169 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_managers.py
--rw-r--r--   0        0        0     1628 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_math.py
--rw-r--r--   0        0        0     2593 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_middleware.py
--rw-r--r--   0        0        0     1200 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_mixins_models.py
--rw-r--r--   0        0        0     1669 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_models.py
--rw-r--r--   0        0        0     1780 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_rest_api_mixins.py
--rw-r--r--   0        0        0      664 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_scrubbing_service.py
--rw-r--r--   0        0        0     1197 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_sentry_helper.py
--rw-r--r--   0        0        0      289 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_utils_cache.py
--rw-r--r--   0        0        0    12741 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_utils_date.py
--rw-r--r--   0        0        0     1593 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_utils_file.py
--rw-r--r--   0        0        0      933 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.0/tests/test_utils_model.py
--rw-r--r--   0        0        0     3807 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.0/tests/test_utils_named_tuple.py
--rw-r--r--   0        0        0     5343 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.0/tests/test_utils_string.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.0/tests/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.0/tests/tests/mixins/__init__.py
--rw-r--r--   0        0        0      371 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.0/tests/tests/mixins/models.py
--rw-r--r--   0        0        0      817 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.0/tests/tests/mixins/test_django_message_framework.py
--rw-r--r--   0        0        0     2483 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.0/tests/tests/mixins/test_request_provider_mixin.py
--rw-r--r--   0        0        0     2057 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.0/tests/tests/test_mail_backends.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.0/tests/view_layer/__init__.py
--rw-r--r--   0        0        0     1891 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.0/tests/view_layer/test_formset_mixins.py
--rw-r--r--   0        0        0     1564 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.0/tests/view_layer/test_htmx_response_mixin.py
--rw-r--r--   0        0        0     3458 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.0/tests/view_layer/test_meta_mixins.py
--rw-r--r--   0        0        0     1361 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.0/tests/view_layer/test_views.py
--rw-r--r--   0        0        0     7583 1970-01-01 00:00:00.000000 ambient-toolbox-8.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2945 2023-05-05 09:18:18.662886 ambient-toolbox-8.1.1/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0       82 2023-05-05 09:18:19.882717 ambient-toolbox-8.1.1/.coveragerc
+-rw-r--r--   0        0        0      288 2023-05-05 09:18:19.884725 ambient-toolbox-8.1.1/.editorconfig
+-rw-r--r--   0        0        0     1700 2023-05-05 09:18:19.907900 ambient-toolbox-8.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3461 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/.gitignore
+-rw-r--r--   0        0        0     3942 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      904 2023-05-05 09:18:19.885751 ambient-toolbox-8.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      551 2023-05-05 09:18:19.886724 ambient-toolbox-8.1.1/.readthedocs.yml
+-rw-r--r--   0        0        0    18404 2023-05-05 09:19:41.463274 ambient-toolbox-8.1.1/CHANGES.md
+-rw-r--r--   0        0        0      964 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/Dockerfile
+-rw-r--r--   0        0        0     1107 2023-05-05 09:18:19.888752 ambient-toolbox-8.1.1/LICENSE.md
+-rw-r--r--   0        0        0      134 2023-05-05 09:18:19.889758 ambient-toolbox-8.1.1/MANIFEST.in
+-rw-r--r--   0        0        0     5340 2023-05-05 09:18:19.905900 ambient-toolbox-8.1.1/README.md
+-rw-r--r--   0        0        0      116 2023-05-05 09:19:41.455920 ambient-toolbox-8.1.1/ambient_toolbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/ambient_toolbox/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/ambient_toolbox/admin/model_admins/__init__.py
+-rw-r--r--   0        0        0     1644 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/ambient_toolbox/admin/model_admins/classes.py
+-rw-r--r--   0        0        0      824 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/ambient_toolbox/admin/model_admins/inlines.py
+-rw-r--r--   0        0        0     4623 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/ambient_toolbox/admin/model_admins/mixins.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/ambient_toolbox/admin/views/__init__.py
+-rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/ambient_toolbox/admin/views/forms.py
+-rw-r--r--   0        0        0     2427 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/ambient_toolbox/admin/views/mixins.py
+-rw-r--r--   0        0        0      206 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/ambient_toolbox/apps.py
+-rw-r--r--   0        0        0      942 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/ambient_toolbox/context_manager.py
+-rw-r--r--   0        0        0      147 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/ambient_toolbox/context_processors.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/ambient_toolbox/drf/__init__.py
+-rw-r--r--   0        0        0     1031 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/ambient_toolbox/drf/fields.py
+-rw-r--r--   0        0        0     1143 2023-05-04 10:28:20.851321 ambient-toolbox-8.1.1/ambient_toolbox/drf/serializers.py
+-rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/drf/tests.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/gitlab/__init__.py
+-rw-r--r--   0        0        0     9623 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/gitlab/coverage.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/graphql/forms/__init__.py
+-rw-r--r--   0        0        0     1687 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/graphql/forms/mutations.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/graphql/schemes/__init__.py
+-rw-r--r--   0        0        0     2065 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/graphql/schemes/mutations.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/graphql/sentry/__init__.py
+-rw-r--r--   0        0        0      419 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/graphql/sentry/utils.py
+-rw-r--r--   0        0        0     1342 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/graphql/sentry/views.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/graphql/tests/__init__.py
+-rw-r--r--   0        0        0     2144 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/graphql/tests/base_test.py
+-rw-r--r--   0        0        0     1360 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2177 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/mail/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/mail/backends/__init__.py
+-rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/mail/backends/whitelist_smtp.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/management/commands/__init__.py
+-rw-r--r--   0        0        0      303 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/management/commands/validate_test_structure.py
+-rw-r--r--   0        0        0     2550 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/managers.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/middleware/__init__.py
+-rw-r--r--   0        0        0     1050 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/middleware/current_user.py
+-rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/mixins/__init__.py
+-rw-r--r--   0        0        0     1958 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/mixins/bleacher.py
+-rw-r--r--   0        0        0     1378 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/mixins/models.py
+-rw-r--r--   0        0        0      246 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/mixins/validation.py
+-rw-r--r--   0        0        0     2592 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/models.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/selectors/__init__.py
+-rw-r--r--   0        0        0      362 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/selectors/base.py
+-rw-r--r--   0        0        0     1061 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/selectors/permission.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/sentry/__init__.py
+-rw-r--r--   0        0        0      668 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/sentry/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/services/__init__.py
+-rw-r--r--   0        0        0     3223 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/services/custom_scrubber.py
+-rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/templatetags/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-04 10:28:20.863829 ambient-toolbox-8.1.1/ambient_toolbox/templatetags/ai_date_tags.py
+-rw-r--r--   0        0        0      675 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.1/ambient_toolbox/templatetags/ai_email_tags.py
+-rw-r--r--   0        0        0      807 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.1/ambient_toolbox/templatetags/ai_file_tags.py
+-rw-r--r--   0        0        0      194 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.1/ambient_toolbox/templatetags/ai_helper_tags.py
+-rw-r--r--   0        0        0     1375 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.1/ambient_toolbox/templatetags/ai_number_tags.py
+-rw-r--r--   0        0        0      384 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.1/ambient_toolbox/templatetags/ai_object_tags.py
+-rw-r--r--   0        0        0      654 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.1/ambient_toolbox/templatetags/ai_string_tags.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.1/ambient_toolbox/tests/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.1/ambient_toolbox/tests/errors.py
+-rw-r--r--   0        0        0     5145 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.1/ambient_toolbox/tests/mixins.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.1/ambient_toolbox/tests/structure_validator/__init__.py
+-rw-r--r--   0        0        0      397 2023-05-04 10:28:20.879472 ambient-toolbox-8.1.1/ambient_toolbox/tests/structure_validator/settings.py
+-rw-r--r--   0        0        0     4634 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/tests/structure_validator/test_structure_validator.py
+-rw-r--r--   0        0        0      261 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/utils/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/utils/cache.py
+-rw-r--r--   0        0        0     5971 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/utils/date.py
+-rw-r--r--   0        0        0     1469 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/utils/file.py
+-rw-r--r--   0        0        0      343 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/utils/log_whodid.py
+-rw-r--r--   0        0        0      574 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/utils/math.py
+-rw-r--r--   0        0        0      935 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/utils/model.py
+-rw-r--r--   0        0        0     3970 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/utils/named_tuple.py
+-rw-r--r--   0        0        0     3804 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/utils/string.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/view_layer/__init__.py
+-rw-r--r--   0        0        0      750 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/view_layer/form_mixins.py
+-rw-r--r--   0        0        0      485 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/view_layer/formset_mixins.py
+-rw-r--r--   0        0        0     2998 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/view_layer/formset_view_mixin.py
+-rw-r--r--   0        0        0     1585 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/view_layer/htmx_mixins.py
+-rw-r--r--   0        0        0     2110 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/view_layer/mixins.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/view_layer/tests/__init__.py
+-rw-r--r--   0        0        0     4124 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/view_layer/tests/mixins.py
+-rw-r--r--   0        0        0     1882 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/ambient_toolbox/view_layer/views.py
+-rw-r--r--   0        0        0      654 2023-05-05 09:18:19.915141 ambient-toolbox-8.1.1/docs/Makefile
+-rw-r--r--   0        0        0     2803 2023-05-05 09:18:19.910900 ambient-toolbox-8.1.1/docs/conf.py
+-rw-r--r--   0        0        0     6731 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/docs/features/admin.md
+-rw-r--r--   0        0        0       35 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/docs/features/changelog.rst
+-rw-r--r--   0        0        0     2313 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/docs/features/context_manager.md
+-rw-r--r--   0        0        0      549 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/docs/features/context_processors.md
+-rw-r--r--   0        0        0     7273 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/docs/features/database_anonymisation.md
+-rw-r--r--   0        0        0     6807 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/docs/features/djangorestframework.md
+-rw-r--r--   0        0        0     2554 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/docs/features/gitlab.md
+-rw-r--r--   0        0        0     6567 2023-05-04 10:28:20.883484 ambient-toolbox-8.1.1/docs/features/graphql.md
+-rw-r--r--   0        0        0     1020 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/mail.md
+-rw-r--r--   0        0        0     5891 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/managers.md
+-rw-r--r--   0        0        0     5951 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/mixins.md
+-rw-r--r--   0        0        0     1553 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/models.md
+-rw-r--r--   0        0        0     4454 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/selectors.md
+-rw-r--r--   0        0        0     1078 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/sentry.md
+-rw-r--r--   0        0        0     4978 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/services.md
+-rw-r--r--   0        0        0     1574 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/setup.md
+-rw-r--r--   0        0        0     5338 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/tests.md
+-rw-r--r--   0        0        0      232 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/utils.rst
+-rw-r--r--   0        0        0      527 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/utils/cache.md
+-rw-r--r--   0        0        0     7417 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/utils/date.md
+-rw-r--r--   0        0        0      737 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/utils/math.md
+-rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/utils/model.md
+-rw-r--r--   0        0        0     2405 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/utils/named_tuple.md
+-rw-r--r--   0        0        0     5861 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/utils/string.md
+-rw-r--r--   0        0        0    15067 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/features/view-layer.md
+-rw-r--r--   0        0        0     1157 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2023-05-05 09:18:19.911901 ambient-toolbox-8.1.1/docs/make.bat
+-rw-r--r--   0        0        0      677 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/manage.py
+-rw-r--r--   0        0        0     4051 2023-05-05 09:18:19.896869 ambient-toolbox-8.1.1/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/pytest.ini
+-rw-r--r--   0        0        0       56 2023-05-05 09:18:19.898901 ambient-toolbox-8.1.1/pytest.init
+-rw-r--r--   0        0        0     1770 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/settings.py
+-rw-r--r--   0        0        0       69 2023-05-05 09:18:19.906900 ambient-toolbox-8.1.1/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/api/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/api/serializers.py
+-rw-r--r--   0        0        0      257 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/api/urls.py
+-rw-r--r--   0        0        0      524 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/api/views.py
+-rw-r--r--   0        0        0      219 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/forms.py
+-rw-r--r--   0        0        0       97 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/managers.py
+-rw-r--r--   0        0        0     6151 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/migrations/__init__.py
+-rw-r--r--   0        0        0     3363 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/models.py
+-rw-r--r--   0        0        0      162 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/selectors.py
+-rw-r--r--   0        0        0     1449 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/templates/403.html
+-rw-r--r--   0        0        0      145 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/templates/testapp/test_template.html
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/tests/missing_init/test_ok.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.1.1/testapp/tests/subdirectory/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/testapp/tests/subdirectory/missing_test_prefix.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/testapp/tests/subdirectory/test_ok.py
+-rw-r--r--   0        0        0      382 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/testapp/urls.py
+-rw-r--r--   0        0        0      505 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/testapp/views.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/admin/model_admin_mixins/__init__.py
+-rw-r--r--   0        0        0     2607 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py
+-rw-r--r--   0        0        0     1900 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py
+-rw-r--r--   0        0        0     1683 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py
+-rw-r--r--   0        0        0     1184 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py
+-rw-r--r--   0        0        0     3871 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py
+-rw-r--r--   0        0        0     1492 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/admin/model_admin_mixins/test_fetch_object_mixin.py
+-rw-r--r--   0        0        0     1909 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/ambient_toolbox/__init__.py
+-rw-r--r--   0        0        0     7503 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/ambient_toolbox/test_test_structure_validator.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/drf/__init__.py
+-rw-r--r--   0        0        0     2579 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/drf/test_fields.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/mixins/__init__.py
+-rw-r--r--   0        0        0      364 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/mixins/validation.py
+-rw-r--r--   0        0        0      499 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/query_selectors/test_base.py
+-rw-r--r--   0        0        0     1631 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/query_selectors/test_permission.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/selectors/__init__.py
+-rw-r--r--   0        0        0      553 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_admin_forms.py
+-rw-r--r--   0        0        0     1612 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_admin_inlines.py
+-rw-r--r--   0        0        0     2651 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_admin_model_admins_classes.py
+-rw-r--r--   0        0        0     2899 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_admin_view_mixins.py
+-rw-r--r--   0        0        0     2218 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_context_manager.py
+-rw-r--r--   0        0        0      822 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_log_whodid.py
+-rw-r--r--   0        0        0     1169 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_managers.py
+-rw-r--r--   0        0        0     1628 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_math.py
+-rw-r--r--   0        0        0     2593 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_middleware.py
+-rw-r--r--   0        0        0     1200 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_mixins_models.py
+-rw-r--r--   0        0        0     1669 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_models.py
+-rw-r--r--   0        0        0     1780 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_rest_api_mixins.py
+-rw-r--r--   0        0        0      664 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_scrubbing_service.py
+-rw-r--r--   0        0        0     1197 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_sentry_helper.py
+-rw-r--r--   0        0        0      289 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_utils_cache.py
+-rw-r--r--   0        0        0    12741 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_utils_date.py
+-rw-r--r--   0        0        0     1593 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_utils_file.py
+-rw-r--r--   0        0        0      933 2023-05-04 10:28:20.911132 ambient-toolbox-8.1.1/tests/test_utils_model.py
+-rw-r--r--   0        0        0     3807 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.1/tests/test_utils_named_tuple.py
+-rw-r--r--   0        0        0     5343 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.1/tests/test_utils_string.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.1/tests/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.1/tests/tests/mixins/__init__.py
+-rw-r--r--   0        0        0      371 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.1/tests/tests/mixins/models.py
+-rw-r--r--   0        0        0      817 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.1/tests/tests/mixins/test_django_message_framework.py
+-rw-r--r--   0        0        0     2483 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.1/tests/tests/mixins/test_request_provider_mixin.py
+-rw-r--r--   0        0        0     2057 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.1/tests/tests/test_mail_backends.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.1/tests/view_layer/__init__.py
+-rw-r--r--   0        0        0     1891 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.1/tests/view_layer/test_formset_mixins.py
+-rw-r--r--   0        0        0     1564 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.1/tests/view_layer/test_htmx_response_mixin.py
+-rw-r--r--   0        0        0     3458 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.1/tests/view_layer/test_meta_mixins.py
+-rw-r--r--   0        0        0     1361 2023-05-04 10:28:20.926757 ambient-toolbox-8.1.1/tests/view_layer/test_views.py
+-rw-r--r--   0        0        0     7729 1970-01-01 00:00:00.000000 ambient-toolbox-8.1.1/PKG-INFO
```

### Comparing `ambient-toolbox-8.1.0/.ambient-package-update/metadata.py` & `ambient-toolbox-8.1.1/.ambient-package-update/metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 This package was previously known as [ai_django_core](https://pypi.org/project/ai-django-core/). Due to the
 misleading nature of the name, we chose to rename it with something more meaningful.
 
 The migration is really simple, just:
 
 * Install ambient-toolbox and remove the dependency to ai-django-core
 * Search and replace all usages of `from ai_django_core...` to `from ambient_toolbox...`
+* The class-based mail functionality was moved to a separate package called
+[django-pony-express](https://pypi.org/project/django-pony-express/).
 """,
     ),
     dependencies=[
         'Django>=2.2.28',
         'bleach>=1.4,<6',
         'python-dateutil>=2.5.3',
     ],
```

### Comparing `ambient-toolbox-8.1.0/.github/workflows/ci.yml` & `ambient-toolbox-8.1.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/.gitignore` & `ambient-toolbox-8.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/.gitlab-ci.yml` & `ambient-toolbox-8.1.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/.pre-commit-config.yaml` & `ambient-toolbox-8.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/.readthedocs.yml` & `ambient-toolbox-8.1.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/CHANGES.md` & `ambient-toolbox-8.1.1/CHANGES.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,489 +1,492 @@
-# Changelog
-
-**8.1.0** (2023-05-04)
-  * Support for Django 4.2 added
-
-**8.0.2** (2023-05-04)
-  * Bugfix in documentation
-
-**8.0.1** (2023-05-04)
-  * Added migration guide to docs
-
-**8.0.0** (2023-05-01)
-  * Rename and re-release package as "ambient-toolbox"
-  * Extracted class-based mails as [django-pony-express](https://test.pypi.org/project/django-pony-express/)
-
-**7.0.0** (2023-03-28)
-  * *Breaking change:* Dropped Python 3.7 support due to end of lifetime
-  * Added `ALWAYS_UPDATE_FIELDS` flag to `CommonInfo` model
-  * Added `ruff` linter and replaced `flake8` and `isort` with it
-  * Excluded not officially supported Python versions for certain Django releases for test matrix
-
-**6.12.0** (2023-03-16)
-  * Added `validate_test_structure` management command for validating project test structure
-  * Fixed syntax error in docs
-  * Fixed typo in docstring of `concat` method
-  * Improved code in test app
-
-**6.11.0** (2023-02-19)
-  * Added `HtmxResponseMixin` for Django views
-  * Added missing `object` class attribute to `ToggleView`
-  * Updated local lint, build and test suite to Python 3.11
-  * Updated readme file for contribution
-
-**6.10.1** (2023-02-13)
-  * Updated bug in documentation
-
-**6.10.0** (2023-02-13)
-  * Added test mixin `DjangoMessagingFrameworkTestMixin`
-  * Added python 3.11 to test matrix and supported versions
-
-**6.9.2** (2023-02-06)
-  * Updated `pre-commit` packages
-
-**6.9.1** (2023-01-25)
-  * Set version border for dependency "bleach" because of breaking changes
-
-**6.9.0** (2023-01-18)
-  * Added "GITLAB_CI_DISABLE_COVERAGE" flag to coverage script for Gitlab pipeline
-  * Fixed typo in the docs
-
-**6.8.4** (2023-01-11)
-  * Moved changelog to "CHANGES.md" to make Dependabot understand/find it
-
-**6.8.3** (2023-01-11)
-  * Fixed bug with filtering in EmailTestService for subject passing a gettext_lazy object (second occurrence)
-
-**6.8.2** (2023-01-11)
-  * Fixed bug with filtering in EmailTestService for subject passing a gettext_lazy object
-
-**6.8.1** (2022-12-20)
-  * Fixed broken init file
-
-**6.8.0** (2022-12-19)
-  * Added `SaveWithoutSignalsMixin` model mixin
-
-**6.7.0** (2022-11-25)
-  * Added `Selector` base class
-  * Added `AbstractUserSpecificSelectorMixin` and `GloballyVisibleSelector` helpers for selector pattern
-  * Added documentation for new selector pattern
-  * Added `django-upgrade` to linting
-  * Added date helper `get_first_and_last_of_month`
-  * Updated linting tools `black` & `pyupgrade`
-  * Added `pyupgrade` and `django-upgrade` to pipeline
-
-**6.6.3** (2022-11-18)
-  * Fixed `BaseViewPermissionTestMixin` to work with custom user models
-
-**6.6.2** (2022-10-12)
-  * Updated documentation of mixin `PermissionModelMixin` in regard to a caveat with default permissions
-
-**6.6.1** (2022-10-12)
-  * Bugfix in documentation of mixin `PermissionModelMixin`
-
-**6.6.0** (2022-10-12)
-  * Added model mixin `PermissionModelMixin` to provide a neat way of handling non-(database)-model-related permissions
-  * Improved mixin documentation
-  * Updated GitHub Actions
-
-**6.5.0** (2022-09-29)
-  * Added view mixin `UserInFormKwargsMixin` to pass the user to a form in a `FormView`, `CreateView` or `UpdateView`
-
-**6.4.0** (2022-09-29)
-  * Models inheriting from `CommonInfo` will automatically save the four CommonInfo fields in addition to the fields
-    selected when using `update_fields` in the models save method.
-
-**6.3.2** (2022-09-29)
-  * Updated gitlab-ci for showing tests in MR
-
-**6.3.1** (2022-09-19)
-  * Updated GitHub test matrix OS
-
-**6.3.0** (2022-09-19)
-  * Integrated `flake8-bugbear` and `pyupgrade` including required code adjustments
-  * Improved security vulnerability scanning
-  * Updated local build and test suite to Python 3.10
-  * Added `flake8-bugbear` to Quality Assurance measures
-  * Added `pyupgrade` to Quality Assurance measures
-
-**6.2.3** (2022-08-15)
-  * Fixed some translations
-
-**6.2.2** (2022-08-12)
-  * Added Django 4.1 to test matrix and compatible versions
-
-**6.2.1** (2022-08-12)
-  * Improved detecting of permission mismatches in view test mixin `BaseViewPermissionTestMixin`
-
-**6.2.0** (2022-07-13)
-  * Added test case for `BaseViewPermissionTestMixin` to ensure that defined permissions exist in the database
-
-**6.1.3** (2022-06-30)
-  * Clarified docs for `GloballyVisibleQuerySet`
-
-**6.1.2** (2022-06-30)
-  * Extended docs for `BaseViewPermissionTestMixin` with limitation when using a caching wrapper
-
-**6.1.1** (2022-06-29)
-  * Fixed unittest for django<3.2
-
-**6.1.0** (2022-06-29)
-  * Added `DjangoPermissionRequiredMixin` for Django views and supporting test mixin `BaseViewPermissionTestMixin`
-  * Increased minimal required bugfix version for Django 2.2
-  * Updated Readme file
-
-**6.0.0** (2022-05-19)
-  * *Breaking change:* Removed `ffmpeg` helper methods `generate_video_thumbnail()` and `get_video_length()`
-  * Added `CleanOnSaveMixin`
-  * black and isort linting integrated
-  * Added pre-commit hooks for linting
-
-**5.14.1** (2022-04-06)
-  * Dropped support for deprecated Python 3.6
-
-**5.14.0** (2022-04-06)
-  * `EmailTestService` can now filter for subjects using regular expressions
-
-**5.13.7** (2022-03-14)
-  * Fixed typo in coverage validator
-
-**5.13.6** (2022-03-11)
-  * Improved console logging for coverage validator
-
-**5.13.5** (2022-02-28)
-  * Improved motivation in class-based email docs
-
-**5.13.4** (2022-02-28)
-  * Added Script for updating mirror
-  * Fixed typo in documentation
-
-**5.13.3** (2022-02-23)
-  * Added GitHub action matrix for running tests on django/python combinations
-  * Updated Ambient email addresses to new domain
-  * Removed django <4.0 restriction
-  * Fixed tests for django 4.0
-
-**5.13.2** (2022-02-21)
-  * `CurrentUserMiddleware` bugfix, cleaning up user variable for single-threaded tests after request processing
-  * Fixed version typo in changelog
-
-**5.13.1** (2022-02-04)
-  * GraphQL docs bugfix
-
-**5.13.0** (2022-02-03)
-  * Added a view which allows logging errors to Sentry normally while using Graphene.
-
-**5.12.1** (2022-01-31)
-  * Fixed bug in Gitlab code coverage compare service documentation
-
-**5.12.0** (2022-01-28)
-  * Added Gitlab code coverage compare service `CoverageService` with documentation
-
-**5.11.1** (2022-01-24)
-  * Added docs for `ToggleView`
-  * Fixed some typos in `Readme.md` and `changelog.md`
-
-**5.11.0** (2022-01-24)
-  * Added generic `ToggleView`
-  * Updated some docstrings in `formset_view_mixin`
-
-**5.10.1** (2021-12-10)
-  * Added docs about GDPR-compliant use of sentry with user data
-  * Fixed some versions to make Sphinx build work again
-
-**5.10.0** (2021-12-10)
-  * Added helper method for sentry to GDPR-compliant remove sensitive user data from event
-  * Updated type hints in `BaseEmailServiceFactory` init method
-  * Improved docs for method `get_start_and_end_date_from_calendar_week`
-
-**5.9.1** (2021-11-25)
-  * Fixed typo in custom scrubber class logging
-  * Rewrote permission manager docs and added better best practice
-  * Update in email testing docs
-
-**5.9.0** (2021-11-18)
-    * Added default truncate of django session table to `AbstractScrubbingService`
-
-**5.8.0** (2021-11-11)
-    * Added `url` parameter to `RequestProviderMixin`
-
-**5.7.4** (2021-11-08)
-    * Added missing documentation about semantic database anonymisation
-    * Added missing documentation about string utils
-    * Added missing documentation about `get_namedtuple_choices()` helper
-    * Added missing documentation about `CrispyLayoutFormMixin`
-    * Added missing documentation about `ClassBasedViewTestMixin`
-
-**5.7.3** (2021-10-22)
-    * Added missing documentation about email testing
-    * Updated Readme file
-
-**5.7.2** (2021-10-21)
-    * Fixed `flit` configuration
-
-**5.7.1** (2021-10-21)
-    * Setup `flit` for release management
-
-**5.7.0** (2021-10-15)
-    * Added admin mixin `DeactivatableChangeViewAdminMixin`
-    * Added `response` parameter to testing middlewares
-
-**5.6.0** (2021-09-01)
-    * Extracted embedded form valid logic to separate method with super call in `_FormsetMixin`
-    * Added documentation about `FormsetCreateViewMixin` and `FormsetUpdateViewMixin`
-
-**5.5.2** (2021-08-24)
-    * Added documentation about `BleacherMixin`
-
-**5.5.1** (2021-08-24)
-    * Added explicit declaration of bleacher field list attribute `BLEACH_FIELD_LIST` in `BleacherMixin`
-
-**5.5.0** (2021-08-02)
-    * Added validation for user object in `RequestProviderMixin`
-    * Added link to changelog in setup.py
-    * Moved minimum django version to 2.2
-
-**5.4.0** (2021-06-28)
-    * Added `__len__` and `__iter__` to EmailTestService
-    * EmailTestService uses EmailTestServiceMail instances, which wrap the underlying Django mail objects, and provide
-      additional assertion functions
-
-**5.3.0** (2021-06-16)
-    * Added `method` kwarg to `RequestProviderMixin.get_request()`
-
-**5.2.2** (2021-05-27)
-    * Fixed a bug in `BaseEmailService` where txt part was rendered sometimes with weird line breaks
-    * Added Bugtracker link to `setup.py`
-
-**5.2.1** (2021-05-12)
-    * Translation files were missing in wheel
-    * Bugfix in docs
-
-**5.2.0** (2021-05-11)
-    * Changed all translatable texts to English base version
-    * Added German translation file for current translatable
-    * Updated RequestProviderMixin.get_request() type hinting
-    * Added documentation for database anonymisation / django-scrubber wrapper
-
-**5.1.1** (2021-04-21)
-    * Extended email attachment functionality to be able to define filename and mimetype
-
-**5.1.0** (2021-04-20)
-    * *Breaking change:* Fixed typo in `WhitelistEmailBackend.whitify_mail_adresses` method name. Method is now
-      called `whitify_mail_addresses`
-    * Moved assignment of `WhitelistEmailBackend` settings var to static methods to be able to overwrite them if needed
-    * Added documentation about `WhitelistEmailBackend`
-    * Added some type hinting to `WhitelistEmailBackend`
-    * Added formset mixin `CountChildrenFormsetMixin`
-    * Added djangorestframework field `RecursiveField`
-    * Added `get_attachments()` method to `BaseEmailService` and extended constructor to accept a
-      variable `attachment_list`
-
-**5.0.0** (2021-03-26)
-    * *Breaking change:* Moved `ReadOnlyAdmin` and `EditableOnlyAdmin` to package `model_admins.classes`
-      and `ReadOnlyTabularInline` to package `model_admins.inlines` to enable better structuring of new admin components
-    * Fixed some inconsistencies within `ReadOnlyAdmin`, `EditableOnlyAdmin` and `ReadOnlyTabularInline` classes
-    * Added `admin.views` package containing a base crispy form, and a mixin to turn any regular django view into a nice
-      and cozy django admin view
-    * Added an abundance of `model_admins.mixins`: `AdminCreateFormMixin`, `AdminNoInlinesForCreateMixin`
-      ,`AdminRequestInFormMixin`, `FetchParentObjectInlineMixin`, `FetchObjectMixin`, `CommonInfoAdminMixin`
-    * Added `RequestProviderMixin` to easily create a dummy request in unittests
-    * Added support for django 3.2 and dropped support for 2.0, 2.1 and 3.0
-    * Added support for Python 3.9 and dropped support for 3.5
-    * Updated test python version to 3.9
-
-**4.2.1** (2021-03-17)
-    * Added some links to setup.py for pypi
-    * Added some documentation for setting up the toolbox
-
-**4.2.0** (2021-03-12)
-    * Added ``GloballyVisibleQuerySet`` including tests and documentation
-    * Added ``BaseViewSetTestMixin`` for the djangorestframework plugin
-    * Fixed some typos in the documentation
-
-**4.1.2** (2021-03-05)
-    * Added kwargs parameter to init-method of `BaseEmailServiceFactory`
-
-**4.1.1** (2021-03-04)
-    * Fixed a bug in the documentation
-
-**4.1.0** (2021-02-25)
-    * Added class `BaseEmailService` for easier email creation and factory `BaseEmailServiceFactory`
-      for multiple (mostly personalised) emails
-    * Added `html2text` as a dependency to be able to automatically process the text part of an email from the html
-      template
-
-**4.0.2** (2021-02-24)
-    * Fixed a bug in ``EmailTestService.assert_body_contains()`` method to make it work for emails NOT having an HTML
-      part
-
-**4.0.1** (2021-01-29)
-    * Optimised code of function `test_get_value_from_tuple_by_key_found()`
-    * Added unittests for named tuple functions
-
-**4.0.0** (2020-11-10)
-    * *Breaking change:* Moved view mixin ``RequestInFormKwargsMixin`` from ``mixin.forms`` to proper place
-      ``mixin.views``
-    * *Breaking change:* Removed string helper function ``restore_windows1252controls()``, ``number_to_text()`` and
-      ``replace_link_pattern()``
-    * *Breaking change:* Removed choice converter function ``get_name_by_value()`` in favour
-      of ``get_value_from_tuple_by_key()``
-    * *Breaking change:* Removed date converter function ``get_seconds()`` because Python 3.6 already provides
-      a `total_seconds()` method
-    * *Breaking change:* Removed date converter function ``get_current_datetime()`` because django already provides
-      the `timezone.now()` method
-    * *Breaking change:* Removed date converter function ``diff_month()`` in favour of ``date_month_delta()``
-    * *Breaking change:* Merged ``converter`` package in ``utils`` package
-    * *Breaking change:* Moved view-layer-based helpers to extra requirement ``view-layer``: `_FormsetMixin`,
-      `FormsetUpdateViewMixin`, `FormsetCreateViewMixin`, `CrispyLayoutFormMixin`, `CustomPermissionMixin`
-      , `RequestInFormKwargsMixin`
-    * Simplified code of function ``float_to_string()``
-    * Added type hinting to lots of helper functions
-    * Updated and restructured documentation
-    * Added security check for dependencies in local pipeline
-    * Removed some old python 2.7 syntax
-
-**3.5.2** (2021-01-07)
-    * Bugfix with args and kwargs in ``ReadOnlyTabularInline``
-
-**3.5.1** (2020-11-19)
-    * Bugfix with args and kwargs in ``ClassBasedViewTestMixin``
-
-**3.5.0** (2020-11-10)
-    * Merged package ``graphene-django-ai`` into this package and enabled graphql-specific installation
-      with `pip install ambient_toolbox[graphql]`
-    * Added some files for readthedocs.io and updated Readme
-
-**3.4.0** (2020-10-30)
-    * Moved tests out of package scope
-    * Updated test python version to 3.8
-    * Added tests for context manager ``TempDisconnectSignal`` with test setup
-
-**3.3.0** (2020-10-30)
-    * Merged package ``ai-drf-core`` into this package and enabled djangorestframework-specific installation
-      with `pip install ambient_toolbox[drf]`
-    * Added ``BaseModelSerializer`` and ``CommonInfoSerializer``
-    * Incremented dependencies django and bleach to previous versions latest bugfix release
-
-**3.2.0** (2020-10-16)
-    * Added ``AbstractPermissionMixin``, ``AbstractUserSpecificQuerySet`` and ``AbstractUserSpecificManager`` abstract
-      managers
-    * Removed deprecated `antivir` package
-    * Added Sphinx documentation setup to package
-
-**3.1.0** (2020-10-14)
-    * Added context manager ``TempDisconnectSignal`` to nicely disable model signals temporarily
-    * Moved dev dependencies to ``extras_require`` in the setup file
-
-**3.0.2** (2020-10-15)
-    * Imports all utils into the modules scope
-    * Re-translated some docstrings into English
-    * Added tests for the `log_whodid` util function
-
-**3.0.1** (2020-10-12)
-    * Added missing ``__init__.py`` file to package mail.services
-
-**3.0.0** (2020-09-09)
-    * *Breaking change:*  Renamed package from `ai` to `ambient_toolbox` to clarify dependencies for usages
-    * Finished code linting
-    * Removed unused imports in antivirus util package
-
-**2.3.0** (2020-08-07)
-    * Changed `ugettext_lazy` to `gettext_lazy` to tackle django 4.0 deprecation warnings
-
-**2.2.1** (2020-07-01)
-    * Removed misleading inheritance of mixin `ClassBasedViewTestMixin` from `TestCase`
-
-**2.2.0** (2020-07-01)
-    * Added response class `CustomPermissionMixin`
-
-**2.1.2** (2020-04-30)
-    * Extended pypi documentation with classifiers
-
-**2.1.1** (2020-04-24)
-    * Refactors open calls to use context managers
-    * Refactors the test setup
-    * Configures coverage
-    * Adds a coverage report to the CI
-
-**2.1.0** (2020-04-20)
-    * Removed password generator method `generate_password`
-    * Renamed math method `round_up_to_decimal` to `round_up_decimal`
-    * Added math method `round_to_decimal`
-    * Updated metadata in setup.cfg
-
-**2.0.0** (2020-04-09)
-    * Dropped Python 2.x support
-    * Removed explicit dependency to package `mock` and using implicit one via unittest
-    * Improved linting
-
-**1.2.14** (2020-04-06)
-    * Fixed a bug with session setup in `ClassBasedViewTestMixin`
-
-**1.2.13** (2020-04-02)
-    * Added ``DELETE`` method for testing mixing `ClassBasedViewTestMixin`
-
-**1.2.12** (2020-02-14)
-    * Added CBV testing mixing `ClassBasedViewTestMixin`
-
-**1.2.11** (2020-01-28)
-    * Bugfix in documentation
-
-**1.2.10** (2020-01-28)
-    * Improved documentation
-
-**1.2.9** (2020-01-02)
-    * Extended and improved class `AbstractScrubbingService`
-
-**1.2.8** (2019-12-13)
-    * Added custom scrubber class `AbstractScrubbingService` to provide a helper for adding custom scrubbing logic for
-      data anonymisation
-
-**1.2.7** (2019-07-11)
-    * Added email testing class `EmailTestService` to provide a wrapper for better email unittests
-
-**1.2.6** (2019-07-02)
-    * Added helper class `tz_today()` to provide an easy getter for a timezone-aware today
-
-**1.2.5** (2019-06-25)
-    * Added helper class `DateHelper` to provide constants to use in django's ORM lookup `__week_day`
-
-**1.2.4** (2019-05-20)
-    * More refactoring on `CurrentUserMiddleware` to make it easier to override internal functions
-
-**1.2.3** (2019-05-20)
-    * Moved `get_current_user` function inside `CurrentUserMiddleware` as a static method to enable devs to override it
-
-**1.2.2** (2019-04-05)
-    * Updated deployment documentation
-    * Added markdown support to Readme file
-
-**1.2.1** (2019-03-25)
-    * Fixed bug causing `CommonInfo` middleware to not set `lastmodified_by` on object creation
-
-**1.2.0** (2019-03-19)
-    * Added `CommonInfo` middleware
-
-**1.1.8**
-    * Readonly admin classes
-    * Date util functions
-    * Clear cache helper
-
-**1.1.7**
-    * Settings for whitelist email services added
-    * Formset mixins added
-
-**1.1.6**
-    * Modifications to antivirus field
-
-**1.1.5**
-    * Updated setup.py with newer information
-
-**1.1.4**
-    * Bleacher mixin bugfix
-
-**1.1.3**
-    * Bleacher mixin added
-
-**< 1.1.3**
-    * Ancient history :)
+# Changelog
+
+**8.1.1** (2023-05-04)
+  * Updated migration docs
+
+**8.1.0** (2023-05-04)
+  * Support for Django 4.2 added
+
+**8.0.2** (2023-05-04)
+  * Bugfix in documentation
+
+**8.0.1** (2023-05-04)
+  * Added migration guide to docs
+
+**8.0.0** (2023-05-01)
+  * Rename and re-release package as "ambient-toolbox"
+  * Extracted class-based mails as [django-pony-express](https://test.pypi.org/project/django-pony-express/)
+
+**7.0.0** (2023-03-28)
+  * *Breaking change:* Dropped Python 3.7 support due to end of lifetime
+  * Added `ALWAYS_UPDATE_FIELDS` flag to `CommonInfo` model
+  * Added `ruff` linter and replaced `flake8` and `isort` with it
+  * Excluded not officially supported Python versions for certain Django releases for test matrix
+
+**6.12.0** (2023-03-16)
+  * Added `validate_test_structure` management command for validating project test structure
+  * Fixed syntax error in docs
+  * Fixed typo in docstring of `concat` method
+  * Improved code in test app
+
+**6.11.0** (2023-02-19)
+  * Added `HtmxResponseMixin` for Django views
+  * Added missing `object` class attribute to `ToggleView`
+  * Updated local lint, build and test suite to Python 3.11
+  * Updated readme file for contribution
+
+**6.10.1** (2023-02-13)
+  * Updated bug in documentation
+
+**6.10.0** (2023-02-13)
+  * Added test mixin `DjangoMessagingFrameworkTestMixin`
+  * Added python 3.11 to test matrix and supported versions
+
+**6.9.2** (2023-02-06)
+  * Updated `pre-commit` packages
+
+**6.9.1** (2023-01-25)
+  * Set version border for dependency "bleach" because of breaking changes
+
+**6.9.0** (2023-01-18)
+  * Added "GITLAB_CI_DISABLE_COVERAGE" flag to coverage script for Gitlab pipeline
+  * Fixed typo in the docs
+
+**6.8.4** (2023-01-11)
+  * Moved changelog to "CHANGES.md" to make Dependabot understand/find it
+
+**6.8.3** (2023-01-11)
+  * Fixed bug with filtering in EmailTestService for subject passing a gettext_lazy object (second occurrence)
+
+**6.8.2** (2023-01-11)
+  * Fixed bug with filtering in EmailTestService for subject passing a gettext_lazy object
+
+**6.8.1** (2022-12-20)
+  * Fixed broken init file
+
+**6.8.0** (2022-12-19)
+  * Added `SaveWithoutSignalsMixin` model mixin
+
+**6.7.0** (2022-11-25)
+  * Added `Selector` base class
+  * Added `AbstractUserSpecificSelectorMixin` and `GloballyVisibleSelector` helpers for selector pattern
+  * Added documentation for new selector pattern
+  * Added `django-upgrade` to linting
+  * Added date helper `get_first_and_last_of_month`
+  * Updated linting tools `black` & `pyupgrade`
+  * Added `pyupgrade` and `django-upgrade` to pipeline
+
+**6.6.3** (2022-11-18)
+  * Fixed `BaseViewPermissionTestMixin` to work with custom user models
+
+**6.6.2** (2022-10-12)
+  * Updated documentation of mixin `PermissionModelMixin` in regard to a caveat with default permissions
+
+**6.6.1** (2022-10-12)
+  * Bugfix in documentation of mixin `PermissionModelMixin`
+
+**6.6.0** (2022-10-12)
+  * Added model mixin `PermissionModelMixin` to provide a neat way of handling non-(database)-model-related permissions
+  * Improved mixin documentation
+  * Updated GitHub Actions
+
+**6.5.0** (2022-09-29)
+  * Added view mixin `UserInFormKwargsMixin` to pass the user to a form in a `FormView`, `CreateView` or `UpdateView`
+
+**6.4.0** (2022-09-29)
+  * Models inheriting from `CommonInfo` will automatically save the four CommonInfo fields in addition to the fields
+    selected when using `update_fields` in the models save method.
+
+**6.3.2** (2022-09-29)
+  * Updated gitlab-ci for showing tests in MR
+
+**6.3.1** (2022-09-19)
+  * Updated GitHub test matrix OS
+
+**6.3.0** (2022-09-19)
+  * Integrated `flake8-bugbear` and `pyupgrade` including required code adjustments
+  * Improved security vulnerability scanning
+  * Updated local build and test suite to Python 3.10
+  * Added `flake8-bugbear` to Quality Assurance measures
+  * Added `pyupgrade` to Quality Assurance measures
+
+**6.2.3** (2022-08-15)
+  * Fixed some translations
+
+**6.2.2** (2022-08-12)
+  * Added Django 4.1 to test matrix and compatible versions
+
+**6.2.1** (2022-08-12)
+  * Improved detecting of permission mismatches in view test mixin `BaseViewPermissionTestMixin`
+
+**6.2.0** (2022-07-13)
+  * Added test case for `BaseViewPermissionTestMixin` to ensure that defined permissions exist in the database
+
+**6.1.3** (2022-06-30)
+  * Clarified docs for `GloballyVisibleQuerySet`
+
+**6.1.2** (2022-06-30)
+  * Extended docs for `BaseViewPermissionTestMixin` with limitation when using a caching wrapper
+
+**6.1.1** (2022-06-29)
+  * Fixed unittest for django<3.2
+
+**6.1.0** (2022-06-29)
+  * Added `DjangoPermissionRequiredMixin` for Django views and supporting test mixin `BaseViewPermissionTestMixin`
+  * Increased minimal required bugfix version for Django 2.2
+  * Updated Readme file
+
+**6.0.0** (2022-05-19)
+  * *Breaking change:* Removed `ffmpeg` helper methods `generate_video_thumbnail()` and `get_video_length()`
+  * Added `CleanOnSaveMixin`
+  * black and isort linting integrated
+  * Added pre-commit hooks for linting
+
+**5.14.1** (2022-04-06)
+  * Dropped support for deprecated Python 3.6
+
+**5.14.0** (2022-04-06)
+  * `EmailTestService` can now filter for subjects using regular expressions
+
+**5.13.7** (2022-03-14)
+  * Fixed typo in coverage validator
+
+**5.13.6** (2022-03-11)
+  * Improved console logging for coverage validator
+
+**5.13.5** (2022-02-28)
+  * Improved motivation in class-based email docs
+
+**5.13.4** (2022-02-28)
+  * Added Script for updating mirror
+  * Fixed typo in documentation
+
+**5.13.3** (2022-02-23)
+  * Added GitHub action matrix for running tests on django/python combinations
+  * Updated Ambient email addresses to new domain
+  * Removed django <4.0 restriction
+  * Fixed tests for django 4.0
+
+**5.13.2** (2022-02-21)
+  * `CurrentUserMiddleware` bugfix, cleaning up user variable for single-threaded tests after request processing
+  * Fixed version typo in changelog
+
+**5.13.1** (2022-02-04)
+  * GraphQL docs bugfix
+
+**5.13.0** (2022-02-03)
+  * Added a view which allows logging errors to Sentry normally while using Graphene.
+
+**5.12.1** (2022-01-31)
+  * Fixed bug in Gitlab code coverage compare service documentation
+
+**5.12.0** (2022-01-28)
+  * Added Gitlab code coverage compare service `CoverageService` with documentation
+
+**5.11.1** (2022-01-24)
+  * Added docs for `ToggleView`
+  * Fixed some typos in `Readme.md` and `changelog.md`
+
+**5.11.0** (2022-01-24)
+  * Added generic `ToggleView`
+  * Updated some docstrings in `formset_view_mixin`
+
+**5.10.1** (2021-12-10)
+  * Added docs about GDPR-compliant use of sentry with user data
+  * Fixed some versions to make Sphinx build work again
+
+**5.10.0** (2021-12-10)
+  * Added helper method for sentry to GDPR-compliant remove sensitive user data from event
+  * Updated type hints in `BaseEmailServiceFactory` init method
+  * Improved docs for method `get_start_and_end_date_from_calendar_week`
+
+**5.9.1** (2021-11-25)
+  * Fixed typo in custom scrubber class logging
+  * Rewrote permission manager docs and added better best practice
+  * Update in email testing docs
+
+**5.9.0** (2021-11-18)
+    * Added default truncate of django session table to `AbstractScrubbingService`
+
+**5.8.0** (2021-11-11)
+    * Added `url` parameter to `RequestProviderMixin`
+
+**5.7.4** (2021-11-08)
+    * Added missing documentation about semantic database anonymisation
+    * Added missing documentation about string utils
+    * Added missing documentation about `get_namedtuple_choices()` helper
+    * Added missing documentation about `CrispyLayoutFormMixin`
+    * Added missing documentation about `ClassBasedViewTestMixin`
+
+**5.7.3** (2021-10-22)
+    * Added missing documentation about email testing
+    * Updated Readme file
+
+**5.7.2** (2021-10-21)
+    * Fixed `flit` configuration
+
+**5.7.1** (2021-10-21)
+    * Setup `flit` for release management
+
+**5.7.0** (2021-10-15)
+    * Added admin mixin `DeactivatableChangeViewAdminMixin`
+    * Added `response` parameter to testing middlewares
+
+**5.6.0** (2021-09-01)
+    * Extracted embedded form valid logic to separate method with super call in `_FormsetMixin`
+    * Added documentation about `FormsetCreateViewMixin` and `FormsetUpdateViewMixin`
+
+**5.5.2** (2021-08-24)
+    * Added documentation about `BleacherMixin`
+
+**5.5.1** (2021-08-24)
+    * Added explicit declaration of bleacher field list attribute `BLEACH_FIELD_LIST` in `BleacherMixin`
+
+**5.5.0** (2021-08-02)
+    * Added validation for user object in `RequestProviderMixin`
+    * Added link to changelog in setup.py
+    * Moved minimum django version to 2.2
+
+**5.4.0** (2021-06-28)
+    * Added `__len__` and `__iter__` to EmailTestService
+    * EmailTestService uses EmailTestServiceMail instances, which wrap the underlying Django mail objects, and provide
+      additional assertion functions
+
+**5.3.0** (2021-06-16)
+    * Added `method` kwarg to `RequestProviderMixin.get_request()`
+
+**5.2.2** (2021-05-27)
+    * Fixed a bug in `BaseEmailService` where txt part was rendered sometimes with weird line breaks
+    * Added Bugtracker link to `setup.py`
+
+**5.2.1** (2021-05-12)
+    * Translation files were missing in wheel
+    * Bugfix in docs
+
+**5.2.0** (2021-05-11)
+    * Changed all translatable texts to English base version
+    * Added German translation file for current translatable
+    * Updated RequestProviderMixin.get_request() type hinting
+    * Added documentation for database anonymisation / django-scrubber wrapper
+
+**5.1.1** (2021-04-21)
+    * Extended email attachment functionality to be able to define filename and mimetype
+
+**5.1.0** (2021-04-20)
+    * *Breaking change:* Fixed typo in `WhitelistEmailBackend.whitify_mail_adresses` method name. Method is now
+      called `whitify_mail_addresses`
+    * Moved assignment of `WhitelistEmailBackend` settings var to static methods to be able to overwrite them if needed
+    * Added documentation about `WhitelistEmailBackend`
+    * Added some type hinting to `WhitelistEmailBackend`
+    * Added formset mixin `CountChildrenFormsetMixin`
+    * Added djangorestframework field `RecursiveField`
+    * Added `get_attachments()` method to `BaseEmailService` and extended constructor to accept a
+      variable `attachment_list`
+
+**5.0.0** (2021-03-26)
+    * *Breaking change:* Moved `ReadOnlyAdmin` and `EditableOnlyAdmin` to package `model_admins.classes`
+      and `ReadOnlyTabularInline` to package `model_admins.inlines` to enable better structuring of new admin components
+    * Fixed some inconsistencies within `ReadOnlyAdmin`, `EditableOnlyAdmin` and `ReadOnlyTabularInline` classes
+    * Added `admin.views` package containing a base crispy form, and a mixin to turn any regular django view into a nice
+      and cozy django admin view
+    * Added an abundance of `model_admins.mixins`: `AdminCreateFormMixin`, `AdminNoInlinesForCreateMixin`
+      ,`AdminRequestInFormMixin`, `FetchParentObjectInlineMixin`, `FetchObjectMixin`, `CommonInfoAdminMixin`
+    * Added `RequestProviderMixin` to easily create a dummy request in unittests
+    * Added support for django 3.2 and dropped support for 2.0, 2.1 and 3.0
+    * Added support for Python 3.9 and dropped support for 3.5
+    * Updated test python version to 3.9
+
+**4.2.1** (2021-03-17)
+    * Added some links to setup.py for pypi
+    * Added some documentation for setting up the toolbox
+
+**4.2.0** (2021-03-12)
+    * Added ``GloballyVisibleQuerySet`` including tests and documentation
+    * Added ``BaseViewSetTestMixin`` for the djangorestframework plugin
+    * Fixed some typos in the documentation
+
+**4.1.2** (2021-03-05)
+    * Added kwargs parameter to init-method of `BaseEmailServiceFactory`
+
+**4.1.1** (2021-03-04)
+    * Fixed a bug in the documentation
+
+**4.1.0** (2021-02-25)
+    * Added class `BaseEmailService` for easier email creation and factory `BaseEmailServiceFactory`
+      for multiple (mostly personalised) emails
+    * Added `html2text` as a dependency to be able to automatically process the text part of an email from the html
+      template
+
+**4.0.2** (2021-02-24)
+    * Fixed a bug in ``EmailTestService.assert_body_contains()`` method to make it work for emails NOT having an HTML
+      part
+
+**4.0.1** (2021-01-29)
+    * Optimised code of function `test_get_value_from_tuple_by_key_found()`
+    * Added unittests for named tuple functions
+
+**4.0.0** (2020-11-10)
+    * *Breaking change:* Moved view mixin ``RequestInFormKwargsMixin`` from ``mixin.forms`` to proper place
+      ``mixin.views``
+    * *Breaking change:* Removed string helper function ``restore_windows1252controls()``, ``number_to_text()`` and
+      ``replace_link_pattern()``
+    * *Breaking change:* Removed choice converter function ``get_name_by_value()`` in favour
+      of ``get_value_from_tuple_by_key()``
+    * *Breaking change:* Removed date converter function ``get_seconds()`` because Python 3.6 already provides
+      a `total_seconds()` method
+    * *Breaking change:* Removed date converter function ``get_current_datetime()`` because django already provides
+      the `timezone.now()` method
+    * *Breaking change:* Removed date converter function ``diff_month()`` in favour of ``date_month_delta()``
+    * *Breaking change:* Merged ``converter`` package in ``utils`` package
+    * *Breaking change:* Moved view-layer-based helpers to extra requirement ``view-layer``: `_FormsetMixin`,
+      `FormsetUpdateViewMixin`, `FormsetCreateViewMixin`, `CrispyLayoutFormMixin`, `CustomPermissionMixin`
+      , `RequestInFormKwargsMixin`
+    * Simplified code of function ``float_to_string()``
+    * Added type hinting to lots of helper functions
+    * Updated and restructured documentation
+    * Added security check for dependencies in local pipeline
+    * Removed some old python 2.7 syntax
+
+**3.5.2** (2021-01-07)
+    * Bugfix with args and kwargs in ``ReadOnlyTabularInline``
+
+**3.5.1** (2020-11-19)
+    * Bugfix with args and kwargs in ``ClassBasedViewTestMixin``
+
+**3.5.0** (2020-11-10)
+    * Merged package ``graphene-django-ai`` into this package and enabled graphql-specific installation
+      with `pip install ambient_toolbox[graphql]`
+    * Added some files for readthedocs.io and updated Readme
+
+**3.4.0** (2020-10-30)
+    * Moved tests out of package scope
+    * Updated test python version to 3.8
+    * Added tests for context manager ``TempDisconnectSignal`` with test setup
+
+**3.3.0** (2020-10-30)
+    * Merged package ``ai-drf-core`` into this package and enabled djangorestframework-specific installation
+      with `pip install ambient_toolbox[drf]`
+    * Added ``BaseModelSerializer`` and ``CommonInfoSerializer``
+    * Incremented dependencies django and bleach to previous versions latest bugfix release
+
+**3.2.0** (2020-10-16)
+    * Added ``AbstractPermissionMixin``, ``AbstractUserSpecificQuerySet`` and ``AbstractUserSpecificManager`` abstract
+      managers
+    * Removed deprecated `antivir` package
+    * Added Sphinx documentation setup to package
+
+**3.1.0** (2020-10-14)
+    * Added context manager ``TempDisconnectSignal`` to nicely disable model signals temporarily
+    * Moved dev dependencies to ``extras_require`` in the setup file
+
+**3.0.2** (2020-10-15)
+    * Imports all utils into the modules scope
+    * Re-translated some docstrings into English
+    * Added tests for the `log_whodid` util function
+
+**3.0.1** (2020-10-12)
+    * Added missing ``__init__.py`` file to package mail.services
+
+**3.0.0** (2020-09-09)
+    * *Breaking change:*  Renamed package from `ai` to `ambient_toolbox` to clarify dependencies for usages
+    * Finished code linting
+    * Removed unused imports in antivirus util package
+
+**2.3.0** (2020-08-07)
+    * Changed `ugettext_lazy` to `gettext_lazy` to tackle django 4.0 deprecation warnings
+
+**2.2.1** (2020-07-01)
+    * Removed misleading inheritance of mixin `ClassBasedViewTestMixin` from `TestCase`
+
+**2.2.0** (2020-07-01)
+    * Added response class `CustomPermissionMixin`
+
+**2.1.2** (2020-04-30)
+    * Extended pypi documentation with classifiers
+
+**2.1.1** (2020-04-24)
+    * Refactors open calls to use context managers
+    * Refactors the test setup
+    * Configures coverage
+    * Adds a coverage report to the CI
+
+**2.1.0** (2020-04-20)
+    * Removed password generator method `generate_password`
+    * Renamed math method `round_up_to_decimal` to `round_up_decimal`
+    * Added math method `round_to_decimal`
+    * Updated metadata in setup.cfg
+
+**2.0.0** (2020-04-09)
+    * Dropped Python 2.x support
+    * Removed explicit dependency to package `mock` and using implicit one via unittest
+    * Improved linting
+
+**1.2.14** (2020-04-06)
+    * Fixed a bug with session setup in `ClassBasedViewTestMixin`
+
+**1.2.13** (2020-04-02)
+    * Added ``DELETE`` method for testing mixing `ClassBasedViewTestMixin`
+
+**1.2.12** (2020-02-14)
+    * Added CBV testing mixing `ClassBasedViewTestMixin`
+
+**1.2.11** (2020-01-28)
+    * Bugfix in documentation
+
+**1.2.10** (2020-01-28)
+    * Improved documentation
+
+**1.2.9** (2020-01-02)
+    * Extended and improved class `AbstractScrubbingService`
+
+**1.2.8** (2019-12-13)
+    * Added custom scrubber class `AbstractScrubbingService` to provide a helper for adding custom scrubbing logic for
+      data anonymisation
+
+**1.2.7** (2019-07-11)
+    * Added email testing class `EmailTestService` to provide a wrapper for better email unittests
+
+**1.2.6** (2019-07-02)
+    * Added helper class `tz_today()` to provide an easy getter for a timezone-aware today
+
+**1.2.5** (2019-06-25)
+    * Added helper class `DateHelper` to provide constants to use in django's ORM lookup `__week_day`
+
+**1.2.4** (2019-05-20)
+    * More refactoring on `CurrentUserMiddleware` to make it easier to override internal functions
+
+**1.2.3** (2019-05-20)
+    * Moved `get_current_user` function inside `CurrentUserMiddleware` as a static method to enable devs to override it
+
+**1.2.2** (2019-04-05)
+    * Updated deployment documentation
+    * Added markdown support to Readme file
+
+**1.2.1** (2019-03-25)
+    * Fixed bug causing `CommonInfo` middleware to not set `lastmodified_by` on object creation
+
+**1.2.0** (2019-03-19)
+    * Added `CommonInfo` middleware
+
+**1.1.8**
+    * Readonly admin classes
+    * Date util functions
+    * Clear cache helper
+
+**1.1.7**
+    * Settings for whitelist email services added
+    * Formset mixins added
+
+**1.1.6**
+    * Modifications to antivirus field
+
+**1.1.5**
+    * Updated setup.py with newer information
+
+**1.1.4**
+    * Bleacher mixin bugfix
+
+**1.1.3**
+    * Bleacher mixin added
+
+**< 1.1.3**
+    * Ancient history :)
```

### Comparing `ambient-toolbox-8.1.0/Dockerfile` & `ambient-toolbox-8.1.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/LICENSE.md` & `ambient-toolbox-8.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/README.md` & `ambient-toolbox-8.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 This package was previously known as [ai_django_core](https://pypi.org/project/ai-django-core/). Due to the
 misleading nature of the name, we chose to rename it with something more meaningful.
 
 The migration is really simple, just:
 
 * Install ambient-toolbox and remove the dependency to ai-django-core
 * Search and replace all usages of `from ai_django_core...` to `from ambient_toolbox...`
+* The class-based mail functionality was moved to a separate package called
+[django-pony-express](https://pypi.org/project/django-pony-express/).
 
 
 ## Installation
 
 - Install the package via pip:
 
   `pip install ambient-toolbox`
```

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/admin/model_admins/classes.py` & `ambient-toolbox-8.1.1/ambient_toolbox/admin/model_admins/classes.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/admin/model_admins/inlines.py` & `ambient-toolbox-8.1.1/ambient_toolbox/admin/model_admins/inlines.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/admin/model_admins/mixins.py` & `ambient-toolbox-8.1.1/ambient_toolbox/admin/model_admins/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/admin/views/forms.py` & `ambient-toolbox-8.1.1/ambient_toolbox/admin/views/forms.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/admin/views/mixins.py` & `ambient-toolbox-8.1.1/ambient_toolbox/admin/views/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/context_manager.py` & `ambient-toolbox-8.1.1/ambient_toolbox/context_manager.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/drf/fields.py` & `ambient-toolbox-8.1.1/ambient_toolbox/drf/fields.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/drf/serializers.py` & `ambient-toolbox-8.1.1/ambient_toolbox/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/drf/tests.py` & `ambient-toolbox-8.1.1/ambient_toolbox/drf/tests.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/gitlab/coverage.py` & `ambient-toolbox-8.1.1/ambient_toolbox/gitlab/coverage.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/graphql/forms/mutations.py` & `ambient-toolbox-8.1.1/ambient_toolbox/graphql/forms/mutations.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/graphql/schemes/mutations.py` & `ambient-toolbox-8.1.1/ambient_toolbox/graphql/schemes/mutations.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/graphql/sentry/views.py` & `ambient-toolbox-8.1.1/ambient_toolbox/graphql/sentry/views.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/graphql/tests/base_test.py` & `ambient-toolbox-8.1.1/ambient_toolbox/graphql/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/locale/de/LC_MESSAGES/django.mo` & `ambient-toolbox-8.1.1/ambient_toolbox/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/locale/de/LC_MESSAGES/django.po` & `ambient-toolbox-8.1.1/ambient_toolbox/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/mail/backends/whitelist_smtp.py` & `ambient-toolbox-8.1.1/ambient_toolbox/mail/backends/whitelist_smtp.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/managers.py` & `ambient-toolbox-8.1.1/ambient_toolbox/managers.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/middleware/current_user.py` & `ambient-toolbox-8.1.1/ambient_toolbox/middleware/current_user.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/mixins/bleacher.py` & `ambient-toolbox-8.1.1/ambient_toolbox/mixins/bleacher.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/mixins/models.py` & `ambient-toolbox-8.1.1/ambient_toolbox/mixins/models.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/models.py` & `ambient-toolbox-8.1.1/ambient_toolbox/models.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/selectors/permission.py` & `ambient-toolbox-8.1.1/ambient_toolbox/selectors/permission.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/sentry/helpers.py` & `ambient-toolbox-8.1.1/ambient_toolbox/sentry/helpers.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/services/custom_scrubber.py` & `ambient-toolbox-8.1.1/ambient_toolbox/services/custom_scrubber.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/templatetags/ai_email_tags.py` & `ambient-toolbox-8.1.1/ambient_toolbox/templatetags/ai_email_tags.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/templatetags/ai_file_tags.py` & `ambient-toolbox-8.1.1/ambient_toolbox/templatetags/ai_file_tags.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/templatetags/ai_number_tags.py` & `ambient-toolbox-8.1.1/ambient_toolbox/templatetags/ai_number_tags.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/templatetags/ai_string_tags.py` & `ambient-toolbox-8.1.1/ambient_toolbox/templatetags/ai_string_tags.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/tests/mixins.py` & `ambient-toolbox-8.1.1/ambient_toolbox/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/tests/structure_validator/test_structure_validator.py` & `ambient-toolbox-8.1.1/ambient_toolbox/tests/structure_validator/test_structure_validator.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/utils/date.py` & `ambient-toolbox-8.1.1/ambient_toolbox/utils/date.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/utils/file.py` & `ambient-toolbox-8.1.1/ambient_toolbox/utils/file.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/utils/math.py` & `ambient-toolbox-8.1.1/ambient_toolbox/utils/math.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/utils/model.py` & `ambient-toolbox-8.1.1/ambient_toolbox/utils/model.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/utils/named_tuple.py` & `ambient-toolbox-8.1.1/ambient_toolbox/utils/named_tuple.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/utils/string.py` & `ambient-toolbox-8.1.1/ambient_toolbox/utils/string.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/view_layer/form_mixins.py` & `ambient-toolbox-8.1.1/ambient_toolbox/view_layer/form_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/view_layer/formset_view_mixin.py` & `ambient-toolbox-8.1.1/ambient_toolbox/view_layer/formset_view_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/view_layer/htmx_mixins.py` & `ambient-toolbox-8.1.1/ambient_toolbox/view_layer/htmx_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/view_layer/mixins.py` & `ambient-toolbox-8.1.1/ambient_toolbox/view_layer/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/view_layer/tests/mixins.py` & `ambient-toolbox-8.1.1/ambient_toolbox/view_layer/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/ambient_toolbox/view_layer/views.py` & `ambient-toolbox-8.1.1/ambient_toolbox/view_layer/views.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/Makefile` & `ambient-toolbox-8.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/conf.py` & `ambient-toolbox-8.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/admin.md` & `ambient-toolbox-8.1.1/docs/features/admin.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/context_manager.md` & `ambient-toolbox-8.1.1/docs/features/context_manager.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/context_processors.md` & `ambient-toolbox-8.1.1/docs/features/context_processors.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/database_anonymisation.md` & `ambient-toolbox-8.1.1/docs/features/database_anonymisation.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/djangorestframework.md` & `ambient-toolbox-8.1.1/docs/features/djangorestframework.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/gitlab.md` & `ambient-toolbox-8.1.1/docs/features/gitlab.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/graphql.md` & `ambient-toolbox-8.1.1/docs/features/graphql.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/mail.md` & `ambient-toolbox-8.1.1/docs/features/mail.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/managers.md` & `ambient-toolbox-8.1.1/docs/features/managers.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/mixins.md` & `ambient-toolbox-8.1.1/docs/features/mixins.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/models.md` & `ambient-toolbox-8.1.1/docs/features/models.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/selectors.md` & `ambient-toolbox-8.1.1/docs/features/selectors.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/sentry.md` & `ambient-toolbox-8.1.1/docs/features/sentry.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/services.md` & `ambient-toolbox-8.1.1/docs/features/services.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/setup.md` & `ambient-toolbox-8.1.1/docs/features/setup.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/tests.md` & `ambient-toolbox-8.1.1/docs/features/tests.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/utils/cache.md` & `ambient-toolbox-8.1.1/docs/features/utils/cache.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/utils/date.md` & `ambient-toolbox-8.1.1/docs/features/utils/date.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/utils/math.md` & `ambient-toolbox-8.1.1/docs/features/utils/math.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/utils/model.md` & `ambient-toolbox-8.1.1/docs/features/utils/model.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/utils/named_tuple.md` & `ambient-toolbox-8.1.1/docs/features/utils/named_tuple.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/utils/string.md` & `ambient-toolbox-8.1.1/docs/features/utils/string.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/features/view-layer.md` & `ambient-toolbox-8.1.1/docs/features/view-layer.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/index.rst` & `ambient-toolbox-8.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/docs/make.bat` & `ambient-toolbox-8.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/manage.py` & `ambient-toolbox-8.1.1/manage.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/settings.py` & `ambient-toolbox-8.1.1/settings.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/testapp/api/views.py` & `ambient-toolbox-8.1.1/testapp/api/views.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/testapp/migrations/0001_initial.py` & `ambient-toolbox-8.1.1/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/testapp/models.py` & `ambient-toolbox-8.1.1/testapp/models.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/testapp/templates/403.html` & `ambient-toolbox-8.1.1/testapp/templates/403.html`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py` & `ambient-toolbox-8.1.1/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py` & `ambient-toolbox-8.1.1/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py` & `ambient-toolbox-8.1.1/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py` & `ambient-toolbox-8.1.1/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py` & `ambient-toolbox-8.1.1/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/admin/model_admin_mixins/test_fetch_object_mixin.py` & `ambient-toolbox-8.1.1/tests/admin/model_admin_mixins/test_fetch_object_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py` & `ambient-toolbox-8.1.1/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/ambient_toolbox/test_test_structure_validator.py` & `ambient-toolbox-8.1.1/tests/ambient_toolbox/test_test_structure_validator.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/drf/test_fields.py` & `ambient-toolbox-8.1.1/tests/drf/test_fields.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/query_selectors/test_permission.py` & `ambient-toolbox-8.1.1/tests/query_selectors/test_permission.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_admin_forms.py` & `ambient-toolbox-8.1.1/tests/test_admin_forms.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_admin_inlines.py` & `ambient-toolbox-8.1.1/tests/test_admin_inlines.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_admin_model_admins_classes.py` & `ambient-toolbox-8.1.1/tests/test_admin_model_admins_classes.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_admin_view_mixins.py` & `ambient-toolbox-8.1.1/tests/test_admin_view_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_context_manager.py` & `ambient-toolbox-8.1.1/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_log_whodid.py` & `ambient-toolbox-8.1.1/tests/test_log_whodid.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_managers.py` & `ambient-toolbox-8.1.1/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_math.py` & `ambient-toolbox-8.1.1/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_middleware.py` & `ambient-toolbox-8.1.1/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_mixins_models.py` & `ambient-toolbox-8.1.1/tests/test_mixins_models.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_models.py` & `ambient-toolbox-8.1.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_rest_api_mixins.py` & `ambient-toolbox-8.1.1/tests/test_rest_api_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_scrubbing_service.py` & `ambient-toolbox-8.1.1/tests/test_scrubbing_service.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_sentry_helper.py` & `ambient-toolbox-8.1.1/tests/test_sentry_helper.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_utils_date.py` & `ambient-toolbox-8.1.1/tests/test_utils_date.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_utils_file.py` & `ambient-toolbox-8.1.1/tests/test_utils_file.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_utils_model.py` & `ambient-toolbox-8.1.1/tests/test_utils_model.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_utils_named_tuple.py` & `ambient-toolbox-8.1.1/tests/test_utils_named_tuple.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/test_utils_string.py` & `ambient-toolbox-8.1.1/tests/test_utils_string.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/tests/mixins/test_django_message_framework.py` & `ambient-toolbox-8.1.1/tests/tests/mixins/test_django_message_framework.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/tests/mixins/test_request_provider_mixin.py` & `ambient-toolbox-8.1.1/tests/tests/mixins/test_request_provider_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/tests/test_mail_backends.py` & `ambient-toolbox-8.1.1/tests/tests/test_mail_backends.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/view_layer/test_formset_mixins.py` & `ambient-toolbox-8.1.1/tests/view_layer/test_formset_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/view_layer/test_htmx_response_mixin.py` & `ambient-toolbox-8.1.1/tests/view_layer/test_htmx_response_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/view_layer/test_meta_mixins.py` & `ambient-toolbox-8.1.1/tests/view_layer/test_meta_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/tests/view_layer/test_views.py` & `ambient-toolbox-8.1.1/tests/view_layer/test_views.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.1.0/PKG-INFO` & `ambient-toolbox-8.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambient-toolbox
-Version: 8.1.0
+Version: 8.1.1
 Summary: Python toolbox of Ambient Digital containing an abundance of useful tools and gadgets.
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
@@ -33,15 +33,15 @@
 Requires-Dist: pre-commit~=3.2 ; extra == "dev"
 Requires-Dist: black~=23.3 ; extra == "dev"
 Requires-Dist: Django~=3.2 ; extra == "dev"
 Requires-Dist: sphinx==4.2.0 ; extra == "dev"
 Requires-Dist: sphinx-rtd-theme==1.0.0 ; extra == "dev"
 Requires-Dist: m2r2==0.3.1 ; extra == "dev"
 Requires-Dist: mistune<2.0.0 ; extra == "dev"
-Requires-Dist: ambient-package-update~=23.5.4 ; extra == "dev"
+Requires-Dist: ambient-package-update~=23.5.5 ; extra == "dev"
 Requires-Dist: gevent~=22.10 ; extra == "dev"
 Requires-Dist: djangorestframework>=3.8.2 ; extra == "drf"
 Requires-Dist: graphene-django>=2.2.0 ; extra == "graphql"
 Requires-Dist: django-graphql-jwt>=0.2.1 ; extra == "graphql"
 Requires-Dist: django-crispy-forms>=1.4.0 ; extra == "view-layer"
 Project-URL: Bugtracker, https://github.com/ambient-innovation/ambient-toolbox/issues
 Project-URL: Changelog, https://ambient-toolbox.readthedocs.io/en/latest/features/changelog.html
@@ -83,14 +83,16 @@
 This package was previously known as [ai_django_core](https://pypi.org/project/ai-django-core/). Due to the
 misleading nature of the name, we chose to rename it with something more meaningful.
 
 The migration is really simple, just:
 
 * Install ambient-toolbox and remove the dependency to ai-django-core
 * Search and replace all usages of `from ai_django_core...` to `from ambient_toolbox...`
+* The class-based mail functionality was moved to a separate package called
+[django-pony-express](https://pypi.org/project/django-pony-express/).
 
 
 ## Installation
 
 - Install the package via pip:
 
   `pip install ambient-toolbox`
```

