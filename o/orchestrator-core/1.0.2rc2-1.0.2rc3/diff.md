# Comparing `tmp/orchestrator-core-1.0.2rc2.tar.gz` & `tmp/orchestrator-core-1.0.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchestrator-core-1.0.2rc2.tar", last modified: Mon Apr 24 12:54:44 2023, max compression
+gzip compressed data, was "orchestrator-core-1.0.2rc3.tar", last modified: Fri May  5 08:14:09 2023, max compression
```

## Comparing `orchestrator-core-1.0.2rc2.tar` & `orchestrator-core-1.0.2rc3.tar`

### file list

```diff
@@ -1,296 +1,316 @@
--rw-r--r--   0        0        0      346 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/.bumpversion.cfg
--rw-r--r--   0        0        0       33 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/.coveragerc
--rw-r--r--   0        0        0     2620 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/.github/workflows/README.md
--rw-r--r--   0        0        0     1851 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/.github/workflows/build-push-container.yml
--rw-r--r--   0        0        0      291 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/.github/workflows/changelog.yml
--rw-r--r--   0        0        0     2341 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      371 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/.github/workflows/gh-pages.yml
--rw-r--r--   0        0        0      550 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0      385 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/.github/workflows/pull-request.yml
--rw-r--r--   0        0        0     1156 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/.github/workflows/run-linting-tests.yml
--rw-r--r--   0        0        0     2099 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/.github/workflows/run-unit-tests.yml
--rw-r--r--   0        0        0     1985 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/.github/workflows/scheduled-build.yml
--rw-r--r--   0        0        0     1782 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/.gitignore
--rw-r--r--   0        0        0     2043 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1150 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/.stignore
--rw-r--r--   0        0        0    29641 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/CHANGELOG.md
--rw-r--r--   0        0        0      333 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/Dockerfile
--rw-r--r--   0        0        0    11409 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/LICENSE
--rw-r--r--   0        0        0      150 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/NOTICE
--rw-r--r--   0        0        0     4813 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/README.md
--rw-r--r--   0        0        0       79 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/codecov.yml
--rw-r--r--   0        0        0       45 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/docs/architecture/application/api.md
--rw-r--r--   0        0        0    16572 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/docs/architecture/application/cli.md
--rw-r--r--   0        0        0    10741 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/docs/architecture/application/domainmodels.md
--rw-r--r--   0        0        0     4347 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/docs/architecture/application/forms.md
--rw-r--r--   0        0        0    48867 2023-04-24 12:54:37.282743 orchestrator-core-1.0.2rc2/docs/architecture/application/openapi.json
--rw-r--r--   0        0        0     5641 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/architecture/application/scaling.md
--rw-r--r--   0        0        0     5514 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/architecture/application/tasks.md
--rw-r--r--   0        0        0     2371 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/architecture/application/websockets.md
--rw-r--r--   0        0        0    11465 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/architecture/application/workflow.md
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/architecture/orchestration/philosophy.md
--rw-r--r--   0        0        0     2080 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/architecture/tldr.md
--rw-r--r--   0        0        0     1694 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/contributing/guidelines.md
--rw-r--r--   0        0        0    10000 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/contributing/testing.md
--rw-r--r--   0        0        0      452 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/css/custom.css
--rw-r--r--   0        0        0     2165 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/css/termynal.css
--rw-r--r--   0        0        0     2135 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/getting-started/base.md
--rw-r--r--   0        0        0      928 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/getting-started/development.md
--rw-r--r--   0        0        0     2367 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/index.md
--rw-r--r--   0        0        0     3897 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/js/termynal.js
--rw-r--r--   0        0        0     5605 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/create-user-group.md
--rw-r--r--   0        0        0     4438 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/create-user.md
--rw-r--r--   0        0        0     7471 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/database-migration.md
--rw-r--r--   0        0        0     3700 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/debian.md
--rw-r--r--   0        0        0     3063 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/docker.md
--rw-r--r--   0        0        0     6106 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/domain-models.md
--rw-r--r--   0        0        0     1952 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/explore.md
--rw-r--r--   0        0        0     3996 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/input-forms.md
--rw-r--r--   0        0        0     3595 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/macos.md
--rw-r--r--   0        0        0     3411 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/modify-user-group.md
--rw-r--r--   0        0        0     2143 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/modify-user.md
--rw-r--r--   0        0        0     2885 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/overview.md
--rw-r--r--   0        0        0     4547 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/register-workflows.md
--rw-r--r--   0        0        0      786 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/scenario.md
--rw-r--r--   0        0        0     1013 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/start-applications.md
--rw-r--r--   0        0        0     2988 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/terminate-user-group.md
--rw-r--r--   0        0        0     1332 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/terminate-user.md
--rw-r--r--   0        0        0     3637 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/beginner/workflow-introduction.md
--rw-r--r--   0        0        0    46296 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/docs/workshops/images/metadata_products.png
--rw-r--r--   0        0        0      771 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/examples/basic/basic_orchestrator.py
--rw-r--r--   0        0        0     3542 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/mkdocs.yml
--rw-r--r--   0        0        0     1267 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/mutmut_config.py
--rw-r--r--   0        0        0     1098 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/__init__.py
--rw-r--r--   0        0        0      571 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/__init__.py
--rw-r--r--   0        0        0      571 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/__init__.py
--rw-r--r--   0        0        0     2871 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/api.py
--rw-r--r--   0        0        0      571 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/__init__.py
--rw-r--r--   0        0        0     2856 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/fixed_input.py
--rw-r--r--   0        0        0     1236 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/health.py
--rw-r--r--   0        0        0    16350 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/processes.py
--rw-r--r--   0        0        0     2703 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/product_blocks.py
--rw-r--r--   0        0        0     3331 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/products.py
--rw-r--r--   0        0        0     2552 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/resource_types.py
--rw-r--r--   0        0        0     5211 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/settings.py
--rw-r--r--   0        0        0     2866 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
--rw-r--r--   0        0        0    11510 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/subscriptions.py
--rw-r--r--   0        0        0      996 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/translations.py
--rw-r--r--   0        0        0     1833 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/user.py
--rw-r--r--   0        0        0     1961 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/workflows.py
--rw-r--r--   0        0        0     1543 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/error_handling.py
--rw-r--r--   0        0        0    11705 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/helpers.py
--rw-r--r--   0        0        0     5636 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/api/models.py
--rw-r--r--   0        0        0     7278 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/app.py
--rw-r--r--   0        0        0      571 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0    13831 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/database.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/domain_gen_helpers/__init__.py
--rw-r--r--   0        0        0     6853 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
--rw-r--r--   0        0        0     1953 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/domain_gen_helpers/helpers.py
--rw-r--r--   0        0        0    10653 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
--rw-r--r--   0        0        0     9423 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py
--rw-r--r--   0        0        0    24095 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
--rw-r--r--   0        0        0     1439 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/domain_gen_helpers/types.py
--rw-r--r--   0        0        0      571 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1165 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/helpers/input_helpers.py
--rw-r--r--   0        0        0      830 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/helpers/print_helpers.py
--rw-r--r--   0        0        0      871 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/main.py
--rwxr-xr-x   0        0        0    20183 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/migrate_domain_models.py
--rwxr-xr-x   0        0        0     8943 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/migrate_workflows.py
--rw-r--r--   0        0        0     4113 2023-04-24 12:54:37.286743 orchestrator-core-1.0.2rc2/orchestrator/cli/migration_helpers.py
--rw-r--r--   0        0        0     1896 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/cli/scheduler.py
--rw-r--r--   0        0        0      571 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/config/__init__.py
--rw-r--r--   0        0        0      734 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/config/assignee.py
--rw-r--r--   0        0        0     2920 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/db/__init__.py
--rw-r--r--   0        0        0    10288 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/db/database.py
--rw-r--r--   0        0        0    23116 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/db/models.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/devtools/__init__.py
--rw-r--r--   0        0        0    16866 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/devtools/populator.py
--rw-r--r--   0        0        0     2554 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/distlock/__init__.py
--rw-r--r--   0        0        0     2528 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/distlock/distlock_manager.py
--rw-r--r--   0        0        0      571 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/distlock/managers/__init__.py
--rw-r--r--   0        0        0     3062 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/distlock/managers/memory_distlock_manager.py
--rw-r--r--   0        0        0     3315 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/distlock/managers/redis_distlock_manager.py
--rw-r--r--   0        0        0      924 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/domain/__init__.py
--rw-r--r--   0        0        0    62310 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/domain/base.py
--rw-r--r--   0        0        0     2659 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/domain/lifecycle.py
--rw-r--r--   0        0        0     2977 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/exception_handlers.py
--rw-r--r--   0        0        0     5434 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/forms/__init__.py
--rw-r--r--   0        0        0     2145 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/forms/network_type_validators.py
--rw-r--r--   0        0        0    11483 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/forms/validators.py
--rw-r--r--   0        0        0       39 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/README
--rw-r--r--   0        0        0      873 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/alembic.ini
--rwxr-xr-x   0        0        0     3365 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/env.py
--rw-r--r--   0        0        0    40397 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/helpers.py
--rw-r--r--   0        0        0      510 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/script.py.mako
--rw-r--r--   0        0        0      905 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/templates/alembic.ini.j2
--rwxr-xr-x   0        0        0     2821 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/templates/env.py.j2
--rw-r--r--   0        0        0       98 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/templates/helpers.py.j2
--rw-r--r--   0        0        0     2641 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
--rw-r--r--   0        0        0     1266 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
--rw-r--r--   0        0        0    38591 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
--rw-r--r--   0        0        0      951 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
--rw-r--r--   0        0        0     1213 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
--rw-r--r--   0        0        0     1556 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
--rw-r--r--   0        0        0     5105 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
--rw-r--r--   0        0        0     7723 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/py.typed
--rw-r--r--   0        0        0     1090 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schedules/__init__.py
--rw-r--r--   0        0        0      832 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schedules/resume_workflows.py
--rw-r--r--   0        0        0     1535 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schedules/scheduling.py
--rw-r--r--   0        0        0      821 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schedules/task_vacuum.py
--rw-r--r--   0        0        0     1053 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schedules/validate_products.py
--rw-r--r--   0        0        0     2131 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schedules/validate_subscriptions.py
--rw-r--r--   0        0        0     2576 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schemas/__init__.py
--rw-r--r--   0        0        0      886 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schemas/base.py
--rw-r--r--   0        0        0     1056 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schemas/engine_settings.py
--rw-r--r--   0        0        0     1346 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schemas/fixed_input.py
--rw-r--r--   0        0        0      842 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schemas/problem_detail.py
--rw-r--r--   0        0        0     3390 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schemas/process.py
--rw-r--r--   0        0        0     1670 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schemas/product.py
--rw-r--r--   0        0        0     1735 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schemas/product_block.py
--rw-r--r--   0        0        0      951 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schemas/resource_type.py
--rw-r--r--   0        0        0     3180 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schemas/subscription.py
--rw-r--r--   0        0        0     1013 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schemas/subscription_descriptions.py
--rw-r--r--   0        0        0     1803 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/schemas/workflow.py
--rw-r--r--   0        0        0     1516 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/security.py
--rw-r--r--   0        0        0      571 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/services/__init__.py
--rw-r--r--   0        0        0     3586 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/services/celery.py
--rw-r--r--   0        0        0    21514 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/services/processes.py
--rw-r--r--   0        0        0     1530 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/services/products.py
--rw-r--r--   0        0        0     3879 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/services/settings.py
--rw-r--r--   0        0        0    24204 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/services/subscriptions.py
--rw-r--r--   0        0        0     4802 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/services/tasks.py
--rw-r--r--   0        0        0     1706 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/services/translations.py
--rw-r--r--   0        0        0     3581 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/settings.py
--rw-r--r--   0        0        0      731 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/targets.py
--rw-r--r--   0        0        0     9605 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/types.py
--rw-r--r--   0        0        0      571 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/utils/__init__.py
--rw-r--r--   0        0        0     5593 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/utils/crypt.py
--rw-r--r--   0        0        0     1477 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/utils/datetime.py
--rw-r--r--   0        0        0     6207 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/utils/docs.py
--rw-r--r--   0        0        0     3839 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/utils/errors.py
--rw-r--r--   0        0        0     8079 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/utils/functional.py
--rw-r--r--   0        0        0     8512 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/utils/json.py
--rw-r--r--   0        0        0     3403 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/utils/redis.py
--rw-r--r--   0        0        0     2972 2023-04-24 12:54:37.290743 orchestrator-core-1.0.2rc2/orchestrator/utils/show_process.py
--rw-r--r--   0        0        0     2395 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/utils/speed.py
--rw-r--r--   0        0        0    13148 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/utils/state.py
--rw-r--r--   0        0        0     1077 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/utils/strings.py
--rw-r--r--   0        0        0     7231 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/utils/vlans.py
--rw-r--r--   0        0        0     1323 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/version.py
--rw-r--r--   0        0        0     4476 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/websocket/__init__.py
--rw-r--r--   0        0        0     3535 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py
--rw-r--r--   0        0        0     3194 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/websocket/managers/memory_websocket_manager.py
--rw-r--r--   0        0        0     2900 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/websocket/websocket_manager.py
--rw-r--r--   0        0        0    33580 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/workflow.py
--rw-r--r--   0        0        0     4085 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2135 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/workflows/modify_note.py
--rw-r--r--   0        0        0      909 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/workflows/removed_workflow.py
--rw-r--r--   0        0        0     9204 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/workflows/steps.py
--rw-r--r--   0        0        0      571 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     1510 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py
--rw-r--r--   0        0        0     2120 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/workflows/tasks/resume_workflows.py
--rw-r--r--   0        0        0     8335 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/workflows/tasks/validate_products.py
--rw-r--r--   0        0        0      684 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/workflows/translations/en-GB.json
--rw-r--r--   0        0        0     8839 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/orchestrator/workflows/utils.py
--rw-r--r--   0        0        0     4500 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/pyproject.toml
--rw-r--r--   0        0        0     2385 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/setup.cfg
--rw-r--r--   0        0        0      665 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/setup.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/acceptance_tests/__init__.py
--rw-r--r--   0        0        0     3199 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/acceptance_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
--rw-r--r--   0        0        0     1855 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
--rw-r--r--   0        0        0     1544 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
--rw-r--r--   0        0        0     1529 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
--rw-r--r--   0        0        0     2828 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
--rw-r--r--   0        0        0      588 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/acceptance_tests/test_test_product.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/__init__.py
--rw-r--r--   0        0        0     7530 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/conftest.py
--rw-r--r--   0        0        0     5786 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/test_caching.py
--rw-r--r--   0        0        0     1578 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/test_fixed_inputs.py
--rw-r--r--   0        0        0     1192 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/test_health.py
--rw-r--r--   0        0        0     3049 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/test_helpers.py
--rw-r--r--   0        0        0     1747 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/test_models.py
--rw-r--r--   0        0        0    20143 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/test_processes.py
--rw-r--r--   0        0        0    16019 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/test_processes_ws.py
--rw-r--r--   0        0        0     3742 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/test_product_blocks.py
--rw-r--r--   0        0        0     7942 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/test_products.py
--rw-r--r--   0        0        0     2486 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/test_resource_types.py
--rw-r--r--   0        0        0     1772 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/test_settings.py
--rw-r--r--   0        0        0     2985 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/test_subscription_customer_descriptions.py
--rw-r--r--   0        0        0    37733 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/test_subscriptions.py
--rw-r--r--   0        0        0     2394 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/api/test_workflows.py
--rw-r--r--   0        0        0    25724 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
--rw-r--r--   0        0        0    27170 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
--rw-r--r--   0        0        0      422 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/config.py
--rw-r--r--   0        0        0    20724 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/domain/__init__.py
--rw-r--r--   0        0        0    50075 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/domain/test_base.py
--rw-r--r--   0        0        0     8092 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/domain/test_base_with_list_union.py
--rw-r--r--   0        0        0     4493 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/domain/test_base_with_union.py
--rw-r--r--   0        0        0     2824 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_blocks/__init__.py
--rw-r--r--   0        0        0     1683 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
--rw-r--r--   0        0        0     2569 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
--rw-r--r--   0        0        0     1609 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
--rw-r--r--   0        0        0     2642 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
--rw-r--r--   0        0        0     2590 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
--rw-r--r--   0        0        0     1232 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
--rw-r--r--   0        0        0     1055 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/__init__.py
--rw-r--r--   0        0        0     2372 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
--rw-r--r--   0        0        0     2262 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
--rw-r--r--   0        0        0     4191 2023-04-24 12:54:37.294744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
--rw-r--r--   0        0        0     3240 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py
--rw-r--r--   0        0        0     2341 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
--rw-r--r--   0        0        0     2977 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
--rw-r--r--   0        0        0     2298 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
--rw-r--r--   0        0        0     2282 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
--rw-r--r--   0        0        0     1671 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
--rw-r--r--   0        0        0     1898 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py
--rw-r--r--   0        0        0      527 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/resource_types.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/forms/__init__.py
--rw-r--r--   0        0        0     1462 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/forms/shared.py
--rw-r--r--   0        0        0    25426 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/forms/test_generic_validators.py
--rw-r--r--   0        0        0     7644 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/forms/test_network_validators.py
--rw-r--r--   0        0        0     6626 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/forms/test_post_process.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/schedules/__init__.py
--rw-r--r--   0        0        0      807 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/schedules/test_scheduling.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/services/__init__.py
--rw-r--r--   0        0        0    26695 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/services/test_processes.py
--rw-r--r--   0        0        0     1083 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/services/test_products.py
--rw-r--r--   0        0        0     5830 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/services/test_subscriptions.py
--rw-r--r--   0        0        0     2100 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/services/test_translations.py
--rw-r--r--   0        0        0     7353 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/test_db.py
--rw-r--r--   0        0        0      385 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/test_types.py
--rw-r--r--   0        0        0    12048 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/test_workflow.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/utils/__init__.py
--rw-r--r--   0        0        0      163 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/utils/test_datetime.py
--rw-r--r--   0        0        0     1871 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/utils/test_errors.py
--rw-r--r--   0        0        0     3517 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/utils/test_functional.py
--rw-r--r--   0        0        0     3052 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/utils/test_json.py
--rw-r--r--   0        0        0     1144 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/utils/test_speed.py
--rw-r--r--   0        0        0    11501 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/utils/test_state.py
--rw-r--r--   0        0        0      192 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/utils/test_strings.py
--rw-r--r--   0        0        0     8339 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/utils/test_vlans.py
--rw-r--r--   0        0        0    12492 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/workflows/__init__.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/workflows/conftest.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/workflows/shared/__init__.py
--rw-r--r--   0        0        0     2091 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py
--rw-r--r--   0        0        0        0 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/workflows/tasks/__init__.py
--rw-r--r--   0        0        0     2039 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
--rw-r--r--   0        0        0     2584 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py
--rw-r--r--   0        0        0      288 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/workflows/tasks/test_validate_products.py
--rw-r--r--   0        0        0     3390 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/workflows/test_config_db_code.py
--rw-r--r--   0        0        0     1877 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/workflows/test_generic_workflow_steps.py
--rw-r--r--   0        0        0      987 2023-04-24 12:54:37.298744 orchestrator-core-1.0.2rc2/test/unit_tests/workflows/test_modify_note.py
--rw-r--r--   0        0        0     5198 1970-01-01 00:00:00.000000 orchestrator-core-1.0.2rc2/PKG-INFO
+-rw-r--r--   0        0        0      346 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.bumpversion.cfg
+-rw-r--r--   0        0        0       33 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.coveragerc
+-rw-r--r--   0        0        0     2620 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/README.md
+-rw-r--r--   0        0        0     1851 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/build-push-container.yml
+-rw-r--r--   0        0        0      291 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/changelog.yml
+-rw-r--r--   0        0        0     2341 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      371 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/gh-pages.yml
+-rw-r--r--   0        0        0      550 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1163 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/run-linting-tests.yml
+-rw-r--r--   0        0        0     2106 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0        0        0     1985 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.github/workflows/scheduled-build.yml
+-rw-r--r--   0        0        0     1782 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.gitignore
+-rw-r--r--   0        0        0     2074 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1150 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/.stignore
+-rw-r--r--   0        0        0    29713 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/CHANGELOG.md
+-rw-r--r--   0        0        0      333 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/Dockerfile
+-rw-r--r--   0        0        0    11409 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/LICENSE
+-rw-r--r--   0        0        0      150 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/NOTICE
+-rw-r--r--   0        0        0     4965 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/README.md
+-rw-r--r--   0        0        0       76 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/codecov.yml
+-rw-r--r--   0        0        0       45 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/api.md
+-rw-r--r--   0        0        0    16572 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/cli.md
+-rw-r--r--   0        0        0    10741 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/domainmodels.md
+-rw-r--r--   0        0        0     4347 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/forms.md
+-rw-r--r--   0        0        0    48867 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/openapi.json
+-rw-r--r--   0        0        0     1565 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/python.md
+-rw-r--r--   0        0        0     5641 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/scaling.md
+-rw-r--r--   0        0        0     5514 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/tasks.md
+-rw-r--r--   0        0        0     2371 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/websockets.md
+-rw-r--r--   0        0        0    11465 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/application/workflow.md
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/orchestration/philosophy.md
+-rw-r--r--   0        0        0     2080 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/architecture/tldr.md
+-rw-r--r--   0        0        0     1694 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/contributing/guidelines.md
+-rw-r--r--   0        0        0    10000 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/contributing/testing.md
+-rw-r--r--   0        0        0      452 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/css/custom.css
+-rw-r--r--   0        0        0     2165 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/css/termynal.css
+-rw-r--r--   0        0        0     2135 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/getting-started/base.md
+-rw-r--r--   0        0        0      928 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/getting-started/development.md
+-rw-r--r--   0        0        0     2367 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/index.md
+-rw-r--r--   0        0        0     3897 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/js/termynal.js
+-rw-r--r--   0        0        0     5605 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/create-user-group.md
+-rw-r--r--   0        0        0     4438 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/create-user.md
+-rw-r--r--   0        0        0     7471 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/database-migration.md
+-rw-r--r--   0        0        0     3700 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/debian.md
+-rw-r--r--   0        0        0     3063 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/docker.md
+-rw-r--r--   0        0        0     6106 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/domain-models.md
+-rw-r--r--   0        0        0     1952 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/explore.md
+-rw-r--r--   0        0        0     3996 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/input-forms.md
+-rw-r--r--   0        0        0     3595 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/macos.md
+-rw-r--r--   0        0        0     3411 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/modify-user-group.md
+-rw-r--r--   0        0        0     2143 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/modify-user.md
+-rw-r--r--   0        0        0     2885 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/overview.md
+-rw-r--r--   0        0        0     4547 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/register-workflows.md
+-rw-r--r--   0        0        0      786 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/scenario.md
+-rw-r--r--   0        0        0     1013 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/start-applications.md
+-rw-r--r--   0        0        0     2988 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/terminate-user-group.md
+-rw-r--r--   0        0        0     1332 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/terminate-user.md
+-rw-r--r--   0        0        0     3637 2023-05-05 08:13:53.131969 orchestrator-core-1.0.2rc3/docs/workshops/beginner/workflow-introduction.md
+-rw-r--r--   0        0        0    46296 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/docs/workshops/images/metadata_products.png
+-rw-r--r--   0        0        0      771 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/examples/basic/basic_orchestrator.py
+-rw-r--r--   0        0        0     3601 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/mkdocs.yml
+-rw-r--r--   0        0        0     1267 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/mutmut_config.py
+-rw-r--r--   0        0        0     1098 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/__init__.py
+-rw-r--r--   0        0        0      571 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/__init__.py
+-rw-r--r--   0        0        0      571 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/__init__.py
+-rw-r--r--   0        0        0     2871 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/api.py
+-rw-r--r--   0        0        0      571 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/__init__.py
+-rw-r--r--   0        0        0     2841 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/fixed_input.py
+-rw-r--r--   0        0        0     1236 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/health.py
+-rw-r--r--   0        0        0    12955 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/processes.py
+-rw-r--r--   0        0        0     2703 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/product_blocks.py
+-rw-r--r--   0        0        0     3331 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/products.py
+-rw-r--r--   0        0        0     2552 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/resource_types.py
+-rw-r--r--   0        0        0     5848 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/settings.py
+-rw-r--r--   0        0        0     2866 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    11510 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/subscriptions.py
+-rw-r--r--   0        0        0      996 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/translations.py
+-rw-r--r--   0        0        0     1833 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/user.py
+-rw-r--r--   0        0        0     1961 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/workflows.py
+-rw-r--r--   0        0        0     1543 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/error_handling.py
+-rw-r--r--   0        0        0    11705 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/helpers.py
+-rw-r--r--   0        0        0     5636 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/api/models.py
+-rw-r--r--   0        0        0     7395 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/app.py
+-rw-r--r--   0        0        0      571 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0    13831 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/database.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/__init__.py
+-rw-r--r--   0        0        0     6853 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py
+-rw-r--r--   0        0        0     1953 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/helpers.py
+-rw-r--r--   0        0        0    10653 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/product_block_helpers.py
+-rw-r--r--   0        0        0     9423 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/product_helpers.py
+-rw-r--r--   0        0        0    24095 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py
+-rw-r--r--   0        0        0     1439 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/types.py
+-rw-r--r--   0        0        0      571 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1165 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/helpers/input_helpers.py
+-rw-r--r--   0        0        0      830 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/helpers/print_helpers.py
+-rw-r--r--   0        0        0      871 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/main.py
+-rwxr-xr-x   0        0        0    20183 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/migrate_domain_models.py
+-rwxr-xr-x   0        0        0     8943 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/migrate_workflows.py
+-rw-r--r--   0        0        0     4113 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/migration_helpers.py
+-rw-r--r--   0        0        0     1896 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/cli/scheduler.py
+-rw-r--r--   0        0        0      571 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/config/__init__.py
+-rw-r--r--   0        0        0      770 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/config/assignee.py
+-rw-r--r--   0        0        0     2920 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0    10288 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/database.py
+-rw-r--r--   0        0        0      301 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/filters/__init__.py
+-rw-r--r--   0        0        0     3415 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/filters/filters.py
+-rw-r--r--   0        0        0     4507 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/filters/process.py
+-rw-r--r--   0        0        0    23116 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/models.py
+-rw-r--r--   0        0        0      104 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/range/__init__.py
+-rw-r--r--   0        0        0     1439 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/range/range.py
+-rw-r--r--   0        0        0      240 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/sorting/__init__.py
+-rw-r--r--   0        0        0      368 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/sorting/process.py
+-rw-r--r--   0        0        0     3413 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/db/sorting/sorting.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/devtools/__init__.py
+-rw-r--r--   0        0        0    16866 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/devtools/populator.py
+-rw-r--r--   0        0        0     2554 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/distlock/__init__.py
+-rw-r--r--   0        0        0     2528 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/distlock/distlock_manager.py
+-rw-r--r--   0        0        0      571 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/distlock/managers/__init__.py
+-rw-r--r--   0        0        0     3062 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/distlock/managers/memory_distlock_manager.py
+-rw-r--r--   0        0        0     3315 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/distlock/managers/redis_distlock_manager.py
+-rw-r--r--   0        0        0      924 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/domain/__init__.py
+-rw-r--r--   0        0        0    62844 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/domain/base.py
+-rw-r--r--   0        0        0     2694 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/domain/lifecycle.py
+-rw-r--r--   0        0        0     2977 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/exception_handlers.py
+-rw-r--r--   0        0        0     5434 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/forms/__init__.py
+-rw-r--r--   0        0        0     2145 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/forms/network_type_validators.py
+-rw-r--r--   0        0        0    11483 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/forms/validators.py
+-rw-r--r--   0        0        0     4481 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/graphql/__init__.py
+-rw-r--r--   0        0        0     4265 2023-05-05 08:13:53.135969 orchestrator-core-1.0.2rc3/orchestrator/graphql/authentication.py
+-rw-r--r--   0        0        0     1350 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/extensions/ErrorCollectorExtension.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/extensions/__init__.py
+-rw-r--r--   0        0        0     4325 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/extensions/deprecation_checker_extension.py
+-rw-r--r--   0        0        0     2105 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/pagination.py
+-rw-r--r--   0        0        0     4097 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/resolvers/process.py
+-rw-r--r--   0        0        0     2259 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/schemas/process.py
+-rw-r--r--   0        0        0     2056 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/types.py
+-rw-r--r--   0        0        0      992 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/graphql/utils/get_selected_fields.py
+-rw-r--r--   0        0        0       39 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/README
+-rw-r--r--   0        0        0      873 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/alembic.ini
+-rwxr-xr-x   0        0        0     3365 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/env.py
+-rw-r--r--   0        0        0    40397 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/helpers.py
+-rw-r--r--   0        0        0      510 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/script.py.mako
+-rw-r--r--   0        0        0      905 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/templates/alembic.ini.j2
+-rwxr-xr-x   0        0        0     2821 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/templates/env.py.j2
+-rw-r--r--   0        0        0       98 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/templates/helpers.py.j2
+-rw-r--r--   0        0        0     2641 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py
+-rw-r--r--   0        0        0     1266 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py
+-rw-r--r--   0        0        0    38591 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py
+-rw-r--r--   0        0        0      951 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py
+-rw-r--r--   0        0        0     1213 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py
+-rw-r--r--   0        0        0     1556 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py
+-rw-r--r--   0        0        0     5105 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py
+-rw-r--r--   0        0        0     7723 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/py.typed
+-rw-r--r--   0        0        0     1090 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schedules/__init__.py
+-rw-r--r--   0        0        0      832 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schedules/resume_workflows.py
+-rw-r--r--   0        0        0     1535 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schedules/scheduling.py
+-rw-r--r--   0        0        0      821 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schedules/task_vacuum.py
+-rw-r--r--   0        0        0     1053 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schedules/validate_products.py
+-rw-r--r--   0        0        0     2131 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schedules/validate_subscriptions.py
+-rw-r--r--   0        0        0     2631 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/__init__.py
+-rw-r--r--   0        0        0      886 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/base.py
+-rw-r--r--   0        0        0     1275 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/engine_settings.py
+-rw-r--r--   0        0        0     1346 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/fixed_input.py
+-rw-r--r--   0        0        0      842 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/problem_detail.py
+-rw-r--r--   0        0        0     3390 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/process.py
+-rw-r--r--   0        0        0     1670 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/product.py
+-rw-r--r--   0        0        0     1735 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/product_block.py
+-rw-r--r--   0        0        0      951 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/resource_type.py
+-rw-r--r--   0        0        0     3180 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/subscription.py
+-rw-r--r--   0        0        0     1013 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/subscription_descriptions.py
+-rw-r--r--   0        0        0     1803 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/schemas/workflow.py
+-rw-r--r--   0        0        0     1797 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/security.py
+-rw-r--r--   0        0        0      571 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0     3586 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/celery.py
+-rw-r--r--   0        0        0    22351 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/processes.py
+-rw-r--r--   0        0        0     1530 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/products.py
+-rw-r--r--   0        0        0     3879 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/settings.py
+-rw-r--r--   0        0        0    24204 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/subscriptions.py
+-rw-r--r--   0        0        0     5695 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/tasks.py
+-rw-r--r--   0        0        0     1719 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/services/translations.py
+-rw-r--r--   0        0        0     3741 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/settings.py
+-rw-r--r--   0        0        0      731 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/targets.py
+-rw-r--r--   0        0        0     9397 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/types.py
+-rw-r--r--   0        0        0      571 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/__init__.py
+-rw-r--r--   0        0        0     5593 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/crypt.py
+-rw-r--r--   0        0        0     1477 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/datetime.py
+-rw-r--r--   0        0        0     6207 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/docs.py
+-rw-r--r--   0        0        0     3839 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/errors.py
+-rw-r--r--   0        0        0     8079 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/functional.py
+-rw-r--r--   0        0        0     2817 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/helpers.py
+-rw-r--r--   0        0        0     8512 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/json.py
+-rw-r--r--   0        0        0     3403 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/redis.py
+-rw-r--r--   0        0        0     2972 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/show_process.py
+-rw-r--r--   0        0        0     2395 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/speed.py
+-rw-r--r--   0        0        0    13148 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/state.py
+-rw-r--r--   0        0        0     1077 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/strings.py
+-rw-r--r--   0        0        0     7231 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/utils/vlans.py
+-rw-r--r--   0        0        0     1323 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/version.py
+-rw-r--r--   0        0        0     4476 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/websocket/__init__.py
+-rw-r--r--   0        0        0     3535 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/websocket/managers/broadcast_websocket_manager.py
+-rw-r--r--   0        0        0     3194 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/websocket/managers/memory_websocket_manager.py
+-rw-r--r--   0        0        0     2900 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/websocket/websocket_manager.py
+-rw-r--r--   0        0        0    33615 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflow.py
+-rw-r--r--   0        0        0     4085 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2135 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/modify_note.py
+-rw-r--r--   0        0        0      909 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/removed_workflow.py
+-rw-r--r--   0        0        0     9204 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/steps.py
+-rw-r--r--   0        0        0      571 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     1510 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/cleanup_tasks_log.py
+-rw-r--r--   0        0        0     2120 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/resume_workflows.py
+-rw-r--r--   0        0        0     8335 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/validate_products.py
+-rw-r--r--   0        0        0      684 2023-05-05 08:13:53.139969 orchestrator-core-1.0.2rc3/orchestrator/workflows/translations/en-GB.json
+-rw-r--r--   0        0        0     8839 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/orchestrator/workflows/utils.py
+-rw-r--r--   0        0        0     4574 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/pyproject.toml
+-rw-r--r--   0        0        0     2413 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/setup.cfg
+-rw-r--r--   0        0        0      665 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/setup.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/__init__.py
+-rw-r--r--   0        0        0     3199 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/__init__.py
+-rw-r--r--   0        0        0     1855 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py
+-rw-r--r--   0        0        0     1544 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/main.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1608 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/products/__init__.py
+-rw-r--r--   0        0        0     1211 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/workflows/__init__.py
+-rw-r--r--   0        0        0     2828 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py
+-rw-r--r--   0        0        0      588 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/acceptance_tests/test_test_product.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/__init__.py
+-rw-r--r--   0        0        0     5786 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_caching.py
+-rw-r--r--   0        0        0     1578 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_fixed_inputs.py
+-rw-r--r--   0        0        0     1192 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_health.py
+-rw-r--r--   0        0        0     3049 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_helpers.py
+-rw-r--r--   0        0        0     1747 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_models.py
+-rw-r--r--   0        0        0    20143 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_processes.py
+-rw-r--r--   0        0        0    16019 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_processes_ws.py
+-rw-r--r--   0        0        0     3742 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_product_blocks.py
+-rw-r--r--   0        0        0     7942 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_products.py
+-rw-r--r--   0        0        0     2486 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_resource_types.py
+-rw-r--r--   0        0        0     1772 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_settings.py
+-rw-r--r--   0        0        0     2985 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_subscription_customer_descriptions.py
+-rw-r--r--   0        0        0    37733 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_subscriptions.py
+-rw-r--r--   0        0        0     2394 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/api/test_workflows.py
+-rw-r--r--   0        0        0    25724 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/cli/test_migrate_domain_models_with_instances.py
+-rw-r--r--   0        0        0    27170 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/cli/test_migrate_domain_models_without_instances.py
+-rw-r--r--   0        0        0      422 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/config.py
+-rw-r--r--   0        0        0    20845 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/domain/__init__.py
+-rw-r--r--   0        0        0    50537 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/domain/test_base.py
+-rw-r--r--   0        0        0     8092 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/domain/test_base_with_list_union.py
+-rw-r--r--   0        0        0     4493 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/domain/test_base_with_union.py
+-rw-r--r--   0        0        0     2824 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     7530 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/processes.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/__init__.py
+-rw-r--r--   0        0        0     1683 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py
+-rw-r--r--   0        0        0     2569 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one.py
+-rw-r--r--   0        0        0     1609 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py
+-rw-r--r--   0        0        0     2642 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py
+-rw-r--r--   0        0        0     2590 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py
+-rw-r--r--   0        0        0     1232 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py
+-rw-r--r--   0        0        0     1055 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/__init__.py
+-rw-r--r--   0        0        0     2372 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py
+-rw-r--r--   0        0        0     2262 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union.py
+-rw-r--r--   0        0        0     4191 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py
+-rw-r--r--   0        0        0     3240 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_one.py
+-rw-r--r--   0        0        0     2341 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py
+-rw-r--r--   0        0        0     2977 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py
+-rw-r--r--   0        0        0     2298 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py
+-rw-r--r--   0        0        0     2282 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py
+-rw-r--r--   0        0        0     1671 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py
+-rw-r--r--   0        0        0     1898 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_union.py
+-rw-r--r--   0        0        0      527 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/resource_types.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/forms/__init__.py
+-rw-r--r--   0        0        0     1462 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/forms/shared.py
+-rw-r--r--   0        0        0    25426 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/forms/test_generic_validators.py
+-rw-r--r--   0        0        0     7644 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/forms/test_network_validators.py
+-rw-r--r--   0        0        0     6626 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/forms/test_post_process.py
+-rw-r--r--   0        0        0    10081 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/graphql/test_processes.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/schedules/__init__.py
+-rw-r--r--   0        0        0      807 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/schedules/test_scheduling.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/services/__init__.py
+-rw-r--r--   0        0        0    26695 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/services/test_processes.py
+-rw-r--r--   0        0        0     1083 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/services/test_products.py
+-rw-r--r--   0        0        0     5830 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/services/test_subscriptions.py
+-rw-r--r--   0        0        0     2100 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/services/test_translations.py
+-rw-r--r--   0        0        0     7353 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/test_db.py
+-rw-r--r--   0        0        0      385 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/test_types.py
+-rw-r--r--   0        0        0    12048 2023-05-05 08:13:53.143970 orchestrator-core-1.0.2rc3/test/unit_tests/test_workflow.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_datetime.py
+-rw-r--r--   0        0        0     1871 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_errors.py
+-rw-r--r--   0        0        0     3517 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_functional.py
+-rw-r--r--   0        0        0     3052 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_json.py
+-rw-r--r--   0        0        0     1144 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_speed.py
+-rw-r--r--   0        0        0    11501 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_state.py
+-rw-r--r--   0        0        0      192 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_strings.py
+-rw-r--r--   0        0        0     8339 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_vlans.py
+-rw-r--r--   0        0        0    12492 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/shared/__init__.py
+-rw-r--r--   0        0        0     2091 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/shared/test_validate_subscriptions.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/tasks/__init__.py
+-rw-r--r--   0        0        0     2039 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/tasks/test_clean_up_task_log.py
+-rw-r--r--   0        0        0     2584 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/tasks/test_resume_workflows.py
+-rw-r--r--   0        0        0      288 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/tasks/test_validate_products.py
+-rw-r--r--   0        0        0     3390 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/test_config_db_code.py
+-rw-r--r--   0        0        0     1877 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/test_generic_workflow_steps.py
+-rw-r--r--   0        0        0      987 2023-05-05 08:13:53.147970 orchestrator-core-1.0.2rc3/test/unit_tests/workflows/test_modify_note.py
+-rw-r--r--   0        0        0     5285 1970-01-01 00:00:00.000000 orchestrator-core-1.0.2rc3/PKG-INFO
```

### Comparing `orchestrator-core-1.0.2rc2/.github/workflows/README.md` & `orchestrator-core-1.0.2rc3/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/.github/workflows/build-push-container.yml` & `orchestrator-core-1.0.2rc3/.github/workflows/build-push-container.yml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/.github/workflows/codeql-analysis.yml` & `orchestrator-core-1.0.2rc3/.github/workflows/codeql-analysis.yml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         language: [ 'python' ]
         # CodeQL supports [ 'cpp', 'csharp', 'go', 'java', 'javascript', 'python' ]
         # Learn more:
         # https://docs.github.com/en/free-pro-team@latest/github/finding-security-vulnerabilities-and-errors-in-your-code/configuring-code-scanning#changing-the-languages-that-are-analyzed
 
     steps:
     - name: Checkout repository
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
 
     # Initializes the CodeQL tools for scanning.
     - name: Initialize CodeQL
       uses: github/codeql-action/init@v1
       with:
         languages: ${{ matrix.language }}
         # If you wish to specify custom queries, you can do so here or in a config file.
