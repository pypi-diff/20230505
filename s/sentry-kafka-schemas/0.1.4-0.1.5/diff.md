# Comparing `tmp/sentry-kafka-schemas-0.1.4.tar.gz` & `tmp/sentry-kafka-schemas-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-kafka-schemas-0.1.4.tar", last modified: Wed May  3 20:28:04 2023, max compression
+gzip compressed data, was "sentry-kafka-schemas-0.1.5.tar", last modified: Fri May  5 18:39:29 2023, max compression
```

## Comparing `sentry-kafka-schemas-0.1.4.tar` & `sentry-kafka-schemas-0.1.5.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.330815 sentry-kafka-schemas-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-03 20:28:04.330815 sentry-kafka-schemas-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.318815 sentry-kafka-schemas-0.1.4/python/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.318815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.318815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/codecs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/codecs/msgpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.318815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.314815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.322815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/end-delete-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/end-delete-tag.json
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/end-merge.json
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/end-unmerge-hierarchical.json
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/end-unmerge-with-transaction.json
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/end-unmerge.json
--rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)    61706 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/errors1.json
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/exclude-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/null-values.json
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/replace-group.json
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/start-delete-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/start-merge.json
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/tombstone-events-no-datetime.json
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/tombstone-events-timestamp.json
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/tombstone-events.json
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.314815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/ingest-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.322815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/ingest-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-counter.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-distribution.json
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-set.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.314815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/ingest-replay-recordings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.322815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording-chunk.msgpack
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording.msgpack
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.314815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/outcomes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.326815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/outcomes/1/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-discarded-hash.json
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-lb.json
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-null-values.json
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-pop-us.json
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-relay-internal.json
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/outcomes/1/outcomes2-missing-key-id.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.314815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/snuba-generic-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.326815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.318815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/snuba-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.326815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/snuba-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/snuba-metrics/1/snuba-metrics1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.318815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/snuba-queries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.326815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/snuba-queries/1/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.318815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/subscription-results/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.326815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/subscription-results/1/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.318815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.326815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/transactions/1/
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.326815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:02.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-03 20:28:02.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    68329 2023-05-03 20:28:01.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/events_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-03 20:28:00.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-03 20:28:01.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-03 20:28:02.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-03 20:27:59.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/outcomes_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-03 20:28:01.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-03 20:28:02.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-03 20:28:00.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-03 20:28:00.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-03 20:28:00.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    29430 2023-05-03 20:27:59.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/transactions_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.330815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    90391 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/events.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    36710 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/sentry_kafka_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.330815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/topics/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/topics/events-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/topics/events.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/topics/generic-metrics-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/topics/ingest-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/topics/ingest-replay-recordings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/topics/metrics-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/topics/outcomes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/topics/sessions-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/topics/snuba-generic-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/topics/snuba-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/topics/snuba-queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/topics/transactions-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/topics/transactions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.318815 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-03 20:28:04.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-03 20:28:04.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:28:04.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:28:04.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 20:28:04.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-03 20:28:04.000000 sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:28:04.330815 sentry-kafka-schemas-0.1.4/python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/tests/test_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/tests/test_codeowner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/tests/test_sentry_kafka_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/tests/test_valid_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/python/tests/test_valid_topic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:28:04.330815 sentry-kafka-schemas-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-03 20:27:51.000000 sentry-kafka-schemas-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.856763 sentry-kafka-schemas-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-05 18:39:29.856763 sentry-kafka-schemas-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.844762 sentry-kafka-schemas-0.1.5/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.844762 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.844762 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/codecs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/codecs/msgpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.844762 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.840762 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.848763 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/end-delete-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/end-delete-tag.json
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/end-merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/end-unmerge-hierarchical.json
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/end-unmerge-with-transaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/end-unmerge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61706 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/errors1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/exclude-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/null-values.json
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/replace-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/start-delete-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/start-merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/tombstone-events-no-datetime.json
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/tombstone-events-timestamp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/tombstone-events.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.840762 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/ingest-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.848763 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/ingest-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-counter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-set.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.840762 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/ingest-replay-recordings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.848763 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording-chunk.msgpack
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording.msgpack
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.840762 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/outcomes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.848763 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/outcomes/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-discarded-hash.json
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-lb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-null-values.json
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-pop-us.json
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-relay-internal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/outcomes/1/outcomes2-missing-key-id.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.840762 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/snuba-generic-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.852763 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.840762 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/snuba-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.852763 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/snuba-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/snuba-metrics/1/snuba-metrics1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.840762 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/snuba-queries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.852763 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/snuba-queries/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.840762 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/subscription-results/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.852763 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/subscription-results/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.844762 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.852763 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/transactions/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.852763 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:27.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-05 18:39:27.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67413 2023-05-05 18:39:26.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/events_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-05 18:39:25.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-05 18:39:27.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-05 18:39:27.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-05 18:39:25.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/outcomes_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-05 18:39:26.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-05 18:39:27.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-05 18:39:26.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-05 18:39:26.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-05 18:39:25.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30767 2023-05-05 18:39:25.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/transactions_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.852763 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    89070 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/events.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38314 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/sentry_kafka_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.856763 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/topics/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/topics/events-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/topics/events.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/topics/generic-metrics-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/topics/ingest-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/topics/ingest-replay-recordings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/topics/metrics-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/topics/outcomes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/topics/sessions-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/topics/snuba-generic-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/topics/snuba-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/topics/snuba-queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/topics/transactions-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/topics/transactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.844762 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-05 18:39:29.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-05 18:39:29.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:39:29.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:39:29.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 18:39:29.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 18:39:29.000000 sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:29.856763 sentry-kafka-schemas-0.1.5/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/tests/test_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/tests/test_codeowner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/tests/test_sentry_kafka_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/tests/test_valid_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/python/tests/test_valid_topic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 18:39:29.856763 sentry-kafka-schemas-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-05 18:39:16.000000 sentry-kafka-schemas-0.1.5/setup.py
```

### Comparing `sentry-kafka-schemas-0.1.4/LICENSE` & `sentry-kafka-schemas-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/README.md` & `sentry-kafka-schemas-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/codecs/__init__.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/codecs/json.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/codecs/json.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/codecs/msgpack.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/codecs/msgpack.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/errors1.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/errors1.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/null-values.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/null-values.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Literal, Dict, List, TypedDict
+from typing import Any, TypedDict, List, Literal, Dict
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/events_v1.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/events_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, TypedDict, Tuple, Any, Literal, Union
+from typing import List, Tuple, Union, Dict, TypedDict, Literal, Any
 from typing_extensions import Required
 
 
 ClientSdkInfo = Union["_ClientSdkInfoAnyof0"]
 """
 client_sdk_info.
 
@@ -98,15 +98,15 @@
     """Required property"""
 
     datetime: Required[str]
     """Required property"""
 
 
 
-EventStreamMessage = Union[Tuple[Literal[2], Literal["insert"], "InsertEvent", "_Base"], Tuple[Literal[2], Literal["start_delete_groups"], "_BaseGen777752"], Tuple[Literal[2], Literal["start_merge"], "StartMergeMessageBody"], Tuple[Literal[2], Literal["start_unmerge"], Dict[str, Any]], Tuple[Literal[2], Literal["start_unmerge_hierarchical"], Dict[str, Any]], Tuple[Literal[2], Literal["start_delete_tag"], Dict[str, Any]], Tuple[Literal[2], Literal["end_delete_groups"], "EndDeleteGroupsMessageBody"], Tuple[Literal[2], Literal["end_merge"], "EndMergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge"], "EndUnmergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge_hierarchical"], "EndUnmergeHierarchicalMessageBody"], Tuple[Literal[2], Literal["end_delete_tag"], "EndDeleteTagMessageBody"], Tuple[Literal[2], Literal["tombstone_events"], "TombstoneEventsMessageBody"], Tuple[Literal[2], Literal["replace_group"], "ReplaceGroupMessageBody"], Tuple[Literal[2], Literal["exclude_groups"], "ExcludeGroupsMessageBody"]]
+EventStreamMessage = Union[Tuple[Literal[2], Literal["insert"], "InsertEvent", "_Base"], Tuple[Literal[2], Literal["start_delete_groups"], "_BaseGen40717"], Tuple[Literal[2], Literal["start_merge"], "StartMergeMessageBody"], Tuple[Literal[2], Literal["start_unmerge"], Dict[str, Any]], Tuple[Literal[2], Literal["start_unmerge_hierarchical"], Dict[str, Any]], Tuple[Literal[2], Literal["start_delete_tag"], Dict[str, Any]], Tuple[Literal[2], Literal["end_delete_groups"], "EndDeleteGroupsMessageBody"], Tuple[Literal[2], Literal["end_merge"], "EndMergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge"], "EndUnmergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge_hierarchical"], "EndUnmergeHierarchicalMessageBody"], Tuple[Literal[2], Literal["end_delete_tag"], "EndDeleteTagMessageBody"], Tuple[Literal[2], Literal["tombstone_events"], "TombstoneEventsMessageBody"], Tuple[Literal[2], Literal["replace_group"], "ReplaceGroupMessageBody"], Tuple[Literal[2], Literal["exclude_groups"], "ExcludeGroupsMessageBody"]]
 """
 event_stream_message.
 
 The snuba eventstream message.
 """
 
 
@@ -582,15 +582,15 @@
 
 
 _BaseAnyof0 = Union[str]
 """ A "into-string" type that normalizes header names."""
 
 
 
-class _BaseGen777752(TypedDict, total=False):
+class _BaseGen40717(TypedDict, total=False):
     transaction_id: str
     project_id: Required[int]
     """Required property"""
 
     group_ids: Required[List[int]]
     """Required property"""
 
@@ -629,52 +629,28 @@
 
      Official Sentry SDKs use the entity `sentry`, as in `sentry.python` or
      `sentry.javascript.react-native`. Please use a different entity for your own SDKs.
 
     Required property
     """
 
