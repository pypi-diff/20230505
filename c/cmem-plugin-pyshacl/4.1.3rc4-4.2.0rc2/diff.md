# Comparing `tmp/cmem_plugin_pyshacl-4.1.3rc4.tar.gz` & `tmp/cmem_plugin_pyshacl-4.2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_pyshacl-4.1.3rc4.tar", max compression
+gzip compressed data, was "cmem_plugin_pyshacl-4.2.0rc2.tar", max compression
```

## Comparing `cmem_plugin_pyshacl-4.1.3rc4.tar` & `cmem_plugin_pyshacl-4.2.0rc2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11334 2023-05-04 11:35:32.707267 cmem_plugin_pyshacl-4.1.3rc4/LICENSE
--rw-r--r--   0        0        0     4568 2023-05-04 11:35:32.707267 cmem_plugin_pyshacl-4.1.3rc4/README-public.md
--rwxr-xr-x   0        0        0       46 2023-05-04 11:35:59.715733 cmem_plugin_pyshacl-4.1.3rc4/cmem_plugin_pyshacl/__init__.py
--rw-r--r--   0        0        0    27921 2023-05-04 11:35:32.707267 cmem_plugin_pyshacl-4.1.3rc4/cmem_plugin_pyshacl/plugin_pyshacl.py
--rw-r--r--   0        0        0     1875 2023-05-04 11:35:59.711733 cmem_plugin_pyshacl-4.1.3rc4/pyproject.toml
--rw-r--r--   0        0        0     5940 1970-01-01 00:00:00.000000 cmem_plugin_pyshacl-4.1.3rc4/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-05-05 09:08:21.676634 cmem_plugin_pyshacl-4.2.0rc2/LICENSE
+-rw-r--r--   0        0        0     4312 2023-05-05 09:08:21.676634 cmem_plugin_pyshacl-4.2.0rc2/README-public.md
+-rwxr-xr-x   0        0        0       46 2023-05-05 09:08:51.840615 cmem_plugin_pyshacl-4.2.0rc2/cmem_plugin_pyshacl/__init__.py
+-rw-r--r--   0        0        0    27570 2023-05-05 09:08:21.676634 cmem_plugin_pyshacl-4.2.0rc2/cmem_plugin_pyshacl/plugin_pyshacl.py
+-rw-r--r--   0        0        0     1875 2023-05-05 09:08:51.836615 cmem_plugin_pyshacl-4.2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     5684 1970-01-01 00:00:00.000000 cmem_plugin_pyshacl-4.2.0rc2/PKG-INFO
```

### Comparing `cmem_plugin_pyshacl-4.1.3rc4/LICENSE` & `cmem_plugin_pyshacl-4.2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_pyshacl-4.1.3rc4/README-public.md` & `cmem_plugin_pyshacl-4.2.0rc2/README-public.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,24 +78,24 @@
 Enable SHACL Advanced Features. Default value: *false*.
 
 
 ## Parameter Input
 
 In order to set options via the input the following parameter names can be used:
 