```

### Comparing `orchestrator-core-1.0.2rc2/.github/workflows/publish-package.yml` & `orchestrator-core-1.0.2rc3/.github/workflows/publish-package.yml`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   release:
     types: [created]
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v2
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
```

### Comparing `orchestrator-core-1.0.2rc2/.github/workflows/run-linting-tests.yml` & `orchestrator-core-1.0.2rc3/.github/workflows/run-linting-tests.yml`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 jobs:
   build:
     name: Linting Tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.10', '3.11']
+        python-version: ['3.9', '3.10', '3.11']
       fail-fast: false
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
```

### Comparing `orchestrator-core-1.0.2rc2/.github/workflows/run-unit-tests.yml` & `orchestrator-core-1.0.2rc3/.github/workflows/run-unit-tests.yml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 jobs:
   container_job:
     name: Unit tests
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.10', '3.11']
+        python-version: ['3.9', '3.10', '3.11']
       fail-fast: false
     container: python:${{ matrix.python-version }}-slim
     services:
       postgres:
         image: postgres:12-alpine
         # Provide the password for postgres
         env:
@@ -33,15 +33,15 @@
           --health-cmd "redis-cli ping"
           --health-interval 10s
           --health-timeout 5s
           --health-retries 5
     steps:
       # Downloads a copy of the code in your repository before running CI tests
       - name: Check out repository code
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: Install dependencies
         run: |
           apt update
           apt install curl git build-essential libpq-dev libffi-dev -y
           python -m pip install --upgrade pip
           pip install flit