-    packages: Union[List[Union["_ClientSdkInfoAnyof0PackagesArrayItemAnyof0", None]], None]
-    """
-     List of installed and loaded SDK packages. _Optional._
-
-     A list of packages that were installed as part of this SDK or the activated integrations.
-     Each package consists of a name in the format `source:identifier` and `version`. If the
-     source is a Git repository, the `source` should be `git`, the identifier should be a
-     checkout link and the version should be a Git reference (branch, tag or SHA).
-    """
-
     version: Required[Union[str, None]]
     """
      The version of the SDK. _Required._
 
      It should have the [Semantic Versioning](https://semver.org/) format `MAJOR.MINOR.PATCH`,
      without any prefix (no `v` or anything else in front of the major version number).
 
      Examples: `0.1.0`, `1.0.0`, `4.3.12`
 
     Required property
     """
 
 
 
-_ClientSdkInfoAnyof0PackagesArrayItemAnyof0 = Union["_ClientSdkInfoAnyof0PackagesArrayItemAnyof0Anyof0"]
-""" An installed and loaded package as part of the Sentry SDK."""
-
-
-
-class _ClientSdkInfoAnyof0PackagesArrayItemAnyof0Anyof0(TypedDict, total=False):
-    name: Union[str, None]
-    """ Name of the package."""
-
-    version: Union[str, None]
-    """ Version of the package."""
-
-
-
 _SentryEventContextsAnyof0 = Union[Dict[str, Union["_SentryEventContextsAnyof0Anyof0AdditionalpropertiesAnyof0", None]]]
 """
  The Contexts Interface provides additional context data. Typically, this is data related to the
  current user and the environment. For example, the device or application version. Its canonical
  name is `contexts`.
 
  The `contexts` type can be used to define arbitrary contextual data on the event. It accepts an
```

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypedDict, List, Dict, Literal, Any
+from typing import Literal, Any, TypedDict, Dict, List
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypedDict, Union, List, Dict, Literal
+from typing import TypedDict, Union, List, Literal, Dict
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
 """counter_metric_value."""
```

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal, TypedDict, Any, List, Dict
+from typing import Dict, Any, Literal, TypedDict, List
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypedDict, Any, Dict, Literal, List
+from typing import Dict, Any, TypedDict, Literal, List
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal, List, TypedDict, Any, Dict, Union
+from typing import Literal, Any, Dict, List, TypedDict, Union
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
 """counter_metric_value."""
```

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Any, Dict, Literal, List, TypedDict
+from typing import Any, Union, List, TypedDict, Literal, Dict
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
 """counter_metric_value."""
```

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Dict, TypedDict, Union
+from typing import TypedDict, List, Dict, Any, Union
 from typing_extensions import Required
 
 
 class ClickhouseQueryProfile(TypedDict, total=False):
     """clickhouse_query_profile."""
 
     time_range: Required[Union[int, None]]
```

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, TypedDict, Any, Dict, Literal
+from typing import List, Literal, Any, TypedDict, Dict
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schema_types/transactions_v1.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schema_types/transactions_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,20 @@
-from typing import Dict, Literal, Any, TypedDict, List, Union, Tuple
+from typing import Literal, List, TypedDict, Tuple, Union, Dict, Any
 from typing_extensions import Required
 
 
+ClientSdkInfo = Union["_ClientSdkInfoAnyof0"]
+"""
+client_sdk_info.
+
+ The SDK Interface describes the Sentry SDK and its configuration used to capture and transmit an event.
+"""
+
+
+
 class TransactionEvent(TypedDict, total=False):
     """transaction_event."""
 
     group_id: None
     group_ids: List[int]
     event_id: str
     organization_id: int
@@ -29,14 +38,53 @@
 
 
 _BaseAnyof0 = Union[str]
 """ A "into-string" type that normalizes header names."""
 
 
 
+class _ClientSdkInfoAnyof0(TypedDict, total=False):
+    integrations: Union[List[Union[str, None]], None]
+    """
+     List of integrations that are enabled in the SDK. _Optional._
+
+     The list should have all enabled integrations, including default integrations. Default
+     integrations are included because different SDK releases may contain different default
+     integrations.
+    """
+
+    name: Required[Union[str, None]]
+    """
+     Unique SDK name. _Required._
+
+     The name of the SDK. The format is `entity.ecosystem[.flavor]` where entity identifies the
+     developer of the SDK, ecosystem refers to the programming language or platform where the
+     SDK is to be used and the optional flavor is used to identify standalone SDKs that are part
+     of a major ecosystem.
+
+     Official Sentry SDKs use the entity `sentry`, as in `sentry.python` or
+     `sentry.javascript.react-native`. Please use a different entity for your own SDKs.
+
+    Required property
+    """
+
+    version: Required[Union[str, None]]
+    """
+     The version of the SDK. _Required._
+
+     It should have the [Semantic Versioning](https://semver.org/) format `MAJOR.MINOR.PATCH`,
+     without any prefix (no `v` or anything else in front of the major version number).
+
+     Examples: `0.1.0`, `1.0.0`, `4.3.12`
+
+    Required property
+    """
+
+
+
 class _TransactionEventData(TypedDict, total=False):
     type: Required[str]
     """Required property"""
 
     transaction: Union[str, None]
     """
      Transaction name of the event.
@@ -71,15 +119,15 @@
     """
 
     contexts: Required["_TransactionEventDataContexts"]
     """Required property"""
 
     tags: List[List[Union[None, str]]]
     extra: "_TransactionEventDataExtra"
-    sdk: "_TransactionEventDataSdk"
+    sdk: "ClientSdkInfo"
     project: int
     spans: Required[List["_TransactionEventDataSpansItem"]]
     """Required property"""
 
     measurements: "_TransactionEventDataMeasurements"
     breakdowns: "_TransactionEventDataBreakdowns"
     culprit: str
@@ -829,23 +877,14 @@
     """Required property"""
 
     unit: Required[str]
     """Required property"""
 
 
 
-class _TransactionEventDataSdk(TypedDict, total=False):
-    name: Required[str]
-    """Required property"""
-
-    version: Required[str]
-    """Required property"""
-
-
-
 class _TransactionEventDataSpansItem(TypedDict, total=False):
     timestamp: Required[Union[int, float]]
     """Required property"""
 
     start_timestamp: Required[Union[int, float]]
     """Required property"""
```

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/events.v1.schema.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/events.v1.schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986265696347033%*

 * *Differences: {"'definitions'": "{'ClientSdkInfo': {'anyOf': {0: {'properties': {delete: ['packages']}}}}, "*

 * *                  "delete: ['ClientSdkPackage']}"}*

```diff
@@ -169,31 +169,14 @@
                         "name": {
                             "description": " Unique SDK name. _Required._\n\n The name of the SDK. The format is `entity.ecosystem[.flavor]` where entity identifies the\n developer of the SDK, ecosystem refers to the programming language or platform where the\n SDK is to be used and the optional flavor is used to identify standalone SDKs that are part\n of a major ecosystem.\n\n Official Sentry SDKs use the entity `sentry`, as in `sentry.python` or\n `sentry.javascript.react-native`. Please use a different entity for your own SDKs.",
                             "type": [
                                 "string",
                                 "null"
                             ]
                         },
-                        "packages": {
-                            "description": " List of installed and loaded SDK packages. _Optional._\n\n A list of packages that were installed as part of this SDK or the activated integrations.\n Each package consists of a name in the format `source:identifier` and `version`. If the\n source is a Git repository, the `source` should be `git`, the identifier should be a\n checkout link and the version should be a Git reference (branch, tag or SHA).",
-                            "items": {
-                                "anyOf": [
-                                    {
-                                        "$ref": "#/definitions/ClientSdkPackage"
-                                    },
-                                    {
-                                        "type": "null"
-                                    }
-                                ]
-                            },
-                            "type": [
-                                "array",
-                                "null"
-                            ]
-                        },
                         "version": {
                             "description": " The version of the SDK. _Required._\n\n It should have the [Semantic Versioning](https://semver.org/) format `MAJOR.MINOR.PATCH`,\n without any prefix (no `v` or anything else in front of the major version number).\n\n Examples: `0.1.0`, `1.0.0`, `4.3.12`",
                             "type": [
                                 "string",
                                 "null"
                             ]
                         }
@@ -204,39 +187,14 @@
                     ],
                     "type": "object"
                 }
             ],
             "description": " The SDK Interface describes the Sentry SDK and its configuration used to capture and transmit an event.",
             "title": "client_sdk_info"
         },
-        "ClientSdkPackage": {
-            "anyOf": [
-                {
-                    "additionalProperties": true,
-                    "properties": {
-                        "name": {
-                            "description": " Name of the package.",
-                            "type": [
-                                "string",
-                                "null"
-                            ]
-                        },
-                        "version": {
-                            "description": " Version of the package.",
-                            "type": [
-                                "string",
-                                "null"
-                            ]
-                        }
-                    },
-                    "type": "object"
-                }
-            ],
-            "description": " An installed and loaded package as part of the Sentry SDK."
-        },
         "CloudResourceContext": {
             "anyOf": [
                 {
                     "additionalProperties": true,
                     "properties": {
                         "cloud.account.id": {
                             "description": " The cloud account ID the resource is assigned to.",
```

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9926440354102167%*

 * *Differences: {"'definitions'": "{'Data': {'properties': {'sdk': {'$ref': '#/definitions/ClientSdkInfo'}}}, "*

 * *                  "'ClientSdkInfo': OrderedDict([('title', 'client_sdk_info'), ('description', ' "*

 * *                  'The SDK Interface describes the Sentry SDK and its configuration used to '*

 * *                  "capture and transmit an event.'), ('anyOf', [OrderedDict([('type', 'object'), "*

 * *                  "('required', ['name', 'version']), ('properties', OrderedDict([('integrations', "*

 * *                  "Orde […]*

```diff
@@ -112,14 +112,57 @@
                         }
                     },
                     "type": "object"
                 }
             ],
             "description": " Web browser information."
         },
+        "ClientSdkInfo": {
+            "anyOf": [
+                {
+                    "additionalProperties": true,
+                    "properties": {
+                        "integrations": {
+                            "description": " List of integrations that are enabled in the SDK. _Optional._\n\n The list should have all enabled integrations, including default integrations. Default\n integrations are included because different SDK releases may contain different default\n integrations.",
+                            "items": {
+                                "type": [
+                                    "string",
+                                    "null"
+                                ]
+                            },
+                            "type": [
+                                "array",
+                                "null"
+                            ]
+                        },
+                        "name": {
+                            "description": " Unique SDK name. _Required._\n\n The name of the SDK. The format is `entity.ecosystem[.flavor]` where entity identifies the\n developer of the SDK, ecosystem refers to the programming language or platform where the\n SDK is to be used and the optional flavor is used to identify standalone SDKs that are part\n of a major ecosystem.\n\n Official Sentry SDKs use the entity `sentry`, as in `sentry.python` or\n `sentry.javascript.react-native`. Please use a different entity for your own SDKs.",
+                            "type": [
+                                "string",
+                                "null"
+                            ]
+                        },
+                        "version": {
+                            "description": " The version of the SDK. _Required._\n\n It should have the [Semantic Versioning](https://semver.org/) format `MAJOR.MINOR.PATCH`,\n without any prefix (no `v` or anything else in front of the major version number).\n\n Examples: `0.1.0`, `1.0.0`, `4.3.12`",
+                            "type": [
+                                "string",
+                                "null"
+                            ]
+                        }
+                    },
+                    "required": [
+                        "name",
+                        "version"
+                    ],
+                    "type": "object"
+                }
+            ],
+            "description": " The SDK Interface describes the Sentry SDK and its configuration used to capture and transmit an event.",
+            "title": "client_sdk_info"
+        },
         "CloudResourceContext": {
             "anyOf": [
                 {
                     "additionalProperties": true,
                     "properties": {
                         "cloud.account.id": {
                             "description": " The cloud account ID the resource is assigned to.",
@@ -320,15 +363,15 @@
                     "description": " The release version of the application.\n\n **Release versions must be unique across all projects in your organization.** This value\n can be the git SHA for the given project, or a product identifier with a semantic version.",
                     "type": [
                         "string",
                         "null"
                     ]
                 },
                 "sdk": {
-                    "$ref": "#/definitions/SDK"
+                    "$ref": "#/definitions/ClientSdkInfo"
                 },
                 "spans": {
                     "items": {
                         "$ref": "#/definitions/Span"
                     },
                     "type": "array"
                 },
@@ -1099,29 +1142,14 @@
                         }
                     },
                     "type": "object"
                 }
             ],
             "description": " Runtime information.\n\n Runtime context describes a runtime in more detail. Typically, this context is present in\n `contexts` multiple times if multiple runtimes are involved (for instance, if you have a\n JavaScript application running on top of JVM)."
         },
-        "SDK": {
-            "properties": {
-                "name": {
-                    "type": "string"
-                },
-                "version": {
-                    "type": "string"
-                }
-            },
-            "required": [
-                "name",
-                "version"
-            ],
-            "type": "object"
-        },
         "Span": {
             "properties": {
                 "data": {
                     "type": [
                         "object",
                         "null"
                     ]
```

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/sentry_kafka_schemas.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/sentry_kafka_schemas.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas/types.py` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas/types.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/sentry_kafka_schemas.egg-info/SOURCES.txt` & `sentry-kafka-schemas-0.1.5/python/sentry_kafka_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/tests/test_codecs.py` & `sentry-kafka-schemas-0.1.5/python/tests/test_codecs.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,15 +21,17 @@
         "group_id": 2,
     }
 
 
 @pytest.mark.parametrize("codec_cls", [JsonCodec, MsgpackCodec])
 def test_json_codec(codec_cls: Codec[Any]) -> None:
     schema_path = Path.joinpath(Path(__file__).parent, "test.schema.json")
-    with open(schema_path, mode="r") as f:
+    with open(schema_path, mode="rb") as f:
         schema = json.loads(f.read())
 
     codec: JsonCodec[Example] = JsonCodec(json_schema=schema)
 
     data = get_example_data()
 
-    assert codec.decode(codec.encode(data, validate=False), validate=True) == data
+    data_intermediate = codec.encode(data, validate=False)
+    assert isinstance(data_intermediate, bytes)
+    assert codec.decode(data_intermediate, validate=True) == data
```

### Comparing `sentry-kafka-schemas-0.1.4/python/tests/test_codeowner.py` & `sentry-kafka-schemas-0.1.5/python/tests/test_codeowner.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/tests/test_examples.py` & `sentry-kafka-schemas-0.1.5/python/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/tests/test_valid_schemas.py` & `sentry-kafka-schemas-0.1.5/python/tests/test_valid_schemas.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/python/tests/test_valid_topic_data.py` & `sentry-kafka-schemas-0.1.5/python/tests/test_valid_topic_data.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.4/setup.py` & `sentry-kafka-schemas-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def get_requirements() -> Sequence[str]:
     with open("python/requirements.txt") as fp:
         return [x.strip() for x in fp if not x.startswith("#")]
 
 setup(
     name="sentry-kafka-schemas",
-    version="0.1.4",
+    version="0.1.5",
     author="Sentry",
     author_email="oss@sentry.io",
     url="https://github.com/getsentry/sentry-kafka-schemas",
     description="Kafka topics and schemas for Sentry",
     zip_safe=False,
     install_requires=get_requirements(),
     packages=find_packages(where="python/", exclude=["generate_python_types.py", "tests/"]),
```