-| Option                                         | Name                                  |
-|------------------------------------------------|---------------------------------------|
-| Data graph URI                                 | data_graph_uri                        |
-| SHACL graph URI                                | shacl_graph_uri                       |
-| Generate validation graph                      | generate_graph                        |
-| Validation graph URI                           | validation_graph_uri                  |
-| Output entities                                | output_values                         |
-| Clear validation graph                         | clear_validation_graph                |
-| Resolve owl:imports                            | owl_imports_resolution                |
-| Blank node skolemization                       | skolemize_validation_graph            |
-| Add labels                                     | add_labels_to_validation_graph        |
-| Add labels from data and SHACL graphs          | include_graphs_labels                 |
-| Add shui:conforms flag to focus node resources | add_shui_conforms_to_validation_graph | 
-| Meta-SHACL                                     | meta_shacl                            |
-| Ontology graph URI                             | ontology_graph_uri                    |
-| Inference                                      | inference                             |
-| Advanced                                       | advanced                              |
+| Option                                         | Name                   |
+|------------------------------------------------|------------------------|
+| Data graph URI                                 | data_graph_uri         |
+| SHACL graph URI                                | shacl_graph_uri        |
+| Generate validation graph                      | generate_graph         |
+| Validation graph URI                           | validation_graph_uri   |
+| Output entities                                | output_entities        |
+| Clear validation graph                         | clear_validation_graph |
+| Resolve owl:imports                            | owl_imports            |
+| Blank node skolemization                       | skolemize              |
+| Add labels                                     | add_labels             |
+| Add labels from data and SHACL graphs          | include_graphs_labels  |
+| Add shui:conforms flag to focus node resources | add_shui_conforms      | 
+| Meta-SHACL                                     | meta_shacl             |
+| Ontology graph URI                             | ontology_graph_uri     |
+| Inference                                      | inference              |
+| Advanced                                       | advanced               |
```

### Comparing `cmem_plugin_pyshacl-4.1.3rc4/cmem_plugin_pyshacl/plugin_pyshacl.py` & `cmem_plugin_pyshacl-4.2.0rc2/cmem_plugin_pyshacl/plugin_pyshacl.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             description="If enabled, the validation graph is posted to the CMEM "
                         "instance with the graph URI specified with the `Validation "
                         "graph URI` option.",
             default_value=False
         ),
         PluginParameter(
             param_type=BoolParameterType(),
-            name="output_values",
+            name="output_entities",
             label="Output entities",
             description="If enabled, the plugin outputs the validation results as "
                         "entities and can be connected to, for instance, a CSV "
                         "dataset to produce a results table.",
             default_value=False
         ),
         PluginParameter(
@@ -155,33 +155,33 @@
             label="Clear validation graph",
             description="If enabled, the validation graph is cleared before workflow "
                         "execution.",
             default_value=True
         ),
         PluginParameter(
             param_type=BoolParameterType(),
-            name="owl_imports_resolution",
+            name="owl_imports",
             label="Resolve owl:imports",
             description="If enabled, the graph tree defined with owl:imports in the "
                         "data graph is resolved.",
             default_value=True,
             advanced=True
         ),
         PluginParameter(
             param_type=BoolParameterType(),
-            name="skolemize_validation_graph",
+            name="skolemize",
             label="Blank node skolemization",
             description="If enabled, blank nodes in the validation graph are "
                         "skolemized into URIs.",
             default_value=True,
             advanced=True
         ),
         PluginParameter(
             param_type=BoolParameterType(),
-            name="add_labels_to_validation_graph",
+            name="add_labels",
             label="Add labels",
             description="If enabled, `rdfs:label` triples are added to the validation "
                         "graph for instances of `sh:ValidationReport` and "
                         "`sh:ValidationResult`.",
             default_value=True,
             advanced=True
         ),
