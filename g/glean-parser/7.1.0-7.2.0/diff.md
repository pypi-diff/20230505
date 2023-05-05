# Comparing `tmp/glean_parser-7.1.0.tar.gz` & `tmp/glean_parser-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/glean_parser-7.1.0.tar", last modified: Thu Mar  9 16:30:35 2023, max compression
+gzip compressed data, was "dist/glean_parser-7.2.0.tar", last modified: Fri May  5 16:31:00 2023, max compression
```

## Comparing `glean_parser-7.1.0.tar` & `glean_parser-7.2.0.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 16:30:35.000000 glean_parser-7.1.0/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 16:30:35.000000 glean_parser-7.1.0/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6265 2023-03-09 16:30:17.000000 glean_parser-7.1.0/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      292 2023-03-09 16:30:17.000000 glean_parser-7.1.0/.editorconfig
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 16:30:35.000000 glean_parser-7.1.0/.github/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      323 2023-03-09 16:30:17.000000 glean_parser-7.1.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-03-09 16:30:17.000000 glean_parser-7.1.0/.github/dependabot.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2023-03-09 16:30:17.000000 glean_parser-7.1.0/.github/pull_request_template.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-03-09 16:30:17.000000 glean_parser-7.1.0/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      169 2023-03-09 16:30:17.000000 glean_parser-7.1.0/.swiftlint.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-03-09 16:30:17.000000 glean_parser-7.1.0/AUTHORS.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24646 2023-03-09 16:30:17.000000 glean_parser-7.1.0/CHANGELOG.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-03-09 16:30:17.000000 glean_parser-7.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2023-03-09 16:30:17.000000 glean_parser-7.1.0/CONTRIBUTING.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-03-09 16:30:17.000000 glean_parser-7.1.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      350 2023-03-09 16:30:17.000000 glean_parser-7.1.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2448 2023-03-09 16:30:17.000000 glean_parser-7.1.0/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33281 2023-03-09 16:30:35.000000 glean_parser-7.1.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-03-09 16:30:17.000000 glean_parser-7.1.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 16:30:35.000000 glean_parser-7.1.0/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2023-03-09 16:30:17.000000 glean_parser-7.1.0/docs/Makefile
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 16:30:35.000000 glean_parser-7.1.0/docs/_static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   116026 2023-03-09 16:30:17.000000 glean_parser-7.1.0/docs/_static/glean.jpeg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-03-09 16:30:17.000000 glean_parser-7.1.0/docs/authors.md
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4921 2023-03-09 16:30:17.000000 glean_parser-7.1.0/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2023-03-09 16:30:17.000000 glean_parser-7.1.0/docs/contributing.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24646 2023-03-09 16:30:17.000000 glean_parser-7.1.0/docs/history.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-03-09 16:30:17.000000 glean_parser-7.1.0/docs/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      929 2023-03-09 16:30:17.000000 glean_parser-7.1.0/docs/installation.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      774 2023-03-09 16:30:17.000000 glean_parser-7.1.0/docs/make.bat
--rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-03-09 16:30:17.000000 glean_parser-7.1.0/docs/metrics-yaml.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-03-09 16:30:17.000000 glean_parser-7.1.0/docs/pings-yaml.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-03-09 16:30:17.000000 glean_parser-7.1.0/docs/readme.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-03-09 16:30:17.000000 glean_parser-7.1.0/docs/tags-yaml.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 16:30:35.000000 glean_parser-7.1.0/glean_parser/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/__init__.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     8631 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4405 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/coverage.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/data_review.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11230 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/javascript.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12598 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/kotlin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17622 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/lint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9066 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/markdown.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12384 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15309 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2815 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/pings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6744 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/rust.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 16:30:35.000000 glean_parser-7.1.0/glean_parser/schemas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19566 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/schemas/metrics.1-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23843 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/schemas/metrics.2-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4315 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/schemas/pings.1-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4363 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/schemas/pings.2-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1231 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/schemas/tags.1-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8379 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/swift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/tags.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 16:30:35.000000 glean_parser-7.1.0/glean_parser/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3287 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/templates/data_review.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/templates/javascript.buildinfo.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2669 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/templates/javascript.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/templates/kotlin.buildinfo.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/templates/kotlin.geckoview.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5247 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/templates/kotlin.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3425 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/templates/markdown.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/templates/qmldir.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10797 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/templates/rust.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4809 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/templates/swift.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7962 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/translate.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2037 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/translation_options.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16825 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2118 2023-03-09 16:30:17.000000 glean_parser-7.1.0/glean_parser/validate_ping.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 16:30:35.000000 glean_parser-7.1.0/glean_parser.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33281 2023-03-09 16:30:35.000000 glean_parser-7.1.0/glean_parser.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3062 2023-03-09 16:30:35.000000 glean_parser-7.1.0/glean_parser.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-09 16:30:35.000000 glean_parser-7.1.0/glean_parser.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-03-09 16:30:35.000000 glean_parser-7.1.0/glean_parser.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-09 16:30:35.000000 glean_parser-7.1.0/glean_parser.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      169 2023-03-09 16:30:35.000000 glean_parser-7.1.0/glean_parser.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-03-09 16:30:35.000000 glean_parser-7.1.0/glean_parser.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-03-09 16:30:17.000000 glean_parser-7.1.0/pytest.ini
--rw-r--r--   0 circleci  (1001) circleci  (1002)      479 2023-03-09 16:30:17.000000 glean_parser-7.1.0/requirements_dev.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      155 2023-03-09 16:30:35.000000 glean_parser-7.1.0/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2310 2023-03-09 16:30:17.000000 glean_parser-7.1.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 16:30:35.000000 glean_parser-7.1.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 16:30:35.000000 glean_parser-7.1.0/tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1997 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/all_metrics.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/all_pings.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      885 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/bad_ping.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9453 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/core.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/duplicate_labeled.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/duplicate_send_in_ping.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      104 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/empty.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      755 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/event_key_ordering.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/events_with_types.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3539 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/gecko.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/invalid-ping-names.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/invalid.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      481 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/jwe.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      714 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/metric-with-tags.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      768 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/mixed-expirations.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      672 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/old_event_api.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/ordering.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1451 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/pings.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1799 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/rate.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2540 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/schema-violation.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      548 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/send_if_empty_with_metrics.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/single_labeled.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/smaller.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/tags.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/telemetry_mirror.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      973 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/text.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1377 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/text_invalid.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1535 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/wrong_key.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/data/yaml_nits.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/detekt.yml
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     7083 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13895 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/test_javascript.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14509 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/test_kotlin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13716 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/test_lint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7306 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/test_markdown.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5919 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/test_metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32037 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/test_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/test_pings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8037 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/test_rust.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10767 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/test_swift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1467 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/test_tags.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7318 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/test_translate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1108 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/test_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1295 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/test_validate_ping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1571 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tests/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-09 16:30:35.000000 glean_parser-7.1.0/tools/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4713 2023-03-09 16:30:17.000000 glean_parser-7.1.0/tools/extract_data_categories.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:31:00.000000 glean_parser-7.2.0/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:31:00.000000 glean_parser-7.2.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6784 2023-05-05 16:30:44.000000 glean_parser-7.2.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      292 2023-05-05 16:30:44.000000 glean_parser-7.2.0/.editorconfig
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:31:00.000000 glean_parser-7.2.0/.github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      323 2023-05-05 16:30:44.000000 glean_parser-7.2.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-05-05 16:30:44.000000 glean_parser-7.2.0/.github/dependabot.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2023-05-05 16:30:44.000000 glean_parser-7.2.0/.github/pull_request_template.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-05-05 16:30:44.000000 glean_parser-7.2.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      169 2023-05-05 16:30:44.000000 glean_parser-7.2.0/.swiftlint.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-05-05 16:30:44.000000 glean_parser-7.2.0/AUTHORS.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24746 2023-05-05 16:30:44.000000 glean_parser-7.2.0/CHANGELOG.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-05-05 16:30:44.000000 glean_parser-7.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2023-05-05 16:30:44.000000 glean_parser-7.2.0/CONTRIBUTING.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-05-05 16:30:44.000000 glean_parser-7.2.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      350 2023-05-05 16:30:44.000000 glean_parser-7.2.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2448 2023-05-05 16:30:44.000000 glean_parser-7.2.0/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33413 2023-05-05 16:31:00.000000 glean_parser-7.2.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-05-05 16:30:44.000000 glean_parser-7.2.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:31:00.000000 glean_parser-7.2.0/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2023-05-05 16:30:44.000000 glean_parser-7.2.0/docs/Makefile
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:31:00.000000 glean_parser-7.2.0/docs/_static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   116026 2023-05-05 16:30:44.000000 glean_parser-7.2.0/docs/_static/glean.jpeg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-05-05 16:30:44.000000 glean_parser-7.2.0/docs/authors.md
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4921 2023-05-05 16:30:44.000000 glean_parser-7.2.0/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2023-05-05 16:30:44.000000 glean_parser-7.2.0/docs/contributing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24746 2023-05-05 16:30:44.000000 glean_parser-7.2.0/docs/history.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-05-05 16:30:44.000000 glean_parser-7.2.0/docs/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      929 2023-05-05 16:30:44.000000 glean_parser-7.2.0/docs/installation.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      774 2023-05-05 16:30:44.000000 glean_parser-7.2.0/docs/make.bat
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-05-05 16:30:44.000000 glean_parser-7.2.0/docs/metrics-yaml.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-05-05 16:30:44.000000 glean_parser-7.2.0/docs/pings-yaml.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-05-05 16:30:44.000000 glean_parser-7.2.0/docs/readme.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-05-05 16:30:44.000000 glean_parser-7.2.0/docs/tags-yaml.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:31:00.000000 glean_parser-7.2.0/glean_parser/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/__init__.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     8631 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4405 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/coverage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/data_review.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11230 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/javascript.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12598 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/kotlin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16121 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/lint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9066 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/markdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12384 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15309 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2815 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/pings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6744 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/rust.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:31:00.000000 glean_parser-7.2.0/glean_parser/schemas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19566 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/schemas/metrics.1-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23843 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/schemas/metrics.2-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4315 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/schemas/pings.1-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4363 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/schemas/pings.2-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1231 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/schemas/tags.1-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8379 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/swift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/tags.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:31:00.000000 glean_parser-7.2.0/glean_parser/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3287 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/templates/data_review.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/templates/javascript.buildinfo.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2669 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/templates/javascript.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/templates/kotlin.buildinfo.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/templates/kotlin.geckoview.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5247 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/templates/kotlin.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3425 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/templates/markdown.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/templates/qmldir.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10797 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/templates/rust.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4809 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/templates/swift.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7962 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/translate.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2037 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/translation_options.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16825 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2118 2023-05-05 16:30:44.000000 glean_parser-7.2.0/glean_parser/validate_ping.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:31:00.000000 glean_parser-7.2.0/glean_parser.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33413 2023-05-05 16:31:00.000000 glean_parser-7.2.0/glean_parser.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3062 2023-05-05 16:31:00.000000 glean_parser-7.2.0/glean_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-05 16:31:00.000000 glean_parser-7.2.0/glean_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       69 2023-05-05 16:31:00.000000 glean_parser-7.2.0/glean_parser.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-05 16:31:00.000000 glean_parser-7.2.0/glean_parser.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      152 2023-05-05 16:31:00.000000 glean_parser-7.2.0/glean_parser.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-05 16:31:00.000000 glean_parser-7.2.0/glean_parser.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-05-05 16:30:44.000000 glean_parser-7.2.0/pytest.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      479 2023-05-05 16:30:44.000000 glean_parser-7.2.0/requirements_dev.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      155 2023-05-05 16:31:00.000000 glean_parser-7.2.0/setup.cfg
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2286 2023-05-05 16:30:44.000000 glean_parser-7.2.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:31:00.000000 glean_parser-7.2.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:31:00.000000 glean_parser-7.2.0/tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1997 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/all_metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/all_pings.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      885 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/bad_ping.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9453 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/core.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/duplicate_labeled.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/duplicate_send_in_ping.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      104 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/empty.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      755 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/event_key_ordering.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/events_with_types.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3539 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/gecko.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/invalid-ping-names.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/invalid.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      481 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/jwe.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      714 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/metric-with-tags.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      768 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/mixed-expirations.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      672 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/old_event_api.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/ordering.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1451 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/pings.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1799 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/rate.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2540 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/schema-violation.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      548 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/send_if_empty_with_metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/single_labeled.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/smaller.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/tags.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/telemetry_mirror.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      973 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/text.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1377 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/text_invalid.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1535 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/wrong_key.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/data/yaml_nits.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/detekt.yml
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     7083 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13895 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/test_javascript.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14509 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/test_kotlin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13113 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/test_lint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7306 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/test_markdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5919 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/test_metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32037 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/test_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/test_pings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8037 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/test_rust.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10767 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/test_swift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1467 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/test_tags.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7318 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/test_translate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1108 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1295 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/test_validate_ping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1571 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tests/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:31:00.000000 glean_parser-7.2.0/tools/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4713 2023-05-05 16:30:44.000000 glean_parser-7.2.0/tools/extract_data_categories.py
```

### Comparing `glean_parser-7.1.0/.circleci/config.yml` & `glean_parser-7.2.0/.circleci/config.yml`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,25 @@
           # being available to pip on all of the platforms we need to
           # support, so we need to make sure the dependencies are all
           # pure Python or provide pre-built wheels.
           command: CC=broken_compiler pip install . --user
       - run:
           name: lint
           command: make lint
+  license-check:
+    steps:
+      - run:
+          name: install
+          command: |
+            pip install --user pip-licenses
+            CC=broken_compiler pip install . --user
+      - run:
+          name: license-check
+          command: |
+            pip-licenses --fail-on 'GNU General Public License v3 (GPLv3)'
 
 jobs:
   build-36:
     docker:
       - image: cimg/python:3.6
     steps:
       - test-start
@@ -143,14 +154,21 @@
   lint:
     docker:
       - image: cimg/python:3.9
     steps:
       - test-start
       - lint
 
+  license-check:
+    docker:
+      - image: cimg/python:3.9
+    steps:
+      - test-start
+      - license-check
+
   docs-deploy:
     docker:
       - image: node:8.10.0
     steps:
       - checkout
       - add_ssh_keys:
           fingerprints:
@@ -196,14 +214,18 @@
   version: 2
   build:
     jobs:
       - lint:
           filters:
             tags:
               only: /.*/
+      - license-check:
+          filters:
+            tags:
+              only: /.*/
       - build-36:
           filters:
             tags:
               only: /.*/
       - build-36-min:
           filters:
             tags:
```

