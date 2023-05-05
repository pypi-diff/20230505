# Comparing `tmp/canals-0.1.0.tar.gz` & `tmp/canals-0.1.1.tar.gz`

## Comparing `canals-0.1.0.tar` & `canals-0.1.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.1.0/mkdocs.yml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.1.0/.github/workflows/api-docs.yml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 canals-0.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 canals-0.1.0/canals/__about__.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 canals-0.1.0/canals/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 canals-0.1.0/canals/errors.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 canals-0.1.0/canals/component/__init__.py
--rw-r--r--   0        0        0     8469 2020-02-02 00:00:00.000000 canals-0.1.0/canals/component/component.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 canals-0.1.0/canals/component/save_init_params.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 canals-0.1.0/canals/draw/__init__.py
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 canals-0.1.0/canals/draw/draw.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 canals-0.1.0/canals/draw/graphviz.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 canals-0.1.0/canals/draw/mermaid.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 canals-0.1.0/canals/pipeline/__init__.py
--rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 canals-0.1.0/canals/pipeline/_utils.py
--rw-r--r--   0        0        0    26696 2020-02-02 00:00:00.000000 canals-0.1.0/canals/pipeline/pipeline.py
--rw-r--r--   0        0        0     8637 2020-02-02 00:00:00.000000 canals-0.1.0/canals/pipeline/save_load.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.1.0/docs/index.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 canals-0.1.0/docs/api-docs/component.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.1.0/docs/api-docs/draw.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.1.0/docs/api-docs/pipeline.md
--rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 canals-0.1.0/docs/concepts/components.md
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 canals-0.1.0/docs/concepts/concepts.md
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 canals-0.1.0/docs/concepts/pipelines.md
--rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.1.0/images/canals-logo-dark.png
--rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.1.0/images/canals-logo-light.png
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 canals-0.1.0/test/__init__.py
--rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_save_load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/__init__.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_complex_pipeline.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_fixed_decision_pipeline.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_fixed_merging_pipeline.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_linear_pipeline.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_looping_and_merge_pipeline.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_looping_pipeline.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_parallel_branches_pipeline.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_variable_decision_pipeline.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_variable_merging_pipeline.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/unit/__init__.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/unit/test_component.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/__init__.py
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_accumulate.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_add_value.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_double.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_greet.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_merge_loop.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_parity.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_remainder.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_repeat.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_subtract.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_sum.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_threshold.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 canals-0.1.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.1.0/LICENSE
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 canals-0.1.0/README.md
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 canals-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 canals-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.1.1/mkdocs.yml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.1.1/.github/workflows/api-docs.yml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 canals-0.1.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 canals-0.1.1/canals/__about__.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 canals-0.1.1/canals/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 canals-0.1.1/canals/errors.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 canals-0.1.1/canals/component/__init__.py
+-rw-r--r--   0        0        0     8469 2020-02-02 00:00:00.000000 canals-0.1.1/canals/component/component.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 canals-0.1.1/canals/component/save_init_params.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 canals-0.1.1/canals/draw/__init__.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 canals-0.1.1/canals/draw/draw.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 canals-0.1.1/canals/draw/graphviz.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 canals-0.1.1/canals/draw/mermaid.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 canals-0.1.1/canals/pipeline/__init__.py
+-rw-r--r--   0        0        0     7966 2020-02-02 00:00:00.000000 canals-0.1.1/canals/pipeline/_utils.py
+-rw-r--r--   0        0        0    26696 2020-02-02 00:00:00.000000 canals-0.1.1/canals/pipeline/pipeline.py
+-rw-r--r--   0        0        0     8637 2020-02-02 00:00:00.000000 canals-0.1.1/canals/pipeline/save_load.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.1.1/docs/index.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 canals-0.1.1/docs/api-docs/component.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.1.1/docs/api-docs/draw.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.1.1/docs/api-docs/pipeline.md
+-rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 canals-0.1.1/docs/concepts/components.md
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 canals-0.1.1/docs/concepts/concepts.md
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 canals-0.1.1/docs/concepts/pipelines.md
+-rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.1.1/images/canals-logo-dark.png
+-rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.1.1/images/canals-logo-light.png
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 canals-0.1.1/test/__init__.py
+-rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_save_load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/__init__.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_complex_pipeline.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_fixed_decision_pipeline.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_fixed_merging_pipeline.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_linear_pipeline.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_looping_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_looping_pipeline.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_parallel_branches_pipeline.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_variable_decision_pipeline.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/integration/test_variable_merging_pipeline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/unit/__init__.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 canals-0.1.1/test/pipelines/unit/test_component.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/__init__.py
+-rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_accumulate.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_add_value.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_double.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_greet.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_merge_loop.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_parity.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_remainder.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_repeat.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_subtract.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_sum.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 canals-0.1.1/test/test_components/test_threshold.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 canals-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 canals-0.1.1/README.md
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 canals-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 canals-0.1.1/PKG-INFO
```

### Comparing `canals-0.1.0/.pre-commit-config.yaml` & `canals-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/mkdocs.yml` & `canals-0.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/.github/workflows/tests.yml` & `canals-0.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/canals/component/component.py` & `canals-0.1.1/canals/component/component.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/canals/component/save_init_params.py` & `canals-0.1.1/canals/component/save_init_params.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/canals/draw/draw.py` & `canals-0.1.1/canals/draw/draw.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,21 +76,21 @@
     # Label the edges
     for inp, outp, key, data in graph.edges(keys=True, data=True):
         data["label"] = f"{data['from_socket'].name} -> {data['to_socket'].name}"
         graph.add_edge(inp, outp, key=key, **data)
 
     # Draw the inputs
     graph.add_node("input")
