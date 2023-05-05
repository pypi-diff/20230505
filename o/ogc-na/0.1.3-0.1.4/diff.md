# Comparing `tmp/ogc_na-0.1.3.tar.gz` & `tmp/ogc_na-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ogc_na-0.1.3.tar", last modified: Wed May  3 10:14:54 2023, max compression
+gzip compressed data, was "ogc_na-0.1.4.tar", last modified: Fri May  5 10:29:56 2023, max compression
```

## Comparing `ogc_na-0.1.3.tar` & `ogc_na-0.1.4.tar`

### file list

```diff
@@ -1,52 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.271020 ogc_na-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.267020 ogc_na-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.267020 ogc_na-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-03 10:14:41.000000 ogc_na-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-03 10:14:41.000000 ogc_na-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 10:14:41.000000 ogc_na-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-03 10:14:54.271020 ogc_na-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-03 10:14:41.000000 ogc_na-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.267020 ogc_na-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-03 10:14:41.000000 ogc_na-0.1.3/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-03 10:14:41.000000 ogc_na-0.1.3/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-03 10:14:41.000000 ogc_na-0.1.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-03 10:14:41.000000 ogc_na-0.1.3/docs/tutorials.md
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-03 10:14:41.000000 ogc_na-0.1.3/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.267020 ogc_na-0.1.3/ogc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.271020 ogc_na-0.1.3/ogc/na/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21506 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    30863 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/provenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/update_vocabs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-03 10:14:41.000000 ogc_na-0.1.3/ogc/na/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.271020 ogc_na-0.1.3/ogc_na.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-03 10:14:54.000000 ogc_na-0.1.3/ogc_na.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-03 10:14:54.000000 ogc_na-0.1.3/ogc_na.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:14:54.000000 ogc_na-0.1.3/ogc_na.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-03 10:14:54.000000 ogc_na-0.1.3/ogc_na.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-03 10:14:54.000000 ogc_na-0.1.3/ogc_na.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-03 10:14:41.000000 ogc_na-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.271020 ogc_na-0.1.3/rdf/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-03 10:14:41.000000 ogc_na-0.1.3/rdf/catalog-v001.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-03 10:14:41.000000 ogc_na-0.1.3/rdf/domaincfg.vocab.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 10:14:41.000000 ogc_na-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 10:14:54.271020 ogc_na-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-03 10:14:41.000000 ogc_na-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.271020 ogc_na-0.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:54.271020 ogc_na-0.1.3/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/data/empty.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/data/profile_tree.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/data/profile_tree_cyclic.ttl
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/data/sample-context.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/data/sample-schema-prop-c.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/data/sample-schema.yml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/data/uplift_context_valid.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/test_annotate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/test_ingest_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-03 10:14:41.000000 ogc_na-0.1.3/test/test_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:56.931601 ogc_na-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:56.919601 ogc_na-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:56.923601 ogc_na-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-05 10:29:38.000000 ogc_na-0.1.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-05 10:29:38.000000 ogc_na-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 10:29:38.000000 ogc_na-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-05 10:29:56.931601 ogc_na-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-05 10:29:38.000000 ogc_na-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:56.923601 ogc_na-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-05 10:29:38.000000 ogc_na-0.1.4/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-05 10:29:38.000000 ogc_na-0.1.4/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-05 10:29:38.000000 ogc_na-0.1.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-05-05 10:29:38.000000 ogc_na-0.1.4/docs/tutorials.md
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-05 10:29:38.000000 ogc_na-0.1.4/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:56.919601 ogc_na-0.1.4/ogc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:56.927601 ogc_na-0.1.4/ogc/na/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-05 10:29:38.000000 ogc_na-0.1.4/ogc/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21506 2023-05-05 10:29:38.000000 ogc_na-0.1.4/ogc/na/annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-05-05 10:29:38.000000 ogc_na-0.1.4/ogc/na/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-05 10:29:38.000000 ogc_na-0.1.4/ogc/na/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31236 2023-05-05 10:29:38.000000 ogc_na-0.1.4/ogc/na/ingest_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:56.927601 ogc_na-0.1.4/ogc/na/input_filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-05 10:29:38.000000 ogc_na-0.1.4/ogc/na/input_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-05 10:29:38.000000 ogc_na-0.1.4/ogc/na/input_filters/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14461 2023-05-05 10:29:38.000000 ogc_na-0.1.4/ogc/na/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-05-05 10:29:38.000000 ogc_na-0.1.4/ogc/na/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17174 2023-05-05 10:29:38.000000 ogc_na-0.1.4/ogc/na/update_vocabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-05-05 10:29:38.000000 ogc_na-0.1.4/ogc/na/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-05 10:29:38.000000 ogc_na-0.1.4/ogc/na/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:56.927601 ogc_na-0.1.4/ogc_na.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-05 10:29:56.000000 ogc_na-0.1.4/ogc_na.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-05 10:29:56.000000 ogc_na-0.1.4/ogc_na.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:29:56.000000 ogc_na-0.1.4/ogc_na.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-05 10:29:56.000000 ogc_na-0.1.4/ogc_na.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 10:29:56.000000 ogc_na-0.1.4/ogc_na.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-05 10:29:38.000000 ogc_na-0.1.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:56.927601 ogc_na-0.1.4/rdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-05 10:29:38.000000 ogc_na-0.1.4/rdf/catalog-v001.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-05 10:29:38.000000 ogc_na-0.1.4/rdf/domaincfg.vocab.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 10:29:38.000000 ogc_na-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:29:56.931601 ogc_na-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-05 10:29:38.000000 ogc_na-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:56.931601 ogc_na-0.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:38.000000 ogc_na-0.1.4/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:56.931601 ogc_na-0.1.4/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:29:38.000000 ogc_na-0.1.4/test/data/empty.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-05 10:29:38.000000 ogc_na-0.1.4/test/data/headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-05 10:29:38.000000 ogc_na-0.1.4/test/data/no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-05 10:29:38.000000 ogc_na-0.1.4/test/data/profile_tree.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-05 10:29:38.000000 ogc_na-0.1.4/test/data/profile_tree_cyclic.ttl
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-05 10:29:38.000000 ogc_na-0.1.4/test/data/sample-context.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 10:29:38.000000 ogc_na-0.1.4/test/data/sample-schema-prop-c.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-05 10:29:38.000000 ogc_na-0.1.4/test/data/sample-schema.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-05 10:29:38.000000 ogc_na-0.1.4/test/data/uplift_context_valid.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-05-05 10:29:38.000000 ogc_na-0.1.4/test/test_annotate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 10:29:38.000000 ogc_na-0.1.4/test/test_ingest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-05-05 10:29:38.000000 ogc_na-0.1.4/test/test_input_filters_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-05 10:29:38.000000 ogc_na-0.1.4/test/test_profile.py
```

### Comparing `ogc_na-0.1.3/.github/workflows/python-publish.yml` & `ogc_na-0.1.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/.gitignore` & `ogc_na-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/PKG-INFO` & `ogc_na-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc_na
-Version: 0.1.3
+Version: 0.1.4
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.1.3/README.md` & `ogc_na-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/docs/examples.md` & `ogc_na-0.1.4/docs/examples.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/docs/gen_ref_pages.py` & `ogc_na-0.1.4/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/docs/index.md` & `ogc_na-0.1.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/docs/tutorials.md` & `ogc_na-0.1.4/docs/tutorials.md`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/mkdocs.yml` & `ogc_na-0.1.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/ogc/na/annotate_schema.py` & `ogc_na-0.1.4/ogc/na/annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/ogc/na/domain_config.py` & `ogc_na-0.1.4/ogc/na/domain_config.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/ogc/na/download.py` & `ogc_na-0.1.4/ogc/na/download.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/ogc/na/ingest_json.py` & `ogc_na-0.1.4/ogc/na/ingest_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 from pyld import jsonld
 from rdflib import Graph, DC, DCTERMS, SKOS, OWL, RDF, RDFS, XSD, DCAT
 from rdflib.namespace import Namespace, DefinedNamespace
 
 from ogc.na import util, profile
 from ogc.na.domain_config import UpliftConfigurationEntry, DomainConfiguration
 from ogc.na.provenance import ProvenanceMetadata, FileProvenanceMetadata, generate_provenance
+from ogc.na.input_filters import apply_input_filter
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_NAMESPACES: dict[str, Union[str, DefinedNamespace]] = {
     "dc": DC,
     "xsd": XSD,
     "dct": DCTERMS,
@@ -389,15 +390,16 @@
     :param input_fn: input filename
     :param jsonld_fn: output JSON-lD filename (None for automatic).
         If False, no JSON-LD output will be generated
     :param ttl_fn: output Turtle filename (None for automatic).
         If False, no Turtle output will be generated.
     :param context_fn: YAML context filename. If None, will be autodetected:
         1. From a file with the same name but yml/yaml extension (test.json -> test.yml)
-        2. From a _json-context.yml/_json-context.yaml file in the same directory
+        2. From the domain_cfg
+        3. From a _json-context.yml/_json-context.yaml file in the same directory
     :param domain_cfg: domain configuration with uplift definition locations
     :param base: base URI for JSON-LD
     :param provenance_base_uri: base URI for provenance resources
     :param provenance_process_id: process identifier for provenance tracking
     :param fetch_timeout: timeout (in seconds) for fetching referenced JSON-LD context URLs
     :param fetch_url_whitelist: list of regular expressions to filter referenced JSON-LD context URLs before
         retrieving them. If None, it will not be used; if empty sequence or False, remote fetching operations will
@@ -432,16 +434,23 @@
         contexts = (util.load_yaml(context_fn),)
     else:
         provenance_contexts = context_fn
 
     if not contexts:
         raise MissingContextException('No context file provided and one could not be discovered automatically')
 
-    with open(input_fn, 'r') as j:
-        input_data = json.load(j)
+    # Apply input filter of first context only (if any)
+    input_filters = contexts[0].get('input-filter')
+    if input_filters:
+        if not isinstance(input_filters, dict):
+            raise ValueError('input-filter must be an object')
+        input_data = apply_input_filter(input_fn, input_filters)
+    else:
+        with open(input_fn, 'r') as j:
+            input_data = json.load(j)
 
     provenance_metadata: ProvenanceMetadata | None = None
     if provenance_base_uri is not False:
         used = [FileProvenanceMetadata(filename=input_fn, mime_type='application/json')]
         used.extend(FileProvenanceMetadata(filename=c, mime_type='application/yaml') for c in provenance_contexts)
         provenance_metadata = ProvenanceMetadata(
             used=used,
@@ -631,27 +640,27 @@
     process_id = str(uuid.uuid4())
     if isinstance(input_files, str) or not isinstance(input_files, Sequence):
         input_files = (input_files,)
     if batch:
         logger.info("Input files: %s", input_files)
         remaining_fn: deque = deque()
         for input_file in input_files:
-            remaining_fn.extend(input_file.split(','))
+            if isinstance(input_file, str):
+                remaining_fn.extend(input_file.split(','))
+            else:
+                remaining_fn.append(input_file)
         while remaining_fn:
             fn = str(remaining_fn.popleft())
 
             if re.match(r'.*\.ya?ml$', fn):
                 # Context file found, try to find corresponding JSON/JSON-LD file(s)
                 logger.info('Potential YAML context file found: %s', fn)
                 remaining_fn.extend(filenames_from_context(fn, domain_config=domain_cfg) or [])
                 continue
 
-            if not re.match(r'.*\.json-?(ld)?$', fn):
-                logger.debug('File %s does not match, skipping', fn)
-                continue
             logger.info('File %s matches, processing', fn)
             try:
                 result.append(process_file(
                     fn,
                     jsonld_fn=False if jsonld_fn is False else None,
                     ttl_fn=False if ttl_fn is False else None,
                     context_fn=None,
```