### Comparing `glean_parser-7.1.0/.github/pull_request_template.md` & `glean_parser-7.2.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/.gitignore` & `glean_parser-7.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/CHANGELOG.md` & `glean_parser-7.2.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 ## Unreleased
 
+## 7.2.0
+
+- Remove yamllint integration ([#578](https://github.com/mozilla/glean_parser/pull/578))
+
 ## 7.1.0
 
 - ENHANCEMENT: Labels in `labels:` fields may now contain any printable ASCII characters ([bug 1672273](https://bugzilla.mozilla.org/show_bug.cgi?id=1672273))
 - BUGFIX: Enforce ordering of generation of Pings, Metrics and Tags such that order is deterministic ([bug 1820334](https://bugzilla.mozilla.org/show_bug.cgi?id=1820334))
 
 ## 7.0.0
```

### Comparing `glean_parser-7.1.0/CODE_OF_CONDUCT.md` & `glean_parser-7.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/CONTRIBUTING.md` & `glean_parser-7.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/LICENSE` & `glean_parser-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/Makefile` & `glean_parser-7.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/PKG-INFO` & `glean_parser-7.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean_parser
-Version: 7.1.0
+Version: 7.2.0
 Summary: Parser tools for Mozilla's Glean telemetry
 Home-page: https://github.com/mozilla/glean_parser
 Author: The Glean Team
 Author-email: glean-team@mozilla.com
 License: UNKNOWN
 Description: # Glean Parser
         
@@ -60,14 +60,18 @@
         ```
         
         
         # Changelog
         
         ## Unreleased
         
+        ## 7.2.0
+        
+        - Remove yamllint integration ([#578](https://github.com/mozilla/glean_parser/pull/578))
+        
         ## 7.1.0
         
         - ENHANCEMENT: Labels in `labels:` fields may now contain any printable ASCII characters ([bug 1672273](https://bugzilla.mozilla.org/show_bug.cgi?id=1672273))
         - BUGFIX: Enforce ordering of generation of Pings, Metrics and Tags such that order is deterministic ([bug 1820334](https://bugzilla.mozilla.org/show_bug.cgi?id=1820334))
         
         ## 7.0.0
```

### Comparing `glean_parser-7.1.0/README.md` & `glean_parser-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/docs/Makefile` & `glean_parser-7.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/docs/_static/glean.jpeg` & `glean_parser-7.2.0/docs/_static/glean.jpeg`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/docs/conf.py` & `glean_parser-7.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/docs/contributing.md` & `glean_parser-7.2.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/docs/history.md` & `glean_parser-7.2.0/docs/history.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 ## Unreleased
 
+## 7.2.0
+
+- Remove yamllint integration ([#578](https://github.com/mozilla/glean_parser/pull/578))
+
 ## 7.1.0
 
 - ENHANCEMENT: Labels in `labels:` fields may now contain any printable ASCII characters ([bug 1672273](https://bugzilla.mozilla.org/show_bug.cgi?id=1672273))
 - BUGFIX: Enforce ordering of generation of Pings, Metrics and Tags such that order is deterministic ([bug 1820334](https://bugzilla.mozilla.org/show_bug.cgi?id=1820334))
 
 ## 7.0.0
```

### Comparing `glean_parser-7.1.0/docs/installation.md` & `glean_parser-7.2.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/docs/make.bat` & `glean_parser-7.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/docs/readme.md` & `glean_parser-7.2.0/docs/readme.md`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/__init__.py` & `glean_parser-7.2.0/glean_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/__main__.py` & `glean_parser-7.2.0/glean_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/coverage.py` & `glean_parser-7.2.0/glean_parser/coverage.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/data_review.py` & `glean_parser-7.2.0/glean_parser/data_review.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/javascript.py` & `glean_parser-7.2.0/glean_parser/javascript.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/kotlin.py` & `glean_parser-7.2.0/glean_parser/kotlin.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/lint.py` & `glean_parser-7.2.0/glean_parser/lint.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,14 @@
 from . import metrics
 from . import parser
 from . import pings
 from . import tags
 from . import util
 
 
-from yamllint.config import YamlLintConfig  # type: ignore
-from yamllint import linter  # type: ignore
-
-
 LintGenerator = Generator[str, None, None]
 
 
 class CheckType(enum.Enum):
     warning = 0
     error = 1
 
@@ -495,55 +491,14 @@
             "top-level to affect the entire file.",
             file=file,
         )
 
     return nits
 
 
-def lint_yaml_files(
-    input_filepaths: Iterable[Path],
-    file=sys.stderr,
-    parser_config: Optional[Dict[str, Any]] = None,
-) -> List:
-    """
-    Performs glinter YAML lint on a set of files.
-
-    :param input_filepaths: List of input files to lint.
-    :param file: The stream to write errors to.
-    :returns: List of nits.
-    """
-
-    if parser_config is None:
-        parser_config = {}
-
-    # Generic type since the actual type comes from yamllint, which we don't
-    # control.
-    nits: List = []
-    for path in input_filepaths:
-        if not path.is_file() and parser_config.get("allow_missing_files", False):
-            continue
-
-        # yamllint needs both the file content and the path.
-        file_content = None
-        with path.open("r", encoding="utf-8") as fd:
-            file_content = fd.read()
-
-        problems = linter.run(file_content, YamlLintConfig("extends: default"), path)
-        nits.extend((path, p) for p in problems)
-
-    if len(nits):
-        print("Sorry, Glean found some glinter nits:", file=file)
-        for path, p in nits:
-            print(f"{path} ({p.line}:{p.column}) - {p.message}", file=file)
-        print("", file=file)
-        print("Please fix the above nits to continue.", file=file)
-
-    return [x[1] for x in nits]
-
-
 def glinter(
     input_filepaths: Iterable[Path],
     parser_config: Optional[Dict[str, Any]] = None,
     file=sys.stderr,
 ) -> int:
     """
     Commandline helper for glinter.
@@ -555,17 +510,14 @@
     :return: Non-zero if there were any glinter errors.
     """
     if parser_config is None:
         parser_config = {}
 
     errors = 0
 
-    nits = lint_yaml_files(input_filepaths, file=file, parser_config=parser_config)
-    errors += len(nits)
-
     objs = parser.parse_objects(input_filepaths, parser_config)
     errors += util.report_validation_errors(objs)
 
     nits = lint_metrics(objs.value, parser_config=parser_config, file=file)
     errors += len([nit for nit in nits if nit.check_type == CheckType.error])
 
     if errors == 0:
```

### Comparing `glean_parser-7.1.0/glean_parser/markdown.py` & `glean_parser-7.2.0/glean_parser/markdown.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/metrics.py` & `glean_parser-7.2.0/glean_parser/metrics.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/parser.py` & `glean_parser-7.2.0/glean_parser/parser.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/pings.py` & `glean_parser-7.2.0/glean_parser/pings.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/rust.py` & `glean_parser-7.2.0/glean_parser/rust.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/schemas/metrics.1-0-0.schema.yaml` & `glean_parser-7.2.0/glean_parser/schemas/metrics.1-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/schemas/metrics.2-0-0.schema.yaml` & `glean_parser-7.2.0/glean_parser/schemas/metrics.2-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/schemas/pings.1-0-0.schema.yaml` & `glean_parser-7.2.0/glean_parser/schemas/pings.1-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/schemas/pings.2-0-0.schema.yaml` & `glean_parser-7.2.0/glean_parser/schemas/pings.2-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/schemas/tags.1-0-0.schema.yaml` & `glean_parser-7.2.0/glean_parser/schemas/tags.1-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/swift.py` & `glean_parser-7.2.0/glean_parser/swift.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/tags.py` & `glean_parser-7.2.0/glean_parser/tags.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/templates/data_review.jinja2` & `glean_parser-7.2.0/glean_parser/templates/data_review.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/templates/javascript.jinja2` & `glean_parser-7.2.0/glean_parser/templates/javascript.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/templates/kotlin.buildinfo.jinja2` & `glean_parser-7.2.0/glean_parser/templates/kotlin.buildinfo.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/templates/kotlin.geckoview.jinja2` & `glean_parser-7.2.0/glean_parser/templates/kotlin.geckoview.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/templates/kotlin.jinja2` & `glean_parser-7.2.0/glean_parser/templates/kotlin.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/templates/markdown.jinja2` & `glean_parser-7.2.0/glean_parser/templates/markdown.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/templates/rust.jinja2` & `glean_parser-7.2.0/glean_parser/templates/rust.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/templates/swift.jinja2` & `glean_parser-7.2.0/glean_parser/templates/swift.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/translate.py` & `glean_parser-7.2.0/glean_parser/translate.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/translation_options.py` & `glean_parser-7.2.0/glean_parser/translation_options.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/util.py` & `glean_parser-7.2.0/glean_parser/util.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser/validate_ping.py` & `glean_parser-7.2.0/glean_parser/validate_ping.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/glean_parser.egg-info/PKG-INFO` & `glean_parser-7.2.0/glean_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glean-parser
-Version: 7.1.0
+Version: 7.2.0
 Summary: Parser tools for Mozilla's Glean telemetry
 Home-page: https://github.com/mozilla/glean_parser
 Author: The Glean Team
 Author-email: glean-team@mozilla.com
 License: UNKNOWN
 Description: # Glean Parser
         
@@ -60,14 +60,18 @@
         ```
         
         
         # Changelog
         
         ## Unreleased
         
+        ## 7.2.0
+        
+        - Remove yamllint integration ([#578](https://github.com/mozilla/glean_parser/pull/578))
+        
         ## 7.1.0
         
         - ENHANCEMENT: Labels in `labels:` fields may now contain any printable ASCII characters ([bug 1672273](https://bugzilla.mozilla.org/show_bug.cgi?id=1672273))
         - BUGFIX: Enforce ordering of generation of Pings, Metrics and Tags such that order is deterministic ([bug 1820334](https://bugzilla.mozilla.org/show_bug.cgi?id=1820334))
         
         ## 7.0.0
```

### Comparing `glean_parser-7.1.0/glean_parser.egg-info/SOURCES.txt` & `glean_parser-7.2.0/glean_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/setup.py` & `glean_parser-7.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     "Click>=7",
     "diskcache>=4",
     "iso8601>=0.1.10; python_version<='3.6'",
     "Jinja2>=2.10.1",
     "MarkupSafe>=1.1.1,<=2.0.1",
     "jsonschema>=3.0.2",
     "PyYAML>=5.3.1",
-    "yamllint>=1.18.0",
 ]
 
 setup_requirements = [
     "pytest-runner",
     "setuptools-scm<7; python_version<='3.6'",
     "setuptools-scm>=7; python_version>'3.6'",
 ]
```

### Comparing `glean_parser-7.1.0/tests/data/all_metrics.yaml` & `glean_parser-7.2.0/tests/data/all_metrics.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/all_pings.yaml` & `glean_parser-7.2.0/tests/data/all_pings.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/bad_ping.yamlx` & `glean_parser-7.2.0/tests/data/bad_ping.yamlx`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/core.yaml` & `glean_parser-7.2.0/tests/data/core.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/duplicate_labeled.yaml` & `glean_parser-7.2.0/tests/data/duplicate_labeled.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/duplicate_send_in_ping.yaml` & `glean_parser-7.2.0/tests/data/duplicate_send_in_ping.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/event_key_ordering.yaml` & `glean_parser-7.2.0/tests/data/event_key_ordering.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/events_with_types.yaml` & `glean_parser-7.2.0/tests/data/events_with_types.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/gecko.yaml` & `glean_parser-7.2.0/tests/data/gecko.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/invalid-ping-names.yaml` & `glean_parser-7.2.0/tests/data/invalid-ping-names.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/metric-with-tags.yaml` & `glean_parser-7.2.0/tests/data/metric-with-tags.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/mixed-expirations.yaml` & `glean_parser-7.2.0/tests/data/mixed-expirations.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/old_event_api.yamlx` & `glean_parser-7.2.0/tests/data/old_event_api.yamlx`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/ordering.yaml` & `glean_parser-7.2.0/tests/data/ordering.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/pings.yaml` & `glean_parser-7.2.0/tests/data/pings.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/rate.yaml` & `glean_parser-7.2.0/tests/data/rate.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/schema-violation.yaml` & `glean_parser-7.2.0/tests/data/schema-violation.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/send_if_empty_with_metrics.yaml` & `glean_parser-7.2.0/tests/data/send_if_empty_with_metrics.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/smaller.yaml` & `glean_parser-7.2.0/tests/data/smaller.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/telemetry_mirror.yaml` & `glean_parser-7.2.0/tests/data/telemetry_mirror.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/text.yaml` & `glean_parser-7.2.0/tests/data/text.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/text_invalid.yaml` & `glean_parser-7.2.0/tests/data/text_invalid.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/wrong_key.yamlx` & `glean_parser-7.2.0/tests/data/wrong_key.yamlx`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/data/yaml_nits.yamlx` & `glean_parser-7.2.0/tests/data/yaml_nits.yamlx`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Any copyright is dedicated to the Public Domain.
 # https://creativecommons.org/publicdomain/zero/1.0/
 
 ---
 $schema: moz://mozilla.org/schemas/glean/metrics/2-0-0
 
 page.perf:
-  load_time:
+  load_time:   
    type: timing_distribution
-    gecko_datapoint: GV_PAGE_LOAD_MS   
+    gecko_datapoint: GV_PAGE_LOAD_MS
     time_unit: millisecond
     lifetime: application
     description: >
       A sample timing distribution metric exported from Gecko.
     bugs:
       - 1566356
     data_reviews:
```

### Comparing `glean_parser-7.1.0/tests/test_cli.py` & `glean_parser-7.2.0/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         __main__.main,
         [
             "glinter",
             str(ROOT / "data" / "bad_ping.yamlx"),
         ],
     )
     assert result.exit_code == 1
-    assert "Found 2 errors" in result.output
+    assert "Found 1 errors" in result.output
 
 
 def test_translate_invalid_format(tmpdir):
     """Test passing an invalid format to the 'translate' command."""
     runner = CliRunner()
     result = runner.invoke(
         __main__.main,
```

### Comparing `glean_parser-7.1.0/tests/test_javascript.py` & `glean_parser-7.2.0/tests/test_javascript.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/test_kotlin.py` & `glean_parser-7.2.0/tests/test_kotlin.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/test_lint.py` & `glean_parser-7.2.0/tests/test_lint.py`

 * *Files 6% similar despite different names*

```diff
@@ -194,33 +194,14 @@
 
     nits = lint.lint_metrics(all_metrics.value)
 
     assert len(nits) == 2
     assert set(["MISSPELLED_PING"]) == set(v.check_name for v in nits)
 
 
-def test_yaml_lint(capsys):
-    """Tests yamllint on files with nits."""
-    file_paths = [ROOT / "data" / "core.yaml", ROOT / "data" / "yaml_nits.yamlx"]
-
-    nits = lint.lint_yaml_files(file_paths)
-
-    assert len(nits) == 3
-    # The second rule is empty because it's a syntax error.
-    assert set(["indentation", None, "trailing-spaces"]) == set(v.rule for v in nits)
-
-    captured = capsys.readouterr()
-    lines = captured.out.split("\n")
-    for line in lines:
-        if line.strip() == "":
-            continue
-        assert "yaml_nits.yamlx" in line
-        assert "core.yaml" not in line
-
-
 def test_user_lifetime_expiration():
     """Test that expiring 'user' lifetime metrics generate a warning."""
     contents = [
         {
             "user_data": {
                 "counter": {
                     "type": "counter",
```

### Comparing `glean_parser-7.1.0/tests/test_markdown.py` & `glean_parser-7.2.0/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/test_metrics.py` & `glean_parser-7.2.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/test_parser.py` & `glean_parser-7.2.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/test_pings.py` & `glean_parser-7.2.0/tests/test_pings.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/test_rust.py` & `glean_parser-7.2.0/tests/test_rust.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/test_swift.py` & `glean_parser-7.2.0/tests/test_swift.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/test_tags.py` & `glean_parser-7.2.0/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/test_translate.py` & `glean_parser-7.2.0/tests/test_translate.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/test_utils.py` & `glean_parser-7.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/test_validate_ping.py` & `glean_parser-7.2.0/tests/test_validate_ping.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tests/util.py` & `glean_parser-7.2.0/tests/util.py`

 * *Files identical despite different names*

### Comparing `glean_parser-7.1.0/tools/extract_data_categories.py` & `glean_parser-7.2.0/tools/extract_data_categories.py`

 * *Files identical despite different names*

