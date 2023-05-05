# Comparing `tmp/ansible-builder-3.0.0rc1.tar.gz` & `tmp/ansible-builder-3.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-builder-3.0.0rc1.tar", last modified: Tue Apr 25 05:32:44 2023, max compression
+gzip compressed data, was "ansible-builder-3.0.0rc2.tar", last modified: Fri May  5 21:50:36 2023, max compression
```

## Comparing `ansible-builder-3.0.0rc1.tar` & `ansible-builder-3.0.0rc2.tar`

### file list

```diff
@@ -1,220 +1,215 @@
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.543171 ansible-builder-3.0.0rc1/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      210 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.cherry_picker.toml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      288 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.coveragerc
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       25 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.dockerignore
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.534170 ansible-builder-3.0.0rc1/.github/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.534170 ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2036 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       27 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      623 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/documentation_report.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      600 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       23 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/issue_labeler.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      113 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/patchback.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       37 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/pr_labeler_existing.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       90 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/pr_labeler_new.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.535171 ansible-builder-3.0.0rc1/.github/test-scripts/
--rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     4597 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/.github/test-scripts/setup_pulp.sh
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.535171 ansible-builder-3.0.0rc1/.github/workflows/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4750 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/.github/workflows/ci.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      763 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/workflows/triage_existing.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      734 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.github/workflows/triage_new.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      334 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/.readthedocs.yaml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      547 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/.yamllint
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      306 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/CODEOWNERS
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1176 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/CONTRIBUTING.md
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      827 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/Containerfile
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     9302 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/LICENSE.md
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       42 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/MANIFEST.in
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3008 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/Makefile
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2865 2023-04-25 05:32:44.543171 ansible-builder-3.0.0rc1/PKG-INFO
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1766 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/README.md
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      313 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/SECURITY.md
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      494 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/TODO.org
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.536171 ansible-builder-3.0.0rc1/ansible_builder/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/ansible_builder/__init__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       60 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/__main__.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.536171 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/__init__.py
--rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     6537 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/assemble
--rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     3474 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/check_ansible
--rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     1618 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/check_galaxy
--rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     5909 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/entrypoint
--rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     1480 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/get-extras-packages
--rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     3440 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/install-from-bindep
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    14022 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/introspect.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     8136 2023-04-25 05:05:41.000000 ansible-builder-3.0.0rc1/ansible_builder/cli.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      157 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/ansible_builder/colors.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1198 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/constants.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    17766 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/ansible_builder/containerfile.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    13948 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/ansible_builder/ee_schema.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      407 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/exceptions.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     9107 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/main.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4633 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/policies.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3084 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/requirements.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     8843 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/ansible_builder/user_definition.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     6382 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/ansible_builder/utils.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.536171 ansible-builder-3.0.0rc1/ansible_builder.egg-info/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2865 2023-04-25 05:32:44.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/PKG-INFO
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5217 2023-04-25 05:32:44.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/SOURCES.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        1 2023-04-25 05:32:44.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/dependency_links.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       60 2023-04-25 05:32:44.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/entry_points.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        1 2023-04-25 05:20:20.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/not-zip-safe
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       47 2023-04-25 05:32:44.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/pbr.json
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       45 2023-04-25 05:32:44.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/requires.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       16 2023-04-25 05:32:44.000000 ansible-builder-3.0.0rc1/ansible_builder.egg-info/top_level.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      211 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/bindep.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.537171 ansible-builder-3.0.0rc1/demo/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1353 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/demo/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.537171 ansible-builder-3.0.0rc1/docs/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      612 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/Makefile
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.537171 ansible-builder-3.0.0rc1/docs/_static/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/_static/.gitkeep
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.537171 ansible-builder-3.0.0rc1/docs/_templates/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/_templates/.gitkeep
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2581 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/collection_metadata.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5018 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/docs/conf.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    13751 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/docs/definition.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      543 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/glossary.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2082 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/index.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      861 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/docs/installation.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      819 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/make.bat
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       15 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/docs/requirements.in
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      522 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/docs/requirements.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     8293 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/docs/usage.rst
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.531170 ansible-builder-3.0.0rc1/packaging/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/packaging/rpm/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      257 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/packaging/rpm/Dockerfile.epel-7-x86_64
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      167 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/packaging/rpm/Dockerfile.epel-8-x86_64
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      921 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/packaging/rpm/ansible-builder.spec.j2
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      457 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/packaging/rpm/docker-compose.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      464 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/pytest.ini
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       45 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/requirements.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1197 2023-04-25 05:32:44.543171 ansible-builder-3.0.0rc1/setup.cfg
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      133 2023-04-24 23:43:10.000000 ansible-builder-3.0.0rc1/setup.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/__init__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5587 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/conftest.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/data/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1857 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/README.md
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      108 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/env/settings
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      577 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/project/ansible.posix.at.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      109 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/requirements.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      255 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible.posix.at/run.sh
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/data/ansible_cfg_for_galaxy/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      420 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/ansible_cfg_for_galaxy/ansible-test.cfg
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/ansible_cfg_for_galaxy/requirements.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.531170 ansible-builder-3.0.0rc1/test/data/ansible_collections/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.531170 ansible-builder-3.0.0rc1/test/data/ansible_collections/other/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/data/ansible_collections/other/reqfile/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       44 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/other/reqfile/requirements.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.531170 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.538171 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/bindep/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/bindep/MANIFEST.json
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       53 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/bindep/bindep.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/metadata/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        2 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/metadata/MANIFEST.json
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/metadata/meta/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       59 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/metadata/meta/execution-environment.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       13 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/metadata/my-requirements.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/reqfile/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        2 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/reqfile/MANIFEST.json
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       73 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/reqfile/extra_req.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       67 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/ansible_collections/test/reqfile/requirements.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/blank/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/blank/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       97 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/blank/env/settings
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       15 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/blank/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/blank/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       99 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/blank/project/blank.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      237 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/blank/run.sh
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/build_args/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      107 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/build_args/base-image.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       73 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/build_args/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.539171 ansible-builder-3.0.0rc1/test/data/build_fail/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       78 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/build_fail/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/definition_files/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      187 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/definition_files/bad.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       12 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/definition_files/invalid.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/definition_files/no_galaxy.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/definition_files/no_python.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/needs_git/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/needs_git/execution-environment.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       82 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/needs_git/requirements.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/nested_galaxy_file/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/nested_galaxy_file/foo/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       20 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/nested_galaxy_file/foo/requirements.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       60 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/nested_galaxy_file/nested-galaxy.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/pip/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/pip/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       95 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pip/env/settings
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       64 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pip/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/pip/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      131 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pip/project/pip.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       26 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pip/project/requirements.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      239 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pip/run.sh
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/prepend_steps/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       67 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/prepend_steps/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/pytz/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/pytz/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       30 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pytz/env/extravars
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       96 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pytz/env/settings
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pytz/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.540171 ansible-builder-3.0.0rc1/test/data/pytz/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      294 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pytz/project/pytz.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       35 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/pytz/requirements.yml
--rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)      699 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/run.sh
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/subversion/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       53 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/subversion/bindep.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/subversion/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      102 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/subversion/env/settings
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       50 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/subversion/execution-environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/subversion/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      239 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/subversion/project/subversion.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      241 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/data/subversion/run.sh
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/v2/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5135 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v2/RPM-GPG-KEY-redhat-release
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v2/invalid-keyring
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/v2/sig_req/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      397 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v2/sig_req/ee-good.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      289 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v2/sig_req/ee-no-orig.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.532171 ansible-builder-3.0.0rc1/test/data/v3/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/v3/check_ansible/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      258 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/check_ansible/ee-missing-ansible.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      254 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/check_ansible/ee-missing-runner.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      235 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/check_ansible/ee-skip.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/v3/complete/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      685 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/complete/ee.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/v3/complete/files/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/v3/complete/files/data/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/complete/files/data/a.dat
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.541171 ansible-builder-3.0.0rc1/test/data/v3/complete/files/data/text_files/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/complete/files/data/text_files/a.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/complete/files/random.cfg
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.542171 ansible-builder-3.0.0rc1/test/data/v3/pre_and_post/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      427 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/pre_and_post/ee.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/data/v3/pre_and_post/requirements.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.542171 ansible-builder-3.0.0rc1/test/integration/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/integration/conftest.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    10171 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/integration/test_build.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    13824 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/test/integration/test_create.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1425 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/integration/test_help.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2698 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/integration/test_introspect_cli.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.542171 ansible-builder-3.0.0rc1/test/pulp_integration/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     7877 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/pulp_integration/test_policies.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1715 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/pulp_integration/test_v3.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      114 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/requirements.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-04-25 05:32:44.543171 ansible-builder-3.0.0rc1/test/unit/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/unit/__init__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    10219 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/unit/test_cli.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4871 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/unit/test_containerfile.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1228 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/unit/test_introspect.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4927 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/unit/test_main.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5909 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/unit/test_policies.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1515 2022-03-31 00:02:18.000000 ansible-builder-3.0.0rc1/test/unit/test_requirements.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    11769 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/test/unit/test_user_definition.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3425 2023-04-25 05:29:39.000000 ansible-builder-3.0.0rc1/test/unit/test_utils.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1474 2023-04-24 22:28:45.000000 ansible-builder-3.0.0rc1/tox.ini
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.686055 ansible-builder-3.0.0rc2/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      210 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.cherry_picker.toml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      288 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.coveragerc
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       25 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.dockerignore
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      126 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.git_archival.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       33 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.gitattributes
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.680055 ansible-builder-3.0.0rc2/.github/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.680055 ansible-builder-3.0.0rc2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2036 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       27 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      623 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.github/ISSUE_TEMPLATE/documentation_report.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      600 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       23 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.github/issue_labeler.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      113 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.github/patchback.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       37 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.github/pr_labeler_existing.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       90 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.github/pr_labeler_new.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.680055 ansible-builder-3.0.0rc2/.github/test-scripts/
+-rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     5235 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.github/test-scripts/setup_pulp.sh
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.680055 ansible-builder-3.0.0rc2/.github/workflows/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4934 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.github/workflows/ci.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      761 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.github/workflows/triage_existing.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      732 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.github/workflows/triage_new.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      408 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.gitignore
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      334 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.readthedocs.yaml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      547 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/.yamllint
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      306 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/CODEOWNERS
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3166 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/CONTRIBUTING.md
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      741 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/Containerfile
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     9302 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/LICENSE.md
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3008 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/Makefile
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1058 2023-05-05 21:50:36.686055 ansible-builder-3.0.0rc2/PKG-INFO
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1529 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/README.md
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      313 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/SECURITY.md
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      494 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/TODO.org
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      211 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/bindep.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.680055 ansible-builder-3.0.0rc2/demo/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1766 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/demo/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.681054 ansible-builder-3.0.0rc2/docs/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      612 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/docs/Makefile
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.681054 ansible-builder-3.0.0rc2/docs/_static/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/docs/_static/.gitkeep
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.681054 ansible-builder-3.0.0rc2/docs/_templates/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/docs/_templates/.gitkeep
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2581 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/docs/collection_metadata.rst
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4997 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/docs/conf.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)    13655 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/docs/definition.rst
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      543 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/docs/glossary.rst
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2082 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/docs/index.rst
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      861 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/docs/installation.rst
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      819 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/docs/make.bat
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       41 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/docs/requirements.in
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1428 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/docs/requirements.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     8454 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/docs/usage.rst
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.678054 ansible-builder-3.0.0rc2/packaging/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.681054 ansible-builder-3.0.0rc2/packaging/rpm/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      257 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/packaging/rpm/Dockerfile.epel-7-x86_64
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      167 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/packaging/rpm/Dockerfile.epel-8-x86_64
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      921 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/packaging/rpm/ansible-builder.spec.j2
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      457 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/packaging/rpm/docker-compose.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      211 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/pyproject.toml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      484 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/pytest.ini
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1301 2023-05-05 21:50:36.686055 ansible-builder-3.0.0rc2/setup.cfg
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.678054 ansible-builder-3.0.0rc2/src/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.682054 ansible-builder-3.0.0rc2/src/ansible_builder/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/__init__.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       60 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/__main__.py
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.682054 ansible-builder-3.0.0rc2/src/ansible_builder/_target_scripts/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/_target_scripts/__init__.py
+-rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     6209 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/_target_scripts/assemble
+-rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     3474 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/_target_scripts/check_ansible
+-rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     1618 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/_target_scripts/check_galaxy
+-rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     5909 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/_target_scripts/entrypoint
+-rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     3616 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/_target_scripts/install-from-bindep
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)    14041 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/_target_scripts/introspect.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     8202 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/cli.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      157 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/colors.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1430 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/constants.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)    19168 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/containerfile.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)    14509 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/ee_schema.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      407 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/exceptions.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     9107 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/main.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4633 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/policies.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     9114 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/user_definition.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     7146 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/src/ansible_builder/utils.py
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.682054 ansible-builder-3.0.0rc2/src/ansible_builder.egg-info/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1058 2023-05-05 21:50:36.000000 ansible-builder-3.0.0rc2/src/ansible_builder.egg-info/PKG-INFO
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5098 2023-05-05 21:50:36.000000 ansible-builder-3.0.0rc2/src/ansible_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        1 2023-05-05 21:50:36.000000 ansible-builder-3.0.0rc2/src/ansible_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       60 2023-05-05 21:50:36.000000 ansible-builder-3.0.0rc2/src/ansible_builder.egg-info/entry_points.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       45 2023-05-05 21:50:36.000000 ansible-builder-3.0.0rc2/src/ansible_builder.egg-info/requires.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       16 2023-05-05 21:50:36.000000 ansible-builder-3.0.0rc2/src/ansible_builder.egg-info/top_level.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.682054 ansible-builder-3.0.0rc2/test/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/__init__.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     7454 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/conftest.py
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.683055 ansible-builder-3.0.0rc2/test/data/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1857 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/README.md
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.683055 ansible-builder-3.0.0rc2/test/data/ansible.posix.at/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.683055 ansible-builder-3.0.0rc2/test/data/ansible.posix.at/env/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      108 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible.posix.at/env/settings
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      388 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible.posix.at/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.683055 ansible-builder-3.0.0rc2/test/data/ansible.posix.at/project/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      577 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible.posix.at/project/ansible.posix.at.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      109 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible.posix.at/requirements.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      255 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible.posix.at/run.sh
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.683055 ansible-builder-3.0.0rc2/test/data/ansible_cfg_for_galaxy/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      420 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible_cfg_for_galaxy/ansible-test.cfg
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible_cfg_for_galaxy/requirements.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.678054 ansible-builder-3.0.0rc2/test/data/ansible_collections/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.678054 ansible-builder-3.0.0rc2/test/data/ansible_collections/other/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.683055 ansible-builder-3.0.0rc2/test/data/ansible_collections/other/reqfile/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       78 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible_collections/other/reqfile/requirements.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.678054 ansible-builder-3.0.0rc2/test/data/ansible_collections/test/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.683055 ansible-builder-3.0.0rc2/test/data/ansible_collections/test/bindep/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible_collections/test/bindep/MANIFEST.json
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       53 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible_collections/test/bindep/bindep.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.683055 ansible-builder-3.0.0rc2/test/data/ansible_collections/test/metadata/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        2 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible_collections/test/metadata/MANIFEST.json
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.683055 ansible-builder-3.0.0rc2/test/data/ansible_collections/test/metadata/meta/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       59 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible_collections/test/metadata/meta/execution-environment.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       13 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible_collections/test/metadata/my-requirements.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.683055 ansible-builder-3.0.0rc2/test/data/ansible_collections/test/reqfile/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        2 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible_collections/test/reqfile/MANIFEST.json
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       73 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible_collections/test/reqfile/extra_req.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      106 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/ansible_collections/test/reqfile/requirements.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.683055 ansible-builder-3.0.0rc2/test/data/blank/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.683055 ansible-builder-3.0.0rc2/test/data/blank/env/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       97 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/blank/env/settings
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       15 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/blank/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.683055 ansible-builder-3.0.0rc2/test/data/blank/project/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       99 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/blank/project/blank.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      237 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/blank/run.sh
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.684054 ansible-builder-3.0.0rc2/test/data/build_args/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      344 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/build_args/base-image.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       73 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/build_args/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.684054 ansible-builder-3.0.0rc2/test/data/build_fail/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      190 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/build_fail/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.684054 ansible-builder-3.0.0rc2/test/data/definition_files/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      187 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/definition_files/bad.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       12 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/definition_files/invalid.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/definition_files/no_galaxy.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       56 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/definition_files/no_python.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.684054 ansible-builder-3.0.0rc2/test/data/minimal_fast/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      359 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/minimal_fast/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.684054 ansible-builder-3.0.0rc2/test/data/nested_galaxy_file/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.684054 ansible-builder-3.0.0rc2/test/data/nested_galaxy_file/foo/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       20 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/nested_galaxy_file/foo/requirements.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       60 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/nested_galaxy_file/nested-galaxy.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.684054 ansible-builder-3.0.0rc2/test/data/pip/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.684054 ansible-builder-3.0.0rc2/test/data/pip/env/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       95 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/pip/env/settings
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      361 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/pip/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.684054 ansible-builder-3.0.0rc2/test/data/pip/project/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      131 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/pip/project/pip.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       26 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/pip/project/requirements.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      239 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/pip/run.sh
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.684054 ansible-builder-3.0.0rc2/test/data/pytz/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.684054 ansible-builder-3.0.0rc2/test/data/pytz/env/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       30 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/pytz/env/extravars
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       96 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/pytz/env/settings
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      515 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/pytz/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.684054 ansible-builder-3.0.0rc2/test/data/pytz/project/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      294 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/pytz/project/pytz.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       35 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/pytz/requirements.yml
+-rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)      699 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/run.sh
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.685054 ansible-builder-3.0.0rc2/test/data/subversion/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)       53 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/subversion/bindep.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.685054 ansible-builder-3.0.0rc2/test/data/subversion/env/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      102 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/subversion/env/settings
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      287 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/subversion/execution-environment.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.685054 ansible-builder-3.0.0rc2/test/data/subversion/project/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      239 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/subversion/project/subversion.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      241 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/subversion/run.sh
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.685054 ansible-builder-3.0.0rc2/test/data/v2/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5135 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/v2/RPM-GPG-KEY-redhat-release
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/v2/invalid-keyring
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.685054 ansible-builder-3.0.0rc2/test/data/v2/sig_req/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      397 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/v2/sig_req/ee-good.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      289 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/v2/sig_req/ee-no-orig.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.679054 ansible-builder-3.0.0rc2/test/data/v3/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.685054 ansible-builder-3.0.0rc2/test/data/v3/check_ansible/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      258 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/v3/check_ansible/ee-missing-ansible.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      254 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/v3/check_ansible/ee-missing-runner.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      235 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/v3/check_ansible/ee-skip.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.685054 ansible-builder-3.0.0rc2/test/data/v3/complete/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      746 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/v3/complete/ee.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.685054 ansible-builder-3.0.0rc2/test/data/v3/complete/files/
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.685054 ansible-builder-3.0.0rc2/test/data/v3/complete/files/data/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/v3/complete/files/data/a.dat
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.685054 ansible-builder-3.0.0rc2/test/data/v3/complete/files/data/text_files/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/v3/complete/files/data/text_files/a.txt
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/v3/complete/files/random.cfg
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.685054 ansible-builder-3.0.0rc2/test/data/v3/pre_and_post/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      427 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/v3/pre_and_post/ee.yml
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/data/v3/pre_and_post/requirements.yml
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.686055 ansible-builder-3.0.0rc2/test/integration/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/integration/conftest.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     9607 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/integration/test_build.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)    16934 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/integration/test_create.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1425 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/integration/test_help.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2808 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/integration/test_introspect_cli.py
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.686055 ansible-builder-3.0.0rc2/test/pulp_integration/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     6824 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/pulp_integration/test_policies.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1715 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/pulp_integration/test_v3.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)      114 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/requirements.txt
+drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:50:36.686055 ansible-builder-3.0.0rc2/test/unit/
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/unit/__init__.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)    12359 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/unit/test_cli.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4871 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/unit/test_containerfile.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1397 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/unit/test_introspect.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4927 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/unit/test_main.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5909 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/unit/test_policies.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1529 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/unit/test_requirements.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)    12554 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/unit/test_user_definition.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3723 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/test/unit/test_utils.py
+-rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1806 2023-05-05 21:49:37.000000 ansible-builder-3.0.0rc2/tox.ini
```

### Comparing `ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/bug_report.yml` & `ansible-builder-3.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/documentation_report.yml` & `ansible-builder-3.0.0rc2/.github/ISSUE_TEMPLATE/documentation_report.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/.github/ISSUE_TEMPLATE/feature_request.yml` & `ansible-builder-3.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/.github/test-scripts/setup_pulp.sh` & `ansible-builder-3.0.0rc2/.github/test-scripts/setup_pulp.sh`

 * *Files 22% similar despite different names*

```diff
@@ -33,18 +33,37 @@
 docker:
      registry.redhat.io:
          sigstore: https://registry.redhat.io/containers/sigstore
 EOF
 
 
 ##############################################################################