@@ -194,15 +194,15 @@
                         "shapes in the validation graph. The labels are taken from "
                         "the specified data and SHACL graphs.",
             default_value=False,
             advanced=True
         ),
         PluginParameter(
             param_type=BoolParameterType(),
-            name="add_shui_conforms_to_validation_graph",
+            name="add_shui_conforms",
             label="Add shui:conforms flag to focus node resources.",
             description="If enabled, `shui:conforms false` triples are added to the "
                         "focus nodes in the validation graph.",
             default_value=False,
             advanced=True
         ),
         PluginParameter(
@@ -265,38 +265,37 @@
     def __init__(
         self,
         data_graph_uri,
         shacl_graph_uri,
         ontology_graph_uri,
         generate_graph,
         validation_graph_uri,
-        output_values,
+        output_entities,
         clear_validation_graph,
-        owl_imports_resolution,
-        skolemize_validation_graph,
-        add_labels_to_validation_graph,
+        owl_imports,
+        skolemize,
+        add_labels,
         include_graphs_labels,
-        add_shui_conforms_to_validation_graph,
+        add_shui_conforms,
         meta_shacl,
         inference,
         advanced
     ) -> None:
         self.data_graph_uri = data_graph_uri
         self.shacl_graph_uri = shacl_graph_uri
         self.ontology_graph_uri = ontology_graph_uri
         self.validation_graph_uri = validation_graph_uri
         self.generate_graph = generate_graph
-        self.output_values = output_values
-        self.owl_imports_resolution = owl_imports_resolution
+        self.output_entities = output_entities
+        self.owl_imports = owl_imports
         self.clear_validation_graph = clear_validation_graph
-        self.skolemize_validation_graph = skolemize_validation_graph
-        self.add_labels_to_validation_graph = add_labels_to_validation_graph
+        self.skolemize = skolemize
+        self.add_labels = add_labels
         self.include_graphs_labels = include_graphs_labels
-        self.add_shui_conforms_to_validation_graph =  \
-            add_shui_conforms_to_validation_graph
+        self.add_shui_conforms = add_shui_conforms
         self.meta_shacl = meta_shacl
         self.inference = inference
         self.advanced = advanced
 
         discover_plugins_in_module("cmem_plugin_pyshacl")
         this_plugin = Plugin.plugins[0]
 
@@ -327,15 +326,15 @@
         validation_graph.add((
             validation_report_uri,
             PROV.generatedAtTime,
             Literal(utctime, datatype=XSD.dateTime)
         ))
         return validation_graph
 
-    def add_labels(
+    def add_labels_val(
             self,
             validation_graph,
             data_graph,
             shacl_graph,
             validation_result_uris):
         """
         add labels
@@ -369,15 +368,15 @@
             label = f"SHACL: {result_path}: {message}"
             validation_graph.add((validation_result_uri, RDFS.label, Literal(label)))
             if self.include_graphs_labels:
                 focus_node = validation_graph.value(
                     subject=validation_result_uri,
                     predicate=SH.focusNode
                 )
-                if self.add_shui_conforms_to_validation_graph:
+                if self.add_shui_conforms:
                     focus_nodes.append(focus_node)
                 label = get_label(data_graph, focus_node)
                 if label:
                     validation_graph.add((focus_node, RDFS.label, label))
                 value = validation_graph.value(
                     subject=validation_result_uri,
                     predicate=SH.value
@@ -392,15 +391,20 @@
                     predicate=SH.sourceShape
                 )
                 label = get_label(shacl_graph, source_shape)
                 if label:
                     validation_graph.add((source_shape, RDFS.label, label))
         return validation_graph, focus_nodes
 
-    def add_shui_conforms(self, validation_graph, validation_result_uris, focus_nodes):
+    def add_shui_conforms_val(
+            self,
+            validation_graph,
+            validation_result_uris,
+            focus_nodes
+    ):
         """
         add shui conforms flag
         """
         self.log.info("Adding shui:conforms flags to validation graph")
         itr = focus_nodes if focus_nodes else validation_result_uris
         for i in itr:
             subj = i if focus_nodes else validation_graph.value(
@@ -527,15 +531,15 @@
     def get_graph(self, uri):
         """
         get graph from cmem
         """
         graph = Graph()
         graph.parse(data=get(
                 uri,
-                owl_imports_resolution=self.owl_imports_resolution).text,
+                owl_imports_resolution=self.owl_imports).text,
                 format="turtle")
         return graph
 
     def process_inputs(self, inputs):
         """
         process input parameters
         """
@@ -549,15 +553,15 @@
 
     # pylint: disable-msg=too-many-branches
     def check_parameters(self):
         """
         validate plugin parameters
         """
         self.log.info("Validating parameters...")
-        if not self.output_values and not self.generate_graph:
+        if not self.output_entities and not self.generate_graph:
             raise ValueError("Generate validation graph or Output values parameter "
                              "needs to be set to true")
         if not validator_url(self.data_graph_uri):
             raise ValueError("Data graph URI parameter is invalid")
         if not validator_url(self.shacl_graph_uri):
             raise ValueError("SHACL graph URI parameter is invalid")
         graphs_dict = {graph["iri"]: graph["assignedClasses"]
@@ -596,15 +600,15 @@
                     raise ValueError(f"Invalid truth value for parameter {param}") \
                         from err
         if self.generate_graph:
             if not validator_url(self.validation_graph_uri):
                 raise ValueError("Validation graph URI parameter is invalid")
             if self.validation_graph_uri in graphs_dict:
                 self.log.warning(f"Graph <{self.validation_graph_uri}> already exists")
-        if not self.add_labels_to_validation_graph:
+        if not self.add_labels:
             self.include_graphs_labels = False
 
         if self.inference not in ("none", "rdfs", "owlrl", "both"):
             raise ValueError("Invalid value for inference parameter")
 
         self.log.info("Parameters OK:")
         for param in self.graph_parameters + self.bool_parameters:
@@ -646,46 +650,46 @@
             meta_shacl=self.meta_shacl,
             inference=self.inference,
             advanced=self.advanced,
             inplace=True
         )
         self.log.info(f"Finished SHACL validation in {e_t(start)} seconds")
         utctime = str(datetime.fromtimestamp(int(time()))).replace(" ", "T") + "Z"
-        if self.output_values:
+        if self.output_entities:
             entities = self.make_entities(
                 validation_graph,
                 data_graph,
                 shacl_graph,
                 utctime
             )
         if self.generate_graph:
-            if self.skolemize_validation_graph:
+            if self.skolemize:
                 self.log.info("Skolemizing validation graph")
                 validation_graph = validation_graph.skolemize(
                     basepath=self.validation_graph_uri
                 )
-            if self.add_labels_to_validation_graph or \
-                    self.add_shui_conforms_to_validation_graph:
+            if self.add_labels or \
+                    self.add_shui_conforms:
                 validation_graph_uris = validation_graph.subjects(
                     RDF.type,
                     SH.ValidationResult
                 )
                 focus_nodes = None
-                if self.add_labels_to_validation_graph:
-                    validation_graph, focus_nodes = self.add_labels(
+                if self.add_labels:
+                    validation_graph, focus_nodes = self.add_labels_val(
                         validation_graph,
                         data_graph,
                         shacl_graph,
                         validation_graph_uris
                     )
-                if self.add_shui_conforms_to_validation_graph:
-                    validation_graph = self.add_shui_conforms(
+                if self.add_shui_conforms:
+                    validation_graph = self.add_shui_conforms_val(
                         validation_graph,
                         validation_graph_uris,
                         focus_nodes
                     )
             validation_graph = self.add_prov(validation_graph, utctime)
             self.post_graph(validation_graph)
-        if self.output_values:
+        if self.output_entities:
             self.log.info("Outputting entities")
             return entities
         return None
```

### Comparing `cmem_plugin_pyshacl-4.1.3rc4/pyproject.toml` & `cmem_plugin_pyshacl-4.2.0rc2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-pyshacl"
-version = "4.1.3rc4"
+version = "4.2.0rc2"
 license = "Apache-2.0"
 description = "Validate your Knowledge Graphs based on tests generated from SHACL shapes."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules"
```

### Comparing `cmem_plugin_pyshacl-4.1.3rc4/PKG-INFO` & `cmem_plugin_pyshacl-4.2.0rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-pyshacl
-Version: 4.1.3rc4
+Version: 4.2.0rc2
 Summary: Validate your Knowledge Graphs based on tests generated from SHACL shapes.
 Home-page: https://github.com/eccenca/cmem-plugin-pyshacl
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,SHACL
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.9,<4.0
@@ -110,25 +110,24 @@
 Enable SHACL Advanced Features. Default value: *false*.
 
 
 ## Parameter Input
 
 In order to set options via the input the following parameter names can be used:
 
-| Option                                         | Name                                  |
-|------------------------------------------------|---------------------------------------|
-| Data graph URI                                 | data_graph_uri                        |
-| SHACL graph URI                                | shacl_graph_uri                       |
-| Generate validation graph                      | generate_graph                        |
-| Validation graph URI                           | validation_graph_uri                  |
-| Output entities                                | output_values                         |
-| Clear validation graph                         | clear_validation_graph                |
-| Resolve owl:imports                            | owl_imports_resolution                |
-| Blank node skolemization                       | skolemize_validation_graph            |
-| Add labels                                     | add_labels_to_validation_graph        |
-| Add labels from data and SHACL graphs          | include_graphs_labels                 |
-| Add shui:conforms flag to focus node resources | add_shui_conforms_to_validation_graph | 
-| Meta-SHACL                                     | meta_shacl                            |
-| Ontology graph URI                             | ontology_graph_uri                    |
-| Inference                                      | inference                             |
-| Advanced                                       | advanced                              |
-
+| Option                                         | Name                   |
+|------------------------------------------------|------------------------|
+| Data graph URI                                 | data_graph_uri         |
+| SHACL graph URI                                | shacl_graph_uri        |
+| Generate validation graph                      | generate_graph         |
+| Validation graph URI                           | validation_graph_uri   |
+| Output entities                                | output_entities        |
+| Clear validation graph                         | clear_validation_graph |
+| Resolve owl:imports                            | owl_imports            |
+| Blank node skolemization                       | skolemize              |
+| Add labels                                     | add_labels             |
+| Add labels from data and SHACL graphs          | include_graphs_labels  |
+| Add shui:conforms flag to focus node resources | add_shui_conforms      | 
+| Meta-SHACL                                     | meta_shacl             |
+| Ontology graph URI                             | ontology_graph_uri     |
+| Inference                                      | inference              |
+| Advanced                                       | advanced               |
```