-    for in_node, in_sockets in find_pipeline_inputs(graph).items():
+    for node, in_sockets in find_pipeline_inputs(graph).items():
         for in_socket in in_sockets:
-            if not in_socket.has_default and not (
-                graph.nodes[in_node]["variadic_input"] and not graph.in_edges(in_node)
-            ):
-                graph.add_edge("input", in_node, label=in_socket.name)
+            node_instance = graph.nodes[node]["instance"]
+            input_node_defaults = hasattr(node_instance, "defaults") and in_socket.name in node_instance.defaults
+            if not input_node_defaults and not (graph.nodes[node]["variadic_input"] and not graph.in_edges(node)):
+                graph.add_edge("input", node, label=in_socket.name)
 
     # Draw the outputs
     graph.add_node("output")
-    for out_node, out_sockets in find_pipeline_outputs(graph).items():
+    for node, out_sockets in find_pipeline_outputs(graph).items():
         for out_socket in out_sockets:
-            graph.add_edge(out_node, "output", label=out_socket.name)
+            graph.add_edge(node, "output", label=out_socket.name)
 
     return graph
```

### Comparing `canals-0.1.0/canals/draw/graphviz.py` & `canals-0.1.1/canals/draw/graphviz.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/canals/draw/mermaid.py` & `canals-0.1.1/canals/draw/mermaid.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/canals/pipeline/_utils.py` & `canals-0.1.1/canals/pipeline/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     type: type
 
 
 @dataclass
 class InputSocket:
     name: str
     type: type
-    has_default: bool
     variadic: bool
     taken_by: Optional[str] = None
 
 
 def parse_connection_name(connection: str) -> Tuple[str, Optional[str]]:
     """
     Returns component-connection pairs from a connect_to/from string
@@ -45,17 +44,16 @@
     run_signature = inspect.signature(component.run)
 
     input_sockets = {}
     for param in run_signature.parameters:
         name = run_signature.parameters[param].name
         variadic = run_signature.parameters[param].kind == inspect.Parameter.VAR_POSITIONAL
         annotation = run_signature.parameters[param].annotation
-        has_default = param in component.defaults.keys()
 
-        socket = InputSocket(name=name, type=annotation, has_default=has_default, variadic=variadic)
+        socket = InputSocket(name=name, type=annotation, variadic=variadic)
         input_sockets[socket.name] = socket
 
     return input_sockets
 
 
 def find_output_sockets(component) -> Dict[str, OutputSocket]:
     """
