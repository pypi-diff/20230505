# Comparing `tmp/llama_index-0.6.0a7.tar.gz` & `tmp/llama_index-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index-0.6.0a7.tar", last modified: Tue May  2 20:09:00 2023, max compression
+gzip compressed data, was "llama_index-0.6.1.tar", last modified: Fri May  5 06:17:27 2023, max compression
```

## Comparing `llama_index-0.6.0a7.tar` & `llama_index-0.6.1.tar`

### file list

```diff
@@ -1,445 +1,449 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-02 20:08:43.000000 llama_index-0.6.0a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-02 20:08:43.000000 llama_index-0.6.0a7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-02 20:08:43.000000 llama_index-0.6.0a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.609001 llama_index-0.6.0a7/llama_index/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/async_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.609001 llama_index-0.6.0a7/llama_index/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/callbacks/llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/callbacks/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.609001 llama_index-0.6.0a7/llama_index/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/composability/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.609001 llama_index-0.6.0a7/llama_index/data_structs/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/data_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/data_structs_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/node_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/struct_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/data_structs/table_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/embeddings/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/embeddings/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/embeddings/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/embeddings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/evaluation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/evaluation/dataset_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/img_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/indices/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/base_retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/indices/common/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/indices/common/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/indices/common_tree/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/common_tree/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/composability/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/empty/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/empty/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.613000 llama_index-0.6.0a7/llama_index/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/keyword_table/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.617001 llama_index-0.6.0a7/llama_index/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/knowledge_graph/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.617001 llama_index-0.6.0a7/llama_index/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/list/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/list/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.617001 llama_index-0.6.0a7/llama_index/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/postprocessor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/postprocessor/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8778 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/postprocessor/pii.py
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/prompt_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.617001 llama_index-0.6.0a7/llama_index/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.617001 llama_index-0.6.0a7/llama_index/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/response_synthesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.617001 llama_index-0.6.0a7/llama_index/indices/response/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24774 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/response/response_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/response/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/service_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.617001 llama_index-0.6.0a7/llama_index/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/struct_store/pandas_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/struct_store/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/tree/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/tree/inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8914 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/vector_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/indices/vector_store/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/langchain_helpers/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/chain_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10838 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/llm_predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/llm_predictor/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/llm_predictor/stable_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/llm_predictor/structured.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/logger/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/node_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/node_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/node_parser/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/node_parser/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/node_parser/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/optimization/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/output_parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/output_parsers/guardrails.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/output_parsers/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/output_parsers/selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.621001 llama_index-0.6.0a7/llama_index/playground/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/playground/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.625001 llama_index-0.6.0a7/llama_index/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/prompts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/prompts/chat_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/prompts/default_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/prompts/prompt_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/prompts/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.625001 llama_index-0.6.0a7/llama_index/query_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/query_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/query_engine/graph_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/query_engine/router_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.625001 llama_index-0.6.0a7/llama_index/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/chatgpt_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/discord_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/faiss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/file/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/docs_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/epub_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/image_caption_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/image_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/image_vision_llm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/ipynb_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/mbox_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/slides_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/tabular_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/file/video_audio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/github_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/github_readers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/google_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/make_com/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/make_com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/mbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/notion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/obsidian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/steamship/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/steamship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/string_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/twitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.629001 llama_index-0.6.0a7/llama_index/readers/weaviate/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/weaviate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/weaviate/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/weaviate/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/web.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/readers/youtube_transcript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/response/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/response/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/response/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/response/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/retrievers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/retrievers/transform_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/selectors/llm_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/selectors/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/selectors/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/docstore/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/docstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/docstore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/storage/index_store/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/index_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/index_store/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/index_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/storage/kvstore/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/kvstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/kvstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/storage/storage_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/token_counter/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/token_counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/token_counter/mock_chain_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/token_counter/token_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/token_counter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.633001 llama_index-0.6.0a7/llama_index/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/tools/query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/tools/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.637001 llama_index-0.6.0a7/llama_index/tts/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/tts/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/tts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/tts/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.637001 llama_index-0.6.0a7/llama_index/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15768 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/opensearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/llama_index/vector_stores/weaviate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.609001 llama_index-0.6.0a7/llama_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-02 20:09:00.000000 llama_index-0.6.0a7/llama_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13551 2023-05-02 20:09:00.000000 llama_index-0.6.0a7/llama_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:09:00.000000 llama_index-0.6.0a7/llama_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-02 20:09:00.000000 llama_index-0.6.0a7/llama_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-02 20:09:00.000000 llama_index-0.6.0a7/llama_index.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.637001 llama_index-0.6.0a7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.637001 llama_index-0.6.0a7/tests/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/callbacks/test_llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.637001 llama_index-0.6.0a7/tests/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/embeddings/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.637001 llama_index-0.6.0a7/tests/indices/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.637001 llama_index-0.6.0a7/tests/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/composability/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/empty/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/keyword_table/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/keyword_table/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/keyword_table/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/knowledge_graph/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/knowledge_graph/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/knowledge_graph/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/list/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/list/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13923 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/postprocessor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/query_transform/mock_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/query_transform/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/test_compose_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/query/test_query_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/struct_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11934 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/struct_store/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/struct_store/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/struct_store/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/test_loading_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/test_node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/test_prompt_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.641001 llama_index-0.6.0a7/tests/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/tree/test_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/tree/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/tree/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/mock_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/mock_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/test_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/test_milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/test_myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/test_pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/test_weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/indices/vector_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/langchain_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/langchain_helpers/test_text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/llm_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/logger/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/mock_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/mock_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/mock_utils/mock_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/mock_utils/mock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/mock_utils/mock_text_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/mock_utils/mock_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/optimization/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/output_parsers/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/output_parsers/test_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/playground/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/playground/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/prompts/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.645001 llama_index-0.6.0a7/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/readers/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/readers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/readers/test_mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/readers/test_string_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/tests/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/selectors/test_llm_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/storage/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/tests/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/storage/docstore/test_mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/storage/docstore/test_simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/tests/token_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/token_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/token_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:09:00.649001 llama_index-0.6.0a7/tests/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/vector_stores/test_qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-02 20:08:44.000000 llama_index-0.6.0a7/tests/vector_stores/test_weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.331372 llama_index-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-05 06:17:12.000000 llama_index-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 06:17:12.000000 llama_index-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-05 06:17:27.331372 llama_index-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-05 06:17:12.000000 llama_index-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.295372 llama_index-0.6.1/llama_index/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.295372 llama_index-0.6.1/llama_index/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/callbacks/llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/callbacks/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.295372 llama_index-0.6.1/llama_index/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/composability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.295372 llama_index-0.6.1/llama_index/data_structs/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/data_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/data_structs/data_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/data_structs/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/data_structs/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/data_structs/struct_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/data_structs/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.295372 llama_index-0.6.1/llama_index/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/embeddings/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/embeddings/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/embeddings/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/embeddings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.295372 llama_index-0.6.1/llama_index/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11972 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/evaluation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/img_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.299372 llama_index-0.6.1/llama_index/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/base_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.299372 llama_index-0.6.1/llama_index/indices/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.299372 llama_index-0.6.1/llama_index/indices/common/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.299372 llama_index-0.6.1/llama_index/indices/common_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/common_tree/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.299372 llama_index-0.6.1/llama_index/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/composability/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.299372 llama_index-0.6.1/llama_index/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/empty/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/empty/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.299372 llama_index-0.6.1/llama_index/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.299372 llama_index-0.6.1/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10428 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/knowledge_graph/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.299372 llama_index-0.6.1/llama_index/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/list/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/list/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.299372 llama_index-0.6.1/llama_index/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/postprocessor/cohere_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/postprocessor/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/postprocessor/pii.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/postprocessor/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/prompt_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.303372 llama_index-0.6.1/llama_index/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.303372 llama_index-0.6.1/llama_index/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/query/response_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.303372 llama_index-0.6.1/llama_index/indices/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24768 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/response/response_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/response/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/service_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.303372 llama_index-0.6.1/llama_index/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/struct_store/pandas_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.303372 llama_index-0.6.1/llama_index/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/tree/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/tree/inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.303372 llama_index-0.6.1/llama_index/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/vector_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/indices/vector_store/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.303372 llama_index-0.6.1/llama_index/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.307372 llama_index-0.6.1/llama_index/langchain_helpers/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/langchain_helpers/chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.307372 llama_index-0.6.1/llama_index/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10838 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/llm_predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/llm_predictor/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/llm_predictor/stable_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/llm_predictor/structured.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.307372 llama_index-0.6.1/llama_index/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/logger/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.307372 llama_index-0.6.1/llama_index/node_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/node_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/node_parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/node_parser/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/node_parser/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.307372 llama_index-0.6.1/llama_index/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/optimization/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.307372 llama_index-0.6.1/llama_index/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/output_parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/output_parsers/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/output_parsers/selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.307372 llama_index-0.6.1/llama_index/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/playground/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.307372 llama_index-0.6.1/llama_index/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/prompts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/prompts/default_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/prompts/prompt_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.307372 llama_index-0.6.1/llama_index/query_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/query_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/query_engine/router_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.311372 llama_index-0.6.1/llama_index/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.311372 llama_index-0.6.1/llama_index/readers/chatgpt_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/discord_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/faiss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.315372 llama_index-0.6.1/llama_index/readers/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/file/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/file/docs_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/file/epub_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/file/image_caption_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/file/image_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/file/image_vision_llm_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/file/ipynb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/file/markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/file/mbox_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/file/slides_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/file/tabular_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/file/video_audio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.315372 llama_index-0.6.1/llama_index/readers/github_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15889 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/github_readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.315372 llama_index-0.6.1/llama_index/readers/google_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.315372 llama_index-0.6.1/llama_index/readers/make_com/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/mbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.315372 llama_index-0.6.1/llama_index/readers/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.315372 llama_index-0.6.1/llama_index/readers/steamship/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/string_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/twitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.315372 llama_index-0.6.1/llama_index/readers/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/weaviate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/weaviate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/readers/youtube_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.315372 llama_index-0.6.1/llama_index/response/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/response/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/response/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.315372 llama_index-0.6.1/llama_index/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/retrievers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.315372 llama_index-0.6.1/llama_index/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/selectors/llm_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/selectors/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/selectors/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.315372 llama_index-0.6.1/llama_index/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.319372 llama_index-0.6.1/llama_index/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/docstore/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/docstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/docstore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.319372 llama_index-0.6.1/llama_index/storage/index_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/index_store/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/index_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.319372 llama_index-0.6.1/llama_index/storage/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/kvstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/storage/storage_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.319372 llama_index-0.6.1/llama_index/token_counter/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/token_counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/token_counter/mock_chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/token_counter/token_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/token_counter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.319372 llama_index-0.6.1/llama_index/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/tools/query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/tools/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.319372 llama_index-0.6.1/llama_index/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/tts/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/tts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/tts/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.323372 llama_index-0.6.1/llama_index/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/lancedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15763 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-05 06:17:13.000000 llama_index-0.6.1/llama_index/vector_stores/weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.295372 llama_index-0.6.1/llama_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-05 06:17:27.000000 llama_index-0.6.1/llama_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-05-05 06:17:27.000000 llama_index-0.6.1/llama_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 06:17:27.000000 llama_index-0.6.1/llama_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 06:17:27.000000 llama_index-0.6.1/llama_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 06:17:27.000000 llama_index-0.6.1/llama_index.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-05 06:17:13.000000 llama_index-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 06:17:27.331372 llama_index-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-05 06:17:13.000000 llama_index-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.323372 llama_index-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.323372 llama_index-0.6.1/tests/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/callbacks/test_llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.323372 llama_index-0.6.1/tests/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/embeddings/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.323372 llama_index-0.6.1/tests/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.323372 llama_index-0.6.1/tests/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/composability/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.323372 llama_index-0.6.1/tests/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/empty/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.323372 llama_index-0.6.1/tests/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/keyword_table/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/keyword_table/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/keyword_table/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.323372 llama_index-0.6.1/tests/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/knowledge_graph/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/knowledge_graph/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/knowledge_graph/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.323372 llama_index-0.6.1/tests/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/list/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/list/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.323372 llama_index-0.6.1/tests/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/postprocessor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.323372 llama_index-0.6.1/tests/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.327372 llama_index-0.6.1/tests/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/query/query_transform/mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/query/query_transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/query/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/query/test_compose_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/query/test_query_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.327372 llama_index-0.6.1/tests/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/struct_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/struct_store/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/struct_store/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/struct_store/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/test_loading_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/test_node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/test_prompt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.327372 llama_index-0.6.1/tests/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/tree/test_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/tree/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/tree/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.327372 llama_index-0.6.1/tests/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/vector_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/vector_store/mock_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/vector_store/mock_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/vector_store/test_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/vector_store/test_lancedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/vector_store/test_milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/vector_store/test_myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/vector_store/test_pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/vector_store/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/vector_store/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/vector_store/test_weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/indices/vector_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.327372 llama_index-0.6.1/tests/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/langchain_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/langchain_helpers/test_text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.327372 llama_index-0.6.1/tests/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/llm_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.327372 llama_index-0.6.1/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/logger/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.327372 llama_index-0.6.1/tests/mock_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/mock_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/mock_utils/mock_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/mock_utils/mock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/mock_utils/mock_text_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/mock_utils/mock_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.327372 llama_index-0.6.1/tests/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/optimization/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.327372 llama_index-0.6.1/tests/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/output_parsers/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/output_parsers/test_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.331372 llama_index-0.6.1/tests/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/playground/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.331372 llama_index-0.6.1/tests/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/prompts/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.331372 llama_index-0.6.1/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/readers/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/readers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/readers/test_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/readers/test_string_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.331372 llama_index-0.6.1/tests/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/selectors/test_llm_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.331372 llama_index-0.6.1/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/storage/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.331372 llama_index-0.6.1/tests/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/storage/docstore/test_mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/storage/docstore/test_simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/storage/test_storage_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.331372 llama_index-0.6.1/tests/token_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/token_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/token_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:27.331372 llama_index-0.6.1/tests/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/vector_stores/test_qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-05 06:17:13.000000 llama_index-0.6.1/tests/vector_stores/test_weaviate.py
```

### Comparing `llama_index-0.6.0a7/LICENSE` & `llama_index-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/PKG-INFO` & `llama_index-0.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,16 @@
-Metadata-Version: 2.1
-Name: llama_index
-Version: 0.6.0a7
-Summary: Interface between LLMs and your data
-Home-page: https://github.com/jerryjliu/llama_index
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 🗂️ LlamaIndex 🦙
 
 LlamaIndex (GPT Index) is a project that provides a central interface to connect your LLM's with external data.
 
-PyPi: 
+PyPI: 
 - LlamaIndex: https://pypi.org/project/llama-index/.
 - GPT Index (duplicate): https://pypi.org/project/gpt-index/.
 
-Documentation:
-- v0.6 (pre-release): https://gpt-index.readthedocs.io/en/latest/.
-- v0.5 (stable): https://gpt-index.readthedocs.io/en/v0.5.27/.
+Documentation: https://gpt-index.readthedocs.io/.
 
 Twitter: https://twitter.com/gpt_index.
 
 Discord: https://discord.gg/dGcwcsnxhU.
 
 ### Ecosystem
 
@@ -30,15 +19,15 @@
 
 
 ## 🚀 Overview
 
 **NOTE**: This README is not updated as frequently as the documentation. Please check out the documentation above for the latest updates!
 
 ### Context
-- LLMs are a phenomenonal piece of technology for knowledge generation and reasoning. They are pre-trained on large amounts of publicly available data.
+- LLMs are a phenomenal piece of technology for knowledge generation and reasoning. They are pre-trained on large amounts of publicly available data.
 - How do we best augment LLMs with our own private data?
 - One paradigm that has emerged is *in-context* learning (the other is finetuning), where we insert context into the input prompt. That way,
 we take advantage of the LLM's reasoning capabilities to generate a response.
 
 To perform LLM's data augmentation in a performant, efficient, and cheap manner, we need to solve two components:
 - Data Ingestion
 - Data Indexing
@@ -55,15 +44,15 @@
    - Dealing with text splitting.
 - Provides users an interface to **query** the index (feed in an input prompt) and obtain a knowledge-augmented output.
 - Offers you a comprehensive toolset trading off cost and performance.
 
 
 ## 💡 Contributing
 
-Interesting in contributing? See our [Contribution Guide](CONTRIBUTING.md) for more details.
+Interested in contributing? See our [Contribution Guide](CONTRIBUTING.md) for more details.
 
 ## 📄 Documentation
 
 Full documentation can be found here: https://gpt-index.readthedocs.io/en/latest/. 
 
 Please check it out for the most up-to-date tutorials, how-to guides, references, and other resources!
```

### Comparing `llama_index-0.6.0a7/README.md` & `llama_index-0.6.1/llama_index.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+Metadata-Version: 2.1
+Name: llama-index
+Version: 0.6.1
+Summary: Interface between LLMs and your data
+Home-page: https://github.com/jerryjliu/llama_index
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 🗂️ LlamaIndex 🦙
 
 LlamaIndex (GPT Index) is a project that provides a central interface to connect your LLM's with external data.
 
-PyPi: 
+PyPI: 
 - LlamaIndex: https://pypi.org/project/llama-index/.
 - GPT Index (duplicate): https://pypi.org/project/gpt-index/.
 
-Documentation:
-- v0.6 (pre-release): https://gpt-index.readthedocs.io/en/latest/.
-- v0.5 (stable): https://gpt-index.readthedocs.io/en/v0.5.27/.
+Documentation: https://gpt-index.readthedocs.io/.
 
 Twitter: https://twitter.com/gpt_index.
 
 Discord: https://discord.gg/dGcwcsnxhU.
 
 ### Ecosystem
 
@@ -21,15 +28,15 @@
 
 
 ## 🚀 Overview
 
 **NOTE**: This README is not updated as frequently as the documentation. Please check out the documentation above for the latest updates!
 
 ### Context
-- LLMs are a phenomenonal piece of technology for knowledge generation and reasoning. They are pre-trained on large amounts of publicly available data.
+- LLMs are a phenomenal piece of technology for knowledge generation and reasoning. They are pre-trained on large amounts of publicly available data.
 - How do we best augment LLMs with our own private data?
 - One paradigm that has emerged is *in-context* learning (the other is finetuning), where we insert context into the input prompt. That way,
 we take advantage of the LLM's reasoning capabilities to generate a response.
 
 To perform LLM's data augmentation in a performant, efficient, and cheap manner, we need to solve two components:
 - Data Ingestion
 - Data Indexing
@@ -46,15 +53,15 @@
    - Dealing with text splitting.
 - Provides users an interface to **query** the index (feed in an input prompt) and obtain a knowledge-augmented output.
 - Offers you a comprehensive toolset trading off cost and performance.
 
 
 ## 💡 Contributing
 
-Interesting in contributing? See our [Contribution Guide](CONTRIBUTING.md) for more details.
+Interested in contributing? See our [Contribution Guide](CONTRIBUTING.md) for more details.
 
 ## 📄 Documentation
 
 Full documentation can be found here: https://gpt-index.readthedocs.io/en/latest/. 
 
 Please check it out for the most up-to-date tutorials, how-to guides, references, and other resources!
```

### Comparing `llama_index-0.6.0a7/llama_index/__init__.py` & `llama_index-0.6.1/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/callbacks/base.py` & `llama_index-0.6.1/llama_index/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/callbacks/llama_debug.py` & `llama_index-0.6.1/llama_index/callbacks/llama_debug.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/callbacks/schema.py` & `llama_index-0.6.1/llama_index/callbacks/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/composability/joint_qa_summary.py` & `llama_index-0.6.1/llama_index/composability/joint_qa_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/data_structs/data_structs.py` & `llama_index-0.6.1/llama_index/data_structs/data_structs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,287 +1,247 @@
-"""File for core data structures."""
+"""Data structures.
 
-import random
-import sys
+Nodes are decoupled from the indices.
+
+"""
+
+import uuid
+from abc import abstractmethod
 from dataclasses import dataclass, field
-from typing import Any, Dict, List, Optional, Set, Tuple
+from typing import Dict, List, Optional, Sequence, Set, Tuple
 
 from dataclasses_json import DataClassJsonMixin
 
+from llama_index.data_structs.node import Node
 from llama_index.data_structs.struct_type import IndexStructType
-from llama_index.schema import BaseDocument
-from llama_index.utils import get_new_int_id
 
 
 @dataclass
-class IndexStruct(BaseDocument, DataClassJsonMixin):
+class IndexStruct(DataClassJsonMixin):
     """A base data struct for a LlamaIndex."""
 
-    # NOTE: the text field, inherited from BaseDocument,
-    # represents a summary of the content of the index struct.
-    # primarily used for composing indices with other indices
-
-    # NOTE: the doc_id field, inherited from BaseDocument,
-    # represents a unique identifier for the index struct
-    # that will be put in the docstore.
-    # Not all index_structs need to have a doc_id. Only index_structs that
-    # represent a complete data structure (e.g. IndexGraph, IndexList),
-    # and are used to compose a higher level index, will have a doc_id.
-
-
-@dataclass
-class Node(IndexStruct):
-    """A generic node of data.
+    index_id: str = field(default_factory=lambda: str(uuid.uuid4()))
+    summary: Optional[str] = None
 
-    Base struct used in most indices.
-
-    """
-
-    def __post_init__(self) -> None:
-        """Post init."""
-        super().__post_init__()
-        # NOTE: for Node objects, the text field is required
-        if self.text is None:
-            raise ValueError("text field not set.")
-
-    # used for GPTTreeIndex
-    index: int = 0
-    child_indices: Set[int] = field(default_factory=set)
-
-    # embeddings
-    embedding: Optional[List[float]] = None
-
-    # reference document id
-    ref_doc_id: Optional[str] = None
-
-    # extra node info
-    node_info: Optional[Dict[str, Any]] = None
-
-    # TODO: store reference instead of actual image
-    # base64 encoded image str
-    image: Optional[str] = None
-
-    def get_text(self) -> str:
-        """Get text."""
-        text = super().get_text()
-        result_text = (
-            text if self.extra_info_str is None else f"{self.extra_info_str}\n\n{text}"
-        )
-        return result_text
+    def get_summary(self) -> str:
+        """Get text summary."""
+        if self.summary is None:
+            raise ValueError("summary field of the index_struct not set.")
+        return self.summary
 
     @classmethod
-    def get_type(cls) -> str:
-        """Get type."""
-        # TODO: consolidate with IndexStructType
-        return "node"
+    @abstractmethod
+    def get_type(cls) -> IndexStructType:
+        """Get index struct type."""
 
 
 @dataclass
 class IndexGraph(IndexStruct):
     """A graph representing the tree-structured index."""
 
-    all_nodes: Dict[int, Node] = field(default_factory=dict)
-    root_nodes: Dict[int, Node] = field(default_factory=dict)
+    # mapping from index in tree to Node doc id.
+    all_nodes: Dict[int, str] = field(default_factory=dict)
+    root_nodes: Dict[int, str] = field(default_factory=dict)
+    node_id_to_children_ids: Dict[str, List[str]] = field(default_factory=dict)
+
+    @property
+    def node_id_to_index(self) -> Dict[str, int]:
+        """Map from node id to index."""
+        return {node_id: index for index, node_id in self.all_nodes.items()}
 
     @property
     def size(self) -> int:
         """Get the size of the graph."""
         return len(self.all_nodes)
 