+# Set up for an insecure registry. Back it up only once for local testing.
+##############################################################################
+
+REGISTRY_FILE="$HOME/.config/containers/registries.conf"
+REGISTRY_FILE_BACKUP="${REGISTRY_FILE}.ORIG"
+if [ -e "$REGISTRY_FILE" ] && [ ! -e "$REGISTRY_FILE_BACKUP" ]
+then
+    echo "Backing up user's Podman registry to $REGISTRY_FILE_BACKUP"
+    mv $REGISTRY_FILE $REGISTRY_FILE_BACKUP
+fi
+
+cat <<EOF > "$REGISTRY_FILE"
+[[registry]]
+location="localhost:8080"
+insecure=true
+EOF
+
+##############################################################################
 # Pull and run the pulp container
 ##############################################################################
 
-podman pull docker.io/pulp/pulp:3.19
+PULP_IMAGE="pulp:3.23.3"
+podman pull docker.io/pulp/$PULP_IMAGE
 
 mkdir pulp
 cd pulp
 mkdir settings pulp_storage pgsql containers
 
 echo "CONTENT_ORIGIN='http://$(hostname):8080'
 ANSIBLE_API_HOSTNAME='http://$(hostname):8080'
@@ -55,15 +74,15 @@
            --publish 8080:80 \
            --name pulp \
            --volume "$(pwd)/settings":/etc/pulp \
            --volume "$(pwd)/pulp_storage":/var/lib/pulp \
            --volume "$(pwd)/pgsql":/var/lib/pgsql \
            --volume "$(pwd)/containers":/var/lib/containers \
            --device /dev/fuse \
-           pulp/pulp
+           $PULP_IMAGE
 
 ##############################################################################
 # Iteratively query the REST API until we get a JSON response (http code will
 # be 200) which will indicate the system is ready.
 ##############################################################################
 
 set +e
```

### Comparing `ansible-builder-3.0.0rc1/.github/workflows/ci.yml` & `ansible-builder-3.0.0rc2/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
       - name: Create tox environment
         run: |
           tox --notest
 
       - name: Run pulp integration tests
         run: |
-          tox
+          tox -- --run-destructive
 
 
   integration:
     runs-on: ubuntu-22.04
     name: Integration - ${{ matrix.py_version.name }}
 
     env:
@@ -123,14 +123,16 @@
 
           - name: '3.11'
             tox_env: integration-py311
 
     steps:
       - name: Checkout
         uses: actions/checkout@v3
+        with:
+          fetch-depth: 0  # this is not ideal, but we need tags available to generate versions in tests
 
       - name: Install Python ${{ matrix.py_version.name }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.py_version.name }}
 
       - name: Install tox
@@ -138,17 +140,17 @@
           python3 -m pip install --upgrade pip
           python3 -m pip install tox
 
       - name: Create tox environment
         run: |
           tox --notest
 
-      - name: Run integration tests
+      - name: Run integration tests (including destructive)
         run: |
-          tox
+          tox -- --run-destructive
 
       - name: Upload coverage report
         uses: codecov/codecov-action@v3
         with:
           files: test/coverage/reports/coverage.xml
           flags: ${{ matrix.py_version.tox_env }}
```

### Comparing `ansible-builder-3.0.0rc1/.github/workflows/triage_existing.yml` & `ansible-builder-3.0.0rc2/.github/workflows/triage_existing.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 jobs:
   triage:
     runs-on: ubuntu-latest
     name: Label
 
     steps:
       - name: Label pull requests
-        uses: actions/labeler@v3
+        uses: actions/labeler@v4
         with:
           repo-token: "${{ secrets.GITHUB_TOKEN }}"
           configuration-path: .github/pr_labeler_existing.yml
         if: github.event_name == 'pull_request_target'
 
       - name: Label issues
-        uses: github/issue-labeler@v2.4.1
+        uses: github/issue-labeler@v2.6
         with:
           repo-token: "${{ secrets.GITHUB_TOKEN }}"
           not-before: 2021-12-07T07:00:00Z
           configuration-path: .github/issue_labeler.yml
           enable-versioned-regex: 0
         if: github.event_name == 'issues'
```

### Comparing `ansible-builder-3.0.0rc1/.github/workflows/triage_new.yml` & `ansible-builder-3.0.0rc2/.github/workflows/triage_new.yml`

 * *Files 14% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 jobs:
   triage:
     runs-on: ubuntu-latest
     name: Label
 
     steps:
       - name: Label pull requests
-        uses: actions/labeler@v3
+        uses: actions/labeler@v4
         with:
           repo-token: "${{ secrets.GITHUB_TOKEN }}"
           configuration-path: .github/pr_labeler_new.yml
         if: github.event_name == 'pull_request_target'
 
       - name: Label issues
-        uses: github/issue-labeler@v2.4.1
+        uses: github/issue-labeler@v2.6
         with:
           repo-token: "${{ secrets.GITHUB_TOKEN }}"
           not-before: 2021-12-07T07:00:00Z
           configuration-path: .github/issue_labeler.yml
           enable-versioned-regex: 0
         if: github.event_name == 'issues'
```

### Comparing `ansible-builder-3.0.0rc1/.yamllint` & `ansible-builder-3.0.0rc2/.yamllint`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/Containerfile` & `ansible-builder-3.0.0rc2/Containerfile`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 ARG BASE_IMAGE=quay.io/centos/centos:stream9
 
 FROM $BASE_IMAGE as builder
 # build this library (meaning ansible-builder)
 COPY . /tmp/src