@@ -148,14 +146,36 @@
     return {
         node: list(data.get("output_sockets", {}).values())
         for node, data in graph.nodes(data=True)
         if not graph.out_edges(node)
     }
 
 
+def _validate_input_sockets_are_connected(graph: networkx.MultiDiGraph, inputs_values: Dict[str, Dict[str, Any]]):
+    valid_inputs = find_pipeline_inputs(graph)
+    for node, sockets in valid_inputs.items():
+        if node in inputs_values:
+            for socket in sockets:
+                node_instance = graph.nodes[node]["instance"]
+                input_in_node_defaults = hasattr(node_instance, "defaults") and socket.name in node_instance.defaults
+                if not input_in_node_defaults and not socket.name in inputs_values[node]:
+                    raise ValueError(f"Missing input: {node}.{socket.name}")
+
+
+def _validate_nodes_receive_only_expected_input(graph: networkx.MultiDiGraph, inputs_values: Dict[str, Dict[str, Any]]):
+    for node, input_data in inputs_values.items():
+        for socket_name in input_data.keys():
+            if not socket_name in graph.nodes[node]["input_sockets"].keys():
+                raise ValueError(f"Component {node} is not expecting any input value called {socket_name}")
+
+            taken_by = graph.nodes[node]["input_sockets"][socket_name].taken_by
+            if taken_by:
+                raise ValueError(f"The input {socket_name} of {node} is already taken by node {taken_by}")
+
+
 def validate_pipeline_input(  # pylint: disable=too-many-branches
     graph: networkx.MultiDiGraph, inputs_values: Dict[str, Dict[str, Any]]
 ) -> Dict[str, Dict[str, Any]]:
     """
     Make sure the pipeline is properly built and that the input received makes sense.
 
     Returns the input values, validated and updated at need.
@@ -166,30 +186,18 @@
 
     # Make sure the input keys are all nodes of the pipeline
     unknown_components = [key for key in inputs_values.keys() if not key in graph.nodes]
     if unknown_components:
         raise ValueError(f"Pipeline received data for unknown component(s): {', '.join(unknown_components)}")
 
     # Make sure all necessary sockets are connected
-    valid_inputs = find_pipeline_inputs(graph)
-    for node, sockets in valid_inputs.items():
-        if node in inputs_values.keys():
-            for socket in sockets:
-                if not socket.has_default and not socket.name in inputs_values[node]:
-                    raise ValueError(f"Missing input: {node}.{socket.name}")
-
-    # Make sure no inputs are given for connected sockets
-    for node, input_data in inputs_values.items():
-        for socket_name in input_data.keys():
-            if not socket_name in graph.nodes[node]["input_sockets"].keys():
-                raise ValueError(f"Component {node} is not expecting any input value called {socket_name}")
+    _validate_input_sockets_are_connected(graph, inputs_values)
 
-            taken_by = graph.nodes[node]["input_sockets"][socket_name].taken_by
-            if taken_by:
-                raise ValueError(f"The input {socket_name} of {node} is already taken by node {taken_by}")
+    # Make sure that the pipeline input is only sent to nodes that won't receive data from other nodes
+    _validate_nodes_receive_only_expected_input(graph, inputs_values)
 
     # Make sure variadic input components are receiving lists
     for component in input_components.keys():
         if graph.nodes[component]["variadic_input"] and component in inputs_values.keys():
             for key, value in inputs_values[component].items():  # should be just one
                 if not isinstance(value, Iterable):
                     inputs_values[component][key] = [value]
```

### Comparing `canals-0.1.0/canals/pipeline/pipeline.py` & `canals-0.1.1/canals/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/canals/pipeline/save_load.py` & `canals-0.1.1/canals/pipeline/save_load.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/docs/index.md` & `canals-0.1.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/docs/concepts/components.md` & `canals-0.1.1/docs/concepts/components.md`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/docs/concepts/concepts.md` & `canals-0.1.1/docs/concepts/concepts.md`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/docs/concepts/pipelines.md` & `canals-0.1.1/docs/concepts/pipelines.md`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/images/canals-logo-dark.png` & `canals-0.1.1/images/canals-logo-dark.png`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/images/canals-logo-light.png` & `canals-0.1.1/images/canals-logo-light.png`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/test_save_load.py` & `canals-0.1.1/test/test_save_load.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/pipelines/integration/test_complex_pipeline.py` & `canals-0.1.1/test/pipelines/integration/test_complex_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py` & `canals-0.1.1/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/pipelines/integration/test_fixed_decision_pipeline.py` & `canals-0.1.1/test/pipelines/integration/test_fixed_decision_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/pipelines/integration/test_fixed_merging_pipeline.py` & `canals-0.1.1/test/pipelines/integration/test_fixed_merging_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/pipelines/integration/test_linear_pipeline.py` & `canals-0.1.1/test/pipelines/integration/test_linear_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/pipelines/integration/test_looping_and_merge_pipeline.py` & `canals-0.1.1/test/pipelines/integration/test_looping_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/pipelines/integration/test_looping_pipeline.py` & `canals-0.1.1/test/pipelines/integration/test_looping_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/pipelines/integration/test_parallel_branches_pipeline.py` & `canals-0.1.1/test/pipelines/integration/test_parallel_branches_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py` & `canals-0.1.1/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/pipelines/integration/test_variable_decision_pipeline.py` & `canals-0.1.1/test/pipelines/integration/test_variable_decision_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/pipelines/integration/test_variable_merging_pipeline.py` & `canals-0.1.1/test/pipelines/integration/test_variable_merging_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/pipelines/unit/test_component.py` & `canals-0.1.1/test/pipelines/unit/test_component.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/test_components/__init__.py` & `canals-0.1.1/test/test_components/__init__.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/test_components/test_accumulate.py` & `canals-0.1.1/test/test_components/test_accumulate.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/test_components/test_add_value.py` & `canals-0.1.1/test/test_components/test_add_value.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/test_components/test_double.py` & `canals-0.1.1/test/test_components/test_double.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/test_components/test_greet.py` & `canals-0.1.1/test/test_components/test_greet.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/test_components/test_merge_loop.py` & `canals-0.1.1/test/test_components/test_merge_loop.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/test_components/test_parity.py` & `canals-0.1.1/test/test_components/test_parity.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/test_components/test_remainder.py` & `canals-0.1.1/test/test_components/test_remainder.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/test_components/test_repeat.py` & `canals-0.1.1/test/test_components/test_repeat.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/test_components/test_subtract.py` & `canals-0.1.1/test/test_components/test_subtract.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/test_components/test_sum.py` & `canals-0.1.1/test/test_components/test_sum.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/test/test_components/test_threshold.py` & `canals-0.1.1/test/test_components/test_threshold.py`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/.gitignore` & `canals-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/LICENSE` & `canals-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/README.md` & `canals-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/pyproject.toml` & `canals-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `canals-0.1.0/PKG-INFO` & `canals-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canals
-Version: 0.1.0
+Version: 0.1.1
 Summary: A component orchestration engine for Haystack
 Project-URL: Documentation, https://github.com/deepset-ai/canals#readme
 Project-URL: Issues, https://github.com/deepset-ai/canals/issues
 Project-URL: Source, https://github.com/deepset-ai/canals
 Author-email: ZanSara <sara.zanzottera@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