-    def get_children(self, parent_node: Optional[Node]) -> Dict[int, Node]:
-        """Get nodes given indices."""
+    def get_index(self, node: Node) -> int:
+        """Get index of node."""
+        return self.node_id_to_index[node.get_doc_id()]
+
+    def insert(
+        self,
+        node: Node,
+        index: Optional[int] = None,
+        children_nodes: Optional[Sequence[Node]] = None,
+    ) -> None:
+        """Insert node."""
+        index = index or self.size
+        node_id = node.get_doc_id()
+
+        self.all_nodes[index] = node_id
+
+        if children_nodes is None:
+            children_nodes = []
+        children_ids = [n.get_doc_id() for n in children_nodes]
+        self.node_id_to_children_ids[node_id] = children_ids
+
+    def get_children(self, parent_node: Optional[Node]) -> Dict[int, str]:
+        """Get children nodes."""
         if parent_node is None:
             return self.root_nodes
         else:
-            return {i: self.all_nodes[i] for i in parent_node.child_indices}
-
-    def insert_under_parent(self, node: Node, parent_node: Optional[Node]) -> None:
+            parent_id = parent_node.get_doc_id()
+            children_ids = self.node_id_to_children_ids[parent_id]
+            return {
+                self.node_id_to_index[child_id]: child_id for child_id in children_ids
+            }
+
+    def insert_under_parent(
+        self, node: Node, parent_node: Optional[Node], new_index: Optional[int] = None
+    ) -> None:
         """Insert under parent node."""
-        if node.index in self.all_nodes:
-            raise ValueError(
-                "Cannot insert a new node with the same index as an existing node."
-            )
+        new_index = new_index or self.size
         if parent_node is None:
-            self.root_nodes[node.index] = node
+            self.root_nodes[new_index] = node.get_doc_id()
+            self.node_id_to_children_ids[node.get_doc_id()] = []
         else:
-            parent_node.child_indices.add(node.index)
+            if parent_node.doc_id not in self.node_id_to_children_ids:
+                self.node_id_to_children_ids[parent_node.get_doc_id()] = []
+            self.node_id_to_children_ids[parent_node.get_doc_id()].append(
+                node.get_doc_id()
+            )
 
-        self.all_nodes[node.index] = node
+        self.all_nodes[new_index] = node.get_doc_id()
 
     @classmethod
-    def get_type(cls) -> str:
+    def get_type(cls) -> IndexStructType:
         """Get type."""
-        return "tree"
+        return IndexStructType.TREE
 
 
 @dataclass
 class KeywordTable(IndexStruct):
     """A table of keywords mapping keywords to text chunks."""
 
-    table: Dict[str, Set[int]] = field(default_factory=dict)
-    text_chunks: Dict[int, Node] = field(default_factory=dict)
-
-    def _get_index(self) -> int:
-        """Get the next index for the text chunk."""
-        # randomly generate until we get a unique index
-        while True:
-            idx = random.randint(0, sys.maxsize)
-            if idx not in self.text_chunks:
-                break
-        return idx
+    table: Dict[str, Set[str]] = field(default_factory=dict)
 
-    def add_node(self, keywords: List[str], node: Node) -> int:
+    def add_node(self, keywords: List[str], node: Node) -> None:
         """Add text to table."""
-        cur_idx = self._get_index()
         for keyword in keywords:
             if keyword not in self.table:
                 self.table[keyword] = set()
-            self.table[keyword].add(cur_idx)
-        self.text_chunks[cur_idx] = node
-        return cur_idx
+            self.table[keyword].add(node.get_doc_id())
 
-    def get_texts(self, keyword: str) -> List[str]:
-        """Get texts given keyword."""
-        if keyword not in self.table:
-            raise ValueError("Keyword not found in table.")
-        return [self.text_chunks[idx].get_text() for idx in self.table[keyword]]
+    @property
+    def node_ids(self) -> Set[str]:
+        """Get all node ids."""
+        return set.union(*self.table.values())
 
     @property
     def keywords(self) -> Set[str]:
         """Get all keywords in the table."""
         return set(self.table.keys())
 
     @property
     def size(self) -> int:
         """Get the size of the table."""
         return len(self.table)
 
     @classmethod
-    def get_type(cls) -> str:
+    def get_type(cls) -> IndexStructType:
         """Get type."""
-        return "keyword_table"
+        return IndexStructType.KEYWORD_TABLE
 
 
 @dataclass
 class IndexList(IndexStruct):
     """A list of documents."""
 
-    nodes: List[Node] = field(default_factory=list)
+    nodes: List[str] = field(default_factory=list)
 
     def add_node(self, node: Node) -> None:
         """Add text to table, return current position in list."""
         # don't worry about child indices for now, nodes are all in order
-        self.nodes.append(node)
+        self.nodes.append(node.get_doc_id())
 
     @classmethod
-    def get_type(cls) -> str:
+    def get_type(cls) -> IndexStructType:
         """Get type."""
-        return "list"
+        return IndexStructType.LIST
 
 
 @dataclass
 class IndexDict(IndexStruct):
     """A simple dictionary of documents."""
 
-    nodes_dict: Dict[int, Node] = field(default_factory=dict)
-    id_map: Dict[str, int] = field(default_factory=dict)
+    # mapping from vector store id to node id
+    nodes_dict: Dict[str, str] = field(default_factory=dict)
+    # mapping from doc_id to vector store id
+    doc_id_dict: Dict[str, List[str]] = field(default_factory=dict)
 
     # TODO: temporary hack to store embeddings for simple vector index
     # this should be empty for all other indices
     embeddings_dict: Dict[str, List[float]] = field(default_factory=dict)
 
     def add_node(
         self,
         node: Node,
         text_id: Optional[str] = None,
     ) -> str:
         """Add text to table, return current position in list."""
-        int_id = get_new_int_id(set(self.nodes_dict.keys()))
-        if text_id in self.id_map:
-            raise ValueError("text_id cannot already exist in index.")
-        elif text_id is not None and not isinstance(text_id, str):
-            raise ValueError("text_id must be a string.")
-        elif text_id is None:
-            text_id = str(int_id)
-        self.id_map[text_id] = int_id
-
-        # don't worry about child indices for now, nodes are all in order
-        self.nodes_dict[int_id] = node
-        return text_id
+        # # don't worry about child indices for now, nodes are all in order
+        # self.nodes_dict[int_id] = node
+        vector_id = text_id if text_id is not None else node.get_doc_id()
+        self.nodes_dict[vector_id] = node.get_doc_id()
+        if node.ref_doc_id is not None:
+            if node.ref_doc_id not in self.doc_id_dict:
+                self.doc_id_dict[node.ref_doc_id] = []
+            self.doc_id_dict[node.ref_doc_id].append(vector_id)
 
-    def get_nodes(self, text_ids: List[str]) -> List[Node]:
-        """Get nodes."""
-        nodes = []
-        for text_id in text_ids:
-            if text_id not in self.id_map:
-                raise ValueError("text_id not found in id_map")
-            elif not isinstance(text_id, str):
-                raise ValueError("text_id must be a string.")
-            int_id = self.id_map[text_id]
-            if int_id not in self.nodes_dict:
-                raise ValueError("int_id not found in nodes_dict")
-            nodes.append(self.nodes_dict[int_id])
-        return nodes
-
-    def get_node(self, text_id: str) -> Node:
-        """Get node."""
-        return self.get_nodes([text_id])[0]
+        return vector_id
 
     def delete(self, doc_id: str) -> None:
-        """Delete a document."""
-        text_ids_to_delete = set()
-        int_ids_to_delete = set()
-        for text_id, int_id in self.id_map.items():
-            node = self.nodes_dict[int_id]
-            if node.ref_doc_id != doc_id:
-                continue
-            text_ids_to_delete.add(text_id)
-            int_ids_to_delete.add(int_id)
-
-        for int_id, text_id in zip(int_ids_to_delete, text_ids_to_delete):
-            del self.nodes_dict[int_id]
-            del self.id_map[text_id]
+        """Delete a Node."""
+        if doc_id not in self.doc_id_dict:
+            return
+        for vector_id in self.doc_id_dict[doc_id]:
+            del self.nodes_dict[vector_id]
+        del self.doc_id_dict[doc_id]
 
     @classmethod
-    def get_type(cls) -> str:
+    def get_type(cls) -> IndexStructType:
         """Get type."""
         return IndexStructType.VECTOR_STORE
 
 
 @dataclass
 class KG(IndexStruct):
     """A table of keywords mapping keywords to text chunks."""
 
     # Unidirectional
 
     table: Dict[str, Set[str]] = field(default_factory=dict)
-    text_chunks: Dict[str, Node] = field(default_factory=dict)
+    # text_chunks: Dict[str, Node] = field(default_factory=dict)
     rel_map: Dict[str, List[Tuple[str, str]]] = field(default_factory=dict)
     embedding_dict: Dict[str, List[float]] = field(default_factory=dict)
 
+    @property
+    def node_ids(self) -> Set[str]:
+        """Get all node ids."""
+        return set.union(*self.table.values())
+
     def add_to_embedding_dict(self, triplet_str: str, embedding: List[float]) -> None:
         """Add embedding to dict."""
         self.embedding_dict[triplet_str] = embedding
 
-    def upsert_triplet(self, triplet: Tuple[str, str, str], node: Node) -> None:
+    def upsert_triplet(self, triplet: Tuple[str, str, str]) -> None:
         """Upsert a knowledge triplet to the graph."""
         subj, relationship, obj = triplet
-        self.add_node([subj, obj], node)
         if subj not in self.rel_map:
             self.rel_map[subj] = []
         self.rel_map[subj].append((obj, relationship))
 
     def add_node(self, keywords: List[str], node: Node) -> None:
         """Add text to table."""
         node_id = node.get_doc_id()
         for keyword in keywords:
             if keyword not in self.table:
                 self.table[keyword] = set()
             self.table[keyword].add(node_id)
-        self.text_chunks[node_id] = node
+        # self.text_chunks[node_id] = node
 
     def get_rel_map_texts(self, keyword: str) -> List[str]:
         """Get the corresponding knowledge for a given keyword."""
         # NOTE: return a single node for now
         if keyword not in self.rel_map:
             return []
         texts = []
@@ -311,94 +271,20 @@
         for keyword in keywords:
             for node_id in self.table.get(keyword, set()):
                 node_ids.append(node_id)
             # TODO: Traverse (with depth > 1)
         return node_ids
 
     @classmethod
-    def get_type(cls) -> str:
-        """Get type."""
-        return "kg"
-
-
-# TODO: remove once we centralize UX around vector index
-
-
-class SimpleIndexDict(IndexDict):
-    """Index dict for simple vector index."""
-
-    @classmethod
-    def get_type(cls) -> str:
+    def get_type(cls) -> IndexStructType:
         """Get type."""
-        return IndexStructType.SIMPLE_DICT
+        return IndexStructType.KG
 
 
-class FaissIndexDict(IndexDict):
-    """Index dict for Faiss vector index."""
-
-    @classmethod
-    def get_type(cls) -> str:
-        """Get type."""
-        return IndexStructType.DICT
-
-
-class WeaviateIndexDict(IndexDict):
-    """Index dict for Weaviate vector index."""
-
-    @classmethod
-    def get_type(cls) -> str:
-        """Get type."""
-        return IndexStructType.WEAVIATE
-
-
-class PineconeIndexDict(IndexDict):
-    """Index dict for Pinecone vector index."""
-
-    @classmethod
-    def get_type(cls) -> str:
-        """Get type."""
-        return IndexStructType.PINECONE
-
-
-class QdrantIndexDict(IndexDict):
-    """Index dict for Qdrant vector index."""
-
-    @classmethod
-    def get_type(cls) -> str:
-        """Get type."""
-        return IndexStructType.QDRANT
-
-
-class ChromaIndexDict(IndexDict):
-    """Index dict for Chroma vector index."""
-
-    @classmethod
-    def get_type(cls) -> str:
-        """Get type."""
-        return IndexStructType.CHROMA
-
-
-class OpensearchIndexDict(IndexDict):
-    """Index dict for Opensearch vector index."""
-
-    @classmethod
-    def get_type(cls) -> str:
-        """Get type."""
-        return IndexStructType.OPENSEARCH
-
-
-class ChatGPTRetrievalPluginIndexDict(IndexDict):
-    """Index dict for ChatGPT Retrieval Plugin."""
-
-    @classmethod
-    def get_type(cls) -> str:
-        """Get type."""
-        return IndexStructType.CHATGPT_RETRIEVAL_PLUGIN
-
-
-class EmptyIndex(IndexStruct):
+@dataclass
+class EmptyIndex(IndexDict):
     """Empty index."""
 
     @classmethod
-    def get_type(cls) -> str:
+    def get_type(cls) -> IndexStructType:
         """Get type."""
         return IndexStructType.EMPTY
```

### Comparing `llama_index-0.6.0a7/llama_index/data_structs/data_structs_v2.py` & `llama_index-0.6.1/llama_index/indices/keyword_table/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,290 +1,222 @@
-"""Data structures v2.
+"""Keyword-table based index.
 
-Nodes are decoupled from the indices.
+Similar to a "hash table" in concept. LlamaIndex first tries
+to extract keywords from the source text, and stores the
+keywords as keys per item. It similarly extracts keywords
+from the query text. Then, it tries to match those keywords to
+existing keywords in the table.
 
 """
 
-import uuid
 from abc import abstractmethod
-from dataclasses import dataclass, field
-from typing import Dict, List, Optional, Sequence, Set, Tuple
+from enum import Enum
+from typing import Any, Optional, Sequence, Set, Union
 
-from dataclasses_json import DataClassJsonMixin
+from llama_index.async_utils import run_async_tasks
+from llama_index.callbacks.schema import CBEventType
+from llama_index.data_structs.data_structs import KeywordTable
+from llama_index.data_structs.node import Node
+from llama_index.indices.base import BaseGPTIndex
+from llama_index.indices.base_retriever import BaseRetriever
+from llama_index.indices.keyword_table.utils import extract_keywords_given_response
+from llama_index.indices.service_context import ServiceContext
+from llama_index.prompts.default_prompts import (
+    DEFAULT_KEYWORD_EXTRACT_TEMPLATE,
+    DEFAULT_QUERY_KEYWORD_EXTRACT_TEMPLATE,
+)
+from llama_index.prompts.prompts import KeywordExtractPrompt
+
+DQKET = DEFAULT_QUERY_KEYWORD_EXTRACT_TEMPLATE
+
+
+class KeywordTableRetrieverMode(str, Enum):
+    DEFAULT = "default"
+    SIMPLE = "simple"
+    RAKE = "rake"
+
+
+class BaseGPTKeywordTableIndex(BaseGPTIndex[KeywordTable]):
+    """GPT Keyword Table Index.
+
+    This index extracts keywords from the text, and maps each
+    keyword to the node(s) that it corresponds to. In this sense it mimicks a
+    "hash table". During index construction, the keyword table is constructed
+    by extracting keywords from each node and creating an internal mapping.
+
+    During query time, the keywords are extracted from the query text, and these
+    keywords are used to index into the keyword table. The retrieved nodes
+    are then used to answer the query.
+
+    Args:
+        keyword_extract_template (Optional[KeywordExtractPrompt]): A Keyword
+            Extraction Prompt
+            (see :ref:`Prompt-Templates`).
+        use_async (bool): Whether to use asynchronous calls. Defaults to False.
 
-from llama_index.data_structs.node_v2 import Node
-from llama_index.data_structs.struct_type import IndexStructType
+    """
 
+    index_struct_cls = KeywordTable
 
-@dataclass
-class V2IndexStruct(DataClassJsonMixin):
-    """A base data struct for a LlamaIndex."""
-
-    index_id: str = field(default_factory=lambda: str(uuid.uuid4()))
-    summary: Optional[str] = None
+    def __init__(
+        self,
+        nodes: Optional[Sequence[Node]] = None,
+        index_struct: Optional[KeywordTable] = None,
+        service_context: Optional[ServiceContext] = None,
+        keyword_extract_template: Optional[KeywordExtractPrompt] = None,
+        max_keywords_per_chunk: int = 10,
+        use_async: bool = False,
+        **kwargs: Any,
+    ) -> None:
+        """Initialize params."""
+        # need to set parameters before building index in base class.
+        self.max_keywords_per_chunk = max_keywords_per_chunk
+        self.keyword_extract_template = (
+            keyword_extract_template or DEFAULT_KEYWORD_EXTRACT_TEMPLATE
+        )
+        # NOTE: Partially format keyword extract template here.
+        self.keyword_extract_template = self.keyword_extract_template.partial_format(
+            max_keywords=self.max_keywords_per_chunk
+        )
+        self._use_async = use_async
+        super().__init__(
+            nodes=nodes,
+            index_struct=index_struct,
+            service_context=service_context,
+            **kwargs,
+        )
 
-    def get_summary(self) -> str:
-        """Get text summary."""
-        if self.summary is None:
-            raise ValueError("summary field of the index_struct not set.")
-        return self.summary
+    def as_retriever(
+        self,
+        retriever_mode: Union[
+            str, KeywordTableRetrieverMode
+        ] = KeywordTableRetrieverMode.DEFAULT,
+        **kwargs: Any,
+    ) -> BaseRetriever:
+        # NOTE: lazy import
+        from llama_index.indices.keyword_table.retrievers import (
+            KeywordTableGPTRetriever,
+            KeywordTableRAKERetriever,
+            KeywordTableSimpleRetriever,
+        )
+
+        if retriever_mode == KeywordTableRetrieverMode.DEFAULT:
+            return KeywordTableGPTRetriever(self, **kwargs)
+        elif retriever_mode == KeywordTableRetrieverMode.SIMPLE:
+            return KeywordTableSimpleRetriever(self, **kwargs)
+        elif retriever_mode == KeywordTableRetrieverMode.RAKE:
+            return KeywordTableRAKERetriever(self, **kwargs)
+        else:
+            raise ValueError(f"Unknown retriever mode: {retriever_mode}")
 
-    @classmethod
     @abstractmethod
-    def get_type(cls) -> IndexStructType:
-        """Get index struct type."""
-
+    def _extract_keywords(self, text: str) -> Set[str]:
+        """Extract keywords from text."""
 
-@dataclass
-class IndexGraph(V2IndexStruct):
-    """A graph representing the tree-structured index."""
-
-    # mapping from index in tree to Node doc id.
-    all_nodes: Dict[int, str] = field(default_factory=dict)
-    root_nodes: Dict[int, str] = field(default_factory=dict)
-    node_id_to_children_ids: Dict[str, List[str]] = field(default_factory=dict)
-
-    @property
-    def node_id_to_index(self) -> Dict[str, int]:
-        """Map from node id to index."""
-        return {node_id: index for index, node_id in self.all_nodes.items()}
-
-    @property
-    def size(self) -> int:
-        """Get the size of the graph."""
-        return len(self.all_nodes)
-
-    def get_index(self, node: Node) -> int:
-        """Get index of node."""
-        return self.node_id_to_index[node.get_doc_id()]
+    async def _async_extract_keywords(self, text: str) -> Set[str]:
+        """Extract keywords from text."""
+        # by default just call sync version
+        return self._extract_keywords(text)
 
-    def insert(
-        self,
-        node: Node,
-        index: Optional[int] = None,
-        children_nodes: Optional[Sequence[Node]] = None,
+    def _add_nodes_to_index(
+        self, index_struct: KeywordTable, nodes: Sequence[Node]
     ) -> None:
-        """Insert node."""
-        index = index or self.size
-        node_id = node.get_doc_id()
-
-        self.all_nodes[index] = node_id
-
-        if children_nodes is None:
-            children_nodes = []
-        children_ids = [n.get_doc_id() for n in children_nodes]
-        self.node_id_to_children_ids[node_id] = children_ids
-
-    def get_children(self, parent_node: Optional[Node]) -> Dict[int, str]:
-        """Get children nodes."""
-        if parent_node is None:
-            return self.root_nodes
-        else:
-            parent_id = parent_node.get_doc_id()
-            children_ids = self.node_id_to_children_ids[parent_id]
-            return {
-                self.node_id_to_index[child_id]: child_id for child_id in children_ids
-            }
+        """Add document to index."""
+        for n in nodes:
+            keywords = self._extract_keywords(n.get_text())
+            index_struct.add_node(list(keywords), n)
 
-    def insert_under_parent(
-        self, node: Node, parent_node: Optional[Node], new_index: Optional[int] = None
+    async def _async_add_nodes_to_index(
+        self, index_struct: KeywordTable, nodes: Sequence[Node]
     ) -> None:
-        """Insert under parent node."""
-        new_index = new_index or self.size
-        if parent_node is None:
-            self.root_nodes[new_index] = node.get_doc_id()
-            self.node_id_to_children_ids[node.get_doc_id()] = []
+        """Add document to index."""
+        for n in nodes:
+            keywords = await self._async_extract_keywords(n.get_text())
+            index_struct.add_node(list(keywords), n)
+
+    def _build_index_from_nodes(self, nodes: Sequence[Node]) -> KeywordTable:
+        """Build the index from nodes."""
+        # do simple concatenation
+        index_struct = KeywordTable(table={})
+        if self._use_async:
+            tasks = [self._async_add_nodes_to_index(index_struct, nodes)]
+            run_async_tasks(tasks)
         else:
-            if parent_node.doc_id not in self.node_id_to_children_ids:
-                self.node_id_to_children_ids[parent_node.get_doc_id()] = []
-            self.node_id_to_children_ids[parent_node.get_doc_id()].append(
-                node.get_doc_id()
-            )
-
-        self.all_nodes[new_index] = node.get_doc_id()
-
-    @classmethod
-    def get_type(cls) -> IndexStructType:
-        """Get type."""
-        return IndexStructType.TREE
-
-
-@dataclass
-class KeywordTable(V2IndexStruct):
-    """A table of keywords mapping keywords to text chunks."""
-
-    table: Dict[str, Set[str]] = field(default_factory=dict)
-
-    def add_node(self, keywords: List[str], node: Node) -> None:
-        """Add text to table."""
-        for keyword in keywords:
-            if keyword not in self.table:
-                self.table[keyword] = set()
-            self.table[keyword].add(node.get_doc_id())
+            self._add_nodes_to_index(index_struct, nodes)
 
-    @property
-    def node_ids(self) -> Set[str]:
-        """Get all node ids."""
-        return set.union(*self.table.values())
+        return index_struct
 
-    @property
-    def keywords(self) -> Set[str]:
-        """Get all keywords in the table."""
-        return set(self.table.keys())
-
-    @property
-    def size(self) -> int:
-        """Get the size of the table."""
-        return len(self.table)
-
-    @classmethod
-    def get_type(cls) -> IndexStructType:
-        """Get type."""
-        return IndexStructType.KEYWORD_TABLE
-
-
-@dataclass
-class IndexList(V2IndexStruct):
-    """A list of documents."""
-
-    nodes: List[str] = field(default_factory=list)
-
-    def add_node(self, node: Node) -> None:
-        """Add text to table, return current position in list."""
-        # don't worry about child indices for now, nodes are all in order
-        self.nodes.append(node.get_doc_id())
-
-    @classmethod
-    def get_type(cls) -> IndexStructType:
-        """Get type."""
-        return IndexStructType.LIST
-
-
-@dataclass
-class IndexDict(V2IndexStruct):
-    """A simple dictionary of documents."""
-
-    # mapping from vector store id to node id
-    nodes_dict: Dict[str, str] = field(default_factory=dict)
-    # mapping from doc_id to vector store id
-    doc_id_dict: Dict[str, List[str]] = field(default_factory=dict)
-
-    # TODO: temporary hack to store embeddings for simple vector index
-    # this should be empty for all other indices
-    embeddings_dict: Dict[str, List[float]] = field(default_factory=dict)
-
-    def add_node(
-        self,
-        node: Node,
-        text_id: Optional[str] = None,
-    ) -> str:
-        """Add text to table, return current position in list."""
-        # # don't worry about child indices for now, nodes are all in order
-        # self.nodes_dict[int_id] = node
-        vector_id = text_id if text_id is not None else node.get_doc_id()
-        self.nodes_dict[vector_id] = node.get_doc_id()
-        if node.ref_doc_id is not None:
-            if node.ref_doc_id not in self.doc_id_dict:
-                self.doc_id_dict[node.ref_doc_id] = []
-            self.doc_id_dict[node.ref_doc_id].append(vector_id)
-
-        return vector_id
-
-    def delete(self, doc_id: str) -> None:
-        """Delete a Node."""
-        if doc_id not in self.doc_id_dict:
-            return
-        for vector_id in self.doc_id_dict[doc_id]:
-            del self.nodes_dict[vector_id]
-        del self.doc_id_dict[doc_id]
-
-    @classmethod
-    def get_type(cls) -> IndexStructType:
-        """Get type."""
-        return IndexStructType.VECTOR_STORE
-
-
-@dataclass
-class KG(V2IndexStruct):
-    """A table of keywords mapping keywords to text chunks."""
-
-    # Unidirectional
-
-    table: Dict[str, Set[str]] = field(default_factory=dict)
-    # text_chunks: Dict[str, Node] = field(default_factory=dict)
-    rel_map: Dict[str, List[Tuple[str, str]]] = field(default_factory=dict)
-    embedding_dict: Dict[str, List[float]] = field(default_factory=dict)
-
-    @property
-    def node_ids(self) -> Set[str]:
-        """Get all node ids."""
-        return set.union(*self.table.values())
-
-    def add_to_embedding_dict(self, triplet_str: str, embedding: List[float]) -> None:
-        """Add embedding to dict."""
-        self.embedding_dict[triplet_str] = embedding
-
-    def upsert_triplet(self, triplet: Tuple[str, str, str]) -> None:
-        """Upsert a knowledge triplet to the graph."""
-        subj, relationship, obj = triplet
-        if subj not in self.rel_map:
-            self.rel_map[subj] = []
-        self.rel_map[subj].append((obj, relationship))
-
-    def add_node(self, keywords: List[str], node: Node) -> None:
-        """Add text to table."""
-        node_id = node.get_doc_id()
-        for keyword in keywords:
-            if keyword not in self.table:
-                self.table[keyword] = set()
-            self.table[keyword].add(node_id)
-        # self.text_chunks[node_id] = node
-
-    def get_rel_map_texts(self, keyword: str) -> List[str]:
-        """Get the corresponding knowledge for a given keyword."""
-        # NOTE: return a single node for now
-        if keyword not in self.rel_map:
-            return []
-        texts = []
-        for obj, rel in self.rel_map[keyword]:
-            texts.append(str((keyword, rel, obj)))
-        return texts
-
-    def get_rel_map_tuples(self, keyword: str) -> List[Tuple[str, str]]:
-        """Get the corresponding knowledge for a given keyword."""
-        # NOTE: return a single node for now
-        if keyword not in self.rel_map:
-            return []
-        return self.rel_map[keyword]
-
-    def get_node_ids(self, keyword: str, depth: int = 1) -> List[str]:
-        """Get the corresponding knowledge for a given keyword."""
-        if depth > 1:
-            raise ValueError("Depth > 1 not supported yet.")
-        if keyword not in self.table:
-            return []
-        keywords = [keyword]
-        # some keywords may correspond to a leaf node, may not be in rel_map
-        if keyword in self.rel_map:
-            keywords.extend([child for child, _ in self.rel_map[keyword]])
-
-        node_ids: List[str] = []
-        for keyword in keywords:
-            for node_id in self.table.get(keyword, set()):
-                node_ids.append(node_id)
-            # TODO: Traverse (with depth > 1)
-        return node_ids
-
-    @classmethod
-    def get_type(cls) -> IndexStructType:
-        """Get type."""
-        return IndexStructType.KG
-
-
-@dataclass
-class EmptyIndex(IndexDict):
-    """Empty index."""
-
-    @classmethod
-    def get_type(cls) -> IndexStructType:
-        """Get type."""
-        return IndexStructType.EMPTY
+    def _insert(self, nodes: Sequence[Node], **insert_kwargs: Any) -> None:
+        """Insert nodes."""
+        for n in nodes:
+            keywords = self._extract_keywords(n.get_text())
+            self._index_struct.add_node(list(keywords), n)
+
+    def _delete(self, doc_id: str, **delete_kwargs: Any) -> None:
+        """Delete a document."""
+        # get set of ids that correspond to node
+        node_idxs_to_delete = set()
+        node_id_list = list(self._index_struct.node_ids)
+        nodes = self._docstore.get_nodes(node_id_list)
+        for node_idx, node in zip(node_id_list, nodes):
+            if node.ref_doc_id != doc_id:
+                continue
+            node_idxs_to_delete.add(node_idx)
+        for node_idx in node_idxs_to_delete:
+            self._docstore.delete_document(node_idx)
+
+        # delete node_idxs from keyword to node idxs mapping
+        keywords_to_delete = set()
+        for keyword, node_idxs in self._index_struct.table.items():
+            if node_idxs_to_delete.intersection(node_idxs):
+                self._index_struct.table[keyword] = node_idxs.difference(
+                    node_idxs_to_delete
+                )
+                if not self._index_struct.table[keyword]:
+                    keywords_to_delete.add(keyword)
+
+        for keyword in keywords_to_delete:
+            del self._index_struct.table[keyword]
+
+
+class GPTKeywordTableIndex(BaseGPTKeywordTableIndex):
+    """GPT Keyword Table Index.
+
+    This index uses a GPT model to extract keywords from the text.
+
+    """
+
+    def _extract_keywords(self, text: str) -> Set[str]:
+        """Extract keywords from text."""
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.LLM,
+            payload={"template": self.keyword_extract_template, "text": text},
+        )
+        response, formatted_prompt = self._service_context.llm_predictor.predict(
+            self.keyword_extract_template,
+            text=text,
+        )
+        keywords = extract_keywords_given_response(response, start_token="KEYWORDS:")
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.LLM,
+            payload={"keywords": keywords, "formatted_prompt": formatted_prompt},
+            event_id=event_id,
+        )
+        return keywords
+
+    async def _async_extract_keywords(self, text: str) -> Set[str]:
+        """Extract keywords from text."""
+        event_id = self._service_context.callback_manager.on_event_start(
+            CBEventType.LLM,
+            payload={"template": self.keyword_extract_template, "text": text},
+        )
+        response, formatted_prompt = await self._service_context.llm_predictor.apredict(
+            self.keyword_extract_template,
+            text=text,
+        )
+        keywords = extract_keywords_given_response(response, start_token="KEYWORDS:")
+        self._service_context.callback_manager.on_event_end(
+            CBEventType.LLM,
+            payload={"keywords": keywords, "formatted_prompt": formatted_prompt},
+            event_id=event_id,
+        )
+        return keywords
```

### Comparing `llama_index-0.6.0a7/llama_index/data_structs/node_v2.py` & `llama_index-0.6.1/llama_index/data_structs/node.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/data_structs/registry.py` & `llama_index-0.6.1/llama_index/data_structs/registry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Index registry."""
 
 from typing import Dict, Type
 