### Comparing `ogc_na-0.1.3/ogc/na/profile.py` & `ogc_na-0.1.4/ogc/na/profile.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/ogc/na/provenance.py` & `ogc_na-0.1.4/ogc/na/provenance.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/ogc/na/update_vocabs.py` & `ogc_na-0.1.4/ogc/na/update_vocabs.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/ogc/na/util.py` & `ogc_na-0.1.4/ogc/na/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 from __future__ import annotations
 import os.path
 import shlex
 from glob import glob
 from pathlib import Path
 from time import time
-from typing import Optional, Union, Any, Hashable
+from typing import Optional, Union, Any, Mapping, Hashable
 
 import requests
 import rfc3987
 from rdflib import Graph
 from pyshacl import validate as shacl_validate
 from urllib.parse import urlparse
 
@@ -108,15 +108,15 @@
 
 
 def is_url(url: str, http_only: bool = False) -> bool:
     """
     Checks whether a string is a valid URL.
 
     :param url: the input string
-    :param http_only: whether to only accept HTTP and HTTPS URL's as valid
+    :param http_only: whether to only accept HTTP and HTTPS URLs as valid
     :return: `True` if this is a valid URL, otherwise `False`
     """
     if not url:
         return False
 
     parsed = urlparse(url)
     if not parsed.scheme or not (parsed.netloc or parsed.path):
