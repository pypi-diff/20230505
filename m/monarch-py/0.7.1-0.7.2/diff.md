# Comparing `tmp/monarch_py-0.7.1.tar.gz` & `tmp/monarch_py-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarch_py-0.7.1.tar", max compression
+gzip compressed data, was "monarch_py-0.7.2.tar", max compression
```

## Comparing `monarch_py-0.7.1.tar` & `monarch_py-0.7.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      955 2023-05-04 00:46:19.213279 monarch_py-0.7.1/pyproject.toml
--rw-r--r--   0        0        0       77 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/__init__.py
--rw-r--r--   0        0        0     1587 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/association_type_mappings.yaml
--rw-r--r--   0        0        0     6581 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/cli.py
--rw-r--r--   0        0        0        0 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/datamodels/__init__.py
--rw-r--r--   0        0        0     8251 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/datamodels/model.py
--rw-r--r--   0        0        0     7319 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/datamodels/model.yaml
--rw-r--r--   0        0        0     3300 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/datamodels/solr.py
--rw-r--r--   0        0        0        0 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/implementations/solr/__init__.py
--rw-r--r--   0        0        0    17565 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/implementations/solr/solr_implementation.py
--rw-r--r--   0        0        0        0 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/implementations/sql/__init__.py
--rw-r--r--   0        0        0     8909 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/implementations/sql/sql_implementation.py
--rw-r--r--   0        0        0        0 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/interfaces/__init__.py
--rw-r--r--   0        0        0     2343 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/interfaces/association_interface.py
--rw-r--r--   0        0        0      985 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/interfaces/entity_interface.py
--rw-r--r--   0        0        0      890 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/interfaces/query_interface.py
--rw-r--r--   0        0        0     3737 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/interfaces/search_interface.py
--rw-r--r--   0        0        0        0 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/service/__init__.py
--rw-r--r--   0        0        0     2052 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/service/solr_service.py
--rw-r--r--   0        0        0     8133 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/solr_cli.py
--rw-r--r--   0        0        0     3330 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/sql_cli.py
--rw-r--r--   0        0        0        0 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/utils/__init__.py
--rw-r--r--   0        0        0     4052 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/utils/association_type_utils.py
--rw-r--r--   0        0        0     3964 2023-05-04 00:46:19.217279 monarch_py-0.7.1/src/monarch_py/utils/solr_cli_utils.py
--rw-r--r--   0        0        0     4937 2023-05-04 00:46:19.217279 monarch_py-0.7.1/src/monarch_py/utils/utils.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      955 2023-05-05 20:41:42.065764 monarch_py-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-05-05 20:41:42.065764 monarch_py-0.7.2/src/monarch_py/__init__.py
+-rw-r--r--   0        0        0     1587 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/association_type_mappings.yaml
+-rw-r--r--   0        0        0     6581 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/cli.py
+-rw-r--r--   0        0        0        0 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/datamodels/__init__.py
+-rw-r--r--   0        0        0     8802 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/datamodels/model.py
+-rw-r--r--   0        0        0     7857 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/datamodels/model.yaml
+-rw-r--r--   0        0        0     3300 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/datamodels/solr.py
+-rw-r--r--   0        0        0        0 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/implementations/solr/__init__.py
+-rw-r--r--   0        0        0    17565 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/implementations/solr/solr_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/implementations/sql/__init__.py
+-rw-r--r--   0        0        0     8909 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/implementations/sql/sql_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/interfaces/__init__.py
+-rw-r--r--   0        0        0     2343 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/interfaces/association_interface.py
+-rw-r--r--   0        0        0      985 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/interfaces/entity_interface.py
+-rw-r--r--   0        0        0      890 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/interfaces/query_interface.py
+-rw-r--r--   0        0        0     3737 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/interfaces/search_interface.py
+-rw-r--r--   0        0        0        0 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/service/__init__.py
+-rw-r--r--   0        0        0     2052 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/service/solr_service.py
+-rw-r--r--   0        0        0     8133 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/solr_cli.py
+-rw-r--r--   0        0        0     3330 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/sql_cli.py
+-rw-r--r--   0        0        0        0 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/utils/__init__.py
+-rw-r--r--   0        0        0     4052 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/utils/association_type_utils.py
+-rw-r--r--   0        0        0     3985 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/utils/solr_cli_utils.py
+-rw-r--r--   0        0        0     4937 2023-05-05 20:41:42.069764 monarch_py-0.7.2/src/monarch_py/utils/utils.py
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.7.2/PKG-INFO
```

### Comparing `monarch_py-0.7.1/pyproject.toml` & `monarch_py-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monarch-py"
-version = "0.7.1"
+version = "0.7.2"
 description = "Monarch Initiative data access library"
 authors = [
     "Kevin Schaper <kevin@tislab.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "The Monarch Initiative <info@monarchinitiative.org>"
 ]
 packages = [
```

### Comparing `monarch_py-0.7.1/src/monarch_py/association_type_mappings.yaml` & `monarch_py-0.7.2/src/monarch_py/association_type_mappings.yaml`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.1/src/monarch_py/cli.py` & `monarch_py-0.7.2/src/monarch_py/cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.1/src/monarch_py/datamodels/model.py` & `monarch_py-0.7.2/src/monarch_py/datamodels/model.py`

 * *Files 25% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     causal_gene = "causal_gene"
     
     
 
 class Association(ConfiguredBaseModel):
     
     aggregator_knowledge_source: Optional[List[str]] = Field(default_factory=list)
-    id: Optional[str] = Field(None)
+    id: str = Field(None)
     subject: Optional[str] = Field(None)
     original_subject: Optional[str] = Field(None)
     subject_namespace: Optional[str] = Field(None)
     subject_category: Optional[List[str]] = Field(default_factory=list)
     subject_closure: Optional[List[str]] = Field(default_factory=list)
     subject_label: Optional[str] = Field(None)
     subject_closure_label: Optional[List[str]] = Field(default_factory=list)
@@ -69,15 +69,15 @@
     pathway: Optional[str] = Field(None)
     relation: Optional[str] = Field(None)
     
 
 
 class Entity(ConfiguredBaseModel):
     
-    id: Optional[str] = Field(None)
+    id: str = Field(None)
     category: Optional[List[str]] = Field(default_factory=list)
     name: Optional[str] = Field(None)
     description: Optional[str] = Field(None)
     xref: Optional[List[str]] = Field(default_factory=list)
     provided_by: Optional[str] = Field(None)
     in_taxon: Optional[str] = Field(None)
     source: Optional[str] = Field(None)
@@ -85,92 +85,92 @@
     type: Optional[str] = Field(None)
     synonym: Optional[List[str]] = Field(default_factory=list)
     
 
 
 class HistoPheno(ConfiguredBaseModel):
     
-    id: Optional[str] = Field(None)
-    items: Optional[List[HistoBin]] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
+    id: str = Field(None)
+    items: List[HistoBin] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
     
 
 
 class Results(ConfiguredBaseModel):
     
-    limit: Optional[int] = Field(None)
-    offset: Optional[int] = Field(None)
-    total: Optional[int] = Field(None)
+    limit: int = Field(None, description="""number of items to return in a response""")
+    offset: int = Field(None, description="""offset into the total number of items""")
+    total: int = Field(None, description="""total number of items matching a query""")
     
 
 
 class AssociationResults(Results):
     
-    items: Optional[List[Association]] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
-    limit: Optional[int] = Field(None)
-    offset: Optional[int] = Field(None)
-    total: Optional[int] = Field(None)
+    items: List[Association] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
+    limit: int = Field(None, description="""number of items to return in a response""")
+    offset: int = Field(None, description="""offset into the total number of items""")
+    total: int = Field(None, description="""total number of items matching a query""")
     
 
 
 class EntityResults(Results):
     
-    items: Optional[List[Entity]] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
-    limit: Optional[int] = Field(None)
-    offset: Optional[int] = Field(None)
-    total: Optional[int] = Field(None)
+    items: List[Entity] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
+    limit: int = Field(None, description="""number of items to return in a response""")
+    offset: int = Field(None, description="""offset into the total number of items""")
+    total: int = Field(None, description="""total number of items matching a query""")
     
 
 
 class SearchResult(Entity):
     
     highlight: Optional[str] = Field(None, description="""matching text snippet containing html tags""")
     score: Optional[float] = Field(None)
-    id: Optional[str] = Field(None)
-    category: Optional[List[str]] = Field(default_factory=list)
-    name: Optional[str] = Field(None)
+    id: str = Field(None)
+    category: List[str] = Field(default_factory=list)
+    name: str = Field(None)
     description: Optional[str] = Field(None)
     xref: Optional[List[str]] = Field(default_factory=list)
     provided_by: Optional[str] = Field(None)
     in_taxon: Optional[str] = Field(None)
     source: Optional[str] = Field(None)
     symbol: Optional[str] = Field(None)
     type: Optional[str] = Field(None)
     synonym: Optional[List[str]] = Field(default_factory=list)
     
 
 
 class SearchResults(Results):
     
-    items: Optional[List[SearchResult]] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
-    facet_fields: Optional[Dict[str, FacetField]] = Field(default_factory=dict)
-    facet_queries: Optional[Dict[str, FacetValue]] = Field(default_factory=dict)
-    limit: Optional[int] = Field(None)
-    offset: Optional[int] = Field(None)
-    total: Optional[int] = Field(None)
+    items: List[SearchResult] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
+    facet_fields: Optional[Dict[str, FacetField]] = Field(default_factory=dict, description="""Collection of facet field responses with the field values and counts""")
+    facet_queries: Optional[Dict[str, FacetValue]] = Field(default_factory=dict, description="""Collection of facet query responses with the query string values and counts""")
+    limit: int = Field(None, description="""number of items to return in a response""")
+    offset: int = Field(None, description="""offset into the total number of items""")
+    total: int = Field(None, description="""total number of items matching a query""")
     
 
 
 class FacetValue(ConfiguredBaseModel):
     
-    label: Optional[str] = Field(None)
-    count: Optional[int] = Field(None, description="""number of items a this facet value""")
+    label: str = Field(None)
+    count: Optional[int] = Field(None, description="""count of documents""")
     
 
 
 class HistoBin(FacetValue):
     
-    id: Optional[str] = Field(None)
-    label: Optional[str] = Field(None)
-    count: Optional[int] = Field(None, description="""number of items a this facet value""")
+    id: str = Field(None)
+    label: str = Field(None)
+    count: Optional[int] = Field(None, description="""count of documents""")
     
 
 
 class FacetField(ConfiguredBaseModel):
     
-    label: Optional[str] = Field(None)
+    label: str = Field(None)
     facet_values: Optional[Dict[str, FacetValue]] = Field(default_factory=dict)
     
 
 
 class AssociationTypeMapping(ConfiguredBaseModel):
     """
     A data class to hold the necessary information to produce association type counts for given  entities with appropriate directional labels
@@ -182,24 +182,24 @@
     predicate: Optional[List[str]] = Field(default_factory=list, description="""The biolink predicate to use in queries for this association type, assuming OR semantics""")
     
 
 
 class AssociationCount(FacetValue):
     
     association_type: Optional[AssociationTypeEnum] = Field(None)
-    label: Optional[str] = Field(None)
-    count: Optional[int] = Field(None, description="""number of items a this facet value""")
+    label: str = Field(None)
+    count: Optional[int] = Field(None, description="""count of documents""")
     
 
 
 class AssociationCountList(ConfiguredBaseModel):
     """
     Container class for a list of association counts
     """
-    items: Optional[List[AssociationCount]] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
+    items: List[AssociationCount] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
     
 
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
 Association.update_forward_refs()
```

### Comparing `monarch_py-0.7.1/src/monarch_py/datamodels/model.yaml` & `monarch_py-0.7.2/src/monarch_py/datamodels/model.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 id: https://w3id.org/monarch/monarch-py
 name: monarch-py
+description: Data datamodels for the Monarch Initiative data access library
 prefixes:
   linkml: https://w3id.org/linkml/
   biolink: https://w3id.org/biolink/
-description: Data datamodels for the Monarch Initiative data access library
 imports:
-- linkml:types
+  - linkml:types
 default_range: string
 
 enums:
   AssociationTypeEnum:
     description: >-
       A grouping label for association types, which are not necessarily 1:1 with
       biolink categories or predicates
@@ -136,14 +136,20 @@
       - offset
       - total
   SearchResult:
     is_a: Entity
     slots:
       - highlight
       - score
+    slot_usage:
+      category:
+        required: true
+      name:
+        required: true
+
   SearchResults:
     is_a: Results
     slots:
       - items
       - facet_fields
       - facet_queries
     slot_usage:
@@ -200,23 +206,25 @@
   aggregator_knowledge_source:
     multivalued: true
   association_type:
     range: AssociationTypeEnum
   category:
     multivalued: true
   count:
-    description: number of items a this facet value
+    description: count of documents
     range: integer
   description:
     range: string
   facet_fields:
+    description: Collection of facet field responses with the field values and counts
     inlined: true
     multivalued: true
     range: FacetField
   facet_queries:
+    description: Collection of facet query responses with the query string values and counts
     inlined: true
     multivalued: true
     range: FacetValue
   facet_values:
     inlined: true
     multivalued: true
     range: FacetValue
@@ -226,28 +234,33 @@
     range: string
   highlight:
     description: matching text snippet containing html tags
     range: string
   id:
     identifier: true
     range: string
+    required: true
   in_taxon:
     range: string
   items:
     description: A collection of items, with the type to be overriden by slot_usage
     range: string
     inlined: true
     inlined_as_list: true
     multivalued: true
+    required: true
   knowledge_source:
     multivalued: true
   label:
     range: string
+    required: true
   limit:
+    description: number of items to return in a response
     range: integer
+    required: true
   name:
     range: string
   negated:
     range: boolean
   object:
     range: string
   object_category:
@@ -257,15 +270,17 @@
   object_closure_label:
     multivalued: true
   object_label:
     range: string
   object_namespace:
     range: string
   offset:
+    description: offset into the total number of items
     range: integer
+    required: true
   onset_qualifier:
     range: string
   original_object:
     range: string
   original_subject:
     range: string
   pathway:
@@ -304,13 +319,15 @@
   subject_namespace:
     range: string
   symbol:
     range: string
   synonym:
     multivalued: true
   total:
+    description: total number of items matching a query
     range: integer
+    required: true
   type:
     range: string
   xref:
     multivalued: true
     range: string
```

### Comparing `monarch_py-0.7.1/src/monarch_py/datamodels/solr.py` & `monarch_py-0.7.2/src/monarch_py/datamodels/solr.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.1/src/monarch_py/implementations/solr/solr_implementation.py` & `monarch_py-0.7.2/src/monarch_py/implementations/solr/solr_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.1/src/monarch_py/implementations/sql/sql_implementation.py` & `monarch_py-0.7.2/src/monarch_py/implementations/sql/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.1/src/monarch_py/interfaces/association_interface.py` & `monarch_py-0.7.2/src/monarch_py/interfaces/association_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.1/src/monarch_py/interfaces/entity_interface.py` & `monarch_py-0.7.2/src/monarch_py/interfaces/entity_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.1/src/monarch_py/interfaces/query_interface.py` & `monarch_py-0.7.2/src/monarch_py/interfaces/query_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.1/src/monarch_py/interfaces/search_interface.py` & `monarch_py-0.7.2/src/monarch_py/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.1/src/monarch_py/service/solr_service.py` & `monarch_py-0.7.2/src/monarch_py/service/solr_service.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.1/src/monarch_py/solr_cli.py` & `monarch_py-0.7.2/src/monarch_py/solr_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.1/src/monarch_py/sql_cli.py` & `monarch_py-0.7.2/src/monarch_py/sql_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.1/src/monarch_py/utils/association_type_utils.py` & `monarch_py-0.7.2/src/monarch_py/utils/association_type_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.1/src/monarch_py/utils/solr_cli_utils.py` & `monarch_py-0.7.2/src/monarch_py/utils/solr_cli_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 
 def check_solr_permissions(update: bool = False) -> None:
     """Checks that the solr data directory has the correct permissions."""
     data_path = monarchstow.base / "solr" / "data"
     # When untarred solr won't necessarily use the same file names for index segments etc
     # so the untarred path needs to be removed before updating
     if update:
-        shutil.rmtree(data_path)
+        shutil.rmtree(data_path, ignore_errors=True)
     monarchstow.ensure_untar(url=SOLR_DATA_URL, force=update)
     if sys.platform in ["linux", "linux2", "darwin"]:
         stat_info = os.stat(data_path)
         if stat_info.st_gid != 8983:
             console.print(
                 f"""
 Solr container requires write access to {monarchstow.base}.
 Please run the following command to set permissions:
-    [grey84 on black]sudo chgrp -R 8983 {monarchstow.base} && \[/]
+    [grey84 on black]sudo chgrp -R 8983 {monarchstow.base} && \ [/]
     [grey84 on black]sudo chmod -R g+w {monarchstow.base}[/]
             """
             )
             sys.exit(1)
 
 
 def check_for_solr(dc: docker.DockerClient, quiet: bool = False):
```

### Comparing `monarch_py-0.7.1/src/monarch_py/utils/utils.py` & `monarch_py-0.7.2/src/monarch_py/utils/utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.1/PKG-INFO` & `monarch_py-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monarch-py
-Version: 0.7.1
+Version: 0.7.2
 Summary: Monarch Initiative data access library
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

