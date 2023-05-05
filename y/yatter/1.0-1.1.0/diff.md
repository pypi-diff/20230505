# Comparing `tmp/yatter-1.0.tar.gz` & `tmp/yatter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yatter-1.0.tar", last modified: Wed Feb 15 13:01:29 2023, max compression
+gzip compressed data, was "yatter-1.1.0.tar", last modified: Fri May  5 08:52:04 2023, max compression
```

## Comparing `yatter-1.0.tar` & `yatter-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 13:01:29.733587 yatter-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-02-15 13:01:29.733587 yatter-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 13:01:29.733587 yatter-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-02-15 13:01:20.000000 yatter-1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 13:01:29.733587 yatter-1.0/yatter/
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-02-15 13:01:20.000000 yatter-1.0/yatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-02-15 13:01:20.000000 yatter-1.0/yatter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-02-15 13:01:20.000000 yatter-1.0/yatter/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-02-15 13:01:20.000000 yatter-1.0/yatter/function.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-02-15 13:01:20.000000 yatter-1.0/yatter/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-02-15 13:01:20.000000 yatter-1.0/yatter/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-02-15 13:01:20.000000 yatter-1.0/yatter/predicateobject.py
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-02-15 13:01:20.000000 yatter-1.0/yatter/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-02-15 13:01:20.000000 yatter-1.0/yatter/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-02-15 13:01:20.000000 yatter-1.0/yatter/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-02-15 13:01:20.000000 yatter-1.0/yatter/termmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 13:01:29.733587 yatter-1.0/yatter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-02-15 13:01:29.000000 yatter-1.0/yatter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-15 13:01:29.000000 yatter-1.0/yatter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 13:01:29.000000 yatter-1.0/yatter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-15 13:01:29.000000 yatter-1.0/yatter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-15 13:01:29.000000 yatter-1.0/yatter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:04.962134 yatter-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-05 08:52:04.962134 yatter-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:52:04.962134 yatter-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-05 08:51:53.000000 yatter-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:04.958133 yatter-1.1.0/yatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-05 08:51:53.000000 yatter-1.1.0/yatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-05 08:51:53.000000 yatter-1.1.0/yatter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-05-05 08:51:53.000000 yatter-1.1.0/yatter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-05 08:51:53.000000 yatter-1.1.0/yatter/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-05 08:51:53.000000 yatter-1.1.0/yatter/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-05-05 08:51:53.000000 yatter-1.1.0/yatter/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-05-05 08:51:53.000000 yatter-1.1.0/yatter/predicateobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13700 2023-05-05 08:51:53.000000 yatter-1.1.0/yatter/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-05 08:51:53.000000 yatter-1.1.0/yatter/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-05 08:51:53.000000 yatter-1.1.0/yatter/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-05 08:51:53.000000 yatter-1.1.0/yatter/termmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:52:04.962134 yatter-1.1.0/yatter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-05 08:52:04.000000 yatter-1.1.0/yatter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-05 08:52:04.000000 yatter-1.1.0/yatter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:52:04.000000 yatter-1.1.0/yatter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 08:52:04.000000 yatter-1.1.0/yatter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 08:52:04.000000 yatter-1.1.0/yatter.egg-info/top_level.txt
```

### Comparing `yatter-1.0/PKG-INFO` & `yatter-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yatter
-Version: 1.0
+Version: 1.1.0
 Summary: A translator from YARRRML to RML mappings.
 Home-page: https://github.com/oeg-upm/yarrrml-translator
 Author: David Chaves-Fraga
 Author-email: david.chaves@upm.es
 License: Apache 2.0
 Project-URL: Source code, https://github.com/oeg-upm/yarrrml-translator
 Project-URL: Issue tracker, https://github.com/oeg-upm/yarrrml-translator/issues
```

### Comparing `yatter-1.0/setup.py` & `yatter-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `yatter-1.0/yatter/__init__.py` & `yatter-1.1.0/yatter/__init__.py`

 * *Files identical despite different names*