-COPY ./ansible_builder/_target_scripts/* /output/scripts/
+COPY ./src/ansible_builder/_target_scripts/* /output/scripts/
 RUN python3 -m ensurepip
 RUN python3 -m pip install --upgrade pip
 RUN python3 -m pip install --no-cache-dir bindep wheel
 RUN /output/scripts/assemble
 
 FROM $BASE_IMAGE
 COPY --from=builder /output/ /output
 # building EEs require the install-from-bindep script, but not the rest of the /output folder
 RUN /output/scripts/install-from-bindep && find /output/* -not -name install-from-bindep -exec rm -rf {} +
 
 # copy the assemble scripts themselves into this container
-COPY ./ansible_builder/_target_scripts/assemble /usr/local/bin/assemble
-COPY ./ansible_builder/_target_scripts/get-extras-packages /usr/local/bin/get-extras-packages
+COPY ./src/ansible_builder/_target_scripts/assemble /usr/local/bin/assemble
```

### Comparing `ansible-builder-3.0.0rc1/LICENSE.md` & `ansible-builder-3.0.0rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/Makefile` & `ansible-builder-3.0.0rc2/Makefile`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/README.md` & `ansible-builder-3.0.0rc2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,44 +3,34 @@
 
 # Ansible Builder
 
 Ansible Builder is a tool that automates the process of building execution
 environments using the schemas and tooling defined in various Ansible
 Collections and by the user.
 
-
 See the readthedocs page for `ansible-builder` at:
 
-https://ansible-builder.readthedocs.io/en/latest/
+https://ansible-builder.readthedocs.io/en/stable/
 
 
 ## Get Involved:
 
 * We use [GitHub issues](https://github.com/ansible/ansible-builder/issues) to
   track bug reports and feature ideas
 * Want to contribute, check out our [guide](CONTRIBUTING.md)
 * Join us in the `#ansible-builder` channel on Libera.chat IRC
-* Join the discussion in
-  [awx-project](https://groups.google.com/forum/#!forum/awx-project)
 * For the full list of Ansible email Lists, IRC channels and working groups,
   check out the [Ansible Mailing
   lists](https://docs.ansible.com/ansible/latest/community/communication.html#mailing-list-information)
-  page of the official Ansible documentation
+  page of the official Ansible documentation.
 
 ## Code of Conduct
 
 We ask all of our community members and contributors to adhere to the [Ansible
 code of
 conduct](http://docs.ansible.com/ansible/latest/community/code_of_conduct.html). If
 you have questions, or need assistance, please reach out to our community team
 at [codeofconduct@ansible.com](mailto:codeofconduct@ansible.com)
 
 ## License
 
 [Apache License v2.0](./LICENSE.md)
-
-## Project Maintainers:
-
-- Shane McDonald (shanemcd@redhat.com)
-- Alan Rominger (arominge@redhat.com)
-- Bianca Henderson (bianca@redhat.com)
-
```

### Comparing `ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/assemble` & `ansible-builder-3.0.0rc2/src/ansible_builder/_target_scripts/assemble`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 RELEASE=$(source /etc/os-release; echo $ID)
 
 # NOTE(pabelanger): Allow users to force either microdnf or dnf as a package
 # manager.
 PKGMGR="${PKGMGR:-}"
 PKGMGR_OPTS="${PKGMGR_OPTS:-}"
+PKGMGR_PRESERVE_CACHE="${PKGMGR_PRESERVE_CACHE:-}"
 
 PYCMD="${PYCMD:=/usr/bin/python3}"
 PIPCMD="${PIPCMD:=$PYCMD -m pip}"
 
 $PYCMD -m ensurepip
 
 if [ -z $PKGMGR ]; then
@@ -54,16 +55,14 @@
 # of the user first creating them or not.
 mkdir -p /output/bindep
 mkdir -p /output/wheels
 mkdir -p /tmp/src
 
 cd /tmp/src
 
-$PKGMGR upgrade -y
-
 function install_bindep {
     # Protect from the bindep builder image use of the assemble script
     # to produce a wheel.  Note we append because we want all
     # sibling packages in here too
     if [ -f bindep.txt ] ; then
         bindep -l newline | sort >> /output/bindep/run.txt || true
         if [ "$RELEASE" == "centos" ] ; then
@@ -110,23 +109,14 @@
         cp /tmp/src/requirements.txt /output/requirements.txt
     fi
     # If we didn't build wheels, we can skip trying to install it.
     if [ $(ls -1 /output/wheels/*whl 2>/dev/null | wc -l) -gt 0 ]; then
         $PIPCMD uninstall -y /output/wheels/*.whl
         $PIPCMD install $CONSTRAINTS $PIP_OPTS --cache-dir=/output/wheels /output/wheels/*whl
     fi
-
-    # Install each of the extras so that we collect all possibly
-    # needed wheels in the wheel cache. get-extras-packages also
-    # writes out the req files into /output/$extra/requirements.txt.
-
-    # FIXME: this doesn't error out the build when it fails, yay
-    for req in $(/build/get-extras-packages) ; do
-        $PIPCMD install $CONSTRAINTS $PIP_OPTS --cache-dir=/output/wheels "$req"
-    done
 }
 
 PACKAGES=$*
 PIP_OPTS="${PIP_OPTS-}"
 
 # bindep the main package
 install_bindep
@@ -167,12 +157,15 @@
 # go through ZUUL_SIBLINGS, if any, and build those wheels too
 for sibling in ${ZUUL_SIBLINGS:-}; do
     pushd .zuul-siblings/${sibling}
     install_wheels
     popd
 done
 
-$PKGMGR clean all
-rm -rf /var/cache/{dnf,yum}
+if [ -z $PKGMGR_PRESERVE_CACHE ]; then
+  $PKGMGR clean all
+  rm -rf /var/cache/{dnf,yum}
+fi
+
 rm -rf /var/lib/dnf/history.*
 rm -rf /var/log/{dnf.*,hawkey.log}
 rm -rf /tmp/venv
```

### Comparing `ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/check_ansible` & `ansible-builder-3.0.0rc2/src/ansible_builder/_target_scripts/check_ansible`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/check_galaxy` & `ansible-builder-3.0.0rc2/src/ansible_builder/_target_scripts/check_galaxy`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/entrypoint` & `ansible-builder-3.0.0rc2/src/ansible_builder/_target_scripts/entrypoint`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/install-from-bindep` & `ansible-builder-3.0.0rc2/src/ansible_builder/_target_scripts/install-from-bindep`

 * *Files 14% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 # limitations under the License.
 
 set -ex
 # NOTE(pabelanger): Allow users to force either microdnf or dnf as a package
 # manager.
 PKGMGR="${PKGMGR:-}"
 PKGMGR_OPTS="${PKGMGR_OPTS:-}"
+PKGMGR_PRESERVE_CACHE="${PKGMGR_PRESERVE_CACHE:-}"
 
 PYCMD="${PYCMD:=/usr/bin/python3}"
 PIPCMD="${PIPCMD:=$PYCMD -m pip}"
+PIP_OPTS="${PIP_OPTS-}"
 
 $PYCMD -m ensurepip
 
 if [ -z $PKGMGR ]; then
     # Expect dnf to be installed, however if we find microdnf default to it.
     PKGMGR=/usr/bin/dnf
     if [ -f "/usr/bin/microdnf" ]; then
@@ -39,16 +41,14 @@
         # NOTE(pabelanger): skip install docs and weak dependencies to
         # make smaller images. Sadly, setting these in dnf.conf don't
         # appear to work.
         PKGMGR_OPTS="--nodocs --setopt install_weak_deps=0"
     fi
 fi
 
-$PKGMGR upgrade -y $PKGMGR_OPTS
-
 if [ -f /output/bindep/run.txt ] ; then
     PACKAGES=$(cat /output/bindep/run.txt)
     if [ ! -z "$PACKAGES" ]; then
         $PKGMGR install -y $PKGMGR_OPTS $PACKAGES
     fi
 fi
 
@@ -65,40 +65,43 @@
 fi
 
 # If a requirements.txt file exists,
 # install it directly so that people can use git url syntax
 # to do things like pick up patched but unreleased versions
 # of dependencies.
 if [ -f /output/requirements.txt ] ; then
-    $PIPCMD install $CONSTRAINTS --cache-dir=/output/wheels -r /output/requirements.txt
+    $PIPCMD install $CONSTRAINTS $PIP_OPTS --cache-dir=/output/wheels -r /output/requirements.txt
 fi
 
 # Add any requested extras to the list of things to install
 EXTRAS=""
 for extra in $* ; do
     EXTRAS="${EXTRAS} -r /output/$extra/requirements.txt"
 done
 
 if [ -f /output/packages.txt ] ; then
   # If a package list was passed to assemble, install that in the final
   # image.
-  $PIPCMD install $CONSTRAINTS --cache-dir=/output/wheels -r /output/packages.txt $EXTRAS
+  $PIPCMD install $CONSTRAINTS $PIP_OPTS --cache-dir=/output/wheels -r /output/packages.txt $EXTRAS
 else
   # Install the wheels. Uninstall any existing version as siblings maybe
   # be built with the same version number as the latest release, but we
   # really want the speculatively built wheels installed over any
   # automatic dependencies.
   # NOTE(pabelanger): It is possible a project may not have a wheel, but does have requirements.txt
   if [ $(ls -1 /output/wheels/*whl 2>/dev/null | wc -l) -gt 0 ]; then
       $PIPCMD uninstall -y /output/wheels/*.whl
-      $PIPCMD install $CONSTRAINTS --cache-dir=/output/wheels /output/wheels/*.whl $EXTRAS
+      $PIPCMD install $CONSTRAINTS $PIP_OPTS --cache-dir=/output/wheels /output/wheels/*.whl $EXTRAS
   elif [ ! -z "$EXTRAS" ] ; then
       $PIPCMD uninstall -y $EXTRAS
-      $PIPCMD install $CONSTRAINTS --cache-dir=/output/wheels $EXTRAS
+      $PIPCMD install $CONSTRAINTS $PIP_OPTS --cache-dir=/output/wheels $EXTRAS
   fi
 fi
 
-# clean up after ourselves
-$PKGMGR clean all
-rm -rf /var/cache/{dnf,yum}
+# clean up after ourselves, unless requested to keep the cache
+if [[ "$PKGMGR_PRESERVE_CACHE" != always ]]; then
+  $PKGMGR clean all
+  rm -rf /var/cache/{dnf,yum}
+fi
+
 rm -rf /var/lib/dnf/history.*
 rm -rf /var/log/{dnf.*,hawkey.log}
```

### Comparing `ansible-builder-3.0.0rc1/ansible_builder/_target_scripts/introspect.py` & `ansible-builder-3.0.0rc2/src/ansible_builder/_target_scripts/introspect.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import logging
 import os
 import sys
 import yaml
 
 import requirements
-from pkg_resources import safe_name
+import importlib.metadata
 
 base_collections_path = '/usr/share/ansible/collections'
 default_file = 'execution-environment.yml'
 logger = logging.getLogger(__name__)
 
 
 def line_is_empty(line):
@@ -326,15 +326,15 @@
     consolidated = []
     seen_pkgs = set()
 
     for collection, lines in collection_py_reqs.items():
         try:
             for req in requirements.parse('\n'.join(lines)):
                 if req.specifier:
-                    req.name = safe_name(req.name)
+                    req.name = importlib.metadata.Prepared(req.name).normalized
                 req.collections = [collection]  # add backref for later
                 if req.name is None:
                     consolidated.append(req)
                     continue
                 if req.name in seen_pkgs:
                     for prior_req in consolidated:
                         if req.name == prior_req.name:
```

### Comparing `ansible-builder-3.0.0rc1/ansible_builder/cli.py` & `ansible-builder-3.0.0rc2/src/ansible_builder/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import logging
 import sys
 import os
-import pkg_resources
+import importlib.metadata
 
 from . import constants
 
 from .colors import MessageColors
 from .exceptions import DefinitionError
 from .main import AnsibleBuilder
 from .policies import PolicyChoices
@@ -39,15 +39,15 @@
         run_introspect(args, logger)
 
     logger.error("An error has occurred.")
     sys.exit(1)
 
 
 def get_version():
-    return pkg_resources.get_distribution('ansible_builder').version
+    return importlib.metadata.version('ansible_builder')
 
 
 def add_container_options(parser):
     """
     Add sub-commands and options relevant to containers.
     """
     create_command_parser = parser.add_parser(
@@ -119,15 +119,15 @@
         '--container-keyring',
         help='GPG keyring for container image validation.',
     )
 
     build_command_parser.add_argument(
         '--squash',
         choices=['new', 'all', 'off'],
-        default='new',
+        default='off',
         help='Squash layers in the final image (choices: %(choices)s). Defaults to "%(default)s". (podman only)'
     )
 
     for p in [create_command_parser, build_command_parser]:
 
         p.add_argument('-f', '--file',
                        default=constants.default_file,
@@ -198,17 +198,19 @@
         args.tag = [constants.default_tag]
 
     return args
 
 
 class BuildArgAction(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):
-        key, *value = values.split('=')
+        key, sep, value = values.partition("=")
         attr = getattr(namespace, self.dest)
 
         # None signifies that the build-arg will come from the environment.
         # This is currently only supported by Docker. Podman will treat any
         # usage of the $VALUE as a literal string.
         if value:
-            attr[key] = value[0]
+            attr[key] = value
+        elif sep == '=' and value == '':
+            attr[key] = ''
         else:
             attr[key] = None
```

### Comparing `ansible-builder-3.0.0rc1/ansible_builder/constants.py` & `ansible-builder-3.0.0rc2/src/ansible_builder/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,18 +9,21 @@
     'docker': 'Dockerfile'
 }
 default_container_runtime = 'podman'
 base_roles_path = '/usr/share/ansible/roles'
 base_collections_path = '/usr/share/ansible/collections'
 
 build_arg_defaults = dict(
+    # empty string values here still allow the build arg to be emitted into the generated Containerfile
     ANSIBLE_GALAXY_CLI_COLLECTION_OPTS='',
     ANSIBLE_GALAXY_CLI_ROLE_OPTS='',
     EE_BASE_IMAGE='quay.io/ansible/ansible-runner:latest',
-    EE_BUILDER_IMAGE='quay.io/ansible/ansible-builder:latest'
+    # this value is removed elsewhere for v3+ schemas
+    EE_BUILDER_IMAGE='quay.io/ansible/ansible-builder:latest',
+    PKGMGR_PRESERVE_CACHE='',
 )
 
 user_content_subfolder = '_build'
 
 if shutil.which('podman'):
     default_container_runtime = 'podman'
 else:
@@ -36,7 +39,9 @@
     'ansible_core': '',
     'ansible_runner': '',
 
     'galaxy': 'requirements.yml',
     'python': 'requirements.txt',
     'system': 'bindep.txt',
 }
+
+FINAL_IMAGE_BIN_PATH = "/opt/builder/bin"
```

### Comparing `ansible-builder-3.0.0rc1/ansible_builder/containerfile.py` & `ansible-builder-3.0.0rc2/src/ansible_builder/containerfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         ])
 
         self._insert_global_args()
         self._insert_custom_steps('prepend_base')
 
         if not self.definition.builder_image:
             if self.definition.python_package_system:
-                self.steps.append('RUN $PKGMGR install $PYPKG -y && $PKGMGR clean all')
+                self.steps.append('RUN $PKGMGR install $PYPKG -y ; if [ -z $PKGMGR_PRESERVE_CACHE ]; then $PKGMGR clean all; fi')
 
             # We should always make sure pip is available for later stages.
             self.steps.append('RUN $PYCMD -m ensurepip')
 
             if self.definition.ansible_ref_install_list:
                 self.steps.append('RUN $PYCMD -m pip install --no-cache-dir $ANSIBLE_INSTALL_REFS')
 
@@ -119,14 +119,15 @@
             # dynamic builder, create from customized base
             image = "base"
 
         self.steps.extend([
             "",
             "# Builder build stage",
             f"FROM {image} as builder",
+            "WORKDIR /build",
         ])
 
         self._insert_global_args()
 
         if image == "base":
             self.steps.append("RUN $PYCMD -m pip install --no-cache-dir bindep pyyaml requirements-parser")
 
@@ -164,15 +165,21 @@
 
         # install init package if specified
         # FUTURE: could move this into the pre-install wheel phase
         if init_pip_pkg := self.definition.container_init.get('package_pip'):
             self.steps.append(f"RUN $PYCMD -m pip install --no-cache-dir '{init_pip_pkg}'")
 
         self._insert_custom_steps('append_final')
+
+        # Purge the temporary /output directory used in intermediate stages
+        self.steps.append("RUN rm -rf /output")
+
         self._prepare_label_steps()
+        if self.definition.version >= 3 and (uid := self.definition.options['user']):
+            self._prepare_user_steps(uid)
         self._prepare_entrypoint_steps()
 
     def write(self):
         """
         Writes the steps (built via the `Containerfile.prepare()` method) for
         the runtime-specific build file (Dockerfile or Containerfile) to the
         context directory.
@@ -185,33 +192,38 @@
     def _insert_global_args(self, include_values: bool = False):
         """
         Insert Containerfile ARGs and, possibly, their values.
 
         An ARG with a None or empty value will not be included.
         """
 
-        # ARGs will be output in the order listed below.
+        # ARGs will be output in the order listed below. Keys with value `None` will be omitted, but empty string values
+        # will still appear in the output (this allows them to be set at runtime).
         global_args = {
             'EE_BASE_IMAGE': self.definition.build_arg_defaults['EE_BASE_IMAGE'],
+            # this is only applicable for < v3 definitions and will be removed elsewhere for newer schema
             'EE_BUILDER_IMAGE': self.definition.build_arg_defaults['EE_BUILDER_IMAGE'],
             'PYCMD': self.definition.python_path or '/usr/bin/python3',
             'PYPKG': self.definition.python_package_system,
+            'PKGMGR_PRESERVE_CACHE': self.definition.build_arg_defaults['PKGMGR_PRESERVE_CACHE'],
             'ANSIBLE_GALAXY_CLI_COLLECTION_OPTS': self.definition.build_arg_defaults['ANSIBLE_GALAXY_CLI_COLLECTION_OPTS'],
             'ANSIBLE_GALAXY_CLI_ROLE_OPTS': self.definition.build_arg_defaults['ANSIBLE_GALAXY_CLI_ROLE_OPTS'],
             'ANSIBLE_INSTALL_REFS': self.definition.ansible_ref_install_list,
         }
 
         if self.definition.version >= 3:
             global_args['PKGMGR'] = self.definition.options['package_manager_path']
 
         for arg, value in global_args.items():
-            if include_values and value:
+            if value is None:
+                continue  # an optional or N/A `ARG` we don't even want to emit
+            if include_values:  # emit `ARG` directives for empty strings so they can be overridden at build-time
                 # quote the value in case it includes spaces
                 self.steps.append(f'ARG {arg}="{value}"')
-            elif value:
+            else:
                 self.steps.append(f"ARG {arg}")
         self.steps.append("")
 
     def _create_folder_copy_files(self):
         """
         Creates the build context directory, and copies any potential context
         files (python, galaxy, or bindep requirements) into it.
@@ -225,38 +237,46 @@
                 continue
 
             requirement_path = self.definition.get_dep_abs_path(item)
             if requirement_path is None:
                 continue
             dest = os.path.join(
                 self.build_context, constants.user_content_subfolder, new_name)
-            copy_file(requirement_path, dest)
+
+            # Ignore modification time of the requirement file because we could
+            # be writing it out dynamically (inline EE reqs), and we only care
+            # about the contents anyway.
+            copy_file(requirement_path, dest, ignore_mtime=True)
 
         if self.original_galaxy_keyring:
             copy_file(self.original_galaxy_keyring, os.path.join(self.build_outputs_dir, constants.default_keyring_name))
 
         self._handle_additional_build_files()
 
         if self.definition.ansible_config:
             copy_file(
                 self.definition.ansible_config,
                 os.path.join(self.build_outputs_dir, 'ansible.cfg')
             )
 
         # HACK: this sucks
         scriptres = importlib.resources.files('ansible_builder._target_scripts')
-        for script in ('assemble', 'get-extras-packages', 'install-from-bindep', 'introspect.py', 'check_galaxy', 'check_ansible', 'entrypoint'):
+        for script in ('assemble', 'install-from-bindep', 'introspect.py', 'check_galaxy', 'check_ansible', 'entrypoint'):
             with importlib.resources.as_file(scriptres / script) as script_path:
-                # FIXME: just use builtin copy?
                 copy_file(str(script_path), os.path.join(scripts_dir, script))
 
-        # later steps depend on base image containing these scripts
+        # Later intermediate stages depend on base image containing these scripts.
+        # Copy them to a location that we do not need in the final image.
         context_dir = Path(self.build_outputs_dir).stem
         self.steps.append(f'COPY {context_dir}/scripts/ /output/scripts/')
 
+        # The final image will have /output purged, but certain scripts we want
+        # to retain in that image.
+        self.steps.append(f'COPY {context_dir}/scripts/entrypoint {constants.FINAL_IMAGE_BIN_PATH}/entrypoint')
+
     def _handle_additional_build_files(self):
         """
         Deal with any files the user wants added to the image build context.
 
         The 'src' value is either an absolute path, or a path relative to the
         EE definition file. For example, 'src' can be a relative path like
         "data_files/configs/*.cfg", but cannot be "/home/user/files/*.cfg",
@@ -411,7 +431,10 @@
             ])
 
     def _prepare_entrypoint_steps(self):
         if ep := self.definition.container_init.get('entrypoint'):
             self.steps.append(f"ENTRYPOINT {ep}")
         if cmd := self.definition.container_init.get('cmd'):
             self.steps.append(f"CMD {cmd}")
+
+    def _prepare_user_steps(self, uid):
+        self.steps.append(f"USER {uid}")
```

### Comparing `ansible-builder-3.0.0rc1/ansible_builder/ee_schema.py` & `ansible-builder-3.0.0rc2/src/ansible_builder/ee_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+import os
+
 from jsonschema import validate, SchemaError, ValidationError
 
+import ansible_builder.constants as constants
 from ansible_builder.exceptions import DefinitionError
 
 
 TYPE_StringOrListOfStrings = {
     "anyOf": [
         {"type": "string"},
         {
@@ -11,14 +14,26 @@
             "items": {
                 "type": "string"
             }
         }
     ]
 }
 
+TYPE_DictOrStringOrListOfStrings = {
+    "anyOf": [
+        {"type": "object"},
+        {"type": "string"},
+        {
+            "type": "array",
+            "items": {
+                "type": "string"
+            }
+        }
+    ]
+}
 
 ############
 # Version 1
 ############
 
 schema_v1 = {
     "type": "object",
@@ -194,27 +209,27 @@
             "properties": {
                 "ANSIBLE_GALAXY_CLI_COLLECTION_OPTS": {
                     "type": "string",
                 },
                 "ANSIBLE_GALAXY_CLI_ROLE_OPTS": {
                     "type": "string",
                 },
+                "PKGMGR_PRESERVE_CACHE": {
+                    "type": "string",
+                },
             },
         },
 
         "dependencies": {
             "description": "The dependency stuff",
             "type": "object",
             "additionalProperties": False,
             "properties": {
                 "python": TYPE_StringOrListOfStrings,
-                "galaxy": {
-                    "description": "The Galaxy dependency file",
-                    "type": "string",
-                },
+                "galaxy": TYPE_DictOrStringOrListOfStrings,
                 "system": TYPE_StringOrListOfStrings,
                 "python_interpreter": {
                     "description": "Python package name and path",
                     "type": "object",
                     "additionalProperties": False,
                     "properties": {
                         "package_system": {
@@ -330,14 +345,18 @@
                     "description": "Default working directory, also often the homedir for ephemeral UIDs",
                     "type": ["string", "null"],
                 },
                 "package_manager_path": {
                     "description": "Path to the system package manager to use",
                     "type": "string",
                 },
+                "user": {
+                    "description": "Sets the username or UID",
+                    "type": "string",
+                },
                 "container_init": {
                     "description": "Customize container startup behavior",
                     "type": "object",
                     "additionalProperties": False,
                     "properties": {
                         "package_pip": {
                             "description": "package to install via pip for entrypoint support",
@@ -409,16 +428,19 @@
     """
     JSONSchema can document a "default" value, but it isn't used for validation.
     This method is used to set any default values for the "options" dictionary
     properties.
     """
     options = ee_def.setdefault('options', {})
 
+    entrypoint_path = os.path.join(constants.FINAL_IMAGE_BIN_PATH, "entrypoint")
+
     options.setdefault('skip_ansible_check', False)
     options.setdefault('relax_passwd_permissions', True)
     options.setdefault('workdir', '/runner')
     options.setdefault('package_manager_path', '/usr/bin/dnf')
     options.setdefault('container_init', {
         'package_pip': 'dumb-init==1.2.5',
-        'entrypoint': '["/output/scripts/entrypoint", "dumb-init"]',
+        'entrypoint': f'["{entrypoint_path}", "dumb-init"]',
         'cmd': '["bash"]',
     })
+    options.setdefault('user', '1000')
```

### Comparing `ansible-builder-3.0.0rc1/ansible_builder/main.py` & `ansible-builder-3.0.0rc2/src/ansible_builder/main.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/ansible_builder/policies.py` & `ansible-builder-3.0.0rc2/src/ansible_builder/policies.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/ansible_builder/user_definition.py` & `ansible-builder-3.0.0rc2/src/ansible_builder/user_definition.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,16 +165,22 @@
         This method will return the absolute path.
         """
         req_file = self.raw.get('dependencies', {}).get(entry)
 
         if not req_file:
             return None
 
-        # HACK: jamming in prototype support for inline deps listing, tempfile handling is ass
-        if (is_list := isinstance(req_file, list)) or (isinstance(req_file, str) and '\n' in req_file):
+        # dump inline-declared deps to files that will be injected directly into the generated context
+        if isinstance(req_file, dict):
+            tf = tempfile.NamedTemporaryFile('w')
+            tf.write(yaml.safe_dump(req_file))
+            tf.flush()  # don't close, it'll clean up on GC
+            _tempfiles.append(tf)
+            req_file = tf.name
+        elif (is_list := isinstance(req_file, list)) or (isinstance(req_file, str) and '\n' in req_file):
             tf = tempfile.NamedTemporaryFile('w')
             if is_list:
                 tf.write('\n'.join(req_file))
             else:
                 tf.write(req_file)
             _tempfiles.append(tf)
             tf.flush()  # don't close, it'll clean up on GC
```

### Comparing `ansible-builder-3.0.0rc1/ansible_builder/utils.py` & `ansible-builder-3.0.0rc2/src/ansible_builder/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -159,15 +159,33 @@
             # a subdir of our build destination directory
             copy_location.mkdir(exist_ok=True)
             copy_directory(child, copy_location)
         else:
             copy_file(str(child), str(copy_location))
 
 
-def copy_file(source: str, dest: str) -> bool:
+def copy_file(source: str, dest: str, ignore_mtime: bool = False) -> bool:
+    """
+    Used to copy a source file to a destination file in the container runtime
+    context subfolder.
+
+    This utility function helps in maintaining the build cache. We only want
+    to copy the file if it doesn't exist, or if it has changed between builds.
+    See the `copy_directory()` function for the directory copy equivalent.
+
+    :param source str: Path to a source file.
+    :param dest str: Path to a destination file within the context subdir.
+    :param ignore_mtime bool: Whether or not mtime should be considered.
+
+    :returns: True if the file was copied, False if not.
+
+    :raises: Exception if called with the path to a directory. This helps to
+        catch programming errors.
+    """
+
     should_copy = False
 
     if os.path.abspath(source) == os.path.abspath(dest):
         logger.info("File %s was placed in build context by user, leaving unmodified.", dest)
         return False
     if Path(source).is_dir():
         raise Exception(f"Source {source} can not be a directory. Please use copy_directory instead.")
@@ -175,15 +193,15 @@
         raise Exception(f"Destination {dest} can not be a directory. Please use copy_directory instead.")
     if not os.path.exists(dest):
         logger.debug("File %s will be created.", dest)
         should_copy = True
     elif not filecmp.cmp(source, dest, shallow=False):
         logger.warning('File %s had modifications and will be rewritten', dest)
         should_copy = True
-    elif os.path.getmtime(source) > os.path.getmtime(dest):
+    elif not ignore_mtime and os.path.getmtime(source) > os.path.getmtime(dest):
         logger.warning('File %s updated time increased and will be rewritten', dest)
         should_copy = True
 
     if should_copy:
         shutil.copy2(source, dest)
     else:
         logger.debug("File %s is already up-to-date.", dest)
```

### Comparing `ansible-builder-3.0.0rc1/ansible_builder.egg-info/SOURCES.txt` & `ansible-builder-3.0.0rc2/src/ansible_builder.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,40 @@
 .cherry_picker.toml
 .coveragerc
 .dockerignore
+.git_archival.txt
+.gitattributes
+.gitignore
 .readthedocs.yaml
 .yamllint
 CODEOWNERS
 CONTRIBUTING.md
 Containerfile
 LICENSE.md
-MANIFEST.in
 Makefile
 README.md
 SECURITY.md
 TODO.org
 bindep.txt
+pyproject.toml
 pytest.ini
-requirements.txt
 setup.cfg
-setup.py
 tox.ini
 .github/issue_labeler.yml
 .github/patchback.yml
 .github/pr_labeler_existing.yml
 .github/pr_labeler_new.yml
 .github/ISSUE_TEMPLATE/bug_report.yml
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/documentation_report.yml
 .github/ISSUE_TEMPLATE/feature_request.yml
 .github/test-scripts/setup_pulp.sh
 .github/workflows/ci.yml
 .github/workflows/triage_existing.yml
 .github/workflows/triage_new.yml
-ansible_builder/__init__.py
-ansible_builder/__main__.py
-ansible_builder/cli.py
-ansible_builder/colors.py
-ansible_builder/constants.py
-ansible_builder/containerfile.py
-ansible_builder/ee_schema.py
-ansible_builder/exceptions.py
-ansible_builder/main.py
-ansible_builder/policies.py
-ansible_builder/requirements.py
-ansible_builder/user_definition.py
-ansible_builder/utils.py
-ansible_builder.egg-info/PKG-INFO
-ansible_builder.egg-info/SOURCES.txt
-ansible_builder.egg-info/dependency_links.txt
-ansible_builder.egg-info/entry_points.txt
-ansible_builder.egg-info/not-zip-safe
-ansible_builder.egg-info/pbr.json
-ansible_builder.egg-info/requires.txt
-ansible_builder.egg-info/top_level.txt
-ansible_builder/_target_scripts/__init__.py
-ansible_builder/_target_scripts/assemble
-ansible_builder/_target_scripts/check_ansible
-ansible_builder/_target_scripts/check_galaxy
-ansible_builder/_target_scripts/entrypoint
-ansible_builder/_target_scripts/get-extras-packages
-ansible_builder/_target_scripts/install-from-bindep
-ansible_builder/_target_scripts/introspect.py
 demo/execution-environment.yml
 docs/Makefile
 docs/collection_metadata.rst
 docs/conf.py
 docs/definition.rst
 docs/glossary.rst
 docs/index.rst
@@ -73,14 +45,39 @@
 docs/usage.rst
 docs/_static/.gitkeep
 docs/_templates/.gitkeep
 packaging/rpm/Dockerfile.epel-7-x86_64
 packaging/rpm/Dockerfile.epel-8-x86_64
 packaging/rpm/ansible-builder.spec.j2
 packaging/rpm/docker-compose.yml
+src/ansible_builder/__init__.py
+src/ansible_builder/__main__.py
+src/ansible_builder/cli.py
+src/ansible_builder/colors.py
+src/ansible_builder/constants.py
+src/ansible_builder/containerfile.py
+src/ansible_builder/ee_schema.py
+src/ansible_builder/exceptions.py
+src/ansible_builder/main.py
+src/ansible_builder/policies.py
+src/ansible_builder/user_definition.py
+src/ansible_builder/utils.py
+src/ansible_builder.egg-info/PKG-INFO
+src/ansible_builder.egg-info/SOURCES.txt
+src/ansible_builder.egg-info/dependency_links.txt
+src/ansible_builder.egg-info/entry_points.txt
+src/ansible_builder.egg-info/requires.txt
+src/ansible_builder.egg-info/top_level.txt
+src/ansible_builder/_target_scripts/__init__.py
+src/ansible_builder/_target_scripts/assemble
+src/ansible_builder/_target_scripts/check_ansible
+src/ansible_builder/_target_scripts/check_galaxy
+src/ansible_builder/_target_scripts/entrypoint
+src/ansible_builder/_target_scripts/install-from-bindep
+src/ansible_builder/_target_scripts/introspect.py
 test/__init__.py
 test/conftest.py
 test/requirements.txt
 test/data/README.md
 test/data/run.sh
 test/data/ansible.posix.at/execution-environment.yml
 test/data/ansible.posix.at/requirements.yml
@@ -105,24 +102,22 @@
 test/data/build_args/base-image.yml
 test/data/build_args/execution-environment.yml
 test/data/build_fail/execution-environment.yml
 test/data/definition_files/bad.yml
 test/data/definition_files/invalid.yml
 test/data/definition_files/no_galaxy.yml
 test/data/definition_files/no_python.yml
-test/data/needs_git/execution-environment.yml
-test/data/needs_git/requirements.txt
+test/data/minimal_fast/execution-environment.yml
 test/data/nested_galaxy_file/nested-galaxy.yml
 test/data/nested_galaxy_file/foo/requirements.yml
 test/data/pip/execution-environment.yml
 test/data/pip/run.sh
 test/data/pip/env/settings
 test/data/pip/project/pip.yml
 test/data/pip/project/requirements.txt
-test/data/prepend_steps/execution-environment.yml
 test/data/pytz/execution-environment.yml
 test/data/pytz/requirements.yml
 test/data/pytz/env/extravars
 test/data/pytz/env/settings
 test/data/pytz/project/pytz.yml
 test/data/subversion/bindep.txt
 test/data/subversion/execution-environment.yml
```

### Comparing `ansible-builder-3.0.0rc1/docs/Makefile` & `ansible-builder-3.0.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/docs/collection_metadata.rst` & `ansible-builder-3.0.0rc2/docs/collection_metadata.rst`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/docs/conf.py` & `ansible-builder-3.0.0rc2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autosectionlabel',
     "sphinx_ansible_theme",
-    'pbr.sphinxext',
 ]
 
 autosectionlabel_prefix_document = True
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
```

### Comparing `ansible-builder-3.0.0rc1/docs/definition.rst` & `ansible-builder-3.0.0rc2/docs/definition.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Execution Environment Definition
 ================================
 
 The execution environment (EE) definition file supports multiple versions.
 
   * Version 1: Supported by all ``ansible-builder`` versions.
   * Version 2: Supported by ``ansible-builder`` versions ``1.2`` and later.
-  * Version 3: Supported by ``ansible-builder`` versions after ``1.2``.
+  * Version 3: Supported by ``ansible-builder`` versions ``3.0`` and later.
 
 If the EE file does not specify a version, version 1 will be assumed.
 
 .. note::
 
     This version of the documentation discusses only the latest format version.
     For further details on older formats, reference previous versions of the
@@ -181,16 +181,17 @@
             package_pip: ansible-runner
         ansible_runner:
             package_pip: ansible-runner==2.3.2
         ansible_runner:
             package_pip: https://github.com/example_user/ansible-runner/archive/refs/heads/ansible-runner.tar.gz
 
     ``galaxy``
-      Galaxy installation requirements. This may either be a filename, or a string
-      representation of the file contents (see below for an example).
+      Galaxy installation requirements. This may either be a filename, a
+      dictionary, or a multi-line string representation of an Ansible Galaxy
+      ``requirements.yml`` file (see below for examples).
 
     ``python``
       The Python installation requirements. This may either be a filename, or a
       list of requirements (see below for an example).
 
     ``python_interpreter``
       A dictionary that defines the Python system package name to be installed by
@@ -222,32 +223,26 @@
 .. code:: yaml
 
     dependencies:
         python:
           - pywinrm
         system:
           - iputils [platform:rpm]
-        galaxy: |
+        galaxy:
           collections:
             - community.windows
             - ansible.utils
         ansible_core:
             package_pip: ansible-core==2.14.2
         ansible_runner:
             package_pip: ansible-runner==2.3.1
         python_interpreter:
             package_system: "python310"
             python_path: "/usr/bin/python3.10"
 
-.. note::
-
-  The ``|`` symbol is a YAML operator that allows you to define a block of text
-  that may contain newline characters as a literal string. Because the ``galaxy``
-  requirements content is expressed in YAML, we need this value to be a string
-  of YAML so that we can pass it along to ``ansible-galaxy``.
 
 images
 ******
 
 This section is a dictionary that is used to define the base image to be used.
 Verification of signed container images is supported with the ``podman`` container
 runtime. How this data is used in relation to a Podman
@@ -298,15 +293,15 @@
         Literal value for the ``ENTRYPOINT`` Containerfile directive. The
         default entrypoint behavior handles signal propagation to subprocesses, as well as attempting to
         ensure at runtime that the container user has a proper environment with a valid writeable
         home directory, represented in ``/etc/passwd``, with the ``HOME`` envvar set to match. The default
         entrypoint script may emit warnings to ``stderr`` in cases where it is unable to suitably adjust the
         user runtime environment. This behavior can be ignored or elevated to a fatal error; consult the
         source for the ``entrypoint`` target script for more details. The default value is
-        ``["/output/scripts/entrypoint", "dumb-init"]``.
+        ``["/opt/builder/bin/entrypoint", "dumb-init"]``.
 
       ``package_pip``
         Package to install via pip for entrypoint support. This package will be installed in the final build image.
         The default value is ``dumb-init==1.2.5``.
 
     ``package_manager_path``
       A string with the path to the package manager (dnf or microdnf) to use.
@@ -331,27 +326,32 @@
     ``workdir``
       Default current working directory for new processes started under the final container
       image. Some container runtimes also use this value as ``HOME`` for dynamically-created
       users in the ``root`` (GID 0) group. When this value is specified, the directory will be
       created (if it doesn't already exist), set to ``root`` group ownership, and ``rwx`` group
       permissions recursively applied to it. The default value is ``/runner``.
 
+    ``user``
+      This sets the username or UID to use as the default user for the final container image.
+      The default value ``1000``.
+
 
 Example ``options`` section:
 
 .. code:: yaml
 
     options:
         container_init:
             package_pip: dumb-init>=1.2.5
             entrypoint: '["dumb-init"]'
             cmd: '["csh"]'
         package_manager_path: /usr/bin/microdnf
         relax_password_permissions: false
         skip_ansible_check: true
         workdir: /myworkdir
+        user: bob
 
 version
 *******
 
 This is an integer value that sets the version of the format being used. This
 must be ``3`` for the v3 version.
```

### Comparing `ansible-builder-3.0.0rc1/docs/glossary.rst` & `ansible-builder-3.0.0rc2/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/docs/index.rst` & `ansible-builder-3.0.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/docs/installation.rst` & `ansible-builder-3.0.0rc2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/docs/make.bat` & `ansible-builder-3.0.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/docs/usage.rst` & `ansible-builder-3.0.0rc2/docs/usage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,20 @@
 
 By default, the Containerfile / Dockerfile outputted by Ansible Builder contains a build argument ``EE_BASE_IMAGE``, which can be useful for rebuilding Execution Environments without modifying any files.
 
 .. code::
 
    $ ansible-builder build --build-arg FOO=bar
 
+To use different build arguments, you can specify ``--build-arg`` multiple times:
+
+.. code::
+
+   $ ansible-builder build --build-arg FOO=bar --build-arg SIMPLE=sample
+
 To use a custom base image:
 
 .. code::
 
    $ ansible-builder build --build-arg EE_BASE_IMAGE=registry.example.com/another-ee
 
 
@@ -217,18 +223,18 @@
 
 ``--squash``
 ************
 
 This option controls the final image layer squashing. Valid values are:
 
 * ``new``: Squash all of the final image's new layers into a single new layer
-  (preexisting layers are not squashed). This is the default.
+  (preexisting layers are not squashed).
 * ``all``: Squash all of the final image's layers, including those inherited
   from the base image, into a single new layer.
-* ``off``: Turn off layer squashing.
+* ``off``: Turn off layer squashing. This is the default.
 
 .. note::
 
    This flag is compatible only with the ``podman`` runtime and will be ignored
    for any other runtime. Docker is not supported since layer image squashing is
    considered an experimental feature.
 
@@ -245,15 +251,15 @@
 
 
 Examples
 --------
 
 The example in ``test/data/pytz`` requires the ``awx.awx`` collection in
 the execution environment definition. The lookup plugin
-``awx.awx.tower_schedule_rrule`` requires the PyPI ``pytz`` and another
+``awx.awx.schedule_rrule`` requires the PyPI ``pytz`` and another
 library to work. If ``test/data/pytz/execution-environment.yml`` file is
 given to the ``ansible-builder build`` command, then it will install the
 collection inside the image, read ``requirements.txt`` inside of the
 collection, and then install ``pytz`` into the image.
 
 The image produced can be used inside of an ``ansible-runner`` project
 by placing these variables inside the ``env/settings`` file, inside of
@@ -265,15 +271,15 @@
     ---
     container_image: image-name
     process_isolation_executable: podman # or docker
     process_isolation: true
 
 The ``awx.awx`` collection is a subset of content included in the default
 AWX execution environment. More details can be found at the
-`awx-ee <https://github.com/ansible/awx-ee>`__ repository.
+`awx-ee <https://github.com/ansible/awx-ee>`_ repository.
 
 
 Deprecated Features
 -------------------
 
 The ``--base-image`` CLI option has been removed.
 See the ``--build-arg`` option for a replacement.
```

### Comparing `ansible-builder-3.0.0rc1/packaging/rpm/ansible-builder.spec.j2` & `ansible-builder-3.0.0rc2/packaging/rpm/ansible-builder.spec.j2`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/setup.cfg` & `ansible-builder-3.0.0rc2/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 name = ansible-builder
 author = Ansible, Inc.
 author_email = info@ansible.com
 summary = "A tool for building Ansible Execution Environments"
 home_page = https://ansible-builder.readthedocs.io
 description_file = README.md
 description_content_type = text/markdown
-license_file = LICENSE.md
+license_files = 
+	LICENSE.md
 license = Apache Software License, Version 2.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
@@ -25,24 +26,28 @@
 	Topic :: System :: Systems Administration
 	Topic :: Utilities
 
 [flake8]
 ignore = W503
 max-line-length = 160
 
-[entry_points]
+[options]
+include_package_data = true
+install_requires = 
+	PyYAML
+	requirements_parser
+	bindep
+	jsonschema
+python_requires = >=3.9
+
+[options.package_data]
+ansible_builder._target_scripts = 
+	*
+
+[options.entry_points]
 console_scripts = 
 	ansible-builder = ansible_builder.cli:run
 
-[files]
-packages = 
-	ansible_builder
-
-[pbr]
-skip_changelog = yes
-skip_authors = yes
-skip_reno = yes
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ansible-builder-3.0.0rc1/test/conftest.py` & `ansible-builder-3.0.0rc2/test/conftest.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 KEEP_IMAGES = bool(os.environ.get('KEEP_IMAGES', False))
 
 CONTAINER_RUNTIMES = (
     'docker',
     'podman',
 )
 
+FOUND_RUNTIMES = set()
+
+GOOD_CONTENT = {'version': 1}
+
 
 @pytest.fixture(autouse=True)
 def do_not_run_commands(request, mocker):
     if 'run_command' in request.keywords:
         yield
         return
     cmd_mock = mocker.MagicMock(return_value=[1, [
@@ -30,14 +34,29 @@
 
 
 @pytest.fixture(scope='session')
 def data_dir():
     return pathlib.Path(pathlib.Path(__file__).parent).joinpath('data')
 
 
+def pytest_addoption(parser):
+    parser.addoption(
+        '--run-destructive',
+        action='store_true',
+        default=False,
+        help='Run tests that may be destructive to the host'
+    )
+    parser.addoption(
+        '--skip-runtime',
+        choices=CONTAINER_RUNTIMES,
+        action='append',
+        help='Skip tests for a container runtime engine'
+    )
+
+
 @pytest.fixture
 def exec_env_definition_file(tmp_path):
 
     def _write_file(content=None):
         path = tmp_path / 'aee'
         path.mkdir()
         path = path / 'execution-env.yml'
@@ -51,25 +70,22 @@
         path.write_text(write_str)
 
         return path
 
     return _write_file
 
 
-good_content = {'version': 1}
-
-
 @pytest.fixture
 def good_exec_env_definition_path(tmp_path):
     path = tmp_path / 'aee'
     path.mkdir()
     path = path / 'execution-env.yml'
 
     with path.open('w') as outfile:
-        yaml.dump(good_content, outfile)
+        yaml.dump(GOOD_CONTENT, outfile)
 
     return path
 
 
 @pytest.fixture
 def galaxy_requirements_file(tmp_path):
 
@@ -82,48 +98,69 @@
             yaml.dump(content, outfile)
 
         return path
 
     return _write_file
 
 
+# This will be called once for every xdist worker session. For more info, see:
+# https://pytest-xdist.readthedocs.io/en/stable/how-it-works.html#how-it-works
+def pytest_sessionstart(session):
+    """Find the available runtimes only once per test session."""
+    skip_runtimes = session.config.getoption('--skip-runtime') or []
+    for runtime in CONTAINER_RUNTIMES:
+        if shutil.which(runtime) and runtime not in skip_runtimes:
+            FOUND_RUNTIMES.add(runtime)
+
+
+def pytest_collection_modifyitems(session, config, items):
+    # mark destructive items as skipped if `--run-destructive` was not specified
+    if not config.getoption('--run-destructive'):
+        for destructive_item in (i for i in items if any(i.iter_markers(name='destructive'))):
+            destructive_item.add_marker(pytest.mark.skip(reason='test is potentially destructive to the host (add --run-destructive to allow)'))
+
+    # mark serial items as skipped if it looks like we're running with some obvious kinds of parallelism
+    numproc = getattr(config.known_args_namespace, 'numprocesses', None)
+
+    if isinstance(numproc, int) and numproc > 1:
+        for serial_item in (i for i in items if any(i.iter_markers(name='serial'))):
+            serial_item.add_marker(pytest.mark.skip(reason='test requires serial execution (add --numprocesses 0 to allow)'))
+
+
 def pytest_generate_tests(metafunc):
     """If a test uses the custom marker ``test_all_runtimes``, generate marks
     for all supported container runtimes. The requires the test to accept
     and use the ``runtime`` argument.
 
+    This also serves to identify the runtime being tested through the pytest
+    output by appending "[<runtime>]" to the test name.
+
     Based on examples from https://docs.pytest.org/en/latest/example/parametrize.html.
     """
-
     for mark in getattr(metafunc.function, 'pytestmark', []):
         if getattr(mark, 'name', '') == 'test_all_runtimes':
             args = tuple(
                 pytest.param(
                     runtime,
                     marks=pytest.mark.skipif(
-                        shutil.which(runtime) is None,
-                        reason=f'{runtime} is not installed',
-                    ),
-                )
-                for runtime in CONTAINER_RUNTIMES
+                        runtime not in FOUND_RUNTIMES,
+                        reason=f'{runtime} skipped or not found'),
+                ) for runtime in CONTAINER_RUNTIMES
             )
             metafunc.parametrize('runtime', args)
             break
 
 
 @pytest.fixture
 def build_dir_and_ee_yml(tmp_path):
     """Fixture to return temporary file maker."""
-
     def tmp_dir_and_file(ee_contents):
         tmp_file = tmp_path / 'ee.txt'
         tmp_file.write_text(ee_contents)
-
         return tmp_path, tmp_file
-
     return tmp_dir_and_file
 
 
 def run(args, *a, allow_error=False, **kw):
     kw["encoding"] = "utf-8"
     if "check" not in kw:
         # By default we want to fail if a command fails to run. Tests that
@@ -166,15 +203,14 @@
     return '_'.join([
         TAG_PREFIX,
         request.node.name.lower().replace('[', '_').replace(']', '_'),
         str(uuid.uuid4())[:10]
     ])
 
 
-@pytest.mark.test_all_runtimes
 def delete_image(runtime, image_name):
     if KEEP_IMAGES:
         return
     # delete given image, if the test happened to make one
     # allow error in case that image was not created
     regexp = re.compile(r'(no such image)|(image not known)|(image is in use by a container)', re.IGNORECASE)
     r = run(f'{runtime} rmi -f {image_name}', allow_error=True)
@@ -185,23 +221,25 @@
             raise Exception(f'Teardown failed (rc={r.rc}):\n{r.stdout}\n{r.stderr}')
 
 
 @pytest.fixture
 def podman_ee_tag(request):
     image_name = gen_image_name(request)
     yield image_name
-    delete_image('podman', image_name)
+    # FIXME: defer to end?
+    # delete_image('podman', image_name)
 
 
 @pytest.fixture
 @pytest.mark.test_all_runtimes
 def ee_tag(request, runtime):
     image_name = gen_image_name(request)
     yield image_name
-    delete_image(runtime, image_name)
+    # FIXME: defer to end?
+    # delete_image(runtime, image_name)
 
 
 class CompletedProcessProxy(object):
     def __init__(self, result):
         self.result = result
 
     def __getattr__(self, attr):
```

### Comparing `ansible-builder-3.0.0rc1/test/data/README.md` & `ansible-builder-3.0.0rc2/test/data/README.md`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/test/data/ansible.posix.at/project/ansible.posix.at.yml` & `ansible-builder-3.0.0rc2/test/data/ansible.posix.at/project/ansible.posix.at.yml`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/test/data/run.sh` & `ansible-builder-3.0.0rc2/test/data/run.sh`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/test/data/v2/RPM-GPG-KEY-redhat-release` & `ansible-builder-3.0.0rc2/test/data/v2/RPM-GPG-KEY-redhat-release`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/test/data/v3/complete/ee.yml` & `ansible-builder-3.0.0rc2/test/data/v3/complete/ee.yml`

 * *Files 16% similar despite different names*

```diff
@@ -5,25 +5,31 @@
   base_image:
     name: registry.redhat.io/ansible-automation-platform-21/ee-minimal-rhel8:latest
 
 build_arg_defaults:
   ANSIBLE_GALAXY_CLI_COLLECTION_OPTS: '--foo'
   ANSIBLE_GALAXY_CLI_ROLE_OPTS: '--bar'
 
+options:
+  user: '1001'
+
 dependencies:
   ansible_core:
     package_pip: ansible-core==2.13
   ansible_runner:
     package_pip: ansible-runner==2.3.1
   python_interpreter:
     package_system: "mypython3"
     python_path: "/usr/local/bin/mypython"
-  galaxy: |
+  galaxy:
     collections:
       - ansible.utils
+    roles:
+      - blar
+      - blar2
   python:
     - six
     - PyYaml==6.0
   system:
     - python311
     - mysql
```

### Comparing `ansible-builder-3.0.0rc1/test/integration/test_build.py` & `ansible-builder-3.0.0rc2/test/integration/test_build.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,219 +24,206 @@
     assert 'thisisnotacommand: command not found' in (r.stdout + r.stderr), (r.stdout + r.stderr)
 
 
 @pytest.mark.test_all_runtimes
 def test_blank_execution_environment(cli, runtime, ee_tag, tmp_path, data_dir):
     """Just makes sure that the build process does not require any particular input"""
     bc = tmp_path
-    ee_def = data_dir / 'blank' / 'execution-environment.yml'
+    ee_def = data_dir / 'minimal_fast' / 'execution-environment.yml'
     cli(
-        f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
+        f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
     )
     result = cli(f'{runtime} run --rm {ee_tag} echo "This is a simple test"')
     assert 'This is a simple test' in result.stdout, result.stdout
 
 
 @pytest.mark.test_all_runtimes
 def test_multiple_tags(cli, runtime, ee_tag, tmp_path, data_dir):
     """Make sure multiple tagging works"""
     bc = tmp_path
-    ee_def = data_dir / 'blank' / 'execution-environment.yml'
+    ee_def = data_dir / 'minimal_fast' / 'execution-environment.yml'
     cli(
-        f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} -t testmultitags --container-runtime {runtime}'
+        f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} -t testmultitags --container-runtime {runtime}'
     )
     result = cli(f'{runtime} run --rm {ee_tag} echo "test: test_multiple_tags 1"')
     assert 'test: test_multiple_tags 1' in result.stdout, result.stdout
 
     result = cli(f'{runtime} run --rm testmultitags echo "test: test_multiple_tags 2"')
     assert 'test: test_multiple_tags 2' in result.stdout, result.stdout
     delete_image(runtime, 'testmultitags')
 
 
 @pytest.mark.test_all_runtimes
 def test_user_system_requirement(cli, runtime, ee_tag, tmp_path, data_dir):
     bc = tmp_path
     ee_def = data_dir / 'subversion' / 'execution-environment.yml'
-    command = f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
+    command = f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
     cli(command)
     result = cli(
         f'{runtime} run --rm {ee_tag} svn --help'
     )
     assert 'Subversion is a tool for version control' in result.stdout, result.stdout
 
 
 @pytest.mark.test_all_runtimes
 def test_collection_system_requirement(cli, runtime, ee_tag, tmp_path, data_dir):
     bc = tmp_path
     ee_def = data_dir / 'ansible.posix.at' / 'execution-environment.yml'
     cli(
-        f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v3'
+        f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v3'
     )
     result = cli(
         f'{runtime} run --rm {ee_tag} at -V'
     )
     assert 'at version' in result.stderr, result.stderr
 
 
 @pytest.mark.test_all_runtimes
 def test_user_python_requirement(cli, runtime, ee_tag, tmp_path, data_dir):
     bc = tmp_path
     ee_def = data_dir / 'pip' / 'execution-environment.yml'
-    command = f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
+    command = f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
     cli(command)
     result = cli(
-        f'{runtime} run --rm {ee_tag} pip3 show awxkit'
+        f'{runtime} run --rm {ee_tag} /usr/libexec/platform-python -m pip show awxkit'
     )
     assert 'The official command line interface for Ansible AWX' in result.stdout, result.stdout
+
+    # TODO: not sure why we're checking for this be missing...
     for py_library in ('requirements-parser'):
         result = cli(
-            f'{runtime} run --rm {ee_tag} pip3 show {py_library}', allow_error=True
+            f'{runtime} run --rm {ee_tag} /usr/libexec/platform-python -m pip show {py_library}', allow_error=True
         )
         assert result.rc != 0, py_library
 
 
 @pytest.mark.test_all_runtimes
-def test_python_git_requirement(cli, runtime, ee_tag, tmp_path, data_dir):
-    bc = tmp_path
-    ee_def = data_dir / 'needs_git' / 'execution-environment.yml'
-    command = f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
-    cli(command)
-    result = cli(f'{runtime} run --rm {ee_tag} pip3 freeze')
-    assert 'flask' in result.stdout.lower(), result.stdout
-
-
-@pytest.mark.test_all_runtimes
-def test_prepended_steps(cli, runtime, ee_tag, tmp_path, data_dir):
-    """
-    Tests that prepended steps are in final stage
-    """
-    bc = tmp_path
-    ee_def = data_dir / 'prepend_steps' / 'execution-environment.yml'
-    cli(
-        f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime}'
-    )
-
-    _file = 'Dockerfile' if runtime == 'docker' else 'Containerfile'
-    content = open(os.path.join(bc, _file), 'r').read()
-
-    stages_content = content.split('FROM')
-
-    assert 'RUN whoami' in stages_content[-1]
-
-
-@pytest.mark.test_all_runtimes
 def test_build_args_basic(cli, runtime, ee_tag, tmp_path, data_dir):
     bc = tmp_path
     ee_def = data_dir / 'build_args' / 'execution-environment.yml'
     result = cli(
-        f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime} --build-arg FOO=bar -v3'
+        f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime} --build-arg FOO=bar -v3 --no-cache'
     )
     assert 'FOO=bar' in result.stdout
 
 
 @pytest.mark.test_all_runtimes
 def test_build_args_from_environment(cli, runtime, ee_tag, tmp_path, data_dir):
-    if runtime == 'podman':
-        pytest.skip('Skipped. Podman does not support this')
-
     bc = tmp_path
     ee_def = data_dir / 'build_args' / 'execution-environment.yml'
-    os.environ['FOO'] = 'secretsecret'
+    # need a unique value to avoid the cache for this, but don't want the perf hit of --no-cache
+    os.environ['FOO'] = f'secretsecret_{ee_tag}'
     result = cli(
-        f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime} --build-arg FOO -v3'
+        f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime} --build-arg FOO -v3'
     )
-    assert 'secretsecret' in result.stdout
+    assert 'secretsecret_' in result.stdout
 
 
 @pytest.mark.test_all_runtimes
 def test_base_image_build_arg(cli, runtime, ee_tag, tmp_path, data_dir):
     bc = tmp_path
     ee_def = data_dir / 'build_args' / 'base-image.yml'
     os.environ['FOO'] = 'secretsecret'
 
     # Build with custom image tag, then use that as input to --build-arg EE_BASE_IMAGE
-    cli(f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag}-custom --container-runtime {runtime} -v3')
-    cli(f'ansible-builder build --no-cache -c {bc} -f {ee_def} -t {ee_tag}-custom '
-        f'--container-runtime {runtime} --build-arg EE_BASE_IMAGE={ee_tag}-custom -v3')
+    cli(f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v3')
+    cli(f'ansible-builder build -c {bc} -f {ee_def} -t {ee_tag} '
+        f'--container-runtime {runtime} --build-arg EE_BASE_IMAGE={ee_tag} -v3')
 
-    result = cli(f"{runtime} run --rm {ee_tag}-custom cat /base_image")
-    assert f"{ee_tag}-custom" in result.stdout
+    result = cli(f"{runtime} run --rm {ee_tag} cat /base_image")
+    assert f"{ee_tag}" in result.stdout
 
 
 @pytest.mark.test_all_runtimes
-@pytest.mark.xfail(reason='Unreliable on podman')
 def test_has_pytz(cli, runtime, data_dir, ee_tag, tmp_path):
     ee_def = data_dir / 'pytz' / 'execution-environment.yml'
-    cli(f'ansible-builder build --no-cache -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3')
+    cli(f'ansible-builder build -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3')
     result = cli(f'{runtime} run --rm {ee_tag} pip3 show pytz')
 
     assert 'World timezone definitions, modern and historical' in result.stdout
 
 
+@pytest.mark.destructive
 @pytest.mark.test_all_runtimes
-@pytest.mark.xfail(reason='Unreliable on podman')
 def test_build_layer_reuse(cli, runtime, data_dir, ee_tag, tmp_path):
-    ee_def = data_dir / 'pytz' / 'execution-environment.yml'
+    ee_def = data_dir / 'minimal_fast' / 'execution-environment.yml'
 
-    if runtime == 'docker':
-        # Prune the build cache. This command does not exist for podman.
-        cli(f'{runtime} builder prune --force')
+    containerfile_name = 'Dockerfile' if runtime == 'docker' else 'Containerfile'
 
-    cli(f'ansible-builder build -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3')
-    result = cli(f'ansible-builder build -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3')
+    build_cmd = f'ansible-builder build -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3'
+
+    no_cache_result = cli(build_cmd + ' --no-cache')
+
+    pass1_containerfile = (tmp_path / containerfile_name).read_text()
+
+    assert 'hi mom' in no_cache_result.stdout, no_cache_result.stdout
+
+    cache_result = cli(build_cmd)
+    pass2_containerfile = (tmp_path / containerfile_name).read_text()
 
     # Get the range of lines that contain the step we want to ensure used the cached layer
-    out_lines = result.stdout.splitlines()
-    test_index = [idx for idx, value in enumerate(out_lines) if 'RUN /output/install-from-bindep && rm -rf /output/wheels' in value][0]
+    out_lines = cache_result.stdout.splitlines()
+    test_index = [idx for idx, value in enumerate(out_lines) if 'RUN echo "$(echo hi) $(echo mom)"' in value][0]
 
-    assert 'Collecting pytz' not in result.stdout, result.stdout
+    assert pass1_containerfile == pass2_containerfile
+
+    assert 'hi mom' not in cache_result.stdout, cache_result.stdout
     assert any('cache' in line.lower() for line in out_lines[test_index:])
 
 
 @pytest.mark.test_all_runtimes
 def test_collection_verification_off(cli, runtime, data_dir, ee_tag, tmp_path):
     """
     Test that, by default, collection verification is off via the env var.
     """
-    ee_def = data_dir / 'ansible.posix.at' / 'execution-environment.yml'
+    # FIXME: we could still make this even a lot faster with `minimal_fast` plus aliasing `ansible-galaxy` to `/bin/true`
+    ee_def = data_dir / 'pytz' / 'execution-environment.yml'
     result = cli(f'ansible-builder build --no-cache -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3')
     assert "RUN ANSIBLE_GALAXY_DISABLE_GPG_VERIFY=1 ansible-galaxy" in result.stdout
 
 
 @pytest.mark.test_all_runtimes
 def test_collection_verification_on(cli, runtime, data_dir, ee_tag, tmp_path):
     """
     Test that collection verification is on when given a keyring.
     """
     keyring = tmp_path / "mykeyring.gpg"
     keyring.touch()
-    ee_def = data_dir / 'ansible.posix.at' / 'execution-environment.yml'
+
+    # FIXME: we could still make this even a lot faster with `minimal_fast` plus aliasing `ansible-galaxy` to `/bin/true`
+    ee_def = data_dir / 'pytz' / 'execution-environment.yml'
 
     # ansible-galaxy might error (older Ansible), but that should be ok
     result = cli(f'ansible-builder build --no-cache --galaxy-keyring {keyring} -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3',
                  allow_error=True)
 
     keyring_copy = tmp_path / constants.user_content_subfolder / constants.default_keyring_name
     assert keyring_copy.exists()
 
     assert "RUN ANSIBLE_GALAXY_DISABLE_GPG_VERIFY=1 ansible-galaxy" not in result.stdout
     assert f"--keyring \"{constants.default_keyring_name}\"" in result.stdout
 
 
-@pytest.mark.xfail(reason="Needs ansible 2.13")
 @pytest.mark.test_all_runtimes
 def test_galaxy_signing_extra_args(cli, runtime, data_dir, ee_tag, tmp_path):
     """
     Test that all extra signing args for gpg are passed into the container file.
     """
-    pytest.xfail("failing configuration (but should work)")
 
     keyring = tmp_path / "mykeyring.gpg"
     keyring.touch()
-    ee_def = data_dir / 'ansible.posix.at' / 'execution-environment.yml'
+
+    # FIXME: we could still make this even a lot faster with `minimal_fast` plus aliasing `ansible-galaxy` to `/bin/true`
+    ee_def = data_dir / 'pytz' / 'execution-environment.yml'
 
     result = cli(f'ansible-builder build --no-cache -c {tmp_path} -f {ee_def} -t {ee_tag} --container-runtime {runtime} -v 3 '
-                 f'--galaxy-keyring {keyring} --galaxy-ignore-signature-status-code 500 '
+                 f'--galaxy-keyring {keyring} --galaxy-ignore-signature-status-code NODATA '
                  f'--galaxy-required-valid-signature-count 3', allow_error=True)
 
-    assert "--galaxy-ignore-signature-status-code 500" in result.stdout
-    assert "--galaxy-required-valid-signature-count 3" in result.stdout
+    assert "--ignore-signature-status-code NODATA" in result.stdout
+    assert "--required-valid-signature-count 3" in result.stdout
+
+
+@pytest.mark.serial
+def test_placeholder_serial():
+    # easiest way to prevent failures when there are no serial tests
+    pass
```

### Comparing `ansible-builder-3.0.0rc1/test/integration/test_create.py` & `ansible-builder-3.0.0rc2/test/integration/test_create.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 
+import yaml
+
 from ansible_builder import constants
 
 
 def test_definition_syntax_error(cli, data_dir):
     ee_def = os.path.join(data_dir, 'definition_files', 'invalid.yml')
     r = cli(f'ansible-builder create -f {ee_def}', allow_error=True)
     assert r.rc != 0
@@ -50,14 +52,62 @@
     """
     tmpdir, eeyml = build_dir_and_ee_yml("")
     result = cli(f"ansible-builder create -c {tmpdir} -f {eeyml} -v 6", allow_error=True)
     assert result.rc != 0
     assert 'invalid choice: 6 (choose from 0, 1, 2, 3)' in (result.stdout + result.stderr)
 
 
+def test_inline_str_galaxy_requirements(cli, build_dir_and_ee_yml):
+    """
+    Ensure that galaxy requirements specified as an inline multi-line string appear in the generated build context
+    """
+    ee_str = """
+    version: 3
+    dependencies:
+      galaxy: |
+        collections:  # a comment
+        - name: community.general
+        roles:
+        - name: foo.bar  # another comment
+    """
+    tmpdir, eeyml = build_dir_and_ee_yml(ee_str)
+    cli(f'ansible-builder create -c {tmpdir} -f {eeyml} --output-filename Containerfile')
+
+    req_out = tmpdir / '_build/requirements.yml'
+
+    assert req_out.exists()
+    req_out_content = req_out.read_text()
+    assert "# a comment" in req_out_content
+    assert "# another comment" in req_out_content
+    assert yaml.safe_load(req_out_content) == {'collections': [{'name': 'community.general'}], 'roles': [{'name': 'foo.bar'}]}
+
+
+def test_inline_mapping_galaxy_requirements(cli, build_dir_and_ee_yml):
+    """
+    Ensure that galaxy requirements specified as an inline mapping appear in the generated build context
+    """
+    ee_str = """
+    version: 3
+    dependencies:
+      galaxy:
+        collections:
+        - name: community.general
+        roles:
+        - name: foo.bar
+    """
+    tmpdir, eeyml = build_dir_and_ee_yml(ee_str)
+    cli(f'ansible-builder create -c {tmpdir} -f {eeyml} --output-filename Containerfile')
+
+    req_out = tmpdir / '_build/requirements.yml'
+
+    assert req_out.exists()
+    req_out_content = req_out.read_text()
+    assert yaml.safe_load(req_out_content) == {'collections': [{'name': 'community.general'}], 'roles': [{'name': 'foo.bar'}]}
+
+
 def test_collection_verification_off(cli, build_dir_and_ee_yml):
     """
     Test that, by default, collection verification is off via the env var.
     """
     ee = [
         'dependencies:',
         '  galaxy: requirements.yml',
@@ -130,14 +180,38 @@
     assert containerfile.exists()
     text = containerfile.read_text()
 
     assert "--ignore-signature-status-code 500" in text
     assert "--required-valid-signature-count 3" in text
 
 
+def test_v1v2_prepended_steps(cli, build_dir_and_ee_yml):
+    """
+    Tests that prepended steps are in final stage
+    """
+    custom_step_text = 'RUN echo "hi mom from a prepended step"'
+
+    ee = f"""
+        additional_build_steps:
+          prepend: |
+            {custom_step_text}
+    """
+    tmpdir, eeyml = build_dir_and_ee_yml(ee)
+    cli(f'ansible-builder create -c {tmpdir} -f {eeyml} --output-filename Containerfile')
+
+    containerfile = tmpdir / "Containerfile"
+    assert containerfile.exists()
+    text = containerfile.read_text()
+
+    # ensure the custom step text is present and comes before the copy from build stage
+    parts = text.partition(custom_step_text)
+    assert parts[1] == custom_step_text
+    assert "COPY --from=builder" in parts[2]
+
+
 def test_v2_default_images(cli, build_dir_and_ee_yml):
     """
     Test that the base and builder images will use the defaults if not given.
     """
     ee = [
         'version: 2',
     ]
@@ -238,20 +312,24 @@
 
     # verify that the ansible-galaxy command check is performed
     assert 'RUN /output/scripts/check_galaxy' in text
 
     # verify that the ansible/runner check is performed
     assert 'RUN /output/scripts/check_ansible' in text
 
+    # /output should be removed in final image
+    assert 'RUN rm -rf /output' in text
+
     # verify that the default init is being installed and that ENTRYPOINT is set
     assert "RUN $PYCMD -m pip install --no-cache-dir 'dumb-init==" in text
     assert 'WORKDIR /runner' in text
     assert 'RUN chmod ug+rw /etc/passwd' in text
     assert 'RUN mkdir -p /runner' in text
-    assert 'ENTRYPOINT ["/output/scripts/entrypoint", "dumb-init"]' in text
+    assert f'ENTRYPOINT ["{constants.FINAL_IMAGE_BIN_PATH}/entrypoint", "dumb-init"]' in text
+    assert 'USER 1001' in text
 
     # check additional_build_files
     myconfigs_path = tmp_path / constants.user_content_subfolder / "myconfigs"
     assert myconfigs_path.is_dir()
     random_file = myconfigs_path / "random.cfg"
     assert random_file.exists()
 
@@ -388,9 +466,29 @@
     tmpdir, eeyml = build_dir_and_ee_yml(ee)
     cli(f'ansible-builder create -c {tmpdir} -f {eeyml} --output-filename Containerfile')
 
     containerfile = tmpdir / "Containerfile"
     assert containerfile.exists()
     text = containerfile.read_text()
 
-    assert "WORKDIR" not in text
+    assert "WORKDIR" not in text.replace('WORKDIR /build', '')  # intermediate stages set WORKDIR- ignore those
     assert "mkdir -p /runner" not in text
+
+
+def test_v3_set_user_id(cli, build_dir_and_ee_yml):
+    """
+    Test that a custom 'options.user' sets it
+    """
+    tmpdir, eeyml = build_dir_and_ee_yml(
+        """
+        version: 3
+        options:
+          user: bob
+        """
+    )
+    cli(f'ansible-builder create -c {tmpdir} -f {eeyml} --output-filename Containerfile')
+
+    containerfile = tmpdir / "Containerfile"
+    assert containerfile.exists()
+    text = containerfile.read_text()
+
+    assert "USER bob" in text
```

### Comparing `ansible-builder-3.0.0rc1/test/integration/test_help.py` & `ansible-builder-3.0.0rc2/test/integration/test_help.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/test/integration/test_introspect_cli.py` & `ansible-builder-3.0.0rc2/test/integration/test_introspect_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,29 +32,31 @@
     dest_file = tmp_path / 'req.txt'
     cli(f'ansible-builder introspect {data_dir} --write-pip={dest_file}')
 
     assert dest_file.read_text() == '\n'.join([
         'pyvcloud>=14  # from collection test.metadata',
         'pytz  # from collection test.reqfile',
         'python-dateutil>=2.8.2  # from collection test.reqfile',
+        'jinja2>=3.0  # from collection test.reqfile',
         'tacacs_plus  # from collection test.reqfile',
         'pyvcloud>=18.0.10  # from collection test.reqfile',
         '',
     ])
 
 
 def test_introspect_write_python_and_sanitize(cli, data_dir, tmp_path):
     dest_file = tmp_path / 'req.txt'
     cli(f'ansible-builder introspect {data_dir} --write-pip={dest_file} --sanitize')
 
     assert dest_file.read_text() == '\n'.join([
         'pyvcloud>=14,>=18.0.10  # from collection test.metadata,test.reqfile',
         'pytz  # from collection test.reqfile',
-        'python-dateutil>=2.8.2  # from collection test.reqfile',
-        'tacacs-plus  # from collection test.reqfile',
+        'python_dateutil>=2.8.2  # from collection test.reqfile',
+        'jinja2>=3.0  # from collection test.reqfile',
+        'tacacs_plus  # from collection test.reqfile',
         '',
     ])
 
 
 def test_introspect_with_sanitize_user_reqs(cli, data_dir, tmp_path):
     user_file = tmp_path / 'requirements.txt'
     user_file.write_text("ansible\npytest\n")
```

### Comparing `ansible-builder-3.0.0rc1/test/pulp_integration/test_policies.py` & `ansible-builder-3.0.0rc2/test/pulp_integration/test_policies.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,78 +10,53 @@
 
 # All tests in this file require podman to be installed. Skip them all if it isn't.
 pytestmark = pytest.mark.skipif(shutil.which("podman") is None, reason="podman not installed")
 
 RUN_UUID = str(uuid.uuid4())
 USER_POLICY_PATH = '~/.config/containers/policy.json'
 BACKUP_POLICY_PATH = f'~/.config/containers/policy.json.{RUN_UUID}'
-USER_REGISTRIES_PATH = '~/.config/containers/registries.conf'
-BACKUP_REGISTRIES_PATH = f'~/.config/containers/registries.conf.{RUN_UUID}'
 
 
-@pytest.mark.serial
+@pytest.mark.serial  # operations on global shared state in setup (system container policy, image store)
+@pytest.mark.destructive  # messes with the system container policy files and prunes container image store
 class TestPolicies:
     """
     All tests within this class must run serially since they all make use of
     the test user's policy.json file which is acting as our system-level
-    podman policy file. The user's registries.conf is also altered.
+    podman policy file.
     """
 
     @classmethod
     def setup_class(cls):
         """
         These tests will make use of "system" podman files (USER_POLICY_PATH).
         In order to assist developers with local testing, we'll move this file
         out of the way (BACKUP_POLICY_PATH) and restore it during test teardown.
 
-        Our pulp-based test registry does not use secure connections, so we must
-        modify our registries.conf file so that podman commands will not fail.
-        The original registries.conf file should be restored during teardown.
-
         After all tests are done, remove images downloaded from pulp repo and
         dangling (<none>) images.
         """
         user_policy = Path(USER_POLICY_PATH).expanduser()
         if user_policy.exists():
             target = Path(BACKUP_POLICY_PATH).expanduser()
             user_policy.rename(target)
 
-        user_registries = Path(USER_REGISTRIES_PATH).expanduser()
-        if user_registries.exists():
-            target = Path(BACKUP_REGISTRIES_PATH).expanduser()
-            user_registries.rename(target)
-
-        data = '[[registry]]\nlocation="localhost:8080"\ninsecure=true\n'
-        conf = Path(USER_REGISTRIES_PATH).expanduser()
-        conf.parent.mkdir(parents=True, exist_ok=True)
-        conf.write_text(data)
-
-        try:
             cmd = 'podman image prune --force'
             subprocess.run(cmd.split())
-            cmd = 'podman rmi localhost:8080/testrepo/ansible-builder-rhel8:latest'
-            subprocess.run(cmd.split())
-        except Exception:
-            pass
 
     @classmethod
     def teardown_class(cls):
         """
         Restore the user policy.json file.
         """
         renamed_policy = Path(BACKUP_POLICY_PATH).expanduser()
         if renamed_policy.exists():
             target = Path(USER_POLICY_PATH).expanduser()
             renamed_policy.rename(target)
 
-        renamed_registries = Path(BACKUP_REGISTRIES_PATH).expanduser()
-        if renamed_registries.exists():
-            target = Path(USER_REGISTRIES_PATH).expanduser()
-            renamed_registries.rename(target)
-
     def write_policy(self, data):
         policy = Path(USER_POLICY_PATH).expanduser()
         policy.parent.mkdir(parents=True, exist_ok=True)
         policy.write_text(data)
 
     def test_ignore_all(self, cli, tmp_path, data_dir, podman_ee_tag):
         """
```

### Comparing `ansible-builder-3.0.0rc1/test/pulp_integration/test_v3.py` & `ansible-builder-3.0.0rc2/test/pulp_integration/test_v3.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/test/unit/test_cli.py` & `ansible-builder-3.0.0rc2/test/unit/test_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 import pytest
+import runpy
+
 
 from ansible_builder import constants
 from ansible_builder.main import AnsibleBuilder
 from ansible_builder.cli import parse_args
 from ansible_builder.policies import PolicyChoices
 
 
@@ -32,14 +34,44 @@
     content = {'version': 1}
     path = str(exec_env_definition_file(content=content))
 
     aee = prepare(['build', '-f', path, '--build-arg', 'ANSIBLE_GALAXY_CLI_ROLE_OPTS=--ignore-errors', '-c', str(tmp_path)])
     assert aee.build_args == {'ANSIBLE_GALAXY_CLI_ROLE_OPTS': '--ignore-errors'}
 
 
+def test_build_args_empty_value(exec_env_definition_file, tmp_path):
+    content = {'version': 3}
+    path = str(exec_env_definition_file(content=content))
+
+    aee = prepare(['build', '-f', path, '--build-arg', 'ANSIBLE_GALAXY_CLI_ROLE_OPTS=', '-c', str(tmp_path)])
+    assert aee.build_args == {'ANSIBLE_GALAXY_CLI_ROLE_OPTS': ''}
+
+
+def test_build_args_no_trailing_equal(exec_env_definition_file, tmp_path):
+    content = {'version': 3}
+    path = str(exec_env_definition_file(content=content))
+
+    aee = prepare(['build', '-f', path, '--build-arg', 'ANSIBLE_GALAXY_CLI_ROLE_OPTS', '-c', str(tmp_path)])
+    assert aee.build_args == {'ANSIBLE_GALAXY_CLI_ROLE_OPTS': None}
+
+
+def test_build_args_multiple_equal_sign_value(exec_env_definition_file, tmp_path):
+    content = {'version': 3}
+    path = str(exec_env_definition_file(content=content))
+
+    aee = prepare(['build', '-f', path,
+                   '--build-arg', 'ANSIBLE_GALAXY_CLI_ROLE_OPTS=',
+                   '--build-arg', 'PYTHON_CONFIG_SETTINGS=--config-setting=--global-option=--tag-build=SUFFIX',
+                   '-c', str(tmp_path)])
+    assert aee.build_args == {
+        'PYTHON_CONFIG_SETTINGS': '--config-setting=--global-option=--tag-build=SUFFIX',
+        'ANSIBLE_GALAXY_CLI_ROLE_OPTS': ''
+    }
+
+
 def test_build_context(good_exec_env_definition_path, tmp_path):
     path = str(good_exec_env_definition_path)
     build_context = str(tmp_path)
 
     aee = prepare(['build', '-f', path, '-c', build_context])
     assert aee.build_context == build_context
 
@@ -216,61 +248,88 @@
                  ])
 
 
 def test_squash_default(exec_env_definition_file, tmp_path):
     '''
     Test the squash CLI option with default.
     '''
-    content = {'version': 2}
+    content = {'version': 3}
     path = str(exec_env_definition_file(content=content))
     aee = prepare(['build',
                    '-f', path,
                    '-c', str(tmp_path),
                    '--container-runtime', 'podman',
                    ])
-    assert '--squash' in aee.build_command
-    assert '--squash-all' not in aee.build_command
+    assert '--squash' not in aee.build_command
 
 
 def test_squash_all(exec_env_definition_file, tmp_path):
     '''
     Test the squash CLI option with 'all'.
     '''
-    content = {'version': 2}
+    content = {'version': 3}
     path = str(exec_env_definition_file(content=content))
     aee = prepare(['build',
                    '-f', path,
                    '-c', str(tmp_path),
                    '--container-runtime', 'podman',
                    '--squash', 'all'
                    ])
     assert '--squash-all' in aee.build_command
 
 
 def test_squash_off(exec_env_definition_file, tmp_path):
     '''
     Test the squash CLI option with 'off'.
     '''
-    content = {'version': 2}
+    content = {'version': 3}
     path = str(exec_env_definition_file(content=content))
     aee = prepare(['build',
                    '-f', path,
                    '-c', str(tmp_path),
                    '--container-runtime', 'podman',
                    '--squash', 'off'
                    ])
     assert '--squash' not in aee.build_command
 
 
+def test_squash_new(exec_env_definition_file, tmp_path):
+    '''
+    Test the squash CLI option with 'new'.
+    '''
+    content = {'version': 3}
+    path = str(exec_env_definition_file(content=content))
+    aee = prepare(['build',
+                   '-f', path,
+                   '-c', str(tmp_path),
+                   '--container-runtime', 'podman',
+                   '--squash', 'new'
+                   ])
+    assert '--squash' in aee.build_command
+    assert '--squash-all' not in aee.build_command
+
+
 def test_squash_ignored(exec_env_definition_file, tmp_path):
     '''
     Test the squash CLI option is ignored with docker.
     '''
-    content = {'version': 2}
+    content = {'version': 3}
     path = str(exec_env_definition_file(content=content))
     aee = prepare(['build',
                    '-f', path,
                    '-c', str(tmp_path),
                    '--container-runtime', 'docker',
                    '--squash', 'all'
                    ])
     assert '--squash' not in aee.build_command
+
+
+def test_as_executable_module(capsys):
+    """
+    Test __main__ shim as if invoked by `python -m ansible_builder`
+    """
+    with pytest.raises(SystemExit) as sysexit:
+        runpy.run_module('ansible_builder', run_name='__main__', alter_sys=True)
+
+    assert sysexit.value.code == 2  # default rc for "usage"
+    captured = capsys.readouterr()
+    assert "usage" in captured.err
```

### Comparing `ansible-builder-3.0.0rc1/test/unit/test_containerfile.py` & `ansible-builder-3.0.0rc2/test/unit/test_containerfile.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/test/unit/test_introspect.py` & `ansible-builder-3.0.0rc2/test/unit/test_introspect.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import os
 
-from ansible_builder._target_scripts.introspect import process, process_collection, simple_combine
-from ansible_builder.requirements import sanitize_requirements
+from ansible_builder._target_scripts.introspect import process, process_collection, simple_combine, sanitize_requirements
 
 
 def test_multiple_collection_metadata(data_dir):
 
     files = process(data_dir)
     files['python'] = sanitize_requirements(files['python'])
     files['system'] = simple_combine(files['system'])
 
     assert files == {'python': [
         'pyvcloud>=14,>=18.0.10  # from collection test.metadata,test.reqfile',
         'pytz  # from collection test.reqfile',
         # python-dateutil should appear only once even though referenced in
         # multiple places, once with a dash and another with an underscore in the name.
-        'python-dateutil>=2.8.2  # from collection test.reqfile',
-        'tacacs-plus  # from collection test.reqfile'
+        'python_dateutil>=2.8.2  # from collection test.reqfile',
+        # jinja2 should appear only once even though referenced in multiple
+        # places, once with uppercase and another with lowercase in the name.
+        'jinja2>=3.0  # from collection test.reqfile',
+        'tacacs_plus  # from collection test.reqfile'
     ], 'system': [
         'subversion [platform:rpm]  # from collection test.bindep',
         'subversion [platform:dpkg]  # from collection test.bindep'
     ]}
 
 
 def test_single_collection_metadata(data_dir):
```

### Comparing `ansible-builder-3.0.0rc1/test/unit/test_main.py` & `ansible-builder-3.0.0rc2/test/unit/test_main.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/test/unit/test_policies.py` & `ansible-builder-3.0.0rc2/test/unit/test_policies.py`

 * *Files identical despite different names*

### Comparing `ansible-builder-3.0.0rc1/test/unit/test_requirements.py` & `ansible-builder-3.0.0rc2/test/unit/test_requirements.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ansible_builder.requirements import sanitize_requirements
+from ansible_builder._target_scripts.introspect import sanitize_requirements
 
 
 def test_combine_entries():
     assert sanitize_requirements({
         'foo.bar': ['foo>1.0'],
         'bar.foo': ['foo>=2.0']
     }) == ['foo>1.0,>=2.0  # from collection foo.bar,bar.foo']
```

### Comparing `ansible-builder-3.0.0rc1/test/unit/test_user_definition.py` & `ansible-builder-3.0.0rc2/test/unit/test_user_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -211,14 +211,40 @@
         )
         definition = UserDefinition(path)
         definition.validate()
 
         value = definition.raw.get('options', {}).get('skip_ansible_check')
         assert value is False
 
+    def test_v3_user_id(self, exec_env_definition_file):
+        """
+        Test that options.user defaults to 1000
+        """
+        path = exec_env_definition_file(
+            "{'version': 3}"
+        )
+        definition = UserDefinition(path)
+        definition.validate()
+
+        value = definition.raw.get('options', {}).get('user')
+        assert value == '1000'
+
+    def test_v3_set_user_name(self, exec_env_definition_file):
+        """
+        Test that options.user sets to username
+        """
+        path = exec_env_definition_file(
+            "{'version': 3, 'options': {'user': 'bob'}}"
+        )
+        definition = UserDefinition(path)
+        definition.validate()
+
+        value = definition.raw.get('options', {}).get('user')
+        assert value == 'bob'
+
 
 class TestImageDescription:
 
     def test_bad_programmer(self):
         with pytest.raises(ValueError) as error:
             ImageDescription({}, 'invalid_image_key')
         assert "Invalid image key used for initialization: invalid_image_key" in str(error)
```

### Comparing `ansible-builder-3.0.0rc1/test/unit/test_utils.py` & `ansible-builder-3.0.0rc2/test/unit/test_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,23 @@
     new_mtime = stat.st_mtime + 1
     os.utime(source_file, (new_atime, new_mtime))
 
     assert copy_file(source_file, dest_file)
     assert not copy_file(source_file, dest_file)
 
 
+def test_copy_touched_file_ignore_mtime(dest_file, source_file):
+    stat = pathlib.Path(source_file).stat()
+    new_atime = stat.st_atime + 1
+    new_mtime = stat.st_mtime + 1
+    os.utime(source_file, (new_atime, new_mtime))
+
+    assert not copy_file(source_file, dest_file, ignore_mtime=True)
+
+
 def test_copy_file_with_destination_directory(dest_file, source_file):
     # Change source file to trigger copy_file
     source_file.write_text('foo\nbar\nzoo')
 
     with pytest.raises(Exception) as err:
         copy_file(source_file, '/tmp')
     assert "can not be a directory" in str(err.value.args[0])
```

### Comparing `ansible-builder-3.0.0rc1/tox.ini` & `ansible-builder-3.0.0rc2/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 [tox]
 envlist = linters, unit
 isolated_build = True
 
+[shared]
+pytest_cov_args = --cov --cov-report html --cov-report term --cov-report xml
+
 [testenv]
 description = Run all tests with {basepython}
 usedevelop = True
 deps =
     -r {toxinidir}/test/requirements.txt
-commands = pytest {posargs}
+commands = pytest -n auto {posargs}
 
 [testenv:linters{,-py39,-py310,-py311}]
 description = Run code linters
 commands =
     flake8 --version
-    flake8 ansible_builder test
+    flake8 src/ansible_builder test
     yamllint --version
     yamllint -s .
-    mypy ansible_builder
+    mypy src/ansible_builder
 
 [testenv:unit{,-py39,-py310,-py311}]
 description = Run unit tests
-commands = pytest {posargs:test/unit}
+commands = pytest -n auto test/unit {posargs} {[shared]pytest_cov_args}
 
 [testenv:pulp-integration{-py39,-py310,-py311}]
 # Some of these tests must run serially because of a shared resource
 # (the system policy.json file).
 description = Run pulp integration tests
 commands =
-    pytest -n 1 -m "serial" {posargs:test/pulp_integration}
-    pytest -m "not serial" {posargs:test/pulp_integration}
+    pytest -n auto -m "not serial" test/pulp_integration {posargs} {[shared]pytest_cov_args}
+    pytest -n 0 -m "serial" test/pulp_integration {posargs} {[shared]pytest_cov_args}
 
 [testenv:integration{,-py39,-py310,-py311}]
 description = Run integration tests
 # rootless podman reads $HOME
 passenv =
     HOME
     KEEP_IMAGES
-commands = pytest {posargs:test/integration}
+commands =
+    pytest -n auto -m "not serial" test/integration {posargs} {[shared]pytest_cov_args}
+    pytest -n 0 -m "serial" test/integration {posargs} {[shared]pytest_cov_args}
 
 [testenv:docs]
 description = Build documentation
 deps = -r{toxinidir}/docs/requirements.txt
 commands =
     sphinx-build -T -E -W -n --keep-going {tty:--color} -j auto -d docs/build/doctrees -b html docs docs/build/html
```