@@ -157,15 +157,15 @@
 def dump_yaml(content: Any, filename: str | Path | None = None,
               **kwargs) -> str | None:
     """
     Generates YAML output.
 
     :param content: content to convert to YAML.
     :param filename: optional filename to dump the content into. If None, string content will be returned.
-    :param kwargs: other args to pass to yaml.dump
+    :param kwargs: other args to pass to `yaml.dump()`
     """
     kwargs.setdefault('sort_keys', False)
     if filename:
         with open(filename, 'w') as f:
             return yaml.dump(content, f, Dumper=YamlDumper, **kwargs)
     else:
         return yaml.dump(content, Dumper=YamlDumper, **kwargs)
@@ -225,7 +225,17 @@
             return
         if len(self._cache) >= self._maxsize and key not in self._cache:
             key_to_remove = min(self._last_access, key=self._last_access.get)
             del self._cache[key_to_remove]
             del self._last_access[key_to_remove]
         self._cache[key] = value
         self._last_access[key] = time()
+
+
+def deep_update(orig_dict: dict, with_dict: dict, replace: bool = False) -> dict:
+    dest = orig_dict if replace else {**orig_dict}
+    for k, v in with_dict.items():
+        if isinstance(v, Mapping):
+            dest[k] = deep_update(orig_dict.get(k, {}), with_dict, replace)
+        else:
+            dest[k] = v
+    return dest
```

### Comparing `ogc_na-0.1.3/ogc/na/validation.py` & `ogc_na-0.1.4/ogc/na/validation.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/ogc_na.egg-info/PKG-INFO` & `ogc_na-0.1.4/ogc_na.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogc-na
-Version: 0.1.3
+Version: 0.1.4
 Summary: OGC Naming Authority tools
 Author-email: Rob Atkinson <ratkinson@ogc.org>, Piotr Zaborowski <pzaborowski@ogc.org>, Alejandro Villar <avillar@ogc.org>
 Project-URL: Homepage, https://github.com/opengeospatial/ogc-na-tools/
 Project-URL: Documentation, https://opengeospatial.github.com/ogc-na-tools/
 Project-URL: Repository, https://github.com/opengeospatial/ogc-na-tools.git
 Keywords: ogc,ogc-na,naming authority,ogc rainbow,definitions server
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ogc_na-0.1.3/ogc_na.egg-info/SOURCES.txt` & `ogc_na-0.1.4/ogc_na.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -16,25 +16,30 @@
 ogc/na/download.py
 ogc/na/ingest_json.py
 ogc/na/profile.py
 ogc/na/provenance.py
 ogc/na/update_vocabs.py
 ogc/na/util.py
 ogc/na/validation.py