### Comparing `yatter-1.0/yatter/__main__.py` & `yatter-1.1.0/yatter/__main__.py`

 * *Files identical despite different names*

### Comparing `yatter-1.0/yatter/constants.py` & `yatter-1.1.0/yatter/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,16 @@
     'trig':'TriG',
 }
 
 YARRRML_REFERENCE_FORMULATIONS = {
     'csv': 'CSV',
     'json': 'JSONPath',
     'xpath': 'XPath',
-    'jsonpath': 'JSONPath'
+    'jsonpath': 'JSONPath',
+    "shp": "SHP"
 }
 
 YARRRML_DATABASES_DRIVER = {
     'mysql': 'com.mysql.jdbc.Driver',
     'postgresql': 'org.postgresql.Driver',
     'sqlserver': 'com.microsoft.sqlserver.jdbc.SQLServerDriver'
 }
```

### Comparing `yatter-1.0/yatter/function.py` & `yatter-1.1.0/yatter/function.py`

 * *Files identical despite different names*

### Comparing `yatter-1.0/yatter/mapping.py` & `yatter-1.1.0/yatter/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from .import *
+prefixes = {}
 
 
 def add_mapping(mapping, mappings, it):
     map_template = "<" + mapping + "_" + str(it) + "> a "
     if mappings[mapping]:
         if mappings[mapping] == "non_asserted":
             map_template += STAR_NON_ASSERTED_CLASS + ", "
     map_template += R2RML_TRIPLES_MAP + ";\n\n"
     return map_template
 
 
 def add_prefix(data):
+    global prefixes
     template = []
     common_prefixes = []
     if YARRRML_PREFIXES in data:
         prefixes = data.get(YARRRML_PREFIXES)
         for prefix in prefixes:
             prefix_uri = data.get(YARRRML_PREFIXES).get(prefix)
             check_common_prefixes(prefix_uri, common_prefixes)
@@ -117,9 +119,9 @@
     return mappings, mapping_format
 
 
 
 def merge_mapping_section_by_key(key,yarrrml_list):
     output = {key:{}}
     for yarrrml_mapping in yarrrml_list:
-        output[key] =  output[key] | yarrrml_mapping
+        output[key] = output[key] | yarrrml_mapping
     return output
```

### Comparing `yatter-1.0/yatter/predicateobject.py` & `yatter-1.1.0/yatter/predicateobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import rdflib
 from .constants import *
 from .graph import add_inverse_graph
 from .source import get_initial_sources, add_source, add_table
 from .subject import add_subject
 from .termmap import generate_rml_termmap, check_type
+from .mapping import prefixes
 from ruamel.yaml import YAML
 
-
 def get_object_access(predicate_object_map):
     if YARRRML_OBJECT in predicate_object_map:
         object_access = YARRRML_OBJECT
     elif YARRRML_OBJECT_SHORTCUT in predicate_object_map:
         object_access = YARRRML_OBJECT_SHORTCUT
     elif YARRRML_OBJECTS in predicate_object_map:
         object_access = YARRRML_OBJECTS
@@ -139,15 +139,15 @@
     predicate_list = get_predicate_list(predicate_object, predicate_access)
     object_list = get_object_list(predicate_object, object_access)
     graph_list = get_graph_list(predicate_object, graph_access)
 
     for pm in predicate_list:
         pm_value = pm
         execution = False
-        if YARRRML_VALUE in pm:
+        if YARRRML_VALUE in pm and type(pm) is dict:
             pm_value = pm[YARRRML_VALUE]
         elif YARRRML_FUNCTION in pm:
             pm_value = pm[YARRRML_FUNCTION]
             execution = True
         template += generate_rml_termmap(R2RML_PREDICATE, R2RML_PREDICATE_CLASS, pm_value,"\t\t\t")
         if execution:
             template = template.replace(R2RML_CONSTANT + " " + pm_value, RML_EXECUTION + " <" + pm_value + ">")