@@ -54,11 +54,11 @@
         env:
           POSTGRES_DB: orchestrator-core-test
           POSTGRES_USER: nwa
           POSTGRES_PASSWORD: nwa
           POSTGRES_HOST: postgres
           ENVIRONMENT: TESTING
       - name: "Upload coverage to Codecov"
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v3
         with:
           fail_ci_if_error: true
           files: ./coverage.xml
```

### Comparing `orchestrator-core-1.0.2rc2/.github/workflows/scheduled-build.yml` & `orchestrator-core-1.0.2rc3/.github/workflows/scheduled-build.yml`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/.gitignore` & `orchestrator-core-1.0.2rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/.pre-commit-config.yaml` & `orchestrator-core-1.0.2rc3/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   python: python3
 repos:
   - repo: https://github.com/timothycrosley/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.13.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.1.0]
@@ -37,27 +37,28 @@
           - flake8-logging-format
           - flake8-pep3101
           - flake8-print
           - flake8-rst
           - flake8-rst-docstrings
           - flake8-tidy-imports
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.0.1
+    rev: v1.2.0
     hooks:
       - id: mypy
         additional_dependencies:
           - pydantic
           - types-toml
           - types-pytz
           - types-python-dateutil
           - types-requests
           - types-Deprecated
           - types-redis
           - types-orjson
           - types-tabulate
+          - strawberry-graphql
         args:
           - --no-warn-unused-ignores
           - --allow-untyped-decorators
         exclude: (test/.*|migrations/.*)
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
@@ -66,10 +67,10 @@
       - id: python-check-mock-methods
       - id: rst-backticks
   - repo: https://github.com/shellcheck-py/shellcheck-py
     rev: v0.9.0.2
     hooks:
       - id: shellcheck
   - repo: https://github.com/andreoliwa/nitpick
-    rev: v0.31.0
+    rev: v0.33.1
     hooks:
       - id: nitpick-check
```