+ogc/na/input_filters/__init__.py
+ogc/na/input_filters/csv.py
 ogc_na.egg-info/PKG-INFO
 ogc_na.egg-info/SOURCES.txt
 ogc_na.egg-info/dependency_links.txt
 ogc_na.egg-info/requires.txt
 ogc_na.egg-info/top_level.txt
 rdf/catalog-v001.xml
 rdf/domaincfg.vocab.ttl
 test/__init__.py
 test/test_annotate_schema.py
 test/test_ingest_json.py
+test/test_input_filters_csv.py
 test/test_profile.py
 test/data/empty.ttl
+test/data/headers.csv
+test/data/no-headers.csv
 test/data/profile_tree.ttl
 test/data/profile_tree_cyclic.ttl
 test/data/sample-context.jsonld
 test/data/sample-schema-prop-c.yml
 test/data/sample-schema.yml
 test/data/uplift_context_valid.yml
```

### Comparing `ogc_na-0.1.3/pyproject.toml` & `ogc_na-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/rdf/domaincfg.vocab.ttl` & `ogc_na-0.1.4/rdf/domaincfg.vocab.ttl`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/test/data/uplift_context_valid.yml` & `ogc_na-0.1.4/test/data/uplift_context_valid.yml`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/test/test_annotate_schema.py` & `ogc_na-0.1.4/test/test_annotate_schema.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/test/test_ingest_json.py` & `ogc_na-0.1.4/test/test_ingest_json.py`

 * *Files identical despite different names*

### Comparing `ogc_na-0.1.3/test/test_profile.py` & `ogc_na-0.1.4/test/test_profile.py`

 * *Files identical despite different names*