@@ -161,16 +161,21 @@
             if YARRRML_IRI in om[0]:
                 object_value = om[0].split(YARRRML_IRI)[0]
                 iri = True
             if mapping_format == STAR_URI:
                 template += generate_rml_termmap(STAR_OBJECT, R2RML_OBJECT_CLASS,
                                                  object_value, "\t\t\t", mapping_format)
             else:
-                template += generate_rml_termmap(R2RML_OBJECT, R2RML_OBJECT_CLASS,
+                object_map = generate_rml_termmap(R2RML_OBJECT, R2RML_OBJECT_CLASS,
                                              object_value, "\t\t\t", mapping_format)
+
+                if object_value not in prefixes and ":" not in object_value and R2RML_CONSTANT in object_map:
+                    object_map = object_map.replace(object_value, f"\"{object_value}\"")
+
+                template += object_map
             if len(om) == 2:
                 types = check_type(om[1])
                 if types != "error":
                     if types == YARRRML_LANGUAGE:
                         if "$(" in om[1]:
                             template = template[0:len(template) - 5] + generate_rml_termmap(RML_LANGUAGE_MAP, RML_LANGUAGE_MAP_CLASS,
                                              om[1].replace("~lang",""), "\t\t\t\t", mapping_format) + "\t\t];\n"
@@ -197,15 +202,15 @@
                 if YARRRML_CONDITION in om:
                     template += ref_mapping(data, mapping, om, YARRRML_NON_ASSERTED, STAR_QUOTED, mapping_format)
                 else:
                     template += generate_rml_termmap(STAR_OBJECT, STAR_CLASS,om, "\t\t\t", mapping_format)
             else:
                template += ref_mapping(data, mapping, om, YARRRML_QUOTED, STAR_QUOTED, mapping_format)
         else:
-            if YARRRML_VALUE in om:
+            if YARRRML_VALUE in om and type(om) is dict:
                 object_value = om.get(YARRRML_VALUE)
             else:
                 object_value = om
                 if YARRRML_IRI in om:
                     object_value = om.split(YARRRML_IRI)[0]
                     iri = True
             if mapping_format == STAR_URI:
@@ -307,15 +312,17 @@
     return template
 
 
 def add_inverse_pom(mapping_id, rdf_mapping, classes, prefixes):
     yarrrml_poms = []
     yaml = YAML()
     for c in classes:
-        yarrrml_poms.append(['rdf:type', c.toPython()])
+        yarrrml_pom = yaml.seq(['rdf:type', c.toPython()])
+        yarrrml_pom.fa.set_flow_style()
+        yarrrml_poms.append(yarrrml_pom)
 
     query = f'SELECT ?predicate ?predicateValue ?object ?objectValue ?termtype ?datatype ?datatypeMapValue ' \
             f'?language ?languageMapValue ?parentTriplesMap ?child ?parent ?graphValue' \
             f' WHERE {{ ' \
             f'<{mapping_id}> {R2RML_PREDICATE_OBJECT_MAP} ?predicateObjectMap . ' \
             f'?predicateObjectMap {R2RML_PREDICATE}|{R2RML_SHORTCUT_PREDICATE} ?predicate .' \
             f'OPTIONAL {{ ?predicate {R2RML_CONSTANT} ?predicateValue . }}' \
```

### Comparing `yatter-1.0/yatter/source.py` & `yatter-1.1.0/yatter/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import re
 import rdflib
 from .constants import *
 from ruamel.yaml import YAML
 
 def get_initial_sources(data):
     list_initial_sources = []
@@ -81,15 +82,15 @@
     return final_list
 
 
 def add_source_simplified(mapping, source):
     source_rdf = ""
     file_path = re.sub("~.*", "", source[0])
     reference_formulation = source[0].split('~')[1]
-    source_extension = file_path.split('.')[1]
+    source_extension = os.path.splitext(file_path)[1].replace(".","")
     ref_formulation_rml = YARRRML_REFERENCE_FORMULATIONS[reference_formulation]
 
     if switch_in_reference_formulation(reference_formulation) != source_extension:
         raise Exception(
             "ERROR: mismatch extension and referenceFormulation in source " + source + " in mapping " + mapping)
     else:
         if len(source) == 1:  # do not have iterator
@@ -166,26 +167,26 @@
         raise Exception("ERROR: no access to the source in mapping " + mapping)
 
     return source_rdf
 
 
 def switch_in_reference_formulation(value):
     value = value.lower()
-    if value == "csv":
-        switcher = value
-    elif "json" in value:
+    if "json" in value:
         if "path" in value:
             switcher = "json"
         else:
             switcher = "jsonpath"
     elif "x" in value:
         if "path" in value:
             switcher = "xml"
         else:
             switcher = "xpath"
+    else:
+        switcher = value
     return switcher
 
 
 def generate_database_connections(data, list_initial_sources):
     database = []
     sources_ids = set()
     for mapping in data.get(YARRRML_MAPPINGS):
```

### Comparing `yatter-1.0/yatter/subject.py` & `yatter-1.1.0/yatter/subject.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 subject_termmap=subject_termmap.replace(R2RML_REFOBJECT_CLASS,STAR_CLASS).replace(STAR_OBJECT,STAR_SUBJECT).replace("\t\t\t\t","\t\t\t\t\t").replace("\t\t","\t")
             else:
                 subject_termmap = generate_rml_termmap(STAR_SUBJECT, STAR_CLASS, individual_subject, "\t\t")
         elif mapping_format == STAR_URI:
             subject_termmap = generate_rml_termmap(STAR_SUBJECT, R2RML_SUBJECT_CLASS, individual_subject, "\t\t")
         else:
             subject_value = individual_subject
-            if YARRRML_VALUE in individual_subject:
+            if YARRRML_VALUE in individual_subject and type(individual_subject) is dict:
                 subject_value = individual_subject.get(YARRRML_VALUE)
             elif YARRRML_FUNCTION in individual_subject:
                 subject_value = individual_subject.get(YARRRML_FUNCTION)
 
             subject_termmap = generate_rml_termmap(R2RML_SUBJECT, R2RML_SUBJECT_CLASS, subject_value, "\t\t", mapping_format)
 
             if YARRRML_FUNCTION in individual_subject:
```

### Comparing `yatter-1.0/yatter/target.py` & `yatter-1.1.0/yatter/target.py`

 * *Files identical despite different names*

### Comparing `yatter-1.0/yatter/termmap.py` & `yatter-1.1.0/yatter/termmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 ## Generates a TermMap (subject, predicate, object) based on the property, class and the text
 def generate_rml_termmap(rml_property, rml_class, text, identation, mapping_format=RML_URI):
     template = identation[0:-1] + rml_property + " [\n"+identation+"a " + rml_class + ";\n" + identation
     term_map = get_termmap_type(text, mapping_format)
     if term_map == R2RML_TEMPLATE:
         text = generate_rml_template(text)
-        text = text.replace('"',r'\"')
+        text = text.replace('"', r'\"')
     elif term_map == RML_REFERENCE or term_map == R2RML_COLUMN:
         text = text.replace("$(", "").replace(")", "")
         text = text.replace('"', r'\"')
     elif term_map == R2RML_CONSTANT and text == "a":
         text = RDF_TYPE
 
     if term_map == STAR_QUOTED:
```

### Comparing `yatter-1.0/yatter.egg-info/PKG-INFO` & `yatter-1.1.0/yatter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yatter
-Version: 1.0
+Version: 1.1.0
 Summary: A translator from YARRRML to RML mappings.
 Home-page: https://github.com/oeg-upm/yarrrml-translator
 Author: David Chaves-Fraga
 Author-email: david.chaves@upm.es
 License: Apache 2.0
 Project-URL: Source code, https://github.com/oeg-upm/yarrrml-translator
 Project-URL: Issue tracker, https://github.com/oeg-upm/yarrrml-translator/issues
```