### Comparing `orchestrator-core-1.0.2rc2/.stignore` & `orchestrator-core-1.0.2rc3/.stignore`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/CHANGELOG.md` & `orchestrator-core-1.0.2rc3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 ## [Unreleased]
 
-- Allow user to extend the default translation set, instead of overwriting everything  
+- Allow user to extend the default translation set, instead of overwriting everything
+- Return worker status information in the `/api/settings/status` endpoint
 
 ## [0.4.0-rc1](https://github.com/workfloworchestrator/orchestrator-core/tree/0.4.0-rc1) (2022-03-08)
 
 [Full Changelog](https://github.com/workfloworchestrator/orchestrator-core/compare/0.3.8...0.4.0-rc1)
 
 **Merged pull requests:**
```

### Comparing `orchestrator-core-1.0.2rc2/LICENSE` & `orchestrator-core-1.0.2rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/README.md` & `orchestrator-core-1.0.2rc3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Orchestrator-Core
 [![Downloads](https://pepy.tech/badge/orchestrator-core/month)](https://pepy.tech/project/orchestrator-core)
 [![codecov](https://codecov.io/gh/workfloworchestrator/orchestrator-core/branch/main/graph/badge.svg?token=5ANQFI2DHS)](https://codecov.io/gh/workfloworchestrator/orchestrator-core)
 [![pypi_version](https://img.shields.io/pypi/v/orchestrator-core?color=%2334D058&label=pypi%20package)](https://pypi.org/project/orchestrator-core)
-
+[![Supported python versions](https://img.shields.io/pypi/pyversions/orchestrator-core.svg?color=%2334D058)](https://pypi.org/project/orchestrator-core)
 <p align="center"><em>Production ready Orchestration Framework to manage product lifecyle and workflows. Easy to use, Built on top of FastAPI</em></p>
 
 
 ## Documentation
 Can be found [here](https://workfloworchestrator.org/orchestrator-core/)
 
 ## Usage
```

### Comparing `orchestrator-core-1.0.2rc2/docs/architecture/application/cli.md` & `orchestrator-core-1.0.2rc3/docs/architecture/application/cli.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/architecture/application/domainmodels.md` & `orchestrator-core-1.0.2rc3/docs/architecture/application/domainmodels.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/architecture/application/forms.md` & `orchestrator-core-1.0.2rc3/docs/architecture/application/forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/architecture/application/openapi.json` & `orchestrator-core-1.0.2rc3/docs/architecture/application/openapi.json`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/architecture/application/scaling.md` & `orchestrator-core-1.0.2rc3/docs/architecture/application/scaling.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/architecture/application/tasks.md` & `orchestrator-core-1.0.2rc3/docs/architecture/application/tasks.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/architecture/application/websockets.md` & `orchestrator-core-1.0.2rc3/docs/architecture/application/websockets.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/architecture/application/workflow.md` & `orchestrator-core-1.0.2rc3/docs/architecture/application/workflow.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/architecture/tldr.md` & `orchestrator-core-1.0.2rc3/docs/architecture/tldr.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/contributing/guidelines.md` & `orchestrator-core-1.0.2rc3/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/contributing/testing.md` & `orchestrator-core-1.0.2rc3/docs/contributing/testing.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/css/termynal.css` & `orchestrator-core-1.0.2rc3/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/getting-started/base.md` & `orchestrator-core-1.0.2rc3/docs/getting-started/base.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/getting-started/development.md` & `orchestrator-core-1.0.2rc3/docs/getting-started/development.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/index.md` & `orchestrator-core-1.0.2rc3/docs/index.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/js/custom.js` & `orchestrator-core-1.0.2rc3/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/js/termynal.js` & `orchestrator-core-1.0.2rc3/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/create-user-group.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/create-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/create-user.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/create-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/database-migration.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/database-migration.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/debian.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/debian.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/docker.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/docker.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/domain-models.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/domain-models.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/explore.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/explore.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/input-forms.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/input-forms.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/macos.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/macos.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/modify-user-group.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/modify-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/modify-user.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/modify-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/overview.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/overview.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/register-workflows.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/register-workflows.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/scenario.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/scenario.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/start-applications.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/start-applications.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/terminate-user-group.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/terminate-user-group.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/terminate-user.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/terminate-user.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/beginner/workflow-introduction.md` & `orchestrator-core-1.0.2rc3/docs/workshops/beginner/workflow-introduction.md`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/docs/workshops/images/metadata_products.png` & `orchestrator-core-1.0.2rc3/docs/workshops/images/metadata_products.png`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/examples/basic/basic_orchestrator.py` & `orchestrator-core-1.0.2rc3/examples/basic/basic_orchestrator.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/mkdocs.yml` & `orchestrator-core-1.0.2rc3/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
       - Validating input through forms: architecture/application/forms.md
       - Domain Models: architecture/application/domainmodels.md
     - Documentation:
       - Command Line Interface: architecture/application/cli.md
       - Web sockets: architecture/application/websockets.md
       - Api Docs: architecture/application/api.md
       - Scaling: architecture/application/scaling.md
+      - Python version: architecture/application/python.md
   - Workshops:
     - Beginner:
       - Overview: workshops/beginner/overview.md
       - Installation:
         - Manual:
           - Debian: workshops/beginner/debian.md
           - MacOS: workshops/beginner/macos.md
```

### Comparing `orchestrator-core-1.0.2rc2/mutmut_config.py` & `orchestrator-core-1.0.2rc3/mutmut_config.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This is the orchestrator workflow engine."""
 
-__version__ = "1.0.2rc2"
+__version__ = "1.0.2rc3"
 
 from orchestrator.app import OrchestratorCore
 from orchestrator.settings import app_settings, oauth2_settings
 from orchestrator.workflow import begin, conditional, done, focussteps, inputstep, retrystep, step, steplens, workflow
 
 __all__ = [
     "OrchestratorCore",
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/api.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/api.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/fixed_input.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/fixed_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             fi_data = first_true(data["fixed_inputs"], None, lambda i: i["name"] == fi_name)  # noqa: B023
             if not fi_data:
                 if issubclass(fi_type, Enum):
                     data["fixed_inputs"].append(
                         {
                             "name": fi_name,
                             "description": (fi_type.__doc__ or fi_name).splitlines()[0],
-                            "values": list(map(lambda v: str(v.value), fi_type)),  # type:ignore
+                            "values": list(map(lambda v: str(v.value), fi_type)),
                         }
                     )
                 else:
                     raise ValueError(f"{fi_name} of {product_name} should be an enum.")
 
             if not first_true(data["by_tag"][product.tag], None, lambda i: fi_name in i):  # noqa: B023
                 data["by_tag"][product.tag].append({fi_name: True})
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/health.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/health.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/processes.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/processes.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,31 +23,25 @@
 import structlog
 from fastapi import Query, Request, WebSocket
 from fastapi.param_functions import Body, Depends, Header
 from fastapi.routing import APIRouter
 from fastapi_etag.dependency import CacheHit
 from more_itertools import chunked
 from oauth2_lib.fastapi import OIDCUserModel
-from sqlalchemy import String, cast
 from sqlalchemy.orm import contains_eager, defer, joinedload
 from sqlalchemy.sql import expression
 from sqlalchemy.sql.functions import count
 from starlette.responses import Response
 
 from orchestrator.api.error_handling import raise_status
 from orchestrator.api.helpers import VALID_SORT_KEYS, enrich_process
 from orchestrator.config.assignee import Assignee
-from orchestrator.db import (
-    EngineSettingsTable,
-    ProcessSubscriptionTable,
-    ProcessTable,
-    ProductTable,
-    SubscriptionTable,
-    db,
-)
+from orchestrator.db import EngineSettingsTable, ProcessSubscriptionTable, ProcessTable, SubscriptionTable, db
+from orchestrator.db.filters import Filter
+from orchestrator.db.filters.process import filter_processes
 from orchestrator.schemas import (
     ProcessIdSchema,
     ProcessListItemSchema,
     ProcessResumeAllSchema,
     ProcessSchema,
     ProcessSubscriptionBaseSchema,
     ProcessSubscriptionSchema,
@@ -243,14 +237,19 @@
     process = _get_process(pid)
     p = load_process(process)
 
     data = show_process(process, p)
     return data
 
 
+def handle_process_error(message: str, **kwargs: Any) -> None:
+    logger.debug(message, **kwargs)
+    raise_status(HTTPStatus.BAD_REQUEST, message)
+
+
 @router.get("/", response_model=List[ProcessListItemSchema])
 def processes_filterable(
     response: Response,
     range: Optional[str] = None,
     sort: Optional[str] = None,
     filter: Optional[str] = None,
     if_none_match: Optional[str] = Header(None),
@@ -268,82 +267,17 @@
         .joinedload(SubscriptionTable.product),
         defer("traceback"),
     )
 
     if _filter is not None:
         if len(_filter) == 0 or (len(_filter) % 2) > 0:
             raise_status(HTTPStatus.BAD_REQUEST, "Invalid number of filter arguments")
-        for filter_pair in chunked(_filter, 2):
-            field, value = filter_pair
-            field = field.lower()
-            if value is not None:
-                if field == "istask":
-                    value_as_bool = value.lower() in ("yes", "y", "ye", "true", "1", "ja")
-                    query = query.filter(ProcessTable.is_task.is_(value_as_bool))
-                elif field == "assignee":
-                    assignees = value.split("-")
-                    query = query.filter(ProcessTable.assignee.in_(assignees))
-                elif field == "status":
-                    statuses = value.split("-")
-                    query = query.filter(ProcessTable.last_status.in_(statuses))
-                elif field == "workflow":
-                    query = query.filter(ProcessTable.workflow.ilike("%" + value + "%"))
-                elif field == "creator":
-                    query = query.filter(ProcessTable.created_by.ilike("%" + value + "%"))
-                elif field == "organisation":
-                    try:
-                        value_as_uuid = UUID(value)
-                    except (ValueError, AttributeError):
-                        msg = "Not a valid customer_id, must be a UUID: '{value}'"
-                        logger.exception(msg)
-                        raise_status(HTTPStatus.BAD_REQUEST, msg)
-                    process_subscriptions = (
-                        db.session.query(ProcessSubscriptionTable)
-                        .join(SubscriptionTable)
-                        .filter(SubscriptionTable.customer_id == value_as_uuid)
-                        .subquery()
-                    )
-                    query = query.filter(ProcessTable.pid == process_subscriptions.c.pid)
-                elif field == "product":
-                    process_subscriptions = (
-                        db.session.query(ProcessSubscriptionTable)
-                        .join(SubscriptionTable, ProductTable)
-                        .filter(ProductTable.name.ilike("%" + value + "%"))
-                        .subquery()
-                    )
-                    query = query.filter(ProcessTable.pid == process_subscriptions.c.pid)
-                elif field == "tag":
-                    tags = value.split("-")
-                    process_subscriptions = (
-                        db.session.query(ProcessSubscriptionTable)
-                        .join(SubscriptionTable, ProductTable)
-                        .filter(ProductTable.tag.in_(tags))
-                        .subquery()
-                    )
-                    query = query.filter(ProcessTable.pid == process_subscriptions.c.pid)
-                elif field == "subscriptions":
-                    process_subscriptions = (
-                        db.session.query(ProcessSubscriptionTable)
-                        .join(SubscriptionTable)
-                        .filter(SubscriptionTable.description.ilike("%" + value + "%"))
-                        .subquery()
-                    )
-                    query = query.filter(ProcessTable.pid == process_subscriptions.c.pid)
-                elif field == "pid":
-                    query = query.filter(cast(ProcessTable.pid, String).ilike("%" + value + "%"))
-                elif field == "target":
-                    targets = value.split("-")
-                    process_subscriptions = (
-                        db.session.query(ProcessSubscriptionTable)
-                        .filter(ProcessSubscriptionTable.workflow_target.in_(targets))
-                        .subquery()
-                    )
-                    query = query.filter(ProcessTable.pid == process_subscriptions.c.pid)
-                else:
-                    raise_status(HTTPStatus.BAD_REQUEST, f"Invalid filter '{field}'")
+
+        pydantic_filters = [Filter(field=field.lower(), value=value) for field, value in chunked(_filter, 2)]
+        query = filter_processes(query, pydantic_filters, handle_process_error)
 
     if _sort is not None and len(_sort) >= 2:
         for item in chunked(_sort, 2):
             if item and len(item) == 2 and item[0] in VALID_SORT_KEYS:
                 sort_key = VALID_SORT_KEYS[item[0]]
                 if item[1].upper() == "DESC":
                     query = query.order_by(expression.desc(ProcessTable.__dict__[sort_key]))
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/product_blocks.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/products.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/resource_types.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/settings.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,45 +7,44 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from http import HTTPStatus
-from typing import Optional
+from typing import Optional, Union
 
 import structlog
 from fastapi import Query, WebSocket
 from fastapi.param_functions import Depends
 from fastapi.routing import APIRouter
 from oauth2_lib.fastapi import OIDCUserModel
 from redis.asyncio import Redis as AIORedis
 
 from orchestrator.api.error_handling import raise_status
 from orchestrator.db import EngineSettingsTable
-from orchestrator.schemas import EngineSettingsBaseSchema, EngineSettingsSchema, GlobalStatusEnum
+from orchestrator.schemas import EngineSettingsBaseSchema, EngineSettingsSchema, GlobalStatusEnum, WorkerStatus
 from orchestrator.security import oidc_user
 from orchestrator.services import settings
-from orchestrator.services.processes import SYSTEM_USER
-from orchestrator.settings import app_settings
+from orchestrator.services.processes import SYSTEM_USER, ThreadPoolWorkerStatus
+from orchestrator.settings import ExecutorType, app_settings
 from orchestrator.utils.json import json_dumps
 from orchestrator.utils.redis import delete_keys_matching_pattern
 from orchestrator.websocket import WS_CHANNELS, websocket_manager
 
 router = APIRouter()
 logger = structlog.get_logger()
 
-
 CACHE_FLUSH_OPTIONS: dict[str, str] = {
     "all": "All caches",
 }
 
 
 @router.delete("/cache/{name}")
-async def clear_cache(name: str) -> int | None:
+async def clear_cache(name: str) -> Union[int, None]:
     cache: AIORedis = AIORedis(host=app_settings.CACHE_HOST, port=app_settings.CACHE_PORT)
     if name not in CACHE_FLUSH_OPTIONS:
         raise_status(HTTPStatus.BAD_REQUEST, "Invalid cache name")
 
     key_name = "orchestrator:*" if name == "all" else f"orchestrator:{name}:*"
     return await delete_keys_matching_pattern(cache, key_name)
 
@@ -82,31 +81,53 @@
         user_name = user.user_name if user else SYSTEM_USER
         settings.post_update_to_slack(EngineSettingsSchema.from_orm(result), user_name)
 
     status_response = generate_engine_status_response(result)
     if websocket_manager.enabled:
         # send engine status to socket.
         await websocket_manager.broadcast_data(
-            [WS_CHANNELS.ENGINE_SETTINGS], {"engine-status": generate_engine_status_response(result)}
+            [WS_CHANNELS.ENGINE_SETTINGS],
+            {"engine-status": generate_engine_status_response(result)},
         )
 
     return status_response
 
 
+def get_worker_status() -> WorkerStatus:
+    """
+    Return information job workers and queues.
+
+    Returns:
+    - The number of queued jobs
+    - The number of workers
+    - The number of running jobs
+    - The number of successful and unsuccessful jobs
+    """
+
+    if app_settings.EXECUTOR == ExecutorType.WORKER:
+        from orchestrator.services.tasks import CeleryJobWorkerStatus
+
+        return CeleryJobWorkerStatus()
+    else:
+        return ThreadPoolWorkerStatus()
+
+
 @router.get("/status", response_model=EngineSettingsSchema)
 def get_global_status() -> EngineSettingsSchema:
     """
     Retrieve the global status object.
 
     Returns:
         The global status of the engine
 
     """
     engine_settings = EngineSettingsTable.query.one()
-    return generate_engine_status_response(engine_settings)
+    response = generate_engine_status_response(engine_settings)
+    response.worker_status = get_worker_status()
+    return response
 
 
 if app_settings.ENABLE_WEBSOCKETS:
 
     @router.websocket("/ws-status/")
     async def websocket_get_global_status(websocket: WebSocket, token: str = Query(...)) -> None:
         error = await websocket_manager.authorize(websocket, token)
@@ -120,15 +141,17 @@
 
         await websocket.send_text(json_dumps({"engine-status": generate_engine_status_response(engine_settings)}))
 
         channel = WS_CHANNELS.ENGINE_SETTINGS
         await websocket_manager.connect(websocket, channel)
 
 
-def generate_engine_status_response(engine_settings: EngineSettingsTable) -> EngineSettingsSchema:
+def generate_engine_status_response(
+    engine_settings: EngineSettingsTable,
+) -> EngineSettingsSchema:
     """
     Generate the correct engine status response.
 
     Args:
         engine_settings: Engine settings database object
 
     Returns:
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/subscriptions.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/translations.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/user.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/api_v1/endpoints/workflows.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/api_v1/endpoints/workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/error_handling.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/error_handling.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/helpers.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/api/models.py` & `orchestrator-core-1.0.2rc3/orchestrator/api/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/app.py` & `orchestrator-core-1.0.2rc3/orchestrator/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from orchestrator.cli.main import app as cli_app
 from orchestrator.db import db, init_database
 from orchestrator.db.database import DBSessionMiddleware
 from orchestrator.distlock import init_distlock_manager
 from orchestrator.domain import SUBSCRIPTION_MODEL_REGISTRY, SubscriptionModel
 from orchestrator.exception_handlers import form_error_handler, problem_detail_handler
 from orchestrator.forms import FormException
+from orchestrator.graphql import graphql_router
 from orchestrator.services.processes import ProcessDataBroadcastThread
 from orchestrator.settings import AppSettings, app_settings, tracer_provider
 from orchestrator.version import GIT_COMMIT_HASH
 from orchestrator.websocket import init_websocket_manager
 
 logger = structlog.get_logger(__name__)
 
@@ -87,14 +88,15 @@
             on_startup=startup_functions,
             on_shutdown=shutdown_functions,
             **kwargs,
         )
 
         initialise_logging()
 
+        api_router.include_router(graphql_router, prefix="/graphql")
         self.include_router(api_router, prefix="/api")
 
         init_database(base_settings)
 
         self.add_middleware(ClearStructlogContextASGIMiddleware)
         self.add_middleware(SessionMiddleware, secret_key=base_settings.SESSION_SECRET)
         self.add_middleware(DBSessionMiddleware, database=db)
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/database.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/fixed_input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/domain_gen_helpers/helpers.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/domain_gen_helpers/product_block_helpers.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/product_block_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/domain_gen_helpers/product_helpers.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/product_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/resource_type_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/domain_gen_helpers/types.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/domain_gen_helpers/types.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/helpers/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/helpers/input_helpers.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/helpers/input_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/helpers/print_helpers.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/helpers/print_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/main.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/migrate_domain_models.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/migrate_domain_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/migrate_workflows.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/migrate_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/migration_helpers.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/migration_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/cli/scheduler.py` & `orchestrator-core-1.0.2rc3/orchestrator/cli/scheduler.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/config/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/config/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/config/assignee.py` & `orchestrator-core-1.0.2rc3/orchestrator/targets.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+
 from orchestrator.types import strEnum
 
 
-class Assignee(strEnum):
-    NOC = "NOC"
+class Target(strEnum):
+    CREATE = "CREATE"
+    MODIFY = "MODIFY"
+    TERMINATE = "TERMINATE"
     SYSTEM = "SYSTEM"
-    CHANGES = "CHANGES"
-    KLANTSUPPORT = "KLANTSUPPORT"
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/db/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/db/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/db/database.py` & `orchestrator-core-1.0.2rc3/orchestrator/db/database.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/db/models.py` & `orchestrator-core-1.0.2rc3/orchestrator/db/models.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/devtools/populator.py` & `orchestrator-core-1.0.2rc3/orchestrator/devtools/populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/distlock/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/distlock/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/distlock/distlock_manager.py` & `orchestrator-core-1.0.2rc3/orchestrator/distlock/distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/distlock/managers/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/distlock/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/distlock/managers/memory_distlock_manager.py` & `orchestrator-core-1.0.2rc3/orchestrator/distlock/managers/memory_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/distlock/managers/redis_distlock_manager.py` & `orchestrator-core-1.0.2rc3/orchestrator/distlock/managers/redis_distlock_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/domain/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/domain/base.py` & `orchestrator-core-1.0.2rc3/orchestrator/domain/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import sys
 from collections import defaultdict
 from datetime import datetime
 from itertools import groupby, zip_longest
 from operator import attrgetter
 from typing import (
     Any,
     Callable,
@@ -181,15 +182,26 @@
 
     @classmethod
     def _find_special_fields(cls: Type) -> None:
         """Make and store a list of resource_type fields and product block fields."""
         cls._non_product_block_fields_ = {}
         cls._product_block_fields_ = {}
 
-        from inspect import get_annotations
+        if sys.version_info >= (3, 10):
+            from inspect import get_annotations
+        else:
+            # python 3.9 compatibility
+            def get_annotations(obj: Any) -> dict:
+                if hasattr(obj, "__annotations__"):
+                    return obj.__annotations__
+
+                if isinstance(obj, type) and "__annotations__" in obj.__dict__:
+                    return obj.__dict__["__annotations__"]
+
+                raise Exception(f"Cannot resolve type annotations for object {obj!r}")
 
         annotations = get_annotations(cls)
 
         # Retrieve type hints with evaluated ForwardRefs (for nested blocks)
         type_hints = get_type_hints(cls, localns={cls.__name__: cls})
 
         # But this also returns inherited fields so cross-check against the annotations
@@ -1155,15 +1167,15 @@
             description=description,
             status=status,
             insync=insync,
             start_date=start_date,
             end_date=end_date,
             note=note,
             **fixed_inputs,
-            **instances,
+            **instances,  # type: ignore
         )
         model._db_model = subscription
         return model
 
     @classmethod
     def from_other_lifecycle(
         cls: Type[S],
@@ -1259,15 +1271,15 @@
                 description=subscription.description,
                 status=status,
                 insync=subscription.insync,
                 start_date=subscription.start_date,
                 end_date=subscription.end_date,
                 note=subscription.note,
                 **fixed_inputs,
-                **instances,
+                **instances,  # type: ignore
             )
             model._db_model = subscription
             return model
         except ValidationError:
             logger.exception(
                 "Subscription is not correct in database", loaded_fixed_inputs=fixed_inputs, loaded_instances=instances
             )
@@ -1309,15 +1321,15 @@
                 description=subscription.description,
                 status=status,
                 insync=subscription.insync,
                 start_date=subscription.start_date,
                 end_date=subscription.end_date,
                 note=subscription.note,
                 **fixed_inputs,
-                **instances,
+                **instances,  # type: ignore
             )
             model._db_model = subscription
             return model
         except ValidationError:
             logger.exception(
                 "Subscription is not correct in database", loaded_fixed_inputs=fixed_inputs, loaded_instances=instances
             )
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/domain/lifecycle.py` & `orchestrator-core-1.0.2rc3/orchestrator/domain/lifecycle.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Type, TypeVar
 
+import strawberry
 import structlog
 
 from orchestrator.types import SubscriptionLifecycle, strEnum
 
 logger = structlog.get_logger(__name__)
 
 
+@strawberry.enum
 class ProductLifecycle(strEnum):
     ACTIVE = "active"
     PRE_PRODUCTION = "pre production"
     PHASE_OUT = "phase out"
     END_OF_LIFE = "end of life"
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/exception_handlers.py` & `orchestrator-core-1.0.2rc3/orchestrator/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/forms/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/forms/network_type_validators.py` & `orchestrator-core-1.0.2rc3/orchestrator/forms/network_type_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/forms/validators.py` & `orchestrator-core-1.0.2rc3/orchestrator/forms/validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/migrations/alembic.ini` & `orchestrator-core-1.0.2rc3/orchestrator/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/migrations/env.py` & `orchestrator-core-1.0.2rc3/orchestrator/migrations/env.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/migrations/helpers.py` & `orchestrator-core-1.0.2rc3/orchestrator/migrations/helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/migrations/templates/alembic.ini.j2` & `orchestrator-core-1.0.2rc3/orchestrator/migrations/templates/alembic.ini.j2`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/migrations/templates/env.py.j2` & `orchestrator-core-1.0.2rc3/orchestrator/migrations/templates/env.py.j2`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py` & `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2020-10-19_3323bcb934e7_fix_tsv_triggers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py` & `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2020-10-19_a76b9185b334_add_generic_workflows_to_core.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py` & `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2020-10-19_c112305b07d3_initial_schema_migration.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py` & `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2021-04-06_3c8b9185c221_add_validate_products_task.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py` & `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2021-07-01_6896a54e9483_add_product_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py` & `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2021-11-17_19cdd3ab86f6_fix_parse_websearch.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py` & `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2022-02-16_bed6bc0b197a_rename_parent_and_child_block_relations.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py` & `orchestrator-core-1.0.2rc3/orchestrator/migrations/versions/schema/2023-03-06_e05bb1967eff_add_subscriptions_search_view.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schedules/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schedules/resume_workflows.py` & `orchestrator-core-1.0.2rc3/orchestrator/schedules/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schedules/scheduling.py` & `orchestrator-core-1.0.2rc3/orchestrator/schedules/scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schedules/task_vacuum.py` & `orchestrator-core-1.0.2rc3/orchestrator/schedules/task_vacuum.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schedules/validate_products.py` & `orchestrator-core-1.0.2rc3/orchestrator/schedules/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schedules/validate_subscriptions.py` & `orchestrator-core-1.0.2rc3/orchestrator/schedules/validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schemas/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/schemas/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from orchestrator.schemas.engine_settings import EngineSettingsBaseSchema, EngineSettingsSchema, GlobalStatusEnum
+from orchestrator.schemas.engine_settings import (
+    EngineSettingsBaseSchema,
+    EngineSettingsSchema,
+    GlobalStatusEnum,
+    WorkerStatus,
+)
 from orchestrator.schemas.fixed_input import FixedInputConfigurationSchema, FixedInputSchema
 from orchestrator.schemas.problem_detail import ProblemDetailSchema
 from orchestrator.schemas.process import (
     ProcessBaseSchema,
     ProcessIdSchema,
     ProcessListItemSchema,
     ProcessResumeAllSchema,
@@ -56,10 +61,11 @@
     "SubscriptionDescriptionSchema",
     "SubscriptionSchema",
     "SubscriptionDomainModelSchema",
     "SubscriptionWorkflowListsSchema",
     "SubscriptionIdSchema",
     "ResourceTypeSchema",
     "ResourceTypeBaseSchema",
+    "WorkerStatus",
     "WorkflowSchema",
     "WorkflowWithProductTagsSchema",
 )
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schemas/base.py` & `orchestrator-core-1.0.2rc3/orchestrator/schemas/base.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schemas/engine_settings.py` & `orchestrator-core-1.0.2rc3/orchestrator/schemas/engine_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,13 +23,21 @@
     PAUSING = "PAUSING"
 
 
 class EngineSettingsBaseSchema(OrchestratorBaseModel):
     global_lock: bool
 
 
+class WorkerStatus(OrchestratorBaseModel):
+    executor_type: str
+    number_of_workers_online: int = 0
+    number_of_queued_jobs: int = 0
+    number_of_running_jobs: int = 0
+
+
 class EngineSettingsSchema(EngineSettingsBaseSchema):
     global_status: Optional[GlobalStatusEnum]
     running_processes: int
+    worker_status: Optional[WorkerStatus]
 
     class Config:
         orm_mode = True
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schemas/fixed_input.py` & `orchestrator-core-1.0.2rc3/orchestrator/schemas/fixed_input.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schemas/problem_detail.py` & `orchestrator-core-1.0.2rc3/orchestrator/schemas/problem_detail.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schemas/process.py` & `orchestrator-core-1.0.2rc3/orchestrator/schemas/process.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schemas/product.py` & `orchestrator-core-1.0.2rc3/orchestrator/schemas/product.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schemas/product_block.py` & `orchestrator-core-1.0.2rc3/orchestrator/schemas/product_block.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schemas/resource_type.py` & `orchestrator-core-1.0.2rc3/orchestrator/schemas/resource_type.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schemas/subscription.py` & `orchestrator-core-1.0.2rc3/orchestrator/schemas/subscription.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schemas/subscription_descriptions.py` & `orchestrator-core-1.0.2rc3/orchestrator/schemas/subscription_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/schemas/workflow.py` & `orchestrator-core-1.0.2rc3/orchestrator/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/security.py` & `orchestrator-core-1.0.2rc3/orchestrator/security.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from authlib.integrations.starlette_client import OAuth
 from nwastdlib.url import URL
-from oauth2_lib.fastapi import OIDCUser, opa_decision
+from oauth2_lib.fastapi import OIDCUser, opa_decision, opa_graphql_decision
 
 from orchestrator.settings import oauth2_settings
 
 oauth_client_credentials = OAuth()
 
 well_known_endpoint = URL(oauth2_settings.OIDC_CONF_WELL_KNOWN_URL)
 
@@ -33,7 +33,18 @@
     oauth2_settings.OIDC_CONF_WELL_KNOWN_URL,
     oauth2_settings.OAUTH2_RESOURCE_SERVER_ID,
     oauth2_settings.OAUTH2_RESOURCE_SERVER_SECRET,
     enabled=oauth2_settings.OAUTH2_ACTIVE,
 )
 
 opa_security_default = opa_decision(oauth2_settings.OPA_URL, oidc_user, enabled=oauth2_settings.OAUTH2_ACTIVE)
+
+
+opa_security_graphql = opa_graphql_decision(oauth2_settings.OPA_URL, oidc_user, enabled=oauth2_settings.OAUTH2_ACTIVE)
+
+
+def get_oidc_user() -> OIDCUser:
+    return oidc_user
+
+
+def get_opa_security_graphql():  # type: ignore
+    return opa_security_graphql
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/services/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/services/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/services/celery.py` & `orchestrator-core-1.0.2rc3/orchestrator/services/celery.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/services/processes.py` & `orchestrator-core-1.0.2rc3/orchestrator/services/processes.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from sqlalchemy.orm import joinedload
 
 from orchestrator.api.error_handling import raise_status
 from orchestrator.config.assignee import Assignee
 from orchestrator.db import EngineSettingsTable, ProcessStepTable, ProcessSubscriptionTable, ProcessTable, db
 from orchestrator.distlock import distlock_manager
 from orchestrator.forms import FormValidationError, post_process
+from orchestrator.schemas.engine_settings import WorkerStatus
 from orchestrator.settings import ExecutorType, app_settings
 from orchestrator.targets import Target
 from orchestrator.types import BroadcastFunc, State
 from orchestrator.utils.datetime import nowtz
 from orchestrator.utils.errors import error_state_to_dict
 from orchestrator.websocket import (
     WS_CHANNELS,
@@ -48,15 +49,14 @@
 from orchestrator.workflows import get_workflow
 from orchestrator.workflows.removed_workflow import removed_workflow
 
 logger = structlog.get_logger(__name__)
 
 StateMerger = Merger([(dict, ["merge"])], ["override"], ["override"])
 
-
 SYSTEM_USER = "SYSTEM"
 
 _workflow_executor = None
 
 
 def get_execution_context() -> Dict[str, Callable]:
     from orchestrator.services.celery import CELERY_EXECUTION_CONTEXT
@@ -141,15 +141,19 @@
             if step_state.get("class") == "AssertionError" or step_state.get("class") == "InconsistentData":
                 p.assignee = Assignee.NOC
                 p.last_status = ProcessStatus.INCONSISTENT_DATA
             # If we encounter a connectivity issue with an underlying api:
             elif step_state.get("class") == "MaxRetryError" or (
                 step_state.get("class") == "ApiException"
                 and step_state.get("status_code")
-                in (HTTPStatus.BAD_GATEWAY, HTTPStatus.SERVICE_UNAVAILABLE, HTTPStatus.GATEWAY_TIMEOUT)
+                in (
+                    HTTPStatus.BAD_GATEWAY,
+                    HTTPStatus.SERVICE_UNAVAILABLE,
+                    HTTPStatus.GATEWAY_TIMEOUT,
+                )
             ):
                 p.assignee = Assignee.SYSTEM
                 p.last_status = ProcessStatus.API_UNAVAILABLE
             else:
                 p.assignee = Assignee.SYSTEM
 
         # check if last error state is identical to determine if we add a new step or update the last one
@@ -170,25 +174,35 @@
 
     db.session.add(p)
 
     if current_step is None:
         # add a new entry to the process stat
         logger.info("Adding a new process step with state info")
         current_step = ProcessStepTable(
-            pid=stat.pid, name=step.name, status=process_state.status, state=step_state, created_by=stat.current_user
+            pid=stat.pid,
+            name=step.name,
+            status=process_state.status,
+            state=step_state,
+            created_by=stat.current_user,
         )
     else:
         # update the last one with the repeated info
         retries = current_step.state.get("retries", 0) + 1
         executed_at = current_step.state.get("executed_at", [])
         executed_at.append(str(current_step.executed_at))
 
         # write new state info and execution date
-        current_step.state = {**step_state, "retries": retries, "executed_at": executed_at}
-        logger.info("Updating existing process step with state info about the error", retries=retries)
+        current_step.state = step_state | {
+            "retries": retries,
+            "executed_at": executed_at,
+        }
+        logger.info(
+            "Updating existing process step with state info about the error",
+            retries=retries,
+        )
 
     # Always explicitly set this instead of leaving it to the database to prevent failing tests
     # Test will fail if multiple steps have the same timestamp
     current_step.executed_at = nowtz()
 
     db.session.add(current_step)
     try:
@@ -239,15 +253,19 @@
 
     Returns: None, there is no one to listen at this point
 
     """
 
     p = ProcessTable.query.get(pid)
     if p is None:
-        logger.error("Failed to write failure to database: Process with PID %s not found", pid, pid=pid)
+        logger.error(
+            "Failed to write failure to database: Process with PID %s not found",
+            pid,
+            pid=pid,
+        )
         return
 
     logger.warning("Writing only process state to DB as step couldn't be found", pid=pid)
     p.last_step = "Unknown"
     if p.last_status != ProcessStatus.WAITING:
         p.last_status = ProcessStatus.FAILED
     p.failed_reason = str(ex)
@@ -300,15 +318,15 @@
                 except Exception as ex:
                     # We still have access to the database, so we can log at least something
                     _db_log_process_ex(pid, ex)
                     raise
                 finally:
                     _update_running_processes("-")
         except Exception as ex:
-            # We lost access to database here so we can only log
+            # We lost access to database here, so we can only log
             logger.exception("Unknown workflow failure", pid=pid)
             result = Failed(ex)
 
         return result
 
     _update_running_processes("+")
     if app_settings.EXECUTOR == ExecutorType.THREADPOOL:
@@ -352,15 +370,19 @@
     try:
         state = post_process(workflow.initial_input_form, initial_state, user_inputs)
     except FormValidationError:
         logger.exception("Validation errors", user_inputs=user_inputs)
         raise
 
     pstat = ProcessStat(
-        pid, workflow=workflow, state=Success({**state, **initial_state}), log=workflow.steps, current_user=user
+        pid,
+        workflow=workflow,
+        state=Success(state | initial_state),
+        log=workflow.steps,
+        current_user=user,
     )
 
     _db_create_process(pstat)
 
     return pstat
 
 
@@ -465,15 +487,17 @@
 
     """
     resume_func = get_execution_context()["resume"]
     return resume_func(process, user_inputs=user_inputs, user=user, broadcast_func=broadcast_func)
 
 
 async def _async_resume_processes(
-    processes: List[ProcessTable], user_name: str, broadcast_func: Optional[Callable] = None
+    processes: List[ProcessTable],
+    user_name: str,
+    broadcast_func: Optional[Callable] = None,
 ) -> bool:
     """Asynchronously resume multiple failed processes.
 
     Args:
         processes: Processes from database
         user_name: User who requested resuming the processes
 
@@ -556,15 +580,21 @@
 
     if not workflow:
         workflow = removed_workflow
 
     log = _restore_log(process.steps)
     pstate, remaining = _recoverwf(workflow, log)
 
-    return ProcessStat(pid=process.pid, workflow=workflow, state=pstate, log=remaining, current_user=SYSTEM_USER)
+    return ProcessStat(
+        pid=process.pid,
+        workflow=workflow,
+        state=pstate,
+        log=remaining,
+        current_user=SYSTEM_USER,
+    )
 
 
 class ProcessDataBroadcastThread(threading.Thread):
     def __init__(self, _websocket_manager: WebSocketManager, *args, **kwargs) -> None:  # type: ignore
         super().__init__(*args, **kwargs)
         self.shutdown = False
         self.queue: queue.Queue = queue.Queue()
@@ -608,7 +638,16 @@
     """
     broadcast_queue: queue.Queue = request.app.broadcast_thread.queue
 
     def _queue_put(pid: UUID, data: Dict) -> None:
         broadcast_queue.put((str(pid), data))
 
     return _queue_put
+
+
+class ThreadPoolWorkerStatus(WorkerStatus):
+    def __init__(self) -> None:
+        super().__init__(executor_type="threadpool")
+        thread_pool = get_thread_pool()
+        self.number_of_workers_online = getattr(thread_pool, "_max_workers", -1)
+        self.number_of_queued_jobs = thread_pool._work_queue.qsize() if hasattr(thread_pool, "_work_queue") else 0
+        self.number_of_running_jobs = len(getattr(thread_pool, "_threads", []))
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/services/products.py` & `orchestrator-core-1.0.2rc3/orchestrator/services/products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/services/settings.py` & `orchestrator-core-1.0.2rc3/orchestrator/services/settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/services/subscriptions.py` & `orchestrator-core-1.0.2rc3/orchestrator/services/subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/services/tasks.py` & `orchestrator-core-1.0.2rc3/orchestrator/services/tasks.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,32 +13,32 @@
 from functools import partial
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional
 from uuid import UUID
 
 import structlog
 from celery import Celery, Task
+from celery.app.control import Inspect
 from celery.utils.log import get_task_logger
 from kombu.serialization import registry
 
 from orchestrator.api.error_handling import raise_status
+from orchestrator.schemas.engine_settings import WorkerStatus
 from orchestrator.services.processes import _get_process, _run_process_async, safe_logstep, thread_resume_process
 from orchestrator.types import State
 from orchestrator.utils.json import json_dumps, json_loads
 from orchestrator.workflow import ProcessStat, Success, runwf
 from orchestrator.workflows import get_workflow
 
 logger = get_task_logger(__name__)
 
 local_logger = structlog.get_logger(__name__)
 
-
 _celery: Optional[Celery] = None
 
-
 NEW_TASK = "tasks.new_task"
 NEW_WORKFLOW = "tasks.new_workflow"
 RESUME_TASK = "tasks.resume_task"
 RESUME_WORKFLOW = "tasks.resume_workflow"
 
 
 def get_celery_task(task_name: str) -> Task:
@@ -72,15 +72,21 @@
     def start_process(pid: UUID, workflow_key: str, state: Dict[str, Any], user: str) -> Optional[UUID]:
         try:
             workflow = get_workflow(workflow_key)
 
             if not workflow:
                 raise_status(HTTPStatus.NOT_FOUND, "Workflow does not exist")
 
-            pstat = ProcessStat(pid, workflow=workflow, state=Success(state), log=workflow.steps, current_user=user)
+            pstat = ProcessStat(
+                pid,
+                workflow=workflow,
+                state=Success(state),
+                log=workflow.steps,
+                current_user=user,
+            )
 
             safe_logstep_with_func = partial(safe_logstep, broadcast_func=None)
             pid = _run_process_async(pstat.pid, lambda: runwf(pstat, safe_logstep_with_func))
 
         except Exception as exc:
             local_logger.error("Worker failed to execute workflow", pid=pid, details=str(exc))
             return None
@@ -112,7 +118,25 @@
         local_logger.info("Resume task", pid=pid)
         return resume_process(pid, user_inputs=user_inputs, user=user)
 
     @celery.task(log=local_logger, name=RESUME_WORKFLOW)  # type: ignore
     def resume_workflow(pid: UUID, user_inputs: Optional[List[State]], user: str) -> Optional[UUID]:
         local_logger.info("Resume workflow", pid=pid)
         return resume_process(pid, user_inputs=user_inputs, user=user)
+
+
+class CeleryJobWorkerStatus(WorkerStatus):
+    def __init__(self) -> None:
+        super().__init__(executor_type="celery")
+        if not _celery:
+            logger.error("Can't create CeleryJobStatistics. Celery is not initialised.")
+            return
+
+        inspection: Inspect = _celery.control.inspect()
+        stats = inspection.stats()
+        self.number_of_workers_online = len(stats)
+
+        def sum_items(d: dict) -> int:
+            return sum(len(l) for _, l in d.items())
+
+        self.number_of_queued_jobs = sum_items(inspection.scheduled()) + sum_items(inspection.reserved())
+        self.number_of_running_jobs = sum(len(tasks) for w, tasks in inspection.active().items())
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/services/translations.py` & `orchestrator-core-1.0.2rc3/orchestrator/services/translations.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import json
 from pathlib import Path
-from typing import Dict
+from typing import Dict, Union
 
 from orchestrator.settings import app_settings
 
-Translations = Dict[str, dict | str]
+Translations = Dict[str, Union[dict, str]]
 
 
 def _load_translations_file(language: str, translations_dir: Path) -> Translations:
     filename = translations_dir / f"{language}.json"
     if not filename.exists():
         return {}
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/settings.py` & `orchestrator-core-1.0.2rc3/orchestrator/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -72,14 +72,18 @@
     TRACE_HOST: str = "http://localhost:4317"
     TRANSLATIONS_DIR: Optional[Path] = None
     WEBSOCKET_BROADCASTER_URL: str = "memory://"
     ENABLE_WEBSOCKETS: bool = True
     DISABLE_INSYNC_CHECK: bool = False
     DEFAULT_PRODUCT_WORKFLOWS: List[str] = ["modify_note"]
     SKIP_MODEL_FOR_MIGRATION_DB_DIFF: List[str] = []
+    SERVE_GRAPHQL_UI: bool = True
+    MUTATIONS_ENABLED: bool = False
+    FEDEREATION_ENABLED: bool = False
+    ENVIRONMENT_IGNORE_MUTATION_DISABLED: list = []
 
 
 class Oauth2Settings(BaseSettings):
     OAUTH2_ACTIVE: bool = False
     OAUTH2_RESOURCE_SERVER_ID: str = ""
     OAUTH2_RESOURCE_SERVER_SECRET: str = ""
     OAUTH2_TOKEN_URL: str = ""
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/targets.py` & `orchestrator-core-1.0.2rc3/orchestrator/workflows/removed_workflow.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from orchestrator.types import strEnum
+from orchestrator.workflow import StepList, workflow
 
 
-class Target(strEnum):
-    CREATE = "CREATE"
-    MODIFY = "MODIFY"
-    TERMINATE = "TERMINATE"
-    SYSTEM = "SYSTEM"
+# This workflow has been made to create the initial import process for a SN7 subscription
+# it does not do anything but is needed for the correct showing in the GUI.
+@workflow("Dummy workflow to replace removed workflows")
+def removed_workflow() -> StepList:
+    return StepList()
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/types.py` & `orchestrator-core-1.0.2rc3/orchestrator/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,16 @@
 # limitations under the License.
 
 from enum import Enum
 from http import HTTPStatus
 from typing import Any, Callable, Dict, Generator, List, Literal, Optional, Tuple, Type, TypedDict, TypeVar, Union
 from uuid import UUID
 
-try:
-    # python3.10 introduces types.UnionType for the new union and optional type defs.
-    from types import UnionType
-
-    union_types = [Union, UnionType]
-except ImportError:
-    union_types = [Union]
-
 from pydantic import BaseModel
-from pydantic.typing import get_args, get_origin
+from pydantic.typing import get_args, get_origin, is_union
 
 UUIDstr = str
 State = Dict[str, Any]
 JSON = Any
 # ErrorState is either a string containing an error message, a catched Exception or a tuple containing a message and
 # a HTTP status code
 ErrorState = Union[str, Exception, Tuple[str, Union[int, HTTPStatus]]]
@@ -243,15 +235,15 @@
     >>> is_optional_type(Optional[int], str)
     False
     >>> is_optional_type(Optional[State], int)
     False
     >>> is_optional_type(Optional[State], State)
     True
     """
-    if get_origin(t) in union_types and None.__class__ in get_args(t):
+    if is_union(get_origin(t)) and None.__class__ in get_args(t):
         for arg in get_args(t):
             if arg is None.__class__:
                 continue
 
             return not test_type or is_of_type(arg, test_type)
     return False
 
@@ -268,15 +260,15 @@
     >>> is_union_type(Union[int, str], Union[int, str])
     True
     >>> is_union_type(Union[int, None])
     True
     >>> is_union_type(int)
     False
     """
-    if get_origin(t) not in union_types:
+    if not is_union(get_origin(t)):
         return False
     if not test_type:
         return True
 
     if is_of_type(t, test_type):
         return True
     for arg in get_args(t):
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/utils/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/utils/crypt.py` & `orchestrator-core-1.0.2rc3/orchestrator/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/utils/datetime.py` & `orchestrator-core-1.0.2rc3/orchestrator/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/utils/docs.py` & `orchestrator-core-1.0.2rc3/orchestrator/utils/docs.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/utils/errors.py` & `orchestrator-core-1.0.2rc3/orchestrator/utils/errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/utils/functional.py` & `orchestrator-core-1.0.2rc3/orchestrator/utils/functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/utils/json.py` & `orchestrator-core-1.0.2rc3/orchestrator/utils/json.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/utils/redis.py` & `orchestrator-core-1.0.2rc3/orchestrator/utils/redis.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/utils/show_process.py` & `orchestrator-core-1.0.2rc3/orchestrator/utils/show_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/utils/speed.py` & `orchestrator-core-1.0.2rc3/orchestrator/utils/speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/utils/state.py` & `orchestrator-core-1.0.2rc3/orchestrator/utils/state.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/utils/strings.py` & `orchestrator-core-1.0.2rc3/orchestrator/utils/strings.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/utils/vlans.py` & `orchestrator-core-1.0.2rc3/orchestrator/utils/vlans.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/version.py` & `orchestrator-core-1.0.2rc3/orchestrator/version.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/websocket/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/websocket/managers/broadcast_websocket_manager.py` & `orchestrator-core-1.0.2rc3/orchestrator/websocket/managers/broadcast_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/websocket/managers/memory_websocket_manager.py` & `orchestrator-core-1.0.2rc3/orchestrator/websocket/managers/memory_websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/websocket/websocket_manager.py` & `orchestrator-core-1.0.2rc3/orchestrator/websocket/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/workflow.py` & `orchestrator-core-1.0.2rc3/orchestrator/workflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     Union,
     cast,
     overload,
     runtime_checkable,
 )
 from uuid import UUID
 
+import strawberry
 import structlog
 from nwastdlib import const, identity
 from structlog.contextvars import bound_contextvars
 from structlog.stdlib import BoundLogger
 
 from orchestrator.config.assignee import Assignee
 from orchestrator.db import EngineSettingsTable, db, transactional
@@ -399,14 +400,15 @@
         return ProcessStat(**{**asdict(self), **vs})
 
 
 S = TypeVar("S")
 F = TypeVar("F")
 
 
+@strawberry.enum
 class ProcessStatus(strEnum):
     CREATED = "created"
     RUNNING = "running"
     SUSPENDED = "suspended"
     WAITING = "waiting"
     ABORTED = "aborted"
     FAILED = "failed"
```

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/workflows/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/workflows/modify_note.py` & `orchestrator-core-1.0.2rc3/orchestrator/workflows/modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/workflows/steps.py` & `orchestrator-core-1.0.2rc3/orchestrator/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/workflows/tasks/__init__.py` & `orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/workflows/tasks/cleanup_tasks_log.py` & `orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/cleanup_tasks_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/workflows/tasks/resume_workflows.py` & `orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/workflows/tasks/validate_products.py` & `orchestrator-core-1.0.2rc3/orchestrator/workflows/tasks/validate_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/workflows/translations/en-GB.json` & `orchestrator-core-1.0.2rc3/orchestrator/workflows/translations/en-GB.json`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/orchestrator/workflows/utils.py` & `orchestrator-core-1.0.2rc3/orchestrator/workflows/utils.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/pyproject.toml` & `orchestrator-core-1.0.2rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     "Framework :: FastAPI",
     "Intended Audience :: Developers",
     "Intended Audience :: Telecommunications Industry",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.9",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "alembic==1.5.4",
     "broadcaster[redis]==0.2.0",
     "click==8.0.3",
@@ -61,22 +62,23 @@
     "redis~=4.4.2",
     "schedule==1.1.0",
     "sentry-sdk[fastapi]==1.15.0",
     "SQLAlchemy==1.4.28",
     "SQLAlchemy-Utils==0.40.0",
     "typer==0.7.0",
     "uvicorn[standard]~=0.20.0",
-    "nwa-stdlib~=1.4.6",
-    "oauth2-lib~=1.2.5",
+    "nwa-stdlib~=1.4.7",
+    "oauth2-lib~=1.2.8",
     "markupsafe==2.0.1",
     "bandit==1.7.2",
-    "tabulate==0.9.0"
+    "tabulate==0.9.0",
+    "strawberry-graphql==0.171.1"
 ]
 description-file = "README.md"
-requires-python = ">3.9,<3.12"
+requires-python = ">=3.9,<3.12"
 
 [project.urls]
 documentation = "https://workfloworchestrator.org/orchestrator-core/"
 
 [project.optional-dependencies]
 celery = [
     "celery~=5.2.7"
@@ -98,15 +100,15 @@
     "flake8-print",
     "flake8-rst",
     "flake8-rst-docstrings",
     "flake8-tidy-imports",
     "isort",
     "structlog",
     "jsonref",
-    "mypy==1.0.1",
+    "mypy",
     "pytest",
     "pytest-cov",
     "pytest-httpx",
     "pytest-xdist",
     "requests-mock",
     "urllib3_mock",
     "types-Deprecated",
```

### Comparing `orchestrator-core-1.0.2rc2/setup.cfg` & `orchestrator-core-1.0.2rc3/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 warn_no_return = True
 warn_unreachable = True
 implicit_reexport = False
 strict_equality = True
 show_error_codes = True
 show_column_numbers = True
 ;lineprecision_report = mypy-coverage
-plugins = pydantic.mypy
+plugins = pydantic.mypy, strawberry.ext.mypy_plugin
 
 ;Suppress "note: By default the bodies of untyped functions are not checked"
 disable_error_code = annotation-unchecked
 
 [pydantic-mypy]
 init_forbid_extra = True
 init_typed = True
```

### Comparing `orchestrator-core-1.0.2rc2/setup.py` & `orchestrator-core-1.0.2rc3/setup.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/acceptance_tests/conftest.py` & `orchestrator-core-1.0.2rc3/test/acceptance_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py` & `orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/devtools/populator/test_product_populator.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/acceptance_tests/fixtures/test_orchestrator/main.py` & `orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/main.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py` & `orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/product_blocks/test_product_blocks.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,36 +9,37 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from ipaddress import IPv4Address, IPv6Address
+from typing import Union
 from uuid import UUID
 
 from orchestrator.domain.base import ProductBlockModel
 from orchestrator.types import SubscriptionLifecycle
 
 
 class TestProductBlockInactive(ProductBlockModel, product_block_name="Test Product Block"):
-    an_int: int | None = None
-    a_str: str | None = None
-    a_bool: bool | None = None
-    an_uuid: UUID | None = None
-    an_ipv4: IPv4Address | None = None
-    an_ipv6: IPv6Address | None = None
+    an_int: Union[int, None] = None
+    a_str: Union[str, None] = None
+    a_bool: Union[bool, None] = None
+    an_uuid: Union[UUID, None] = None
+    an_ipv4: Union[IPv4Address, None] = None
+    an_ipv6: Union[IPv6Address, None] = None
 
 
 class TestProductBlockProvisioning(TestProductBlockInactive, lifecycle=[SubscriptionLifecycle.PROVISIONING]):
     an_int: int
     a_str: str
-    a_bool: bool | None = None
+    a_bool: Union[bool, None] = None
     an_uuid: UUID
-    an_ipv4: IPv4Address | None = None
-    an_ipv6: IPv6Address | None = None
+    an_ipv4: Union[IPv4Address, None] = None
+    an_ipv6: Union[IPv6Address, None] = None
 
 
 class TestProductBlock(TestProductBlockProvisioning, lifecycle=[SubscriptionLifecycle.ACTIVE]):
     an_int: int
     a_str: str
     a_bool: bool
     an_uuid: UUID
```

### Comparing `orchestrator-core-1.0.2rc2/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py` & `orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/products/test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py` & `orchestrator-core-1.0.2rc3/test/acceptance_tests/fixtures/test_orchestrator/workflows/create_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/acceptance_tests/test_test_product.py` & `orchestrator-core-1.0.2rc3/test/acceptance_tests/test_test_product.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/api/conftest.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/api/test_caching.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_caching.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/api/test_fixed_inputs.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_fixed_inputs.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/api/test_health.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_health.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/api/test_helpers.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_helpers.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/api/test_models.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_models.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/api/test_processes.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/api/test_processes_ws.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_processes_ws.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/api/test_product_blocks.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_product_blocks.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/api/test_products.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/api/test_resource_types.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/api/test_settings.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_settings.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/api/test_subscription_customer_descriptions.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_subscription_customer_descriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/api/test_subscriptions.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/api/test_workflows.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/cli/test_migrate_domain_models_with_instances.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/cli/test_migrate_domain_models_with_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/cli/test_migrate_domain_models_without_instances.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/cli/test_migrate_domain_models_without_instances.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/conftest.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from orchestrator.domain import SUBSCRIPTION_MODEL_REGISTRY, SubscriptionModel
 from orchestrator.domain.base import ProductBlockModel
 from orchestrator.forms import FormPage
 from orchestrator.services.translations import generate_translations
 from orchestrator.settings import app_settings
 from orchestrator.types import SubscriptionLifecycle, UUIDstr
 from orchestrator.utils.json import json_dumps
+from test.unit_tests.fixtures.processes import mocked_processes, mocked_processes_resumeall, test_workflow  # noqa: F401
 from test.unit_tests.fixtures.products.product_blocks.product_block_list_nested import (  # noqa: F401
     test_product_block_list_nested,
     test_product_block_list_nested_db_in_use_by_block,
 )
 from test.unit_tests.fixtures.products.product_blocks.product_block_one import (  # noqa: F401
     test_product_block_one,
     test_product_block_one_db,
```

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/domain/test_base.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/domain/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from datetime import datetime
 from typing import List, Optional, TypeVar
 from unittest import mock
 from uuid import uuid4
 
 import pytest
 import pytz
@@ -1094,19 +1095,27 @@
 
     assert _is_constrained_list_type(ListType) is True
     assert _is_constrained_list_type(SubscriptionInstanceList[int]) is True
     assert _is_constrained_list_type(Optional[int]) is False
     assert _is_constrained_list_type(List[int]) is False
 
 
-def test_diff_in_db(test_product_one, test_product_type_one):
+def test_diff_in_db_empty(test_product_one, test_product_type_one):
     ProductTypeOneForTestInactive, _, _ = test_product_type_one
 
     assert ProductTypeOneForTestInactive.diff_product_in_database(test_product_one) == {}
 
+
+@pytest.mark.skipif(
+    sys.version_info < (3, 10), reason="Python 3.10 changed behavior of object.__annotations__ on empty derived class"
+)
+def test_diff_in_db_when_no_fields(test_product_one, test_product_type_one):
+    # As of Python 3.10, __annotations__ of an empty derived class no longer contain inherited fields
+    # Skipping this test for <3.10 because we have no usecase for empty derived classes + it's very difficult to fix this
+
     class Wrong(SubscriptionModel):
         pass
 
     assert (
         Wrong.diff_product_in_database(test_product_one)
         == {
             "TestProductOne": {
```

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/domain/test_base_with_list_union.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/domain/test_base_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/domain/test_base_with_union.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/domain/test_base_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/__init__.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_block_with_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_blocks/product_sub_block_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_list_union_overlap.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_one_nested.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_list_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_one.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_two.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_sub_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/product_types/product_type_union.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/product_types/product_type_union.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/fixtures/products/resource_types.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/fixtures/products/resource_types.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/forms/shared.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/forms/shared.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/forms/test_generic_validators.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/forms/test_generic_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/forms/test_network_validators.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/forms/test_network_validators.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/forms/test_post_process.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/forms/test_post_process.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/schedules/test_scheduling.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/schedules/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/services/test_processes.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/services/test_processes.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/services/test_products.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/services/test_products.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/services/test_subscriptions.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/services/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/services/test_translations.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/services/test_translations.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/test_db.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/test_db.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/test_workflow.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/utils/test_errors.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/utils/test_functional.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/utils/test_json.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/utils/test_speed.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_speed.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/utils/test_state.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_state.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/utils/test_vlans.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/utils/test_vlans.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/workflows/__init__.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/workflows/shared/test_validate_subscriptions.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/workflows/shared/test_validate_subscriptions.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/workflows/tasks/test_clean_up_task_log.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/workflows/tasks/test_clean_up_task_log.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/workflows/tasks/test_resume_workflows.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/workflows/tasks/test_resume_workflows.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/workflows/test_config_db_code.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/workflows/test_config_db_code.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/workflows/test_generic_workflow_steps.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/workflows/test_generic_workflow_steps.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/test/unit_tests/workflows/test_modify_note.py` & `orchestrator-core-1.0.2rc3/test/unit_tests/workflows/test_modify_note.py`

 * *Files identical despite different names*

### Comparing `orchestrator-core-1.0.2rc2/PKG-INFO` & `orchestrator-core-1.0.2rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: orchestrator-core
-Version: 1.0.2rc2
+Version: 1.0.2rc3
 Summary: Open source orchestration software for NREN's
-Requires-Python: >3.9,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
@@ -20,14 +20,15 @@
 Classifier: Framework :: FastAPI
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: alembic==1.5.4
 Requires-Dist: broadcaster[redis]==0.2.0
 Requires-Dist: click==8.0.3
 Requires-Dist: deepmerge==0.1.0
 Requires-Dist: fastapi~=0.91.0
@@ -51,19 +52,20 @@
 Requires-Dist: redis~=4.4.2
 Requires-Dist: schedule==1.1.0
 Requires-Dist: sentry-sdk[fastapi]==1.15.0
 Requires-Dist: SQLAlchemy==1.4.28
 Requires-Dist: SQLAlchemy-Utils==0.40.0
 Requires-Dist: typer==0.7.0
 Requires-Dist: uvicorn[standard]~=0.20.0
-Requires-Dist: nwa-stdlib~=1.4.6
-Requires-Dist: oauth2-lib~=1.2.5
+Requires-Dist: nwa-stdlib~=1.4.7
+Requires-Dist: oauth2-lib~=1.2.8
 Requires-Dist: markupsafe==2.0.1
 Requires-Dist: bandit==1.7.2
 Requires-Dist: tabulate==0.9.0
+Requires-Dist: strawberry-graphql==0.171.1
 Requires-Dist: celery~=5.2.7 ; extra == "celery"
 Requires-Dist: toml ; extra == "dev"
 Requires-Dist: bumpversion ; extra == "dev"
 Requires-Dist: mypy_extensions ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pydocstyle ; extra == "dev"
 Requires-Dist: python-dotenv ; extra == "dev"
@@ -87,15 +89,15 @@
 Requires-Dist: flake8-print ; extra == "test"
 Requires-Dist: flake8-rst ; extra == "test"
 Requires-Dist: flake8-rst-docstrings ; extra == "test"
 Requires-Dist: flake8-tidy-imports ; extra == "test"
 Requires-Dist: isort ; extra == "test"
 Requires-Dist: structlog ; extra == "test"
 Requires-Dist: jsonref ; extra == "test"
-Requires-Dist: mypy==1.0.1 ; extra == "test"
+Requires-Dist: mypy ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-httpx ; extra == "test"
 Requires-Dist: pytest-xdist ; extra == "test"
 Requires-Dist: requests-mock ; extra == "test"
 Requires-Dist: urllib3_mock ; extra == "test"
 Requires-Dist: types-Deprecated ; extra == "test"
```