-from llama_index.data_structs.data_structs_v2 import (
+from llama_index.data_structs.data_structs import (
     KG,
     EmptyIndex,
     IndexDict,
     IndexGraph,
     IndexList,
     KeywordTable,
-    V2IndexStruct,
+    IndexStruct,
 )
 from llama_index.data_structs.struct_type import IndexStructType
-from llama_index.data_structs.table_v2 import PandasStructTable, SQLStructTable
+from llama_index.data_structs.table import PandasStructTable, SQLStructTable
 
 
-INDEX_STRUCT_TYPE_TO_INDEX_STRUCT_CLASS: Dict[IndexStructType, Type[V2IndexStruct]] = {
+INDEX_STRUCT_TYPE_TO_INDEX_STRUCT_CLASS: Dict[IndexStructType, Type[IndexStruct]] = {
     IndexStructType.TREE: IndexGraph,
     IndexStructType.LIST: IndexList,
     IndexStructType.KEYWORD_TABLE: KeywordTable,
     IndexStructType.VECTOR_STORE: IndexDict,
     IndexStructType.SQL: SQLStructTable,
     IndexStructType.PANDAS: PandasStructTable,
     IndexStructType.KG: KG,
```

### Comparing `llama_index-0.6.0a7/llama_index/data_structs/struct_type.py` & `llama_index-0.6.1/llama_index/data_structs/struct_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,17 @@
             for more information on the Pinecone vector store index.
         DEEPLAKE ("deeplake"): DeepLake Vector Store Index.
             See :ref:`Ref-Indices-VectorStore`
             for more information on the Pinecone vector store index.
         QDRANT ("qdrant"): Qdrant Vector Store Index.
             See :ref:`Ref-Indices-VectorStore`
             for more information on the Qdrant vector store index.
+        LANCEDB ("lancedb"): LanceDB Vector Store Index
+            See :ref:`Ref-Indices-VectorStore`
+            for more information on the LanceDB vector store index.
         MILVUS ("milvus"): Milvus Vector Store Index.
             See :ref:`Ref-Indices-VectorStore`
             for more information on the Milvus vector store index.
         CHROMA ("chroma"): Chroma Vector Store Index.
             See :ref:`Ref-Indices-VectorStore`
             for more information on the Chroma vector store index.
         OPENSEARCH ("opensearch"): Opensearch Vector Store Index.
@@ -62,14 +65,15 @@
     # faiss
     DICT = "dict"
     # simple
     SIMPLE_DICT = "simple_dict"
     WEAVIATE = "weaviate"
     PINECONE = "pinecone"
     QDRANT = "qdrant"
+    LANCEDB = "lancedb"
     MILVUS = "milvus"
     CHROMA = "chroma"
     MYSCALE = "myscale"
     VECTOR_STORE = "vector_store"
     OPENSEARCH = "opensearch"
     CHATGPT_RETRIEVAL_PLUGIN = "chatgpt_retrieval_plugin"
     DEEPLAKE = "deeplake"
```

### Comparing `llama_index-0.6.0a7/llama_index/data_structs/table.py` & `llama_index-0.6.1/llama_index/data_structs/table.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from dataclasses import dataclass, field
 from typing import Any, Dict
 
 from dataclasses_json import DataClassJsonMixin
 
 from llama_index.data_structs.data_structs import IndexStruct
+from llama_index.data_structs.struct_type import IndexStructType
 
 
 @dataclass
 class StructDatapoint(DataClassJsonMixin):
     """Struct outputs."""
 
     # map from field name to StructValue
@@ -24,21 +25,21 @@
 @dataclass
 class SQLStructTable(BaseStructTable):
     """SQL struct outputs."""
 
     context_dict: Dict[str, str] = field(default_factory=dict)
 
     @classmethod
-    def get_type(cls) -> str:
+    def get_type(cls) -> IndexStructType:
         """Get type."""
         # TODO: consolidate with IndexStructType
-        return "sql"
+        return IndexStructType.SQL
 
 
 @dataclass
 class PandasStructTable(BaseStructTable):
     """Pandas struct outputs."""
 
     @classmethod
-    def get_type(cls) -> str:
+    def get_type(cls) -> IndexStructType:
         """Get type."""
-        return "pandas"
+        return IndexStructType.PANDAS
```

### Comparing `llama_index-0.6.0a7/llama_index/embeddings/base.py` & `llama_index-0.6.1/llama_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/embeddings/google.py` & `llama_index-0.6.1/llama_index/embeddings/google.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/embeddings/langchain.py` & `llama_index-0.6.1/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/embeddings/openai.py` & `llama_index-0.6.1/llama_index/embeddings/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     https://github.com/openai/openai-python/blob/main/openai/embeddings_utils.py
 
     Copied here to avoid importing unnecessary dependencies
     like matplotlib, plotly, scipy, sklearn.
 
     """
     text = text.replace("\n", " ")
-    return openai.Embedding.create(input=[text], engine=engine)["data"][0]["embedding"]
+    return openai.Embedding.create(input=[text], model=engine)["data"][0]["embedding"]
 
 
 @retry(wait=wait_random_exponential(min=1, max=20), stop=stop_after_attempt(6))
 async def aget_embedding(text: str, engine: Optional[str] = None) -> List[float]:
     """Asynchronously get embedding.
 
     NOTE: Copied from OpenAI's embedding utils:
@@ -116,15 +116,15 @@
     Copied here to avoid importing unnecessary dependencies
     like matplotlib, plotly, scipy, sklearn.
 
     """
     # replace newlines, which can negatively affect performance.
     text = text.replace("\n", " ")
 
-    return (await openai.Embedding.acreate(input=[text], engine=engine))["data"][0][
+    return (await openai.Embedding.acreate(input=[text], model=engine))["data"][0][
         "embedding"
     ]
 
 
 @retry(wait=wait_random_exponential(min=1, max=20), stop=stop_after_attempt(6))
 def get_embeddings(
     list_of_text: List[str],
@@ -140,16 +140,15 @@
 
     """
     assert len(list_of_text) <= 2048, "The batch size should not be larger than 2048."
 
     # replace newlines, which can negatively affect performance.
     list_of_text = [text.replace("\n", " ") for text in list_of_text]
 
-    data = openai.Embedding.create(input=list_of_text, engine=engine).data
-    data = sorted(data, key=lambda x: x["index"])  # maintain the same order as input.
+    data = openai.Embedding.create(input=list_of_text, model=engine).data
     return [d["embedding"] for d in data]
 
 
 @retry(wait=wait_random_exponential(min=1, max=20), stop=stop_after_attempt(6))
 async def aget_embeddings(
     list_of_text: List[str], engine: Optional[str] = None
 ) -> List[List[float]]:
@@ -163,16 +162,15 @@
 
     """
     assert len(list_of_text) <= 2048, "The batch size should not be larger than 2048."
 
     # replace newlines, which can negatively affect performance.
     list_of_text = [text.replace("\n", " ") for text in list_of_text]
 
-    data = (await openai.Embedding.acreate(input=list_of_text, engine=engine)).data
-    data = sorted(data, key=lambda x: x["index"])  # maintain the same order as input.
+    data = (await openai.Embedding.acreate(input=list_of_text, model=engine)).data
     return [d["embedding"] for d in data]
 
 
 class OpenAIEmbedding(BaseEmbedding):
     """OpenAI class for embeddings.
 
     Args:
```

### Comparing `llama_index-0.6.0a7/llama_index/embeddings/utils.py` & `llama_index-0.6.1/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/evaluation/base.py` & `llama_index-0.6.1/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/evaluation/dataset_generation.py` & `llama_index-0.6.1/llama_index/evaluation/dataset_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Document,
     GPTListIndex,
     QuestionAnswerPrompt,
     ServiceContext,
     LLMPredictor,
 )
 from llama_index.indices.postprocessor.node import KeywordNodePostprocessor
-from llama_index.data_structs.node_v2 import Node, NodeWithScore
+from llama_index.data_structs.node import Node, NodeWithScore
 
 from langchain.chat_models import ChatOpenAI
 
 DEFAULT_QUESTION_GENERATION_PROMPT = """Context information is below.\n"
 "\n---------------------\n{context_str}\n---------------------\n"
 "Given the context information and not prior knowledge.\n"
 "generate only questions based on the below query.\n"
```

### Comparing `llama_index-0.6.0a7/llama_index/img_utils.py` & `llama_index-0.6.1/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/__init__.py` & `llama_index-0.6.1/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/base.py` & `llama_index-0.6.1/llama_index/indices/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Base index classes."""
 import logging
 from abc import ABC, abstractmethod
 from typing import Any, Generic, List, Optional, Sequence, Type, TypeVar
 
 from llama_index.callbacks.schema import CBEventType
-from llama_index.data_structs.data_structs_v2 import V2IndexStruct
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.data_structs import IndexStruct
+from llama_index.data_structs.node import Node
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.service_context import ServiceContext
 from llama_index.readers.schema.base import Document
 from llama_index.storage.docstore.types import BaseDocumentStore
 from llama_index.storage.storage_context import StorageContext
 from llama_index.token_counter.token_counter import llm_token_counter
 
-IS = TypeVar("IS", bound=V2IndexStruct)
+IS = TypeVar("IS", bound=IndexStruct)
 IndexType = TypeVar("IndexType", bound="BaseGPTIndex")
 
 logger = logging.getLogger(__name__)
 
 
 class BaseGPTIndex(Generic[IS], ABC):
     """Base LlamaIndex.
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/base_retriever.py` & `llama_index-0.6.1/llama_index/indices/base_retriever.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from typing import List
-from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.data_structs.node import NodeWithScore
 
 from llama_index.indices.query.schema import QueryBundle, QueryType
 
 
 class BaseRetriever(ABC):
     """Base retriever."""
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/common/struct_store/base.py` & `llama_index-0.6.1/llama_index/indices/common/struct_store/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Common classes for structured operations."""
 
 import logging
 from abc import abstractmethod
 from typing import Any, Callable, Dict, List, Optional, Sequence, cast
 
 from llama_index.callbacks.schema import CBEventType
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 from llama_index.data_structs.table import StructDatapoint
 from llama_index.indices.response.response_builder import get_response_builder
 from llama_index.indices.service_context import ServiceContext
 from llama_index.langchain_helpers.chain_wrapper import LLMPredictor
 from llama_index.langchain_helpers.sql_wrapper import SQLDatabase
 from llama_index.langchain_helpers.text_splitter import TextSplitter
 from llama_index.prompts.default_prompt_selectors import (
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/common/struct_store/schema.py` & `llama_index-0.6.1/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/common/struct_store/sql.py` & `llama_index-0.6.1/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/common_tree/base.py` & `llama_index-0.6.1/llama_index/indices/common_tree/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 import asyncio
 import logging
 from typing import Dict, List, Optional, Sequence, Tuple
 
 from llama_index.async_utils import run_async_tasks
 from llama_index.callbacks.schema import CBEventType
-from llama_index.data_structs.data_structs_v2 import IndexGraph
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.data_structs import IndexGraph
+from llama_index.data_structs.node import Node
 from llama_index.storage.docstore import BaseDocumentStore
 from llama_index.storage.docstore.registry import get_default_docstore
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.utils import get_sorted_node_list, truncate_text
 from llama_index.prompts.prompts import SummaryPrompt
 
 logger = logging.getLogger(__name__)
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/composability/graph.py` & `llama_index-0.6.1/llama_index/indices/composability/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Composability graphs."""
 
 from typing import Any, Dict, List, Optional, Sequence, Type, cast
 
-from llama_index.data_structs.data_structs_v2 import V2IndexStruct
-from llama_index.data_structs.node_v2 import IndexNode, DocumentRelationship
+from llama_index.data_structs.data_structs import IndexStruct
+from llama_index.data_structs.node import IndexNode, DocumentRelationship
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.service_context import ServiceContext
 
 
 class ComposableGraph:
     """Composable graph."""
@@ -30,15 +30,15 @@
         return self._all_indices
 
     @property
     def root_index(self) -> BaseGPTIndex:
         return self._all_indices[self._root_id]
 
     @property
-    def index_struct(self) -> V2IndexStruct:
+    def index_struct(self) -> IndexStruct:
         return self._all_indices[self._root_id].index_struct
 
     @property
     def service_context(self) -> ServiceContext:
         return self._all_indices[self._root_id].service_context
 
     @classmethod
@@ -69,15 +69,15 @@
 
         if len(children_indices) != len(index_summaries):
             raise ValueError("indices and index_summaries must have same length!")
 
         # construct index nodes
         index_nodes = []
         for index, summary in zip(children_indices, index_summaries):
-            assert isinstance(index.index_struct, V2IndexStruct)
+            assert isinstance(index.index_struct, IndexStruct)
             index_node = IndexNode(
                 text=summary,
                 index_id=index.index_id,
                 relationships={DocumentRelationship.SOURCE: index.index_id},
             )
             index_nodes.append(index_node)
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/empty/base.py` & `llama_index-0.6.1/llama_index/indices/empty/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 An index that doesn't contain any documents. Can only be used for
 pure LLM calls.
 
 """
 
 from typing import Any, Optional, Sequence
 
-from llama_index.data_structs.data_structs_v2 import EmptyIndex
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.data_structs import EmptyIndex
+from llama_index.data_structs.node import Node
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.service_context import ServiceContext
 
 
 class GPTEmptyIndex(BaseGPTIndex[EmptyIndex]):
     """GPT Empty Index.
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/empty/retrievers.py` & `llama_index-0.6.1/llama_index/indices/empty/retrievers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Default query for GPTEmptyIndex."""
 from typing import Any, List, Optional
 from llama_index.indices.base_retriever import BaseRetriever
 
-from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.data_structs.node import NodeWithScore
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.prompts.default_prompts import DEFAULT_SIMPLE_INPUT_PROMPT
 from llama_index.prompts.prompts import SimpleInputPrompt
 
 from llama_index.indices.empty.base import GPTEmptyIndex
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/keyword_table/__init__.py` & `llama_index-0.6.1/llama_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/keyword_table/rake_base.py` & `llama_index-0.6.1/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/keyword_table/retrievers.py` & `llama_index-0.6.1/llama_index/indices/keyword_table/retrievers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Query for GPTKeywordTableIndex."""
 import logging
 from abc import abstractmethod
 from collections import defaultdict
 from typing import Any, Dict, List, Optional
 
 from llama_index.callbacks.schema import CBEventType
-from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.data_structs.node import NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.keyword_table.base import (
     BaseGPTKeywordTableIndex,
 )
 from llama_index.indices.keyword_table.utils import (
     extract_keywords_given_response,
     rake_extract_keywords,
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/keyword_table/simple_base.py` & `llama_index-0.6.1/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/keyword_table/utils.py` & `llama_index-0.6.1/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/knowledge_graph/base.py` & `llama_index-0.6.1/llama_index/indices/knowledge_graph/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 """
 
 import logging
 from typing import Any, List, Optional, Sequence, Tuple
 
 from llama_index.callbacks.schema import CBEventType
-from llama_index.data_structs.data_structs_v2 import KG
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.data_structs import KG
+from llama_index.data_structs.node import Node
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.prompts.default_prompts import (
     DEFAULT_KG_TRIPLET_EXTRACT_PROMPT,
     DEFAULT_QUERY_KEYWORD_EXTRACT_TEMPLATE,
 )
 from llama_index.prompts.prompts import KnowledgeGraphPrompt
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/knowledge_graph/retrievers.py` & `llama_index-0.6.1/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Query for GPTKGTableIndex."""
 import logging
 from collections import defaultdict
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
 from llama_index.callbacks.schema import CBEventType
-from llama_index.data_structs.node_v2 import Node, NodeWithScore
+from llama_index.data_structs.node import Node, NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.keyword_table.utils import extract_keywords_given_response
 from llama_index.indices.knowledge_graph.base import GPTKnowledgeGraphIndex
 from llama_index.indices.query.embedding_utils import (
     get_top_k_embeddings,
 )
 from llama_index.indices.query.schema import QueryBundle
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/list/base.py` & `llama_index-0.6.1/llama_index/indices/list/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 in sequence in order to answer a given query.
 
 """
 
 from enum import Enum
 from typing import Any, Optional, Sequence, Union
 
-from llama_index.data_structs.data_structs_v2 import IndexList
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.data_structs import IndexList
+from llama_index.data_structs.node import Node
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.service_context import ServiceContext
 
 
 class ListRetrieverMode(str, Enum):
     DEFAULT = "default"
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/list/retrievers.py` & `llama_index-0.6.1/llama_index/indices/list/retrievers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Default query for GPTListIndex."""
 import logging
 from typing import Any, List, Optional, Tuple
 
 from llama_index.callbacks.schema import CBEventType
-from llama_index.data_structs.node_v2 import Node, NodeWithScore
+from llama_index.data_structs.node import Node, NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.embedding_utils import (
     get_top_k_embeddings,
 )
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.list.base import GPTListIndex
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/loading.py` & `llama_index-0.6.1/llama_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/postprocessor/node.py` & `llama_index-0.6.1/llama_index/indices/postprocessor/node.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,47 +3,51 @@
 import re
 from abc import abstractmethod
 from typing import Dict, List, Optional, cast
 
 from pydantic import BaseModel, Field, validator
 
 import logging
+from llama_index.indices.postprocessor.types import BaseNodePostprocessor
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.response.type import ResponseMode
 from llama_index.indices.service_context import ServiceContext
 from llama_index.prompts.prompts import QuestionAnswerPrompt, RefinePrompt
 from llama_index.storage.docstore import BaseDocumentStore
-from llama_index.data_structs.node_v2 import DocumentRelationship, NodeWithScore
-from llama_index.indices.postprocessor.base import BasePostprocessor
+from llama_index.data_structs.node import DocumentRelationship, NodeWithScore
 from llama_index.indices.response.response_builder import get_response_builder
 
 logger = logging.getLogger(__name__)
 
 
-class BaseNodePostprocessor(BasePostprocessor, BaseModel):
+class BasePydanticNodePostprocessor(BaseModel, BaseNodePostprocessor):
     """Node postprocessor."""
 
     class Config:
         arbitrary_types_allowed = True
 
     @abstractmethod
     def postprocess_nodes(
-        self, nodes: List[NodeWithScore], extra_info: Optional[Dict] = None
+        self,
+        nodes: List[NodeWithScore],
+        query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
         """Postprocess nodes."""
 
 
-class KeywordNodePostprocessor(BaseNodePostprocessor):
+class KeywordNodePostprocessor(BasePydanticNodePostprocessor):
     """Keyword-based Node processor."""
 
     required_keywords: List[str] = Field(default_factory=list)
     exclude_keywords: List[str] = Field(default_factory=list)
 
     def postprocess_nodes(
-        self, nodes: List[NodeWithScore], extra_info: Optional[Dict] = None
+        self,
+        nodes: List[NodeWithScore],
+        query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
         """Postprocess nodes."""
         new_nodes = []
         for node_with_score in nodes:
             node = node_with_score.node
             should_use_node = True
             if self.required_keywords is not None:
@@ -62,24 +66,25 @@
 
             if should_use_node:
                 new_nodes.append(node_with_score)
 
         return new_nodes
 
 
-class SimilarityPostprocessor(BaseNodePostprocessor):
+class SimilarityPostprocessor(BasePydanticNodePostprocessor):
     """Similarity-based Node processor."""
 
     similarity_cutoff: float = Field(default=None)
 
     def postprocess_nodes(
-        self, nodes: List[NodeWithScore], extra_info: Optional[Dict] = None
+        self,
+        nodes: List[NodeWithScore],
+        query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
         """Postprocess nodes."""
-        extra_info = extra_info or {}
         sim_cutoff_exists = self.similarity_cutoff is not None
 
         new_nodes = []
         for node in nodes:
             should_use_node = True
             if sim_cutoff_exists:
                 similarity = node.score
@@ -132,15 +137,15 @@
             break
         nodes[prev_node.get_doc_id()] = NodeWithScore(prev_node)
         node = prev_node
         cur_count += 1
     return nodes
 
 
-class PrevNextNodePostprocessor(BaseNodePostprocessor):
+class PrevNextNodePostprocessor(BasePydanticNodePostprocessor):
     """Previous/Next Node post-processor.
 
     Allows users to fetch additional nodes from the document store,
     based on the relationships of the nodes.
 
     NOTE: this is a beta feature.
 
@@ -160,15 +165,17 @@
     def _validate_mode(cls, v: str) -> str:
         """Validate mode."""
         if v not in ["next", "previous", "both"]:
             raise ValueError(f"Invalid mode: {v}")
         return v
 
     def postprocess_nodes(
-        self, nodes: List[NodeWithScore], extra_info: Optional[Dict] = None
+        self,
+        nodes: List[NodeWithScore],
+        query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
         """Postprocess nodes."""
         all_nodes: Dict[str, NodeWithScore] = {}
         for node in nodes:
             all_nodes[node.node.get_doc_id()] = node
             if self.mode == "next":
                 all_nodes.update(get_forward_nodes(node, self.num_nodes, self.docstore))
@@ -222,15 +229,15 @@
     "Context: {context_msg}\n"
     "Question: {query_str}\n"
     "Existing Answer: {existing_answer}\n"
     "Answer: "
 )
 
 
-class AutoPrevNextNodePostprocessor(BaseNodePostprocessor):
+class AutoPrevNextNodePostprocessor(BasePydanticNodePostprocessor):
     """Previous/Next Node post-processor.
 
     Allows users to fetch additional nodes from the document store,
     based on the prev/next relationships of the nodes.
 
     NOTE: difference with PrevNextPostprocessor is that
     this infers forward/backwards direction.
@@ -266,21 +273,21 @@
         elif "next" in pred:
             return "next"
         elif "none" in pred:
             return "none"
         raise ValueError(f"Invalid prediction: {raw_pred}")
 
     def postprocess_nodes(
-        self, nodes: List[NodeWithScore], extra_info: Optional[Dict] = None
+        self,
+        nodes: List[NodeWithScore],
+        query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
         """Postprocess nodes."""
-        if extra_info is None or "query_bundle" not in extra_info:
-            raise ValueError("Missing query bundle in extra info.")
-
-        query_bundle = cast(QueryBundle, extra_info["query_bundle"])
+        if query_bundle is None:
+            raise ValueError("Missing query bundle.")
 
         infer_prev_next_prompt = QuestionAnswerPrompt(
             self.infer_prev_next_tmpl,
         )
         refine_infer_prev_next_prompt = RefinePrompt(self.refine_prev_next_tmpl)
 
         all_nodes: Dict[str, NodeWithScore] = {}
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/postprocessor/node_recency.py` & `llama_index-0.6.1/llama_index/indices/postprocessor/node_recency.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Node recency post-processor."""
 
-from llama_index.indices.postprocessor.node import BaseNodePostprocessor
+from llama_index.indices.postprocessor.node import BasePydanticNodePostprocessor
+from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.service_context import ServiceContext
-from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.data_structs.node import NodeWithScore
 from pydantic import Field
-from typing import Optional, Dict, List, Set
+from typing import Optional, List, Set
 import pandas as pd
 import numpy as np
 from datetime import datetime
 
 
 # NOTE: currently not being used
 # DEFAULT_INFER_RECENCY_TMPL = (
@@ -35,15 +36,15 @@
 #         return True
 #     elif "NO" in pred:
 #         return False
 #     else:
 #         raise ValueError(f"Invalid recency prediction: {pred}.")
 
 
-class FixedRecencyPostprocessor(BaseNodePostprocessor):
+class FixedRecencyPostprocessor(BasePydanticNodePostprocessor):
     """Recency post-processor.
 
     This post-processor does the following steps:
 
     - Decides if we need to use the post-processor given the query
       (is it temporal-related?)
     - If yes, sorts nodes by date.
@@ -55,19 +56,21 @@
     top_k: int = 1
     # infer_recency_tmpl: str = Field(default=DEFAULT_INFER_RECENCY_TMPL)
     date_key: str = "date"
     # if false, then search node info
     in_extra_info: bool = True
 
     def postprocess_nodes(
-        self, nodes: List[NodeWithScore], extra_info: Optional[Dict] = None
+        self,
+        nodes: List[NodeWithScore],
+        query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
         """Postprocess nodes."""
 
-        if extra_info is None or "query_bundle" not in extra_info:
+        if query_bundle is None:
             raise ValueError("Missing query bundle in extra info.")
 
         # query_bundle = cast(QueryBundle, extra_info["query_bundle"])
         # infer_recency_prompt = SimpleInputPrompt(self.infer_recency_tmpl)
         # raw_pred, _ = self.service_context.llm_predictor.predict(
         #     prompt=infer_recency_prompt,
         #     query_str=query_bundle.query_str,
@@ -96,15 +99,15 @@
     "Given the document, we wish to find documents that contain \n"
     "similar context. Note that these documents are older "
     "than the current document, meaning that certain details may be changed. \n"
     "However, the high-level context should be similar.\n"
 )
 
 
-class EmbeddingRecencyPostprocessor(BaseNodePostprocessor):
+class EmbeddingRecencyPostprocessor(BasePydanticNodePostprocessor):
     """Recency post-processor.
 
     This post-processor does the following steps:
 
     - Decides if we need to use the post-processor given the query
       (is it temporal-related?)
     - If yes, sorts nodes by date.
@@ -119,19 +122,21 @@
     date_key: str = "date"
     # if false, then search node info
     in_extra_info: bool = True
     similarity_cutoff: float = Field(default=0.7)
     query_embedding_tmpl: str = Field(default=DEFAULT_QUERY_EMBEDDING_TMPL)
 
     def postprocess_nodes(
-        self, nodes: List[NodeWithScore], extra_info: Optional[Dict] = None
+        self,
+        nodes: List[NodeWithScore],
+        query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
         """Postprocess nodes."""
 
-        if extra_info is None or "query_bundle" not in extra_info:
+        if query_bundle is None:
             raise ValueError("Missing query bundle in extra info.")
 
         # query_bundle = cast(QueryBundle, extra_info["query_bundle"])
         # infer_recency_prompt = SimpleInputPrompt(self.infer_recency_tmpl)
         # raw_pred, _ = self.service_context.llm_predictor.predict(
         #     prompt=infer_recency_prompt,
         #     query_str=query_bundle.query_str,
@@ -183,33 +188,34 @@
         return [
             node
             for node in sorted_nodes
             if node.node.get_doc_id() not in node_ids_to_skip
         ]
 
 
-class TimeWeightedPostprocessor(BaseNodePostprocessor):
+class TimeWeightedPostprocessor(BasePydanticNodePostprocessor):
     """Time-weighted post-processor.
 
     Reranks a set of nodes based on their recency.
 
     """
 
     time_decay: float = Field(default=0.99)
     last_accessed_key: str = "__last_accessed__"
     time_access_refresh: bool = True
     # optionally set now (makes it easier to test)
     now: Optional[float] = None
     top_k: int = 1
 
     def postprocess_nodes(
-        self, nodes: List[NodeWithScore], extra_info: Optional[Dict] = None
+        self,
+        nodes: List[NodeWithScore],
+        query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
         """Postprocess nodes."""
-        extra_info = extra_info or {}
         now = self.now or datetime.now().timestamp()
         # TODO: refactor with get_top_k_embeddings
 
         similarities = []
         for node_with_score in nodes:
             # embedding similarity score
             score = node_with_score.score or 1.0
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/postprocessor/pii.py` & `llama_index-0.6.1/llama_index/indices/postprocessor/pii.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """PII postprocessor."""
 
-from llama_index.indices.postprocessor.node import BaseNodePostprocessor
-from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.indices.postprocessor.node import BasePydanticNodePostprocessor
+from llama_index.data_structs.node import NodeWithScore
 from typing import List, Optional, Dict, Tuple, Callable
+from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.service_context import ServiceContext
 from llama_index.prompts.prompts import QuestionAnswerPrompt
 from copy import deepcopy
 import json
 
 
 DEFAULT_PII_TMPL = (
@@ -33,15 +34,15 @@
     "Context:\n{context_str}\n"
     "Task: {query_str}\n"
     "Output: \n"
     ""
 )
 
 
-class PIINodePostprocessor(BaseNodePostprocessor):
+class PIINodePostprocessor(BasePydanticNodePostprocessor):
     """PII Node processor.
 
     NOTE: the ServiceContext should contain a LOCAL model, not an external API.
 
     NOTE: this is a beta feature, the API might change.
 
     Args:
@@ -68,15 +69,17 @@
         splits = response.split("Output Mapping:")
         text_output = splits[0].strip()
         json_str_output = splits[1].strip()
         json_dict = json.loads(json_str_output)
         return text_output, json_dict
 
     def postprocess_nodes(
-        self, nodes: List[NodeWithScore], extra_info: Optional[Dict] = None
+        self,
+        nodes: List[NodeWithScore],
+        query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
         """Postprocess nodes."""
         # swap out text from nodes, with the original node mappings
         new_nodes = []
         for node_with_score in nodes:
             node = node_with_score.node
             new_text, mapping_info = self.mask_pii(node.get_text())
@@ -85,15 +88,15 @@
             new_node.node_info[self.pii_node_info_key] = mapping_info
             new_node.text = new_text
             new_nodes.append(NodeWithScore(new_node, node_with_score.score))
 
         return new_nodes
 
 
-class NERPIINodePostprocessor(BaseNodePostprocessor):
+class NERPIINodePostprocessor(BasePydanticNodePostprocessor):
     """NER PII Node processor.
 
     Uses a HF transformers model.
 
     """
 
     pii_node_info_key: str = "__pii_node_info__"
@@ -106,15 +109,17 @@
         for entry in response:
             entity_group_tag = f"[{entry['entity_group']}_{entry['start']}]"
             new_text = new_text.replace(entry["word"], entity_group_tag).strip()
             mapping[entity_group_tag] = entry["word"]
         return new_text, mapping
 
     def postprocess_nodes(
-        self, nodes: List[NodeWithScore], extra_info: Optional[Dict] = None
+        self,
+        nodes: List[NodeWithScore],
+        query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
         """Postprocess nodes."""
         from transformers import pipeline
 
         ner = pipeline("ner", grouped_entities=True)
 
         # swap out text from nodes, with the original node mappings
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/prompt_helper.py` & `llama_index-0.6.1/llama_index/indices/prompt_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 structs but keeping token limitations in mind.
 
 """
 
 from typing import Callable, List, Optional, Sequence
 
 from llama_index.constants import MAX_CHUNK_OVERLAP
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 from llama_index.langchain_helpers.chain_wrapper import LLMPredictor
 from llama_index.langchain_helpers.text_splitter import TokenTextSplitter
 from llama_index.prompts.base import Prompt
 from llama_index.utils import globals_helper
 
 
 class PromptHelper:
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/query/base.py` & `llama_index-0.6.1/llama_index/indices/query/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Base query engine."""
 
 import logging
 from abc import ABC, abstractmethod
 from typing import List, Optional, Sequence
-from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.data_structs.node import NodeWithScore
 
 from llama_index.indices.query.schema import QueryBundle, QueryType
 from llama_index.response.schema import (
     RESPONSE_TYPE,
 )
 
 logger = logging.getLogger(__name__)
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/query/embedding_utils.py` & `llama_index-0.6.1/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/query/query_transform/base.py` & `llama_index-0.6.1/llama_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/query/query_transform/prompts.py` & `llama_index-0.6.1/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/query/response_synthesis.py` & `llama_index-0.6.1/llama_index/indices/query/response_synthesis.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     Dict,
     Generator,
     List,
     Optional,
     Sequence,
 )
 
-from llama_index.data_structs.node_v2 import Node, NodeWithScore
-from llama_index.indices.postprocessor.node import BaseNodePostprocessor
+from llama_index.data_structs.node import Node, NodeWithScore
+from llama_index.indices.postprocessor.types import BaseNodePostprocessor
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.response.response_builder import (
     BaseResponseBuilder,
     ResponseMode,
     get_response_builder,
 )
 from llama_index.indices.service_context import ServiceContext
@@ -154,17 +154,15 @@
     def synthesize(
         self,
         query_bundle: QueryBundle,
         nodes: List[NodeWithScore],
         additional_source_nodes: Optional[Sequence[NodeWithScore]] = None,
     ) -> RESPONSE_TYPE:
         for node_processor in self._node_postprocessors:
-            nodes = node_processor.postprocess_nodes(
-                nodes, {"query_bundle": query_bundle}
-            )
+            nodes = node_processor.postprocess_nodes(nodes, query_bundle)
 
         text_chunks = []
         for node_with_score in nodes:
             text = node_with_score.node.get_text()
             if self._optimizer is not None:
                 text = self._optimizer.optimize(query_bundle, text)
             text_chunks.append(text)
@@ -187,17 +185,15 @@
     async def asynthesize(
         self,
         query_bundle: QueryBundle,
         nodes: List[NodeWithScore],
         additional_source_nodes: Optional[Sequence[NodeWithScore]] = None,
     ) -> RESPONSE_TYPE:
         for node_processor in self._node_postprocessors:
-            nodes = node_processor.postprocess_nodes(
-                nodes, {"query_bundle": query_bundle}
-            )
+            nodes = node_processor.postprocess_nodes(nodes, query_bundle)
 
         text_chunks = []
         for node_with_score in nodes:
             text = node_with_score.node.get_text()
             if self._optimizer is not None:
                 text = self._optimizer.optimize(query_bundle, text)
             text_chunks.append(text)
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/query/schema.py` & `llama_index-0.6.1/llama_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/registry.py` & `llama_index-0.6.1/llama_index/indices/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """Index registry."""
 
 from typing import Dict, Type
 
-from llama_index.data_structs.data_structs_v2 import (
+from llama_index.data_structs.data_structs import (
     KG,
     EmptyIndex,
     IndexDict,
     IndexGraph,
     IndexList,
     KeywordTable,
-    V2IndexStruct,
+    IndexStruct,
 )
 from llama_index.data_structs.struct_type import IndexStructType
-from llama_index.data_structs.table_v2 import PandasStructTable, SQLStructTable
+from llama_index.data_structs.table import PandasStructTable, SQLStructTable
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.indices.empty.base import GPTEmptyIndex
 from llama_index.indices.keyword_table.base import GPTKeywordTableIndex
 from llama_index.indices.knowledge_graph.base import GPTKnowledgeGraphIndex
 from llama_index.indices.list.base import GPTListIndex
 from llama_index.indices.struct_store.pandas import GPTPandasIndex
 from llama_index.indices.struct_store.sql import GPTSQLStructStoreIndex
 from llama_index.indices.tree.base import GPTTreeIndex
 from llama_index.indices.vector_store.base import GPTVectorStoreIndex
 
-INDEX_STRUCT_TYPE_TO_INDEX_STRUCT_CLASS: Dict[IndexStructType, Type[V2IndexStruct]] = {
+INDEX_STRUCT_TYPE_TO_INDEX_STRUCT_CLASS: Dict[IndexStructType, Type[IndexStruct]] = {
     IndexStructType.TREE: IndexGraph,
     IndexStructType.LIST: IndexList,
     IndexStructType.KEYWORD_TABLE: KeywordTable,
     IndexStructType.VECTOR_STORE: IndexDict,
     IndexStructType.SQL: SQLStructTable,
     IndexStructType.PANDAS: PandasStructTable,
     IndexStructType.KG: KG,
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/response/response_builder.py` & `llama_index-0.6.1/llama_index/indices/response/response_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 """
 from abc import ABC, abstractmethod
 import logging
 from typing import Any, Dict, Generator, List, Optional, Sequence, Tuple, cast
 
 from llama_index.callbacks.schema import CBEventType
-from llama_index.data_structs.data_structs_v2 import IndexGraph
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.data_structs import IndexGraph
+from llama_index.data_structs.node import Node
 from llama_index.storage.docstore.registry import get_default_docstore
 from llama_index.indices.common_tree.base import GPTTreeIndexBuilder
 from llama_index.indices.response.type import ResponseMode
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.utils import get_sorted_node_list, truncate_text
 from llama_index.prompts.default_prompt_selectors import DEFAULT_REFINE_PROMPT_SEL
 from llama_index.prompts.default_prompts import (
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/service_context.py` & `llama_index-0.6.1/llama_index/indices/service_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/struct_store/__init__.py` & `llama_index-0.6.1/llama_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/struct_store/base.py` & `llama_index-0.6.1/llama_index/indices/struct_store/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Struct store."""
 
 import re
 from typing import Any, Callable, Dict, Generic, Optional, Sequence, TypeVar
 
-from llama_index.data_structs.node_v2 import Node
-from llama_index.data_structs.table_v2 import BaseStructTable
+from llama_index.data_structs.node import Node
+from llama_index.data_structs.table import BaseStructTable
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.indices.service_context import ServiceContext
 from llama_index.prompts.default_prompts import DEFAULT_SCHEMA_EXTRACT_PROMPT
 from llama_index.prompts.prompts import SchemaExtractPrompt
 
 BST = TypeVar("BST", bound=BaseStructTable)
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/struct_store/container_builder.py` & `llama_index-0.6.1/llama_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/struct_store/pandas.py` & `llama_index-0.6.1/llama_index/indices/struct_store/pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Pandas csv structured store."""
 
 from typing import Any, Optional, Sequence
 
-from llama_index.data_structs.node_v2 import Node
-from llama_index.data_structs.table_v2 import PandasStructTable
+from llama_index.data_structs.node import Node
+from llama_index.data_structs.table import PandasStructTable
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.struct_store.base import BaseGPTStructStoreIndex
 
 import pandas as pd
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/struct_store/pandas_query.py` & `llama_index-0.6.1/llama_index/indices/struct_store/pandas_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/struct_store/sql.py` & `llama_index-0.6.1/llama_index/indices/struct_store/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """SQL Structured Store."""
 from enum import Enum
 from typing import Any, Optional, Sequence, Union
 
 from collections import defaultdict
-from llama_index.data_structs.node_v2 import Node
-from llama_index.data_structs.table_v2 import SQLStructTable
+from llama_index.data_structs.node import Node
+from llama_index.data_structs.table import SQLStructTable
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.common.struct_store.schema import SQLContextContainer
 from llama_index.indices.common.struct_store.sql import SQLStructDatapointExtractor
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.struct_store.base import BaseGPTStructStoreIndex
 from llama_index.indices.struct_store.container_builder import (
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/struct_store/sql_query.py` & `llama_index-0.6.1/llama_index/indices/struct_store/sql_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/tree/__init__.py` & `llama_index-0.6.1/llama_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/indices/tree/all_leaf_retriever.py` & `llama_index-0.6.1/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Summarize query."""
 
 import logging
 from typing import Any, List, cast
 
 
-from llama_index.data_structs.data_structs_v2 import IndexGraph
-from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.data_structs.data_structs import IndexGraph
+from llama_index.data_structs.node import NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.utils import get_sorted_node_list
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_NUM_CHILDREN = 10
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/tree/base.py` & `llama_index-0.6.1/llama_index/indices/tree/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tree-based index."""
 
 from enum import Enum
 from typing import Any, Optional, Sequence, Union
 
 # from llama_index.data_structs.data_structs import IndexGraph
-from llama_index.data_structs.data_structs_v2 import IndexGraph
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.data_structs import IndexGraph
+from llama_index.data_structs.node import Node
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.common_tree.base import GPTTreeIndexBuilder
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.tree.inserter import GPTTreeIndexInserter
 from llama_index.prompts.default_prompts import (
     DEFAULT_INSERT_PROMPT,
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/tree/inserter.py` & `llama_index-0.6.1/llama_index/indices/tree/inserter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """GPT Tree Index inserter."""
 
 from typing import Optional, Sequence
 
-from llama_index.data_structs.data_structs_v2 import IndexGraph
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.data_structs import IndexGraph
+from llama_index.data_structs.node import Node
 from llama_index.storage.docstore import BaseDocumentStore
 from llama_index.storage.docstore.registry import get_default_docstore
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.utils import (
     extract_numbers_given_response,
     get_sorted_node_list,
 )
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/tree/select_leaf_embedding_retriever.py` & `llama_index-0.6.1/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Query Tree using embedding similarity between query and node text."""
 
 import logging
 from typing import Dict, List, Tuple, cast
 
 
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.tree.select_leaf_retriever import (
     TreeSelectLeafRetriever,
 )
 from llama_index.indices.utils import get_sorted_node_list
 
 logger = logging.getLogger(__name__)
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/tree/select_leaf_retriever.py` & `llama_index-0.6.1/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Leaf query mechanism."""
 
 import logging
 from typing import Any, Dict, List, Optional, cast
 
 from langchain.input import print_text
 
-from llama_index.data_structs.node_v2 import Node, NodeWithScore
+from llama_index.data_structs.node import Node, NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.response.response_builder import get_response_builder
 from llama_index.indices.tree.base import GPTTreeIndex
 from llama_index.indices.utils import (
     extract_numbers_given_response,
     get_sorted_node_list,
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/tree/tree_root_retriever.py` & `llama_index-0.6.1/llama_index/indices/tree/tree_root_retriever.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Retrieve query."""
 import logging
 from typing import Any, List
 
-from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.data_structs.node import NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.utils import get_sorted_node_list
 
 logger = logging.getLogger(__name__)
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/utils.py` & `llama_index-0.6.1/llama_index/indices/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Utilities for GPT indices."""
 import logging
 import re
 from typing import Dict, List, Optional, Set
 
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 from llama_index.utils import globals_helper, truncate_text
 from llama_index.vector_stores.types import VectorStoreQueryResult
 
 _logger = logging.getLogger(__name__)
 
 
 def get_sorted_node_list(node_dict: Dict[int, Node]) -> List[Node]:
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/vector_store/base.py` & `llama_index-0.6.1/llama_index/indices/vector_store/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Base vector store index.
 
 An index that that is built on top of an existing vector store.
 
 """
 
-from typing import Any, Dict, List, Optional, Sequence, Set, Tuple
+from typing import Any, Dict, List, Optional, Sequence, Tuple
 
 from llama_index.callbacks.schema import CBEventType
 from llama_index.async_utils import run_async_tasks
-from llama_index.data_structs.data_structs_v2 import IndexDict
-from llama_index.data_structs.node_v2 import ImageNode, IndexNode, Node
+from llama_index.data_structs.data_structs import IndexDict
+from llama_index.data_structs.node import ImageNode, IndexNode, Node
 from llama_index.indices.base import BaseGPTIndex
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.service_context import ServiceContext
 from llama_index.storage.storage_context import StorageContext
 from llama_index.token_counter.token_counter import llm_token_counter
-from llama_index.vector_stores.types import NodeEmbeddingResult, VectorStore
+from llama_index.vector_stores.types import (
+    NodeWithEmbedding,
+    VectorStore,
+)
 
 
 class GPTVectorStoreIndex(BaseGPTIndex[IndexDict]):
     """Base GPT Vector Store Index.
 
     Args:
         use_async (bool): Whether to use asynchronous calls. Defaults to False.
@@ -53,87 +56,74 @@
     def as_retriever(self, **kwargs: Any) -> BaseRetriever:
         # NOTE: lazy import
         from llama_index.indices.vector_store.retrievers import VectorIndexRetriever
 
         return VectorIndexRetriever(self, **kwargs)
 
     def _get_node_embedding_results(
-        self, nodes: Sequence[Node], existing_node_ids: Set
-    ) -> List[NodeEmbeddingResult]:
+        self, nodes: Sequence[Node]
+    ) -> List[NodeWithEmbedding]:
         """Get tuples of id, node, and embedding.
 
         Allows us to store these nodes in a vector store.
         Embeddings are called in batches.
 
         """
-        id_to_node_map: Dict[str, Node] = {}
         id_to_embed_map: Dict[str, List[float]] = {}
 
-        nodes_embedded = 0
         for n in nodes:
-            new_id = n.get_doc_id()
             if n.embedding is None:
-                nodes_embedded += 1
                 self._service_context.embed_model.queue_text_for_embedding(
-                    new_id, n.get_text()
+                    n.get_doc_id(), n.get_text()
                 )
             else:
-                id_to_embed_map[new_id] = n.embedding
+                id_to_embed_map[n.get_doc_id()] = n.embedding
 
-            id_to_node_map[new_id] = n
         event_id = self._service_context.callback_manager.on_event_start(
             CBEventType.EMBEDDING
         )
 
         # call embedding model to get embeddings
         (
             result_ids,
             result_embeddings,
         ) = self._service_context.embed_model.get_queued_text_embeddings()
         self._service_context.callback_manager.on_event_end(
             CBEventType.EMBEDDING,
-            payload={"num_nodes": nodes_embedded},
+            payload={"num_nodes": len(result_ids)},
             event_id=event_id,
         )
         for new_id, text_embedding in zip(result_ids, result_embeddings):
             id_to_embed_map[new_id] = text_embedding
 
-        result_tups = []
-        for id, embed in id_to_embed_map.items():
-            doc_id = id_to_node_map[id].ref_doc_id
-            if doc_id is None:
-                raise ValueError("Reference doc id is None.")
-            result_tups.append(
-                NodeEmbeddingResult(id, id_to_node_map[id], embed, doc_id=doc_id)
-            )
-        return result_tups
+        results = []
+        for node in nodes:
+            embedding = id_to_embed_map[node.get_doc_id()]
+            result = NodeWithEmbedding(node=node, embedding=embedding)
+            results.append(result)
+        return results
 
     async def _aget_node_embedding_results(
         self,
         nodes: Sequence[Node],
-        existing_node_ids: Set,
-    ) -> List[NodeEmbeddingResult]:
+    ) -> List[NodeWithEmbedding]:
         """Asynchronously get tuples of id, node, and embedding.
 
         Allows us to store these nodes in a vector store.
         Embeddings are called in batches.
 
         """
-        id_to_node_map: Dict[str, Node] = {}
         id_to_embed_map: Dict[str, List[float]] = {}
 
         text_queue: List[Tuple[str, str]] = []
         for n in nodes:
-            new_id = n.get_doc_id()
             if n.embedding is None:
-                text_queue.append((new_id, n.get_text()))
+                text_queue.append((n.get_doc_id(), n.get_text()))
             else:
-                id_to_embed_map[new_id] = n.embedding
-
-            id_to_node_map[new_id] = n
+                id_to_embed_map[n.get_doc_id()] = n.embedding
 
         event_id = self._service_context.callback_manager.on_event_start(
             CBEventType.EMBEDDING
         )
 
         # call embedding model to get embeddings
         (
@@ -147,33 +137,26 @@
             CBEventType.EMBEDDING,
             payload={"num_nodes": len(text_queue)},
             event_id=event_id,
         )
         for new_id, text_embedding in zip(result_ids, result_embeddings):
             id_to_embed_map[new_id] = text_embedding
 
-        result_tups = []
-        for id, embed in id_to_embed_map.items():
-            doc_id = id_to_node_map[id].ref_doc_id
-            if doc_id is None:
-                raise ValueError("Reference doc id is None.")
-            result_tups.append(
-                NodeEmbeddingResult(id, id_to_node_map[id], embed, doc_id=doc_id)
-            )
-        return result_tups
+        results = []
+        for node in nodes:
+            embedding = id_to_embed_map[node.get_doc_id()]
+            result = NodeWithEmbedding(node=node, embedding=embedding)
+            results.append(result)
+        return results
 
     async def _async_add_nodes_to_index(
         self, index_struct: IndexDict, nodes: Sequence[Node]
     ) -> None:
         """Asynchronously add nodes to index."""
-        embedding_results = await self._aget_node_embedding_results(
-            nodes,
-            set(),
-        )
-
+        embedding_results = await self._aget_node_embedding_results(nodes)
         new_ids = self._vector_store.add(embedding_results)
 
         # if the vector store doesn't store text, we need to add the nodes to the
         # index struct and document store
         if not self._vector_store.stores_text:
             for result, new_id in zip(embedding_results, new_ids):
                 index_struct.add_node(result.node, text_id=new_id)
@@ -181,19 +164,15 @@
 
     def _add_nodes_to_index(
         self,
         index_struct: IndexDict,
         nodes: Sequence[Node],
     ) -> None:
         """Add document to index."""
-        embedding_results = self._get_node_embedding_results(
-            nodes,
-            set(),
-        )
-
+        embedding_results = self._get_node_embedding_results(nodes)
         new_ids = self._vector_store.add(embedding_results)
 
         if not self._vector_store.stores_text:
             # NOTE: if the vector store doesn't store text,
             # we need to add the nodes to the index struct and document store
             for result, new_id in zip(embedding_results, new_ids):
                 index_struct.add_node(result.node, text_id=new_id)
@@ -235,12 +214,13 @@
         """Insert nodes.
 
         NOTE: overrides BaseGPTIndex.insert_nodes.
             GPTVectorStoreIndex only stores nodes in document store
             if vector store does not store text
         """
         self._insert(nodes, **insert_kwargs)
+        self._storage_context.index_store.add_index_struct(self._index_struct)
 
     def _delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete a document."""
         self._index_struct.delete(doc_id)
         self._vector_store.delete(doc_id)
```

### Comparing `llama_index-0.6.0a7/llama_index/indices/vector_store/retrievers.py` & `llama_index-0.6.1/llama_index/indices/vector_store/retrievers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Base vector store index query."""
 
 
 from typing import Any, List, Optional
 from llama_index.constants import DEFAULT_SIMILARITY_TOP_K
 
 from llama_index.callbacks.schema import CBEventType
-from llama_index.data_structs.data_structs_v2 import IndexDict
-from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.data_structs.data_structs import IndexDict
+from llama_index.data_structs.node import NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.utils import log_vector_store_query_result
 from llama_index.indices.vector_store.base import GPTVectorStoreIndex
 from llama_index.token_counter.token_counter import llm_token_counter
 from llama_index.vector_stores.types import (
     VectorStoreQuery,
```

### Comparing `llama_index-0.6.0a7/llama_index/langchain_helpers/agents/__init__.py` & `llama_index-0.6.1/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/langchain_helpers/agents/agents.py` & `llama_index-0.6.1/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/langchain_helpers/agents/toolkits.py` & `llama_index-0.6.1/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/langchain_helpers/agents/tools.py` & `llama_index-0.6.1/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/langchain_helpers/memory_wrapper.py` & `llama_index-0.6.1/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/langchain_helpers/sql_wrapper.py` & `llama_index-0.6.1/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/langchain_helpers/text_splitter.py` & `llama_index-0.6.1/llama_index/langchain_helpers/text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/llm_predictor/base.py` & `llama_index-0.6.1/llama_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/llm_predictor/chatgpt.py` & `llama_index-0.6.1/llama_index/llm_predictor/chatgpt.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/llm_predictor/stable_lm.py` & `llama_index-0.6.1/llama_index/llm_predictor/stable_lm.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/llm_predictor/structured.py` & `llama_index-0.6.1/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/logger/base.py` & `llama_index-0.6.1/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/node_parser/interface.py` & `llama_index-0.6.1/llama_index/node_parser/interface.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Node parser interface."""
 from typing import List, Sequence
 
 from abc import ABC, abstractmethod
 
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 from llama_index.readers.schema.base import Document
 
 
 class NodeParser(ABC):
     """Base interface for node parser."""
 
     @abstractmethod
```

### Comparing `llama_index-0.6.0a7/llama_index/node_parser/node_utils.py` & `llama_index-0.6.1/llama_index/node_parser/node_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """General node utils."""
 
 
 import logging
 from typing import List
 
-from llama_index.data_structs.node_v2 import DocumentRelationship, ImageNode, Node
+from llama_index.data_structs.node import DocumentRelationship, ImageNode, Node
 from llama_index.langchain_helpers.text_splitter import (
     TextSplit,
     TextSplitter,
     TokenTextSplitter,
 )
 from llama_index.readers.schema.base import ImageDocument
 from llama_index.schema import BaseDocument
```

### Comparing `llama_index-0.6.0a7/llama_index/node_parser/simple.py` & `llama_index-0.6.1/llama_index/node_parser/simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Simple node parser."""
 from typing import List, Optional, Sequence
 
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 from llama_index.langchain_helpers.text_splitter import TextSplitter, TokenTextSplitter
 from llama_index.node_parser.node_utils import get_nodes_from_document
 from llama_index.readers.schema.base import Document
 from llama_index.node_parser.interface import NodeParser
 
 
 class SimpleNodeParser(NodeParser):
```

### Comparing `llama_index-0.6.0a7/llama_index/optimization/optimizer.py` & `llama_index-0.6.1/llama_index/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/output_parsers/base.py` & `llama_index-0.6.1/llama_index/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/output_parsers/guardrails.py` & `llama_index-0.6.1/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/output_parsers/langchain.py` & `llama_index-0.6.1/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/output_parsers/selection.py` & `llama_index-0.6.1/llama_index/output_parsers/selection.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/playground/base.py` & `llama_index-0.6.1/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/prompts/base.py` & `llama_index-0.6.1/llama_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/prompts/chat_prompts.py` & `llama_index-0.6.1/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/prompts/default_prompt_selectors.py` & `llama_index-0.6.1/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/prompts/default_prompts.py` & `llama_index-0.6.1/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/prompts/prompt_type.py` & `llama_index-0.6.1/llama_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/prompts/prompts.py` & `llama_index-0.6.1/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/query_engine/__init__.py` & `llama_index-0.6.1/llama_index/query_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/query_engine/graph_query_engine.py` & `llama_index-0.6.1/llama_index/query_engine/graph_query_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, List, Optional, Tuple
 
-from llama_index.data_structs.node_v2 import IndexNode, Node, NodeWithScore
+from llama_index.data_structs.node import IndexNode, Node, NodeWithScore
 from llama_index.indices.composability.graph import ComposableGraph
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.response.schema import RESPONSE_TYPE
 
 
 class ComposableGraphQueryEngine(BaseQueryEngine):
```

### Comparing `llama_index-0.6.0a7/llama_index/query_engine/multistep_query_engine.py` & `llama_index-0.6.1/llama_index/query_engine/multistep_query_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Any, Callable, Dict, List, Optional, Tuple, cast
-from llama_index.data_structs.node_v2 import Node, NodeWithScore
+from llama_index.data_structs.node import Node, NodeWithScore
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.query.query_transform.base import StepDecomposeQueryTransform
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.query.response_synthesis import ResponseSynthesizer
 from llama_index.response.schema import RESPONSE_TYPE
```

### Comparing `llama_index-0.6.0a7/llama_index/query_engine/retriever_query_engine.py` & `llama_index-0.6.1/llama_index/query_engine/retriever_query_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Optional, Sequence
 
 from llama_index.callbacks.base import CallbackManager
 from llama_index.callbacks.schema import CBEventType
-from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.data_structs.node import NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
-from llama_index.indices.postprocessor.node import BaseNodePostprocessor
+from llama_index.indices.postprocessor.types import BaseNodePostprocessor
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.query.response_synthesis import ResponseSynthesizer
 from llama_index.indices.response.type import ResponseMode
 from llama_index.indices.service_context import ServiceContext
 from llama_index.optimization.optimizer import BaseTokenUsageOptimizer
 from llama_index.prompts.prompts import (
```

### Comparing `llama_index-0.6.0a7/llama_index/query_engine/transform_query_engine.py` & `llama_index-0.6.1/llama_index/query_engine/transform_query_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List, Optional, Sequence
-from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.data_structs.node import NodeWithScore
 from llama_index.indices.query.base import BaseQueryEngine
 from llama_index.indices.query.query_transform.base import BaseQueryTransform
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.response.schema import RESPONSE_TYPE
 
 
 class TransformQueryEngine(BaseQueryEngine):
```

### Comparing `llama_index-0.6.0a7/llama_index/readers/__init__.py` & `llama_index-0.6.1/llama_index/readers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 )
 from llama_index.readers.google_readers.gdocs import GoogleDocsReader
 from llama_index.readers.json import JSONReader
 from llama_index.readers.make_com.wrapper import MakeWrapper
 from llama_index.readers.mbox import MboxReader
 from llama_index.readers.milvus import MilvusReader
 from llama_index.readers.mongo import SimpleMongoReader
+from llama_index.readers.metal import MetalReader
 from llama_index.readers.myscale import MyScaleReader
 from llama_index.readers.notion import NotionPageReader
 from llama_index.readers.obsidian import ObsidianReader
 from llama_index.readers.pinecone import PineconeReader
 from llama_index.readers.qdrant import QdrantReader
 from llama_index.readers.schema.base import Document
 from llama_index.readers.slack import SlackReader
@@ -52,14 +53,15 @@
     "WikipediaReader",
     "YoutubeTranscriptReader",
     "SimpleDirectoryReader",
     "JSONReader",
     "SimpleMongoReader",
     "NotionPageReader",
     "GoogleDocsReader",
+    "MetalReader",
     "DiscordReader",
     "SlackReader",
     "WeaviateReader",
     "PineconeReader",
     "QdrantReader",
     "MilvusReader",
     "ChromaReader",
```

### Comparing `llama_index-0.6.0a7/llama_index/readers/base.py` & `llama_index-0.6.1/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/chatgpt_plugin/base.py` & `llama_index-0.6.1/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/chroma.py` & `llama_index-0.6.1/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/database.py` & `llama_index-0.6.1/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/deeplake.py` & `llama_index-0.6.1/llama_index/readers/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/discord_reader.py` & `llama_index-0.6.1/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/download.py` & `llama_index-0.6.1/llama_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/elasticsearch.py` & `llama_index-0.6.1/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/faiss.py` & `llama_index-0.6.1/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/file/base.py` & `llama_index-0.6.1/llama_index/readers/file/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/file/base_parser.py` & `llama_index-0.6.1/llama_index/readers/file/base_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/file/docs_parser.py` & `llama_index-0.6.1/llama_index/readers/file/docs_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/file/epub_parser.py` & `llama_index-0.6.1/llama_index/readers/file/epub_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/file/image_caption_parser.py` & `llama_index-0.6.1/llama_index/readers/file/image_caption_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/file/image_parser.py` & `llama_index-0.6.1/llama_index/readers/file/image_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/file/image_vision_llm_parser.py` & `llama_index-0.6.1/llama_index/readers/file/image_vision_llm_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/file/ipynb_parser.py` & `llama_index-0.6.1/llama_index/readers/file/ipynb_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/file/markdown_parser.py` & `llama_index-0.6.1/llama_index/readers/file/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/file/mbox_parser.py` & `llama_index-0.6.1/llama_index/readers/file/mbox_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/file/slides_parser.py` & `llama_index-0.6.1/llama_index/readers/file/slides_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/file/tabular_parser.py` & `llama_index-0.6.1/llama_index/readers/file/tabular_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/file/video_audio.py` & `llama_index-0.6.1/llama_index/readers/file/video_audio.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/github_readers/github_api_client.py` & `llama_index-0.6.1/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/github_readers/github_repository_reader.py` & `llama_index-0.6.1/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from llama_index.readers.github_readers.utils import (
     BufferedGitBlobDataIterator,
     get_file_extension,
     print_if_verbose,
 )
 from llama_index.readers.schema.base import Document
 
-logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
 class GithubRepositoryReader(BaseReader):
     """
     Github repository reader.
```

### Comparing `llama_index-0.6.0a7/llama_index/readers/github_readers/utils.py` & `llama_index-0.6.1/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/google_readers/gdocs.py` & `llama_index-0.6.1/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/google_readers/gsheets.py` & `llama_index-0.6.1/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/json.py` & `llama_index-0.6.1/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/make_com/wrapper.py` & `llama_index-0.6.1/llama_index/readers/make_com/wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Currently cannot load documents.
 
 """
 
 from typing import Any, List, Optional
 
 import requests
-from llama_index.data_structs.node_v2 import Node, NodeWithScore
+from llama_index.data_structs.node import Node, NodeWithScore
 
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 from llama_index.response.schema import Response
 
 
 class MakeWrapper(BaseReader):
```

### Comparing `llama_index-0.6.0a7/llama_index/readers/mbox.py` & `llama_index-0.6.1/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/milvus.py` & `llama_index-0.6.1/llama_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/mongo.py` & `llama_index-0.6.1/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/myscale.py` & `llama_index-0.6.1/llama_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/notion.py` & `llama_index-0.6.1/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/obsidian.py` & `llama_index-0.6.1/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/pinecone.py` & `llama_index-0.6.1/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/schema/base.py` & `llama_index-0.6.1/llama_index/readers/schema/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/slack.py` & `llama_index-0.6.1/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/steamship/file_reader.py` & `llama_index-0.6.1/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/string_iterable.py` & `llama_index-0.6.1/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/twitter.py` & `llama_index-0.6.1/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/weaviate/client.py` & `llama_index-0.6.1/llama_index/readers/weaviate/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 """
 
 import json
 from dataclasses import field
 from typing import Any, Dict, List, Optional, cast
 
-from llama_index.data_structs.data_structs_v2 import Node
-from llama_index.data_structs.node_v2 import DocumentRelationship
+from llama_index.data_structs.data_structs import Node
+from llama_index.data_structs.node import DocumentRelationship
 from llama_index.readers.weaviate.utils import (
     get_by_id,
     parse_get_response,
     validate_client,
 )
 from llama_index.utils import get_new_id
 from llama_index.vector_stores.types import VectorStoreQuery, VectorStoreQueryMode
```

### Comparing `llama_index-0.6.0a7/llama_index/readers/weaviate/reader.py` & `llama_index-0.6.1/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/weaviate/utils.py` & `llama_index-0.6.1/llama_index/readers/weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/web.py` & `llama_index-0.6.1/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/wikipedia.py` & `llama_index-0.6.1/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/readers/youtube_transcript.py` & `llama_index-0.6.1/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/response/notebook_utils.py` & `llama_index-0.6.1/llama_index/response/notebook_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Utils for jupyter notebook."""
 from typing import Any, Dict, Tuple
 
 from IPython.display import Markdown, display
-from llama_index.data_structs.node_v2 import ImageNode, NodeWithScore
+from llama_index.data_structs.node import ImageNode, NodeWithScore
 
 from llama_index.img_utils import b64_2_img
 from llama_index.response.schema import Response
 from llama_index.utils import truncate_text
 
 DEFAULT_THUMBNAIL_SIZE = (512, 512)
```

### Comparing `llama_index-0.6.0a7/llama_index/response/schema.py` & `llama_index-0.6.1/llama_index/response/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Response schema."""
 
 from dataclasses import dataclass, field
 from typing import Any, Dict, Generator, List, Optional, Union
 
-from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.data_structs.node import NodeWithScore
 from llama_index.utils import truncate_text
 
 
 @dataclass
 class Response:
     """Response object.
```

### Comparing `llama_index-0.6.0a7/llama_index/retrievers/__init__.py` & `llama_index-0.6.1/llama_index/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/retrievers/transform_retriever.py` & `llama_index-0.6.1/llama_index/retrievers/transform_retriever.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List, Optional
-from llama_index.data_structs.node_v2 import NodeWithScore
+from llama_index.data_structs.node import NodeWithScore
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.query.query_transform.base import BaseQueryTransform
 from llama_index.indices.query.schema import QueryBundle
 
 
 class TransformRetriever(BaseRetriever):
     """Transform Retriever.
```

### Comparing `llama_index-0.6.0a7/llama_index/schema.py` & `llama_index-0.6.1/llama_index/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             self.doc_id = get_new_id(set())
         if self.doc_hash is None:
             self.doc_hash = self._generate_doc_hash()
 
     def _generate_doc_hash(self) -> str:
         """Generate a hash to represent the document."""
         doc_identity = str(self.text) + str(self.extra_info)
-        return sha256(doc_identity.encode()).hexdigest()
+        return sha256(doc_identity.encode("utf-8", "surrogatepass")).hexdigest()
 
     @classmethod
     @abstractmethod
     def get_type(cls) -> str:
         """Get Document type."""
 
     @classmethod
```

### Comparing `llama_index-0.6.0a7/llama_index/selectors/llm_selectors.py` & `llama_index-0.6.1/llama_index/selectors/llm_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/selectors/prompts.py` & `llama_index-0.6.1/llama_index/selectors/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/selectors/types.py` & `llama_index-0.6.1/llama_index/selectors/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/storage/docstore/__init__.py` & `llama_index-0.6.1/llama_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/storage/docstore/keyval_docstore.py` & `llama_index-0.6.1/llama_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/storage/docstore/mongo_docstore.py` & `llama_index-0.6.1/llama_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/storage/docstore/registry.py` & `llama_index-0.6.1/llama_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/storage/docstore/simple_docstore.py` & `llama_index-0.6.1/llama_index/storage/docstore/simple_docstore.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,10 +68,21 @@
         self,
         persist_path: str = DEFAULT_PERSIST_PATH,
     ) -> None:
         """Persist the store."""
         if isinstance(self._kvstore, BaseInMemoryKVStore):
             self._kvstore.persist(persist_path)
 
+    @classmethod
+    def from_dict(
+        cls, save_dict: dict, namespace: Optional[str] = None
+    ) -> "SimpleDocumentStore":
+        simple_kvstore = SimpleKVStore.from_dict(save_dict)
+        return cls(simple_kvstore, namespace)
+
+    def to_dict(self) -> dict:
+        assert isinstance(self._kvstore, SimpleKVStore)
+        return self._kvstore.to_dict()
+
 
 # alias for backwards compatibility
 DocumentStore = SimpleDocumentStore
```

### Comparing `llama_index-0.6.0a7/llama_index/storage/docstore/types.py` & `llama_index-0.6.1/llama_index/storage/docstore/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from typing import Dict, List, Optional, Sequence
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 
 from llama_index.schema import BaseDocument
 import os
 
 
 DEFAULT_PERSIST_FNAME = "docstore.json"
 DEFAULT_PERSIST_DIR = "./storage"
```

### Comparing `llama_index-0.6.0a7/llama_index/storage/docstore/utils.py` & `llama_index-0.6.1/llama_index/storage/docstore/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from llama_index.constants import DATA_KEY, TYPE_KEY
-from llama_index.data_structs.node_v2 import ImageNode, IndexNode, Node
+from llama_index.data_structs.node import ImageNode, IndexNode, Node
 from llama_index.readers.schema.base import Document
 from llama_index.schema import BaseDocument
 
 
 def doc_to_json(doc: BaseDocument) -> dict:
     return {
         DATA_KEY: doc.to_dict(),
```

### Comparing `llama_index-0.6.0a7/llama_index/storage/index_store/keyval_index_store.py` & `llama_index-0.6.1/llama_index/storage/index_store/keyval_index_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List, Optional
-from llama_index.data_structs.data_structs_v2 import V2IndexStruct
+from llama_index.data_structs.data_structs import IndexStruct
 from llama_index.storage.index_store.types import BaseIndexStore
 from llama_index.storage.index_store.utils import (
     index_struct_to_json,
     json_to_index_struct,
 )
 from llama_index.storage.kvstore.types import BaseKVStore
 
@@ -21,19 +21,19 @@
 
     def __init__(self, kvstore: BaseKVStore, namespace: Optional[str] = None) -> None:
         """Init a KVIndexStore."""
         self._kvstore = kvstore
         namespace = namespace or DEFAULT_NAMESPACE
         self._collection = f"{namespace}/data"
 
-    def add_index_struct(self, index_struct: V2IndexStruct) -> None:
+    def add_index_struct(self, index_struct: IndexStruct) -> None:
         """Add an index struct.
 
         Args:
-            index_struct (V2IndexStruct): index struct
+            index_struct (IndexStruct): index struct
 
         """
         key = index_struct.index_id
         data = index_struct_to_json(index_struct)
         self._kvstore.put(key, data, collection=self._collection)
 
     def delete_index_struct(self, key: str) -> None:
@@ -43,15 +43,15 @@
             key (str): index struct key
 
         """
         self._kvstore.delete(key, collection=self._collection)
 
     def get_index_struct(
         self, struct_id: Optional[str] = None
-    ) -> Optional[V2IndexStruct]:
+    ) -> Optional[IndexStruct]:
         """Get an index struct.
 
         Args:
             struct_id (Optional[str]): index struct id
 
         """
         if struct_id is None:
@@ -60,16 +60,16 @@
             return structs[0]
         else:
             json = self._kvstore.get(struct_id, collection=self._collection)
             if json is None:
                 return None
             return json_to_index_struct(json)
 
-    def index_structs(self) -> List[V2IndexStruct]:
+    def index_structs(self) -> List[IndexStruct]:
         """Get all index structs.
 
         Returns:
-            List[V2IndexStruct]: index structs
+            List[IndexStruct]: index structs
 
         """
         jsons = self._kvstore.get_all(collection=self._collection)
         return [json_to_index_struct(json) for json in jsons.values()]
```

### Comparing `llama_index-0.6.0a7/llama_index/storage/index_store/mongo_index_store.py` & `llama_index-0.6.1/llama_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/storage/index_store/types.py` & `llama_index-0.6.1/llama_index/storage/index_store/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from abc import ABC, abstractmethod
 from typing import List, Optional
 
-from llama_index.data_structs.data_structs_v2 import V2IndexStruct
+from llama_index.data_structs.data_structs import IndexStruct
 import os
 
 DEFAULT_PERSIST_DIR = "./storage"
 DEFAULT_PERSIST_FNAME = "index_store.json"
 DEFAULT_PERSIST_PATH = os.path.join(DEFAULT_PERSIST_DIR, DEFAULT_PERSIST_FNAME)
 
 
 class BaseIndexStore(ABC):
     @abstractmethod
-    def index_structs(self) -> List[V2IndexStruct]:
+    def index_structs(self) -> List[IndexStruct]:
         pass
 
     @abstractmethod
-    def add_index_struct(self, index_struct: V2IndexStruct) -> None:
+    def add_index_struct(self, index_struct: IndexStruct) -> None:
         pass
 
     @abstractmethod
     def delete_index_struct(self, key: str) -> None:
         pass
 
     @abstractmethod
     def get_index_struct(
         self, struct_id: Optional[str] = None
-    ) -> Optional[V2IndexStruct]:
+    ) -> Optional[IndexStruct]:
         pass
 
     def persist(self, persist_path: str = DEFAULT_PERSIST_PATH) -> None:
         """Persist the index store to disk."""
         pass
```

### Comparing `llama_index-0.6.0a7/llama_index/storage/index_store/utils.py` & `llama_index-0.6.1/llama_index/storage/index_store/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from llama_index.constants import DATA_KEY, TYPE_KEY
-from llama_index.data_structs.data_structs_v2 import V2IndexStruct
+from llama_index.data_structs.data_structs import IndexStruct
 from llama_index.data_structs.registry import INDEX_STRUCT_TYPE_TO_INDEX_STRUCT_CLASS
 
 
-def index_struct_to_json(index_struct: V2IndexStruct) -> dict:
+def index_struct_to_json(index_struct: IndexStruct) -> dict:
     index_struct_dict = {
         TYPE_KEY: index_struct.get_type(),
         DATA_KEY: index_struct.to_dict(),
     }
     return index_struct_dict
 
 
-def json_to_index_struct(struct_dict: dict) -> V2IndexStruct:
+def json_to_index_struct(struct_dict: dict) -> IndexStruct:
     type = struct_dict[TYPE_KEY]
     data_dict = struct_dict[DATA_KEY]
     cls = INDEX_STRUCT_TYPE_TO_INDEX_STRUCT_CLASS[type]
     return cls.from_dict(data_dict)
```

### Comparing `llama_index-0.6.0a7/llama_index/storage/kvstore/mongodb_kvstore.py` & `llama_index-0.6.1/llama_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/storage/kvstore/simple_kvstore.py` & `llama_index-0.6.1/llama_index/storage/kvstore/simple_kvstore.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,7 +68,16 @@
         if not os.path.exists(persist_path):
             raise ValueError(f"No existing {__name__} found at {persist_path}.")
 
         logger.debug(f"Loading {__name__} from {persist_path}.")
         with open(persist_path, "r+") as f:
             data = json.load(f)
         return cls(data)
+
+    def to_dict(self) -> dict:
+        """Save the store as dict."""
+        return self._data
+
+    @classmethod
+    def from_dict(cls, save_dict: dict) -> "SimpleKVStore":
+        """Load a SimpleKVStore from dict."""
+        return cls(save_dict)
```

### Comparing `llama_index-0.6.0a7/llama_index/storage/kvstore/types.py` & `llama_index-0.6.1/llama_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/token_counter/mock_chain_wrapper.py` & `llama_index-0.6.1/llama_index/token_counter/mock_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/token_counter/mock_embed_model.py` & `llama_index-0.6.1/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/token_counter/token_counter.py` & `llama_index-0.6.1/llama_index/token_counter/token_counter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/token_counter/utils.py` & `llama_index-0.6.1/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/tools/query_engine.py` & `llama_index-0.6.1/llama_index/tools/query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/tts/bark.py` & `llama_index-0.6.1/llama_index/tts/bark.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/tts/base.py` & `llama_index-0.6.1/llama_index/tts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/tts/elevenlabs.py` & `llama_index-0.6.1/llama_index/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/utils.py` & `llama_index-0.6.1/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/llama_index/vector_stores/__init__.py` & `llama_index-0.6.1/llama_index/vector_stores/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Vector stores."""
 
 from llama_index.vector_stores.chatgpt_plugin import ChatGPTRetrievalPluginClient
 from llama_index.vector_stores.chroma import ChromaVectorStore
 from llama_index.vector_stores.deeplake import DeepLakeVectorStore
 from llama_index.vector_stores.faiss import FaissVectorStore
 from llama_index.vector_stores.milvus import MilvusVectorStore
+from llama_index.vector_stores.lancedb import LanceDBVectorStore
+from llama_index.vector_stores.metal import MetalVectorStore
 from llama_index.vector_stores.myscale import MyScaleVectorStore
 from llama_index.vector_stores.opensearch import (
     OpensearchVectorClient,
     OpensearchVectorStore,
 )
 from llama_index.vector_stores.pinecone import PineconeVectorStore
 from llama_index.vector_stores.qdrant import QdrantVectorStore
@@ -18,14 +20,16 @@
 __all__ = [
     "SimpleVectorStore",
     "FaissVectorStore",
     "PineconeVectorStore",
     "WeaviateVectorStore",
     "QdrantVectorStore",
     "ChromaVectorStore",
+    "MetalVectorStore",
     "OpensearchVectorStore",
     "OpensearchVectorClient",
     "ChatGPTRetrievalPluginClient",
     "MilvusVectorStore",
     "DeepLakeVectorStore",
     "MyScaleVectorStore",
+    "LanceDBVectorStore",
 ]
```

### Comparing `llama_index-0.6.0a7/llama_index/vector_stores/chatgpt_plugin.py` & `llama_index-0.6.1/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,36 +3,35 @@
 import os
 from typing import Any, Dict, List, Optional
 
 import requests
 from requests.adapters import HTTPAdapter, Retry
 from tqdm.auto import tqdm
 
-from llama_index.data_structs.node_v2 import Node, DocumentRelationship
+from llama_index.data_structs.node import Node, DocumentRelationship
 from llama_index.vector_stores.types import (
-    NodeEmbeddingResult,
+    NodeWithEmbedding,
     VectorStore,
     VectorStoreQueryResult,
     VectorStoreQuery,
 )
 
 
-def convert_docs_to_json(embedding_results: List[NodeEmbeddingResult]) -> List[Dict]:
+def convert_docs_to_json(embedding_results: List[NodeWithEmbedding]) -> List[Dict]:
     """Convert docs to JSON."""
     docs = []
     for embedding_result in embedding_results:
         # TODO: add information for other fields as well
         # fields taken from
         # https://rb.gy/nmac9u
         doc_dict = {
             "id": embedding_result.id,
             "text": embedding_result.node.get_text(),
-            # "source": embedding_result.node.source,
             # NOTE: this is the doc_id to reference document
-            "source_id": embedding_result.doc_id,
+            "source_id": embedding_result.ref_doc_id,
             # "url": "...",
             # "created_at": ...,
             # "author": "..."",
         }
         extra_info = embedding_result.node.extra_info
         if extra_info is not None:
             if "source" in extra_info:
@@ -85,15 +84,15 @@
     @property
     def client(self) -> None:
         """Get client."""
         return None
 
     def add(
         self,
-        embedding_results: List[NodeEmbeddingResult],
+        embedding_results: List[NodeWithEmbedding],
     ) -> List[str]:
         """Add embedding_results to index."""
         headers = {"Authorization": f"Bearer {self._bearer_token}"}
 
         docs_to_upload = convert_docs_to_json(embedding_results)
         for i in tqdm(range(0, len(docs_to_upload), self._batch_size)):
             i_end = min(i + self._batch_size, len(docs_to_upload))
```

### Comparing `llama_index-0.6.0a7/llama_index/vector_stores/chroma.py` & `llama_index-0.6.1/llama_index/vector_stores/chroma.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Chroma vector store."""
 import logging
 import math
 from typing import Any, List, cast
 
-from llama_index.data_structs.node_v2 import DocumentRelationship, Node
+from llama_index.data_structs.node import DocumentRelationship, Node
 from llama_index.utils import truncate_text
 from llama_index.vector_stores.types import (
-    NodeEmbeddingResult,
+    NodeWithEmbedding,
     VectorStore,
     VectorStoreQuery,
     VectorStoreQueryResult,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -40,32 +40,32 @@
             import chromadb  # noqa: F401
         except ImportError:
             raise ImportError(import_err_msg)
         from chromadb.api.models.Collection import Collection
 
         self._collection = cast(Collection, chroma_collection)
 
-    def add(self, embedding_results: List[NodeEmbeddingResult]) -> List[str]:
+    def add(self, embedding_results: List[NodeWithEmbedding]) -> List[str]:
         """Add embedding results to index.
 
         Args
-            embedding_results: List[NodeEmbeddingResult]: list of embedding results
+            embedding_results: List[NodeWithEmbedding]: list of embedding results
 
         """
         if not self._collection:
             raise ValueError("Collection not initialized")
 
         embeddings = []
         metadatas = []
         ids = []
         documents = []
         for result in embedding_results:
             embeddings.append(result.embedding)
             extra_info = result.node.extra_info or {}
-            metadatas.append({**extra_info, **{"document_id": result.doc_id}})
+            metadatas.append({**extra_info, **{"document_id": result.ref_doc_id}})
             ids.append(result.id)
             documents.append(result.node.get_text())
 
         self._collection.add(
             embeddings=embeddings,
             ids=ids,
             metadatas=metadatas,
```

### Comparing `llama_index-0.6.0a7/llama_index/vector_stores/deeplake.py` & `llama_index-0.6.1/llama_index/vector_stores/deeplake.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 import logging
 from typing import Any, Dict, List, Optional, cast
 
 import numpy as np
 from llama_index.indices.query.embedding_utils import get_top_k_embeddings
 from llama_index.vector_stores.types import (
-    NodeEmbeddingResult,
+    NodeWithEmbedding,
     VectorStore,
     VectorStoreQuery,
     VectorStoreQueryResult,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -135,19 +135,19 @@
                 )
 
     @property
     def client(self) -> None:
         """Get client."""
         return self.ds
 
-    def add(self, embedding_results: List[NodeEmbeddingResult]) -> List[str]:
+    def add(self, embedding_results: List[NodeWithEmbedding]) -> List[str]:
         """Add the embeddings and their nodes into DeepLake.
 
         Args:
-            embedding_results (List[NodeEmbeddingResult]): The embeddings and their data
+            embedding_results (List[NodeWithEmbedding]): The embeddings and their data
                 to insert.
 
         Raises:
             UserNotLoggedinException: When user is not logged in with credentials
                 or token.
             TokenPermissionError: When dataset does not exist or user doesn't have
                 enough permissions to modify the dataset.
@@ -158,15 +158,15 @@
         """
         data_to_injest = []
         ids = []
 
         for result in embedding_results:
             embedding = result.embedding
             extra_info = result.node.extra_info or {}
-            metadata = {**extra_info, **{"document_id": result.doc_id}}
+            metadata = {**extra_info, **{"document_id": result.ref_doc_id}}
             id = result.id
             text = result.node.get_text()
 
             data_to_injest.append(
                 {
                     "text": text,
                     "metadata": metadata,
```

### Comparing `llama_index-0.6.0a7/llama_index/vector_stores/faiss.py` & `llama_index-0.6.1/llama_index/vector_stores/faiss.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import Any, List, cast
 
 import numpy as np
 
 from llama_index.vector_stores.types import (
     DEFAULT_PERSIST_DIR,
     DEFAULT_PERSIST_FNAME,
-    NodeEmbeddingResult,
+    NodeWithEmbedding,
     VectorStore,
     VectorStoreQueryResult,
     VectorStoreQuery,
 )
 
 import logging
 
@@ -75,22 +75,22 @@
 
         logger.info(f"Loading {__name__} from {persist_path}.")
         faiss_index = faiss.read_index(persist_path)
         return cls(faiss_index=faiss_index)
 
     def add(
         self,
-        embedding_results: List[NodeEmbeddingResult],
+        embedding_results: List[NodeWithEmbedding],
     ) -> List[str]:
         """Add embedding results to index.
 
         NOTE: in the Faiss vector store, we do not store text in Faiss.
 
         Args
-            embedding_results: List[NodeEmbeddingResult]: list of embedding results
+            embedding_results: List[NodeWithEmbedding]: list of embedding results
 
         """
         new_ids = []
         for result in embedding_results:
             text_embedding = result.embedding
             text_embedding_np = np.array(text_embedding, dtype="float32")[np.newaxis, :]
             new_id = str(self._faiss_index.ntotal)
```

### Comparing `llama_index-0.6.0a7/llama_index/vector_stores/milvus.py` & `llama_index-0.6.1/llama_index/vector_stores/milvus.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 An index that is built within Milvus.
 
 """
 import logging
 from typing import Any, List, Optional
 from uuid import uuid4
 
-from llama_index.data_structs.node_v2 import DocumentRelationship, Node
+from llama_index.data_structs.node import DocumentRelationship, Node
 from llama_index.vector_stores.types import (
-    NodeEmbeddingResult,
+    NodeWithEmbedding,
     VectorStore,
     VectorStoreQuery,
     VectorStoreQueryMode,
     VectorStoreQueryResult,
 )
 
 logger = logging.getLogger(__name__)
@@ -283,19 +283,19 @@
         self.search_params["metric_type"] = index["metric_type"]
 
     @property
     def client(self) -> Any:
         """Get client."""
         return self.collection
 
-    def add(self, embedding_results: List[NodeEmbeddingResult]) -> List[str]:
+    def add(self, embedding_results: List[NodeWithEmbedding]) -> List[str]:
         """Add the embeddings and their nodes into Milvus.
 
         Args:
-            embedding_results (List[NodeEmbeddingResult]): The embeddings and their data
+            embedding_results (List[NodeWithEmbedding]): The embeddings and their data
                 to insert.
 
         Raises:
             MilvusException: Failed to insert data.
 
         Returns:
             List[str]: List of ids inserted.
@@ -314,15 +314,15 @@
         doc_ids = []
         texts = []
         embeddings = []
 
         # Process that data we are going to insert
         for result in embedding_results:
             ids.append(result.id)
-            doc_ids.append(result.doc_id)
+            doc_ids.append(result.ref_doc_id)
             texts.append(result.node.get_text())
             embeddings.append(result.embedding)
 
         try:
             # Insert the data into milvus
             self.collection.insert([ids, doc_ids, texts, embeddings])
             logger.debug(
```

### Comparing `llama_index-0.6.0a7/llama_index/vector_stores/myscale.py` & `llama_index-0.6.1/llama_index/vector_stores/myscale.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 An index that is built on top of an existing MyScale cluster.
 
 """
 import json
 import logging
 from typing import Any, Dict, List, Optional, cast
 
-from llama_index.data_structs.node_v2 import DocumentRelationship, Node
+from llama_index.data_structs.node import DocumentRelationship, Node
 from llama_index.indices.service_context import ServiceContext
 from llama_index.readers.myscale import (
     MyScaleSettings,
     escape_str,
     format_list_to_string,
 )
 from llama_index.utils import iter_batch
 from llama_index.vector_stores.types import (
-    NodeEmbeddingResult,
+    NodeWithEmbedding,
     VectorStore,
     VectorStoreQuery,
     VectorStoreQueryResult,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -95,18 +95,18 @@
             search_params=search_params,
             **kwargs,
         )
 
         # schema column name, type, and construct format method
         self.column_config: Dict = {
             "id": {"type": "String", "extract_func": lambda x: x.id},
-            "doc_id": {"type": "String", "extract_func": lambda x: x.doc_id},
+            "doc_id": {"type": "String", "extract_func": lambda x: x.ref_doc_id},
             "text": {
                 "type": "String",
-                "extract_func": lambda x: escape_str(x.node.text),
+                "extract_func": lambda x: escape_str(x.node.get_text()),
             },
             "vector": {
                 "type": "Array(Float32)",
                 "extract_func": lambda x: format_list_to_string(x.embedding),
             },
             "node_info": {
                 "type": "JSON",
@@ -147,15 +147,15 @@
         self.dim = dimension
         self._client.command("SET allow_experimental_object_type=1")
         self._client.command(schema_)
         self._index_existed = True
 
     def _build_insert_statement(
         self,
-        values: List[NodeEmbeddingResult],
+        values: List[NodeWithEmbedding],
     ) -> str:
         _data = []
         for item in values:
             item_value_str = ",".join(
                 [
                     f"'{column['extract_func'](item)}'"
                     for column in self.column_config.values()
@@ -169,20 +169,20 @@
                 VALUES
                     {','.join(_data)}
                 """
         return insert_statement
 
     def add(
         self,
-        embedding_results: List[NodeEmbeddingResult],
+        embedding_results: List[NodeWithEmbedding],
     ) -> List[str]:
         """Add embedding results to index.
 
         Args
-            embedding_results: List[NodeEmbeddingResult]: list of embedding results
+            embedding_results: List[NodeWithEmbedding]: list of embedding results
 
         """
 
         if not embedding_results:
             return []
 
         if not self._index_existed:
```

### Comparing `llama_index-0.6.0a7/llama_index/vector_stores/opensearch.py` & `llama_index-0.6.1/llama_index/vector_stores/opensearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Elasticsearch/Opensearch vector store."""
 import json
 from typing import Any, Dict, List, Optional, cast
 
 from llama_index.data_structs import Node
 from llama_index.vector_stores.types import (
-    NodeEmbeddingResult,
+    NodeWithEmbedding,
     VectorStore,
     VectorStoreQueryResult,
     VectorStoreQuery,
 )
 
 
 class OpensearchVectorClient:
@@ -92,22 +92,22 @@
                 }
             },
         }
         res = self._client.put(f"/{self._index}", json=idx_conf)
         # will 400 if the index already existed, so allow 400 errors right here
         assert res.status_code == 200 or res.status_code == 400
 
-    def index_results(self, results: List[NodeEmbeddingResult]) -> List[str]:
+    def index_results(self, results: List[NodeWithEmbedding]) -> List[str]:
         """Store results in the index."""
         bulk_req: List[Dict[Any, Any]] = []
         for result in results:
             bulk_req.append({"index": {"_index": self._index, "_id": result.id}})
             bulk_req.append(
                 {
-                    self._text_field: result.node.text,
+                    self._text_field: result.node.get_text(),
                     self._embedding_field: result.embedding,
                 }
             )
         bulk = "\n".join([json.dumps(v) for v in bulk_req]) + "\n"
         res = self._client.post(
             "/_bulk", headers={"Content-Type": "application/x-ndjson"}, content=bulk
         )
@@ -176,20 +176,20 @@
     @property
     def client(self) -> Any:
         """Get client."""
         return self._client
 
     def add(
         self,
-        embedding_results: List[NodeEmbeddingResult],
+        embedding_results: List[NodeWithEmbedding],
     ) -> List[str]:
         """Add embedding results to index.
 
         Args
-            embedding_results: List[NodeEmbeddingResult]: list of embedding results
+            embedding_results: List[NodeWithEmbedding]: list of embedding results
 
         """
         self._client.index_results(embedding_results)
         return [result.id for result in embedding_results]
 
     def delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete a document.
```

### Comparing `llama_index-0.6.0a7/llama_index/vector_stores/pinecone.py` & `llama_index-0.6.1/llama_index/vector_stores/pinecone.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 import logging
 import os
 from collections import Counter
 from functools import partial
 from typing import Any, Callable, Dict, List, Optional, cast
 
-from llama_index.data_structs.node_v2 import DocumentRelationship, Node
+from llama_index.data_structs.node import DocumentRelationship, Node
 from llama_index.vector_stores.types import (
-    NodeEmbeddingResult,
+    NodeWithEmbedding,
     VectorStore,
     VectorStoreQuery,
     VectorStoreQueryMode,
     VectorStoreQueryResult,
 )
 
 _logger = logging.getLogger(__name__)
@@ -186,33 +186,32 @@
         self._add_sparse_vector = add_sparse_vector
         if tokenizer is None:
             tokenizer = get_default_tokenizer()
         self._tokenizer = tokenizer
 
     def add(
         self,
-        embedding_results: List[NodeEmbeddingResult],
+        embedding_results: List[NodeWithEmbedding],
     ) -> List[str]:
         """Add embedding results to index.
 
         Args
-            embedding_results: List[NodeEmbeddingResult]: list of embedding results
+            embedding_results: List[NodeWithEmbedding]: list of embedding results
 
         """
         ids = []
         for result in embedding_results:
-            new_id = result.id
+            node_id = result.id
             node = result.node
-            text_embedding = result.embedding
 
             metadata = {
                 "text": node.get_text(),
                 # NOTE: this is the reference to source doc
-                "doc_id": result.doc_id,
-                "id": new_id,
+                "doc_id": node.ref_doc_id,
+                "id": node_id,
             }
             if node.extra_info:
                 # TODO: check if overlap with default metadata keys
                 metadata.update(
                     get_metadata_from_node_info(node.extra_info, "extra_info")
                 )
             if node.node_info:
@@ -229,27 +228,27 @@
                 raise ValueError(
                     "metadata_filters keys overlap with default "
                     f"metadata keys: {intersecting_keys}"
                 )
             metadata.update(self._metadata_filters)
 
             entry = {
-                "id": new_id,
-                "values": text_embedding,
+                "id": node_id,
+                "values": result.embedding,
                 "metadata": metadata,
             }
             if self._add_sparse_vector:
                 sparse_vector = generate_sparse_vectors(
                     [node.get_text()], self._tokenizer
                 )[0]
                 entry.update({"sparse_values": sparse_vector})
             self._pinecone_index.upsert(
                 [entry], namespace=self._namespace, **self._pinecone_kwargs
             )
-            ids.append(new_id)
+            ids.append(node_id)
         return ids
 
     def delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete a document.
 
         Args:
             doc_id (str): document id
```

### Comparing `llama_index-0.6.0a7/llama_index/vector_stores/qdrant.py` & `llama_index-0.6.1/llama_index/vector_stores/qdrant.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 An index that is built on top of an existing Qdrant collection.
 
 """
 import logging
 from typing import Any, List, Optional, cast
 
-from llama_index.data_structs.node_v2 import DocumentRelationship, Node
+from llama_index.data_structs.node import DocumentRelationship, Node
 from llama_index.utils import iter_batch
 from llama_index.vector_stores.types import (
-    NodeEmbeddingResult,
+    NodeWithEmbedding,
     VectorStore,
     VectorStoreQueryResult,
     VectorStoreQuery,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -51,55 +51,55 @@
 
         self._client = cast(qdrant_client.QdrantClient, client)
         self._collection_name = collection_name
         self._collection_initialized = self._collection_exists(collection_name)
 
         self._batch_size = kwargs.get("batch_size", 100)
 
-    def add(self, embedding_results: List[NodeEmbeddingResult]) -> List[str]:
+    def add(self, embedding_results: List[NodeWithEmbedding]) -> List[str]:
         """Add embedding results to index.
 
         Args
-            embedding_results: List[NodeEmbeddingResult]: list of embedding results
+            embedding_results: List[NodeWithEmbedding]: list of embedding results
 
         """
         from qdrant_client.http import models as rest
 
         if len(embedding_results) > 0 and not self._collection_initialized:
             self._create_collection(
                 collection_name=self._collection_name,
                 vector_size=len(embedding_results[0].embedding),
             )
 
         ids = []
         for result_batch in iter_batch(embedding_results, self._batch_size):
-            new_ids = []
+            node_ids = []
             vectors = []
             payloads = []
             for result in result_batch:
-                new_ids.append(result.id)
+                node_ids.append(result.id)
                 vectors.append(result.embedding)
                 node = result.node
                 payloads.append(
                     {
-                        "doc_id": result.doc_id,
+                        "doc_id": result.ref_doc_id,
                         "text": node.get_text(),
                         "extra_info": node.extra_info,
                     }
                 )
 
             self._client.upsert(
                 collection_name=self._collection_name,
                 points=rest.Batch.construct(
-                    ids=new_ids,
+                    ids=node_ids,
                     vectors=vectors,
                     payloads=payloads,
                 ),
             )
-            ids.extend(new_ids)
+            ids.extend(node_ids)
         return ids
 
     def delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete a document.
 
         Args:
             doc_id: (str): document id
```

### Comparing `llama_index-0.6.0a7/llama_index/vector_stores/registry.py` & `llama_index-0.6.1/llama_index/vector_stores/registry.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Dict, Type
 
 from llama_index.vector_stores.chatgpt_plugin import ChatGPTRetrievalPluginClient
 from llama_index.vector_stores.chroma import ChromaVectorStore
 from llama_index.vector_stores.deeplake import DeepLakeVectorStore
 from llama_index.vector_stores.faiss import FaissVectorStore
 from llama_index.vector_stores.milvus import MilvusVectorStore
+from llama_index.vector_stores.lancedb import LanceDBVectorStore
 from llama_index.vector_stores.myscale import MyScaleVectorStore
 from llama_index.vector_stores.opensearch import OpensearchVectorStore
 from llama_index.vector_stores.pinecone import PineconeVectorStore
 from llama_index.vector_stores.qdrant import QdrantVectorStore
 from llama_index.vector_stores.simple import SimpleVectorStore
 from llama_index.vector_stores.types import VectorStore
 from llama_index.vector_stores.weaviate import WeaviateVectorStore
@@ -20,23 +21,25 @@
     WEAVIATE = "weaviate"
     QDRANT = "qdrant"
     PINECONE = "pinecone"
     OPENSEARCH = "opensearch"
     FAISS = "faiss"
     CHROMA = "chroma"
     CHATGPT_PLUGIN = "chatgpt_plugin"
+    LANCEDB = "lancedb"
     MILVUS = "milvus"
     DEEPLAKE = "deeplake"
     MYSCALE = "myscale"
 
 
 VECTOR_STORE_TYPE_TO_VECTOR_STORE_CLASS: Dict[VectorStoreType, Type[VectorStore]] = {
     VectorStoreType.SIMPLE: SimpleVectorStore,
     VectorStoreType.WEAVIATE: WeaviateVectorStore,
     VectorStoreType.QDRANT: QdrantVectorStore,
+    VectorStoreType.LANCEDB: LanceDBVectorStore,
     VectorStoreType.MILVUS: MilvusVectorStore,
     VectorStoreType.PINECONE: PineconeVectorStore,
     VectorStoreType.OPENSEARCH: OpensearchVectorStore,
     VectorStoreType.FAISS: FaissVectorStore,
     VectorStoreType.CHROMA: ChromaVectorStore,
     VectorStoreType.CHATGPT_PLUGIN: ChatGPTRetrievalPluginClient,
     VectorStoreType.DEEPLAKE: DeepLakeVectorStore,
```

### Comparing `llama_index-0.6.0a7/llama_index/vector_stores/simple.py` & `llama_index-0.6.1/llama_index/vector_stores/simple.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from llama_index.indices.query.embedding_utils import (
     get_top_k_embeddings,
     get_top_k_embeddings_learner,
 )
 from llama_index.vector_stores.types import (
     DEFAULT_PERSIST_DIR,
     DEFAULT_PERSIST_FNAME,
-    NodeEmbeddingResult,
+    NodeWithEmbedding,
     VectorStore,
     VectorStoreQueryResult,
     VectorStoreQuery,
     VectorStoreQueryMode,
 )
 
 import logging
@@ -81,21 +81,20 @@
 
     def get(self, text_id: str) -> List[float]:
         """Get embedding."""
         return self._data.embedding_dict[text_id]
 
     def add(
         self,
-        embedding_results: List[NodeEmbeddingResult],
+        embedding_results: List[NodeWithEmbedding],
     ) -> List[str]:
         """Add embedding_results to index."""
         for result in embedding_results:
-            text_id = result.id
-            self._data.embedding_dict[text_id] = result.embedding
-            self._data.text_id_to_doc_id[text_id] = result.doc_id
+            self._data.embedding_dict[result.id] = result.embedding
+            self._data.text_id_to_doc_id[result.id] = result.ref_doc_id
         return [result.id for result in embedding_results]
 
     def delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete a document."""
         text_ids_to_delete = set()
         for text_id, doc_id_ in self._data.text_id_to_doc_id.items():
             if doc_id == doc_id_:
@@ -154,7 +153,15 @@
             )
 
         logger.debug(f"Loading {__name__} from {persist_path}.")
         with open(persist_path, "r+") as f:
             data_dict = json.load(f)
             data = SimpleVectorStoreData.from_dict(data_dict)
         return cls(data)
+
+    @classmethod
+    def from_dict(cls, save_dict: dict) -> "SimpleVectorStore":
+        data = SimpleVectorStoreData.from_dict(save_dict)
+        return cls(data)
+
+    def to_dict(self) -> dict:
+        return self._data.to_dict()
```

### Comparing `llama_index-0.6.0a7/llama_index/vector_stores/types.py` & `llama_index-0.6.1/llama_index/vector_stores/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 """Vector store index types."""
 
 
 from dataclasses import dataclass
 from typing import Any, List, Optional, Protocol, runtime_checkable
 
 from enum import Enum
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 
 
 DEFAULT_PERSIST_DIR = "./storage"
 DEFAULT_PERSIST_FNAME = "vector_store.json"
 
 
 @dataclass
-class NodeEmbeddingResult:
-    """Node embedding result.
+class NodeWithEmbedding:
+    """Node with embedding.
 
     Args:
-        id (str): Node id
         node (Node): Node
         embedding (List[float]): Embedding
-        doc_id (str): Document id
 
     """
 
-    id: str
     node: Node
     embedding: List[float]
-    doc_id: str
+
+    @property
+    def id(self) -> str:
+        return self.node.get_doc_id()
+
+    @property
+    def ref_doc_id(self) -> str:
+        return self.node.ref_doc_id or "None"
 
 
 @dataclass
 class VectorStoreQueryResult:
     """Vector store query result."""
 
     nodes: Optional[List[Node]] = None
@@ -79,15 +83,15 @@
     @property
     def client(self) -> Any:
         """Get client."""
         ...
 
     def add(
         self,
-        embedding_results: List[NodeEmbeddingResult],
+        embedding_results: List[NodeWithEmbedding],
     ) -> List[str]:
         """Add embedding results to vector store."""
         ...
 
     def delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete doc."""
         ...
```

### Comparing `llama_index-0.6.0a7/llama_index/vector_stores/weaviate.py` & `llama_index-0.6.1/llama_index/vector_stores/weaviate.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     add_nodes,
     create_schema,
     delete_document,
     weaviate_query,
 )
 from llama_index.readers.weaviate.utils import get_default_class_prefix
 from llama_index.vector_stores.types import (
-    NodeEmbeddingResult,
+    NodeWithEmbedding,
     VectorStore,
     VectorStoreQueryResult,
     VectorStoreQuery,
 )
 
 
 class WeaviateVectorStore(VectorStore):
@@ -71,20 +71,20 @@
     @property
     def client(self) -> Any:
         """Get client."""
         return self._client
 
     def add(
         self,
-        embedding_results: List[NodeEmbeddingResult],
+        embedding_results: List[NodeWithEmbedding],
     ) -> List[str]:
         """Add embedding results to index.
 
         Args
-            embedding_results: List[NodeEmbeddingResult]: list of embedding results
+            embedding_results: List[NodeWithEmbedding]: list of embedding results
 
         """
         for result in embedding_results:
             node = result.node
             embedding = result.embedding
             # TODO: always store embedding in node
             node.embedding = embedding
```

### Comparing `llama_index-0.6.0a7/llama_index.egg-info/PKG-INFO` & `llama_index-0.6.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
-Name: llama-index
-Version: 0.6.0a7
+Name: llama_index
+Version: 0.6.1
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
 
 LlamaIndex (GPT Index) is a project that provides a central interface to connect your LLM's with external data.
 
-PyPi: 
+PyPI: 
 - LlamaIndex: https://pypi.org/project/llama-index/.
 - GPT Index (duplicate): https://pypi.org/project/gpt-index/.
 
-Documentation:
-- v0.6 (pre-release): https://gpt-index.readthedocs.io/en/latest/.
-- v0.5 (stable): https://gpt-index.readthedocs.io/en/v0.5.27/.
+Documentation: https://gpt-index.readthedocs.io/.
 
 Twitter: https://twitter.com/gpt_index.
 
 Discord: https://discord.gg/dGcwcsnxhU.
 
 ### Ecosystem
 
@@ -30,15 +28,15 @@
 
 
 ## 🚀 Overview
 
 **NOTE**: This README is not updated as frequently as the documentation. Please check out the documentation above for the latest updates!
 
 ### Context
-- LLMs are a phenomenonal piece of technology for knowledge generation and reasoning. They are pre-trained on large amounts of publicly available data.
+- LLMs are a phenomenal piece of technology for knowledge generation and reasoning. They are pre-trained on large amounts of publicly available data.
 - How do we best augment LLMs with our own private data?
 - One paradigm that has emerged is *in-context* learning (the other is finetuning), where we insert context into the input prompt. That way,
 we take advantage of the LLM's reasoning capabilities to generate a response.
 
 To perform LLM's data augmentation in a performant, efficient, and cheap manner, we need to solve two components:
 - Data Ingestion
 - Data Indexing
@@ -55,15 +53,15 @@
    - Dealing with text splitting.
 - Provides users an interface to **query** the index (feed in an input prompt) and obtain a knowledge-augmented output.
 - Offers you a comprehensive toolset trading off cost and performance.
 
 
 ## 💡 Contributing
 
-Interesting in contributing? See our [Contribution Guide](CONTRIBUTING.md) for more details.
+Interested in contributing? See our [Contribution Guide](CONTRIBUTING.md) for more details.
 
 ## 📄 Documentation
 
 Full documentation can be found here: https://gpt-index.readthedocs.io/en/latest/. 
 
 Please check it out for the most up-to-date tutorials, how-to guides, references, and other resources!
```

### Comparing `llama_index-0.6.0a7/llama_index.egg-info/SOURCES.txt` & `llama_index-0.6.1/llama_index.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,20 +22,18 @@
 llama_index/callbacks/llama_debug.py
 llama_index/callbacks/schema.py
 llama_index/composability/__init__.py
 llama_index/composability/base.py
 llama_index/composability/joint_qa_summary.py
 llama_index/data_structs/__init__.py
 llama_index/data_structs/data_structs.py
-llama_index/data_structs/data_structs_v2.py
-llama_index/data_structs/node_v2.py
+llama_index/data_structs/node.py
 llama_index/data_structs/registry.py
 llama_index/data_structs/struct_type.py
 llama_index/data_structs/table.py
-llama_index/data_structs/table_v2.py
 llama_index/embeddings/__init__.py
 llama_index/embeddings/base.py
 llama_index/embeddings/google.py
 llama_index/embeddings/langchain.py
 llama_index/embeddings/openai.py
 llama_index/embeddings/utils.py
 llama_index/evaluation/__init__.py
@@ -70,18 +68,19 @@
 llama_index/indices/knowledge_graph/__init__.py
 llama_index/indices/knowledge_graph/base.py
 llama_index/indices/knowledge_graph/retrievers.py
 llama_index/indices/list/__init__.py
 llama_index/indices/list/base.py
 llama_index/indices/list/retrievers.py
 llama_index/indices/postprocessor/__init__.py
-llama_index/indices/postprocessor/base.py
+llama_index/indices/postprocessor/cohere_rerank.py
 llama_index/indices/postprocessor/node.py
 llama_index/indices/postprocessor/node_recency.py
 llama_index/indices/postprocessor/pii.py
+llama_index/indices/postprocessor/types.py
 llama_index/indices/query/__init__.py
 llama_index/indices/query/base.py
 llama_index/indices/query/embedding_utils.py
 llama_index/indices/query/response_synthesis.py
 llama_index/indices/query/schema.py
 llama_index/indices/query/query_transform/__init__.py
 llama_index/indices/query/query_transform/base.py
@@ -155,14 +154,15 @@
 llama_index/readers/deeplake.py
 llama_index/readers/discord_reader.py
 llama_index/readers/download.py
 llama_index/readers/elasticsearch.py
 llama_index/readers/faiss.py
 llama_index/readers/json.py
 llama_index/readers/mbox.py
+llama_index/readers/metal.py
 llama_index/readers/milvus.py
 llama_index/readers/mongo.py
 llama_index/readers/myscale.py
 llama_index/readers/notion.py
 llama_index/readers/obsidian.py
 llama_index/readers/pinecone.py
 llama_index/readers/qdrant.py
@@ -247,14 +247,16 @@
 llama_index/tts/base.py
 llama_index/tts/elevenlabs.py
 llama_index/vector_stores/__init__.py
 llama_index/vector_stores/chatgpt_plugin.py
 llama_index/vector_stores/chroma.py
 llama_index/vector_stores/deeplake.py
 llama_index/vector_stores/faiss.py
+llama_index/vector_stores/lancedb.py
+llama_index/vector_stores/metal.py
 llama_index/vector_stores/milvus.py
 llama_index/vector_stores/myscale.py
 llama_index/vector_stores/opensearch.py
 llama_index/vector_stores/pinecone.py
 llama_index/vector_stores/qdrant.py
 llama_index/vector_stores/registry.py
 llama_index/vector_stores/simple.py
@@ -310,14 +312,15 @@
 tests/indices/tree/test_index.py
 tests/indices/tree/test_retrievers.py
 tests/indices/vector_store/__init__.py
 tests/indices/vector_store/conftest.py
 tests/indices/vector_store/mock_faiss.py
 tests/indices/vector_store/mock_services.py
 tests/indices/vector_store/test_faiss.py
+tests/indices/vector_store/test_lancedb.py
 tests/indices/vector_store/test_milvus.py
 tests/indices/vector_store/test_myscale.py
 tests/indices/vector_store/test_pinecone.py
 tests/indices/vector_store/test_retrievers.py
 tests/indices/vector_store/test_simple.py
 tests/indices/vector_store/test_weaviate.py
 tests/indices/vector_store/utils.py
@@ -346,14 +349,15 @@
 tests/readers/test_json.py
 tests/readers/test_mongo.py
 tests/readers/test_string_iterable.py
 tests/selectors/__init__.py
 tests/selectors/test_llm_selectors.py
 tests/storage/__init__.py
 tests/storage/conftest.py
+tests/storage/test_storage_context.py
 tests/storage/docstore/__init__.py
 tests/storage/docstore/test_mongo_docstore.py
 tests/storage/docstore/test_simple_docstore.py
 tests/token_predictor/__init__.py
 tests/token_predictor/test_base.py
 tests/vector_stores/__init__.py
 tests/vector_stores/test_qdrant.py
```

### Comparing `llama_index-0.6.0a7/setup.py` & `llama_index-0.6.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,19 +11,20 @@
     __version__ = _f.read().strip()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 install_requires = [
     "dataclasses_json",
-    "langchain>=0.0.152",
+    "langchain>=0.0.154",
     "numpy",
     "tenacity>=8.2.0,<9.0.0",
     "openai>=0.26.4",
     "pandas",
+    "requests<2.30.0",
 ]
 
 # NOTE: if python version >= 3.9, install tiktoken
 # else install transformers
 if sys.version_info >= (3, 9):
     install_requires.extend(["tiktoken"])
 else:
```

### Comparing `llama_index-0.6.0a7/tests/callbacks/test_llama_debug.py` & `llama_index-0.6.1/tests/callbacks/test_llama_debug.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/conftest.py` & `llama_index-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/embeddings/test_base.py` & `llama_index-0.6.1/tests/embeddings/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/composability/test_utils.py` & `llama_index-0.6.1/tests/indices/composability/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict, List, Optional
 
 from llama_index.vector_stores.types import (
-    NodeEmbeddingResult,
+    NodeWithEmbedding,
     VectorStore,
     VectorStoreQueryResult,
     VectorStoreQuery,
 )
 
 
 class MockVectorStore(VectorStore):
@@ -20,15 +20,15 @@
     @property
     def client(self) -> Any:
         """Get client."""
         return None
 
     def add(
         self,
-        embedding_results: List[NodeEmbeddingResult],
+        embedding_results: List[NodeWithEmbedding],
     ) -> List[str]:
         """Add embedding results to vector store."""
         raise NotImplementedError()
 
     def delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         """Delete doc."""
         raise NotImplementedError()
```

### Comparing `llama_index-0.6.0a7/tests/indices/conftest.py` & `llama_index-0.6.1/tests/indices/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 import pytest
-from llama_index.data_structs.node_v2 import DocumentRelationship, Node
+from llama_index.data_structs.node import DocumentRelationship, Node
 
 from llama_index.readers.schema.base import Document
 
 
 @pytest.fixture
 def documents() -> List[Document]:
     """Get documents."""
```

### Comparing `llama_index-0.6.0a7/tests/indices/empty/test_base.py` & `llama_index-0.6.1/tests/indices/empty/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Test empty index."""
 
-from llama_index.data_structs.data_structs_v2 import EmptyIndex
+from llama_index.data_structs.data_structs import EmptyIndex
 from llama_index.indices.empty.base import GPTEmptyIndex
 from llama_index.indices.service_context import ServiceContext
 
 
 def test_empty(
     mock_service_context: ServiceContext,
 ) -> None:
```

### Comparing `llama_index-0.6.0a7/tests/indices/keyword_table/test_base.py` & `llama_index-0.6.1/tests/indices/keyword_table/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/keyword_table/test_retrievers.py` & `llama_index-0.6.1/tests/indices/keyword_table/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/keyword_table/test_utils.py` & `llama_index-0.6.1/tests/indices/keyword_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/knowledge_graph/test_base.py` & `llama_index-0.6.1/tests/indices/knowledge_graph/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Test knowledge graph index."""
 
 from typing import Any, Dict, List, Tuple
 from unittest.mock import patch
 
 import pytest
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 from llama_index.embeddings.base import BaseEmbedding
 from llama_index.indices.knowledge_graph.base import GPTKnowledgeGraphIndex
 from llama_index.indices.service_context import ServiceContext
 from llama_index.readers.schema.base import Document
 from tests.mock_utils.mock_prompts import (
     MOCK_KG_TRIPLET_EXTRACT_PROMPT,
     MOCK_QUERY_KEYWORD_EXTRACT_PROMPT,
```

### Comparing `llama_index-0.6.0a7/tests/indices/knowledge_graph/test_retrievers.py` & `llama_index-0.6.1/tests/indices/knowledge_graph/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/list/test_index.py` & `llama_index-0.6.1/tests/indices/list/test_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Test list index."""
 
 from typing import Dict, List, Tuple
 
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 from llama_index.indices.base_retriever import BaseRetriever
 from llama_index.indices.list.base import GPTListIndex, ListRetrieverMode
 from llama_index.indices.service_context import ServiceContext
 from llama_index.readers.schema.base import Document
 
 
 def test_build_list(
```

### Comparing `llama_index-0.6.0a7/tests/indices/list/test_retrievers.py` & `llama_index-0.6.1/tests/indices/list/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/postprocessor/test_base.py` & `llama_index-0.6.1/tests/indices/postprocessor/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 import pytest
 from llama_index.storage.docstore.simple_docstore import SimpleDocumentStore
 
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.prompts.prompts import Prompt, SimpleInputPrompt
 from llama_index.indices.service_context import ServiceContext
-from llama_index.data_structs.node_v2 import Node, DocumentRelationship, NodeWithScore
+from llama_index.data_structs.node import Node, DocumentRelationship, NodeWithScore
 from llama_index.indices.postprocessor.node import (
     PrevNextNodePostprocessor,
     KeywordNodePostprocessor,
 )
 from llama_index.indices.postprocessor.node_recency import (
     FixedRecencyPostprocessor,
     EmbeddingRecencyPostprocessor,
@@ -171,15 +171,15 @@
     node_with_scores = [NodeWithScore(node) for node in nodes]
 
     service_context = ServiceContext.from_defaults()
 
     postprocessor = FixedRecencyPostprocessor(top_k=1, service_context=service_context)
     query_bundle: QueryBundle = QueryBundle(query_str="What is?")
     result_nodes = postprocessor.postprocess_nodes(
-        node_with_scores, extra_info={"query_bundle": query_bundle}
+        node_with_scores, query_bundle=query_bundle
     )
     assert len(result_nodes) == 1
     assert result_nodes[0].node.get_text() == "date: 2020-01-04\n\nThis is a test v2."
 
     # try in node info
     nodes = [
         Node("Hello world.", doc_id="1", node_info={"date": "2020-01-01"}),
@@ -191,15 +191,15 @@
     service_context = ServiceContext.from_defaults()
 
     postprocessor = FixedRecencyPostprocessor(
         top_k=1, service_context=service_context, in_extra_info=False
     )
     query_bundle = QueryBundle(query_str="What is?")
     result_nodes = postprocessor.postprocess_nodes(
-        node_with_scores, extra_info={"query_bundle": query_bundle}
+        node_with_scores, query_bundle=query_bundle
     )
     assert len(result_nodes) == 1
     assert result_nodes[0].node.get_text() == "This is a test v2."
 
 
 @patch.object(LLMPredictor, "predict", side_effect=mock_recency_predict)
 @patch.object(LLMPredictor, "__init__", return_value=None)
@@ -236,15 +236,15 @@
         top_k=1,
         service_context=service_context,
         in_extra_info=False,
         query_embedding_tmpl="{context_str}",
     )
     query_bundle: QueryBundle = QueryBundle(query_str="What is?")
     result_nodes = postprocessor.postprocess_nodes(
-        nodes_with_scores, extra_info={"query_bundle": query_bundle}
+        nodes_with_scores, query_bundle=query_bundle
     )
     assert len(result_nodes) == 4
     assert result_nodes[0].node.get_text() == "This is a test v2."
     assert cast(Dict, result_nodes[0].node_info)["date"] == "2020-01-04"
     assert result_nodes[1].node.get_text() == "This is another test."
     assert result_nodes[1].node.get_doc_id() == "3v2"
     assert cast(Dict, result_nodes[1].node_info)["date"] == "2020-01-03"
```

### Comparing `llama_index-0.6.0a7/tests/indices/query/conftest.py` & `llama_index-0.6.1/tests/indices/query/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/query/query_transform/test_base.py` & `llama_index-0.6.1/tests/indices/query/query_transform/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/query/test_compose.py` & `llama_index-0.6.1/tests/indices/query/test_compose.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/query/test_compose_vector.py` & `llama_index-0.6.1/tests/indices/query/test_compose_vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 import sys
 from typing import Any, Dict, List
 from unittest.mock import MagicMock
 
 import pytest
 
-from llama_index.data_structs.data_structs_v2 import V2IndexStruct
+from llama_index.data_structs.data_structs import IndexStruct
 from llama_index.embeddings.base import BaseEmbedding
 from llama_index.indices.composability.graph import ComposableGraph
 from llama_index.indices.keyword_table.simple_base import GPTSimpleKeywordTableIndex
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.vector_store.base import GPTVectorStoreIndex
 from llama_index.readers.schema.base import Document
 from llama_index.storage.storage_context import StorageContext
@@ -142,16 +142,16 @@
     # try building a list for every two, then a tree
     vector1 = GPTVectorStoreIndex.from_documents(
         documents[0:2], service_context=mock_service_context, **vector_kwargs
     )
     vector2 = GPTVectorStoreIndex.from_documents(
         documents[2:4], service_context=mock_service_context, **vector_kwargs
     )
-    assert isinstance(vector1.index_struct, V2IndexStruct)
-    assert isinstance(vector2.index_struct, V2IndexStruct)
+    assert isinstance(vector1.index_struct, IndexStruct)
+    assert isinstance(vector2.index_struct, IndexStruct)
     vector1.index_struct.index_id = "vector1"
     vector2.index_struct.index_id = "vector2"
     summaries = [
         "foo bar",
         "apple orange",
     ]
```

### Comparing `llama_index-0.6.0a7/tests/indices/query/test_query_bundle.py` & `llama_index-0.6.1/tests/indices/query/test_query_bundle.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/struct_store/conftest.py` & `llama_index-0.6.1/tests/indices/struct_store/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/struct_store/test_base.py` & `llama_index-0.6.1/tests/indices/struct_store/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from llama_index.indices.struct_store.sql_query import GPTNLStructStoreQueryEngine
 from llama_index.langchain_helpers.sql_wrapper import SQLDatabase
 from llama_index.readers.schema.base import Document
 from llama_index.schema import BaseDocument
 from tests.mock_utils.mock_prompts import (
     MOCK_TABLE_CONTEXT_PROMPT,
 )
-from llama_index.data_structs.node_v2 import Node, DocumentRelationship
+from llama_index.data_structs.node import Node, DocumentRelationship
 
 
 def _delete_table_items(engine: Any, table: Table) -> None:
     """Delete items from a table."""
     delete_stmt = delete(table)
     with engine.connect() as connection:
         connection.execute(delete_stmt)
```

### Comparing `llama_index-0.6.0a7/tests/indices/struct_store/test_pandas.py` & `llama_index-0.6.1/tests/indices/struct_store/test_pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/struct_store/test_sql_query.py` & `llama_index-0.6.1/tests/indices/struct_store/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/test_loading.py` & `llama_index-0.6.1/tests/indices/test_loading.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from pathlib import Path
 from typing import List
 import pytest
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 from llama_index.indices.list.base import GPTListIndex
 from llama_index.indices.loading import (
     load_index_from_storage,
     load_indices_from_storage,
 )
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.vector_store.base import GPTVectorStoreIndex
```

### Comparing `llama_index-0.6.0a7/tests/indices/test_loading_graph.py` & `llama_index-0.6.1/tests/indices/test_loading_graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/test_node_utils.py` & `llama_index-0.6.1/tests/indices/test_node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/test_prompt_helper.py` & `llama_index-0.6.1/tests/indices/test_prompt_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Test PromptHelper."""
 from typing import List, cast
 
 from langchain import PromptTemplate as LangchainPrompt
 
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 from llama_index.indices.prompt_helper import PromptHelper
 from llama_index.prompts.base import Prompt
 from tests.mock_utils.mock_utils import mock_tokenizer
 
 
 class TestPrompt(Prompt):
     """Test prompt class."""
```

### Comparing `llama_index-0.6.0a7/tests/indices/tree/conftest.py` & `llama_index-0.6.1/tests/indices/tree/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/tree/test_embedding_retriever.py` & `llama_index-0.6.1/tests/indices/tree/test_embedding_retriever.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from collections import defaultdict
 from typing import Any, Dict, List
 from unittest.mock import patch
 
 import pytest
 
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.tree.select_leaf_embedding_retriever import (
     TreeSelectLeafEmbeddingRetriever,
 )
 from llama_index.indices.tree.base import GPTTreeIndex
 from llama_index.langchain_helpers.chain_wrapper import (
```

### Comparing `llama_index-0.6.0a7/tests/indices/tree/test_index.py` & `llama_index-0.6.1/tests/indices/tree/test_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Test tree index."""
 
 from typing import Any, Dict, List, Optional
 from unittest.mock import patch
 
-from llama_index.data_structs.data_structs_v2 import IndexGraph
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.data_structs import IndexGraph
+from llama_index.data_structs.node import Node
 from llama_index.indices.service_context import ServiceContext
 from llama_index.storage.docstore import BaseDocumentStore
 from llama_index.indices.tree.base import GPTTreeIndex
 from llama_index.readers.schema.base import Document
 
 
 def _get_left_or_right_node(
```

### Comparing `llama_index-0.6.0a7/tests/indices/tree/test_retrievers.py` & `llama_index-0.6.1/tests/indices/tree/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/vector_store/conftest.py` & `llama_index-0.6.1/tests/indices/vector_store/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/vector_store/mock_faiss.py` & `llama_index-0.6.1/tests/indices/vector_store/mock_faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/vector_store/mock_services.py` & `llama_index-0.6.1/tests/indices/vector_store/mock_services.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/vector_store/test_faiss.py` & `llama_index-0.6.1/tests/indices/vector_store/test_faiss.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Test vector store indexes."""
 
 import os
 from pathlib import Path
 from typing import List
 
 import pytest
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.vector_store.base import GPTVectorStoreIndex
 
 from llama_index.readers.schema.base import Document
 from llama_index.storage.storage_context import StorageContext
 from llama_index.vector_stores.faiss import FaissVectorStore
-from llama_index.vector_stores.types import NodeEmbeddingResult, VectorStoreQuery
+from llama_index.vector_stores.types import NodeWithEmbedding, VectorStoreQuery
 
 
 @pytest.mark.skipif("CI" in os.environ, reason="no FAISS in CI")
 def test_build_faiss(
     documents: List[Document],
     faiss_storage_context: StorageContext,
     mock_service_context: ServiceContext,
@@ -67,19 +67,17 @@
 def test_persist(tmp_path: Path) -> None:
     import faiss
 
     vector_store = FaissVectorStore(faiss_index=faiss.IndexFlatL2(5))
 
     vector_store.add(
         [
-            NodeEmbeddingResult(
-                id="test id",
+            NodeWithEmbedding(
                 node=Node("test text"),
                 embedding=[0, 0, 0, 1, 1],
-                doc_id="test_doc",
             )
         ]
     )
 
     result = vector_store.query(VectorStoreQuery(query_embedding=[0, 0, 0, 1, 1]))
 
     persist_path = str(tmp_path / "faiss.index")
```

### Comparing `llama_index-0.6.0a7/tests/indices/vector_store/test_milvus.py` & `llama_index-0.6.1/tests/indices/vector_store/test_milvus.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from typing import Any, List, Optional
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.vector_store import GPTVectorStoreIndex
 from llama_index.storage.storage_context import StorageContext
 
 from llama_index.vector_stores.types import (
-    NodeEmbeddingResult,
+    NodeWithEmbedding,
     VectorStore,
     VectorStoreQuery,
     VectorStoreQueryResult,
 )
 
 
 class MockMilvusVectorStore(VectorStore):
@@ -44,15 +44,15 @@
 
     @property
     def client(self) -> Any:
         return None
 
     def add(
         self,
-        embedding_results: List[NodeEmbeddingResult],
+        embedding_results: List[NodeWithEmbedding],
     ) -> List[str]:
         return []
 
     def delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         return None
 
     def query(self, query: VectorStoreQuery) -> VectorStoreQueryResult:
```

### Comparing `llama_index-0.6.0a7/tests/indices/vector_store/test_myscale.py` & `llama_index-0.6.1/tests/indices/vector_store/test_myscale.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from llama_index.storage.storage_context import StorageContext
 
 try:
     import clickhouse_connect
 except ImportError:
     clickhouse_connect = None  # type: ignore
 
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 from llama_index.readers.schema.base import Document
 from llama_index.vector_stores import MyScaleVectorStore
 from llama_index.vector_stores.types import VectorStoreQuery
 
 # local test only, update variable here for test
 MYSCALE_CLUSTER_URL = None
 MYSCALE_USERNAME = None
```

### Comparing `llama_index-0.6.0a7/tests/indices/vector_store/test_pinecone.py` & `llama_index-0.6.1/tests/indices/vector_store/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/indices/vector_store/test_retrievers.py` & `llama_index-0.6.1/tests/indices/vector_store/test_retrievers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List, cast
-from llama_index.data_structs.node_v2 import DocumentRelationship, Node
+from llama_index.data_structs.node import DocumentRelationship, Node
 from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.vector_store.base import GPTVectorStoreIndex
 from llama_index.readers.schema.base import Document
 from llama_index.storage.storage_context import StorageContext
 from llama_index.vector_stores.simple import SimpleVectorStore
```

### Comparing `llama_index-0.6.0a7/tests/indices/vector_store/test_simple.py` & `llama_index-0.6.1/tests/indices/vector_store/test_simple.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Test vector store indexes."""
 
 from typing import Any, List, cast
+from llama_index.indices.loading import load_index_from_storage
 
 
 from llama_index.indices.service_context import ServiceContext
 from llama_index.indices.vector_store.base import GPTVectorStoreIndex
 
 from llama_index.readers.schema.base import Document
+from llama_index.storage.storage_context import StorageContext
 from llama_index.vector_stores.simple import SimpleVectorStore
 
 
 def test_build_simple(
     mock_service_context: ServiceContext,
     documents: List[Document],
 ) -> None:
@@ -137,7 +139,31 @@
     ]
     for text_id in index.index_struct.nodes_dict.keys():
         node_id = index.index_struct.nodes_dict[text_id]
         node = index.docstore.get_node(node_id)
         vector_store = cast(SimpleVectorStore, index._vector_store)
         embedding = vector_store.get(text_id)
         assert (node.text, embedding) in actual_node_tups
+
+
+def test_simple_insert_save(
+    documents: List[Document],
+    mock_service_context: ServiceContext,
+) -> None:
+    storage_context = StorageContext.from_defaults()
+    index = GPTVectorStoreIndex.from_documents(
+        documents=documents,
+        service_context=mock_service_context,
+        storage_context=storage_context,
+    )
+    assert isinstance(index, GPTVectorStoreIndex)
+
+    loaded_index = load_index_from_storage(storage_context=storage_context)
+    assert isinstance(loaded_index, GPTVectorStoreIndex)
+    assert index.index_struct == loaded_index.index_struct
+
+    # insert into index
+    index.insert(Document(text="This is a test v3."))
+
+    loaded_index = load_index_from_storage(storage_context=storage_context)
+    assert isinstance(loaded_index, GPTVectorStoreIndex)
+    assert index.index_struct == loaded_index.index_struct
```

### Comparing `llama_index-0.6.0a7/tests/indices/vector_store/test_weaviate.py` & `llama_index-0.6.1/tests/indices/vector_store/test_weaviate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, List, Optional
 from unittest.mock import Mock
 from llama_index.indices.service_context import ServiceContext
 
 from llama_index.indices.vector_store import GPTVectorStoreIndex
 from llama_index.storage.storage_context import StorageContext
 from llama_index.vector_stores.types import (
-    NodeEmbeddingResult,
+    NodeWithEmbedding,
     VectorStore,
     VectorStoreQuery,
     VectorStoreQueryResult,
 )
 
 
 class MockWeaviateVectorStore(VectorStore):
@@ -26,15 +26,15 @@
 
     @property
     def client(self) -> Any:
         return None
 
     def add(
         self,
-        embedding_results: List[NodeEmbeddingResult],
+        embedding_results: List[NodeWithEmbedding],
     ) -> List[str]:
         return []
 
     def delete(self, doc_id: str, **delete_kwargs: Any) -> None:
         return None
 
     def query(self, query: VectorStoreQuery) -> VectorStoreQueryResult:
```

### Comparing `llama_index-0.6.0a7/tests/indices/vector_store/utils.py` & `llama_index-0.6.1/tests/indices/vector_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/langchain_helpers/test_text_splitter.py` & `llama_index-0.6.1/tests/langchain_helpers/test_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/llm_predictor/test_base.py` & `llama_index-0.6.1/tests/llm_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/logger/test_base.py` & `llama_index-0.6.1/tests/logger/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/mock_utils/mock_predict.py` & `llama_index-0.6.1/tests/mock_utils/mock_predict.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/mock_utils/mock_prompts.py` & `llama_index-0.6.1/tests/mock_utils/mock_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/mock_utils/mock_text_splitter.py` & `llama_index-0.6.1/tests/mock_utils/mock_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/mock_utils/mock_utils.py` & `llama_index-0.6.1/tests/mock_utils/mock_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/optimization/test_base.py` & `llama_index-0.6.1/tests/optimization/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/output_parsers/test_base.py` & `llama_index-0.6.1/tests/output_parsers/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/output_parsers/test_selection.py` & `llama_index-0.6.1/tests/output_parsers/test_selection.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/playground/test_base.py` & `llama_index-0.6.1/tests/playground/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/prompts/test_base.py` & `llama_index-0.6.1/tests/prompts/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/readers/test_file.py` & `llama_index-0.6.1/tests/readers/test_file.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/readers/test_json.py` & `llama_index-0.6.1/tests/readers/test_json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/readers/test_mongo.py` & `llama_index-0.6.1/tests/readers/test_mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/selectors/test_llm_selectors.py` & `llama_index-0.6.1/tests/selectors/test_llm_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/storage/conftest.py` & `llama_index-0.6.1/tests/storage/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/storage/docstore/test_mongo_docstore.py` & `llama_index-0.6.1/tests/storage/docstore/test_mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/storage/docstore/test_simple_docstore.py` & `llama_index-0.6.1/tests/storage/docstore/test_simple_docstore.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Test docstore."""
 
 
 from pathlib import Path
 import pytest
-from llama_index.data_structs.node_v2 import Node
+from llama_index.data_structs.node import Node
 from llama_index.storage.docstore import SimpleDocumentStore
 from llama_index.readers.schema.base import Document
 from llama_index.storage.kvstore.simple_kvstore import SimpleKVStore
 
 
 @pytest.fixture()
 def simple_docstore(simple_kvstore: SimpleKVStore) -> SimpleDocumentStore:
@@ -41,7 +41,24 @@
 
     # load from persist dir and get documents
     new_docstore = SimpleDocumentStore.from_persist_path(persist_path)
     gd1 = new_docstore.get_document("d1")
     assert gd1 == doc
     gd2 = new_docstore.get_document("d2")
     assert gd2 == node
+
+
+def test_docstore_dict() -> None:
+    doc = Document("hello world", doc_id="d1", extra_info={"foo": "bar"})
+    node = Node("my node", doc_id="d2", node_info={"node": "info"})
+
+    # add documents and then save to dict
+    docstore = SimpleDocumentStore()
+    docstore.add_documents([doc, node])
+    save_dict = docstore.to_dict()
+
+    # load from dict and get documents
+    new_docstore = SimpleDocumentStore.from_dict(save_dict)
+    gd1 = new_docstore.get_document("d1")
+    assert gd1 == doc
+    gd2 = new_docstore.get_document("d2")
+    assert gd2 == node
```

### Comparing `llama_index-0.6.0a7/tests/test_utils.py` & `llama_index-0.6.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/token_predictor/test_base.py` & `llama_index-0.6.1/tests/token_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.6.0a7/tests/vector_stores/test_qdrant.py` & `llama_index-0.6.1/tests/vector_stores/test_qdrant.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,44 +3,43 @@
 import pytest
 
 try:
     import qdrant_client
 except ImportError:
     qdrant_client = None  # type: ignore
 
-from llama_index.data_structs import Node
+from llama_index.data_structs.node import Node, DocumentRelationship
 from llama_index.vector_stores import QdrantVectorStore
-from llama_index.vector_stores.types import NodeEmbeddingResult, VectorStoreQuery
+from llama_index.vector_stores.types import NodeWithEmbedding, VectorStoreQuery
 
 
 @pytest.fixture
-def node() -> Node:
-    return Node(text="lorem ipsum")
-
-
-@pytest.fixture
-def node_embeddings(node: Node) -> List[NodeEmbeddingResult]:
+def node_embeddings() -> List[NodeWithEmbedding]:
     return [
-        NodeEmbeddingResult(
-            id="c330d77f-90bd-4c51-9ed2-57d8d693b3b0",
+        NodeWithEmbedding(
             embedding=[1.0, 0.0],
-            doc_id="test-0",
-            node=node,
+            node=Node(
+                text="lorem ipsum",
+                doc_id="c330d77f-90bd-4c51-9ed2-57d8d693b3b0",
+                relationships={DocumentRelationship.SOURCE: "test-0"},
+            ),
         ),
-        NodeEmbeddingResult(
-            id="c3d1e1dd-8fb4-4b8f-b7ea-7fa96038d39d",
+        NodeWithEmbedding(
             embedding=[0.0, 1.0],
-            doc_id="test-1",
-            node=node,
+            node=Node(
+                text="lorem ipsum",
+                doc_id="c3d1e1dd-8fb4-4b8f-b7ea-7fa96038d39d",
+                relationships={DocumentRelationship.SOURCE: "test-1"},
+            ),
         ),
     ]
 
 
 @pytest.mark.skipif(qdrant_client is None, reason="qdrant-client not installed")
-def test_add_stores_data(node_embeddings: List[NodeEmbeddingResult]) -> None:
+def test_add_stores_data(node_embeddings: List[NodeWithEmbedding]) -> None:
     client = qdrant_client.QdrantClient(":memory:")
     qdrant_vector_store = QdrantVectorStore(collection_name="test", client=client)
 
     with pytest.raises(ValueError):
         client.count("test")  # That indicates the collection does not exist
 
     qdrant_vector_store.add(node_embeddings)
```

### Comparing `llama_index-0.6.0a7/tests/vector_stores/test_weaviate.py` & `llama_index-0.6.1/tests/vector_stores/test_weaviate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sys
 from unittest.mock import MagicMock
-from llama_index.data_structs.node_v2 import Node
-from llama_index.vector_stores.types import NodeEmbeddingResult
+from llama_index.data_structs.node import DocumentRelationship, Node
+from llama_index.vector_stores.types import NodeWithEmbedding
 
 from llama_index.vector_stores.weaviate import WeaviateVectorStore
 
 
 def test_weaviate_add() -> None:
     # mock import
     sys.modules["weaviate"] = MagicMock()
@@ -13,18 +13,20 @@
     batch_context_manager = MagicMock()
     weaviate_client.batch.__enter__.return_value = batch_context_manager
 
     vector_store = WeaviateVectorStore(weaviate_client=weaviate_client)
 
     vector_store.add(
         [
-            NodeEmbeddingResult(
-                id="test node id",
-                node=Node(text="test node text"),
+            NodeWithEmbedding(
+                node=Node(
+                    text="test node text",
+                    doc_id="test node id",
+                    relationships={DocumentRelationship.SOURCE: "test doc id"},
+                ),
                 embedding=[0.5, 0.5],
-                doc_id="test doc id",
             )
         ]
     )
 
     args, _ = batch_context_manager.add_data_object.call_args
     assert args[-1] == [0.5, 0.5]
```

