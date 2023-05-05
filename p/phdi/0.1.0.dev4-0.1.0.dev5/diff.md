# Comparing `tmp/phdi-0.1.0.dev4.tar.gz` & `tmp/phdi-0.1.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdi-0.1.0.dev4.tar", max compression
+gzip compressed data, was "phdi-0.1.0.dev5.tar", max compression
```

## Comparing `phdi-0.1.0.dev4.tar` & `phdi-0.1.0.dev5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0     7048 2023-04-26 17:41:55.912057 phdi-0.1.0.dev4/LICENSE.md
--rw-r--r--   0        0        0    11787 2023-04-26 17:41:55.912057 phdi-0.1.0.dev4/README.md
--rw-r--r--   0        0        0       27 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/__init__.py
--rw-r--r--   0        0        0      223 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/cloud/README.md
--rw-r--r--   0        0        0        0 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/cloud/__init__.py
--rw-r--r--   0        0        0     8647 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/cloud/azure.py
--rw-r--r--   0        0        0     2516 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/cloud/core.py
--rw-r--r--   0        0        0     6055 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/cloud/gcp.py
--rw-r--r--   0        0        0      163 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/containers/README.md
--rw-r--r--   0        0        0        0 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/containers/__init__.py
--rw-r--r--   0        0        0     2150 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/containers/base_service.py
--rw-r--r--   0        0        0        0 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/__init__.py
--rw-r--r--   0        0        0      292 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/cloud/README.md
--rw-r--r--   0        0        0      119 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/cloud/__init__.py
--rw-r--r--   0        0        0     2111 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/cloud/azure.py
--rw-r--r--   0        0        0      311 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/conversion/README.md
--rw-r--r--   0        0        0       89 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/conversion/__init__.py
--rw-r--r--   0        0        0     8026 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/conversion/convert.py
--rw-r--r--   0        0        0      808 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/geospatial/README.md
--rw-r--r--   0        0        0      294 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/geospatial/__init__.py
--rw-r--r--   0        0        0     3494 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/geospatial/census.py
--rw-r--r--   0        0        0     4521 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/geospatial/core.py
--rw-r--r--   0        0        0     3587 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/geospatial/smarty.py
--rw-r--r--   0        0        0      890 2023-04-26 17:41:56.388037 phdi-0.1.0.dev4/phdi/fhir/harmonization/README.md
--rw-r--r--   0        0        0      335 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/harmonization/__init__.py
--rw-r--r--   0        0        0    11809 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/harmonization/standardization.py
--rw-r--r--   0        0        0      179 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/linkage/__init__.py
--rw-r--r--   0        0        0     3591 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/linkage/link.py
--rw-r--r--   0        0        0      412 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/tabulation/README.md
--rw-r--r--   0        0        0      367 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/tabulation/__init__.py
--rw-r--r--   0        0        0    27459 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/tabulation/tables.py
--rw-r--r--   0        0        0      397 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/transport/README.md
--rw-r--r--   0        0        0      327 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/transport/__init__.py
--rw-r--r--   0        0        0     7383 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/transport/export.py
--rw-r--r--   0        0        0     6822 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/transport/http.py
--rw-r--r--   0        0        0     7005 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/fhir/utils.py
--rw-r--r--   0        0        0      881 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/geospatial/README.md
--rw-r--r--   0        0        0      291 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/geospatial/__init__.py
--rw-r--r--   0        0        0     9294 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/geospatial/census.py
--rw-r--r--   0        0        0     2697 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/geospatial/core.py
--rw-r--r--   0        0        0     5911 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/geospatial/smarty.py
--rw-r--r--   0        0        0     1027 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/harmonization/README.md
--rw-r--r--   0        0        0      869 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/harmonization/__init__.py
--rw-r--r--   0        0        0    28162 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/harmonization/double_metaphone.py
--rw-r--r--   0        0        0    10909 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/harmonization/hl7.py
--rw-r--r--   0        0        0    36359 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/harmonization/phdi_nicknames.csv
--rw-r--r--   0        0        0    11999 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/harmonization/standardization.py
--rw-r--r--   0        0        0     1952 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/harmonization/utils.py
--rw-r--r--   0        0        0      255 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/README.md
--rw-r--r--   0        0        0     1869 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/__init__.py
--rw-r--r--   0        0        0     1948 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/algorithms.py
--rw-r--r--   0        0        0     2288 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/core.py
--rw-r--r--   0        0        0    56895 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/link.py
--rw-r--r--   0        0        0    10945 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/postgres.py
--rw-r--r--   0        0        0     2667 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/seed.py
--rw-r--r--   0        0        0      399 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/linkage/tables.ddl
--rw-r--r--   0        0        0      225 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/tabulation/README.md
--rw-r--r--   0        0        0      134 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/tabulation/__init__.py
--rw-r--r--   0        0        0    11839 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/tabulation/tables.py
--rw-r--r--   0        0        0     2881 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/tabulation/validation_schema.json
--rw-r--r--   0        0        0      225 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/transport/README.md
--rw-r--r--   0        0        0       81 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/transport/__init__.py
--rw-r--r--   0        0        0     2334 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/transport/http.py
--rw-r--r--   0        0        0     1244 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/validation/__init__.py
--rw-r--r--   0        0        0     6260 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/validation/validation.py
--rw-r--r--   0        0        0    17870 2023-04-26 17:41:56.392037 phdi-0.1.0.dev4/phdi/validation/xml_utils.py
--rw-r--r--   0        0        0     1449 2023-04-26 17:41:56.400037 phdi-0.1.0.dev4/pyproject.toml
--rw-r--r--   0        0        0    13606 1970-01-01 00:00:00.000000 phdi-0.1.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0     7048 2023-05-05 20:21:47.950468 phdi-0.1.0.dev5/LICENSE.md
+-rw-r--r--   0        0        0    11787 2023-05-05 20:21:47.950468 phdi-0.1.0.dev5/README.md
+-rw-r--r--   0        0        0       27 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/__init__.py
+-rw-r--r--   0        0        0      223 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/cloud/README.md
+-rw-r--r--   0        0        0        0 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/cloud/__init__.py
+-rw-r--r--   0        0        0     8647 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/cloud/azure.py
+-rw-r--r--   0        0        0     2516 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/cloud/core.py
+-rw-r--r--   0        0        0     6055 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/cloud/gcp.py
+-rw-r--r--   0        0        0      163 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/containers/README.md
+-rw-r--r--   0        0        0        0 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/containers/__init__.py
+-rw-r--r--   0        0        0     2198 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/containers/base_service.py
+-rw-r--r--   0        0        0        0 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/__init__.py
+-rw-r--r--   0        0        0      292 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/cloud/README.md
+-rw-r--r--   0        0        0      119 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/cloud/__init__.py
+-rw-r--r--   0        0        0     2111 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/cloud/azure.py
+-rw-r--r--   0        0        0      311 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/conversion/README.md
+-rw-r--r--   0        0        0       89 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/conversion/__init__.py
+-rw-r--r--   0        0        0     8026 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/conversion/convert.py
+-rw-r--r--   0        0        0      808 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/geospatial/README.md
+-rw-r--r--   0        0        0      294 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/geospatial/__init__.py
+-rw-r--r--   0        0        0     3494 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/geospatial/census.py
+-rw-r--r--   0        0        0     4521 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/geospatial/core.py
+-rw-r--r--   0        0        0     3587 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/geospatial/smarty.py
+-rw-r--r--   0        0        0      890 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/harmonization/README.md
+-rw-r--r--   0        0        0      335 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/harmonization/__init__.py
+-rw-r--r--   0        0        0    11809 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/harmonization/standardization.py
+-rw-r--r--   0        0        0      179 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/linkage/__init__.py
+-rw-r--r--   0        0        0     3591 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/linkage/link.py
+-rw-r--r--   0        0        0      412 2023-05-05 20:21:48.410473 phdi-0.1.0.dev5/phdi/fhir/tabulation/README.md
+-rw-r--r--   0        0        0      367 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/fhir/tabulation/__init__.py
+-rw-r--r--   0        0        0    27459 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/fhir/tabulation/tables.py
+-rw-r--r--   0        0        0      397 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/fhir/transport/README.md
+-rw-r--r--   0        0        0      327 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/fhir/transport/__init__.py
+-rw-r--r--   0        0        0     7383 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/fhir/transport/export.py
+-rw-r--r--   0        0        0     6822 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/fhir/transport/http.py
+-rw-r--r--   0        0        0     7005 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/fhir/utils.py
+-rw-r--r--   0        0        0      881 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/geospatial/README.md
+-rw-r--r--   0        0        0      291 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/geospatial/__init__.py
+-rw-r--r--   0        0        0     9294 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/geospatial/census.py
+-rw-r--r--   0        0        0     2697 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/geospatial/core.py
+-rw-r--r--   0        0        0     5911 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/geospatial/smarty.py
+-rw-r--r--   0        0        0     1027 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/harmonization/README.md
+-rw-r--r--   0        0        0      869 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/harmonization/__init__.py
+-rw-r--r--   0        0        0    28162 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/harmonization/double_metaphone.py
+-rw-r--r--   0        0        0    10909 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/harmonization/hl7.py
+-rw-r--r--   0        0        0    36359 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/harmonization/phdi_nicknames.csv
+-rw-r--r--   0        0        0    11999 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/harmonization/standardization.py
+-rw-r--r--   0        0        0     1952 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/harmonization/utils.py
+-rw-r--r--   0        0        0      255 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/README.md
+-rw-r--r--   0        0        0     1869 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/__init__.py
+-rw-r--r--   0        0        0     1948 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/algorithms.py
+-rw-r--r--   0        0        0     2288 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/core.py
+-rw-r--r--   0        0        0    56924 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/link.py
+-rw-r--r--   0        0        0    10976 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/postgres.py
+-rw-r--r--   0        0        0     2667 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/seed.py
+-rw-r--r--   0        0        0      399 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/linkage/tables.ddl
+-rw-r--r--   0        0        0      225 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/tabulation/README.md
+-rw-r--r--   0        0        0      134 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/tabulation/__init__.py
+-rw-r--r--   0        0        0    11839 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/tabulation/tables.py
+-rw-r--r--   0        0        0     2881 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/tabulation/validation_schema.json
+-rw-r--r--   0        0        0      225 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/transport/README.md
+-rw-r--r--   0        0        0       81 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/transport/__init__.py
+-rw-r--r--   0        0        0     2334 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/transport/http.py
+-rw-r--r--   0        0        0     1244 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/validation/__init__.py
+-rw-r--r--   0        0        0     6260 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/validation/validation.py
+-rw-r--r--   0        0        0    17870 2023-05-05 20:21:48.414473 phdi-0.1.0.dev5/phdi/validation/xml_utils.py
+-rw-r--r--   0        0        0     1438 2023-05-05 20:21:48.422473 phdi-0.1.0.dev5/pyproject.toml
+-rw-r--r--   0        0        0    13594 1970-01-01 00:00:00.000000 phdi-0.1.0.dev5/PKG-INFO
```

### Comparing `phdi-0.1.0.dev4/LICENSE.md` & `phdi-0.1.0.dev5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/README.md` & `phdi-0.1.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/cloud/azure.py` & `phdi-0.1.0.dev5/phdi/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/cloud/core.py` & `phdi-0.1.0.dev5/phdi/cloud/core.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/cloud/gcp.py` & `phdi-0.1.0.dev5/phdi/cloud/gcp.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/containers/base_service.py` & `phdi-0.1.0.dev5/phdi/containers/base_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from fastapi import FastAPI
 from pathlib import Path
+from importlib import metadata
 
 
 class BaseService:
     """
     Base class for all DIBBs services. This class provides a FastAPI instance with DIBBs
     metadata and optionally a health check endpoint.
     """
@@ -23,15 +24,15 @@
         :param include_health_check_endpoint: If True, the standard DIBBs health check
             endpoint will be added.
         """
         description = Path(description_path).read_text(encoding="utf-8")
         self.include_health_check_endpoint = include_health_check_endpoint
         self.app = FastAPI(
             title=service_name,
-            version="0.0.1",
+            version=metadata.version("phdi"),
             contact={
                 "name": "CDC Public Health Data Infrastructure",
                 "url": "https://cdcgov.github.io/phdi-site/",
                 "email": "dmibuildingblocks@cdc.gov",
             },
             license_info={
                 "name": "Creative Commons Zero v1.0 Universal",
```

### Comparing `phdi-0.1.0.dev4/phdi/fhir/cloud/azure.py` & `phdi-0.1.0.dev5/phdi/fhir/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/fhir/conversion/convert.py` & `phdi-0.1.0.dev5/phdi/fhir/conversion/convert.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/fhir/geospatial/README.md` & `phdi-0.1.0.dev5/phdi/fhir/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/fhir/geospatial/census.py` & `phdi-0.1.0.dev5/phdi/fhir/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/fhir/geospatial/core.py` & `phdi-0.1.0.dev5/phdi/fhir/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/fhir/geospatial/smarty.py` & `phdi-0.1.0.dev5/phdi/fhir/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/fhir/harmonization/README.md` & `phdi-0.1.0.dev5/phdi/fhir/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/fhir/harmonization/standardization.py` & `phdi-0.1.0.dev5/phdi/fhir/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/fhir/linkage/link.py` & `phdi-0.1.0.dev5/phdi/fhir/linkage/link.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/fhir/tabulation/tables.py` & `phdi-0.1.0.dev5/phdi/fhir/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/fhir/transport/export.py` & `phdi-0.1.0.dev5/phdi/fhir/transport/export.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/fhir/transport/http.py` & `phdi-0.1.0.dev5/phdi/fhir/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/fhir/utils.py` & `phdi-0.1.0.dev5/phdi/fhir/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/geospatial/README.md` & `phdi-0.1.0.dev5/phdi/geospatial/README.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/geospatial/census.py` & `phdi-0.1.0.dev5/phdi/geospatial/census.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/geospatial/core.py` & `phdi-0.1.0.dev5/phdi/geospatial/core.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/geospatial/smarty.py` & `phdi-0.1.0.dev5/phdi/geospatial/smarty.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/harmonization/README.md` & `phdi-0.1.0.dev5/phdi/harmonization/README.md`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/harmonization/__init__.py` & `phdi-0.1.0.dev5/phdi/harmonization/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/harmonization/double_metaphone.py` & `phdi-0.1.0.dev5/phdi/harmonization/double_metaphone.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/harmonization/hl7.py` & `phdi-0.1.0.dev5/phdi/harmonization/hl7.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/harmonization/phdi_nicknames.csv` & `phdi-0.1.0.dev5/phdi/harmonization/phdi_nicknames.csv`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/harmonization/standardization.py` & `phdi-0.1.0.dev5/phdi/harmonization/standardization.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/harmonization/utils.py` & `phdi-0.1.0.dev5/phdi/harmonization/utils.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/linkage/__init__.py` & `phdi-0.1.0.dev5/phdi/linkage/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/linkage/algorithms.py` & `phdi-0.1.0.dev5/phdi/linkage/algorithms.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/linkage/core.py` & `phdi-0.1.0.dev5/phdi/linkage/core.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/linkage/link.py` & `phdi-0.1.0.dev5/phdi/linkage/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "last_name": "Patient.name.family",
     "birthdate": "Patient.birthDate",
     "address": "Patient.address.line",
     "zip": "Patient.address.postalCode",
     "city": "Patient.address.city",
     "state": "Patient.address.state",
     "sex": "Patient.gender",
-    "mrn": "Patient.identifier.value",
+    "mrn": "Patient.identifier.where(type.coding.code='MR').value",
 }
 
 
 def block_data(data: pd.DataFrame, blocks: List) -> dict:
     """
     Generates dictionary of blocked data where each key is a block
     and each value is a distinct list of lists containing the data
@@ -1406,15 +1406,15 @@
     :return: _description_
     """
     person_resource = {
         "fullUrl": f"urn:uuid:{person_id}",
         "resource": {
             "resourceType": "Person",
             "id": f"{person_id}",
-            "link": [{"target": {"Reference": f"Patient/{patient_id}"}}],
+            "link": [{"target": {"reference": f"Patient/{patient_id}"}}],
         },
         "request": {
             "method": "PUT",
             "url": f"Person/{person_id}",
         },
     }
```

### Comparing `phdi-0.1.0.dev4/phdi/linkage/postgres.py` & `phdi-0.1.0.dev5/phdi/linkage/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.person_table = person_table
         self.fields_to_jsonpaths = {
             "address": """$.address[*].line""",
             "birthdate": "$.birthDate",
             "city": """$.address[*].city""",
             "first_name": """$.name[*].given""",
             "last_name": """$.name[*].family""",
-            "mrn": """$.identifier.value""",
+            "mrn": """$.identifier ?(@.type.coding[0].code=="MR").value""",
             "sex": "$.gender",
             "state": """$.address[*].state""",
             "zip": """$.address[*].postalCode""",
         }
         db_conn = self.get_connection()
         self._close_connections(db_conn=db_conn)
```

### Comparing `phdi-0.1.0.dev4/phdi/linkage/seed.py` & `phdi-0.1.0.dev5/phdi/linkage/seed.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/tabulation/tables.py` & `phdi-0.1.0.dev5/phdi/tabulation/tables.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/tabulation/validation_schema.json` & `phdi-0.1.0.dev5/phdi/tabulation/validation_schema.json`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/transport/http.py` & `phdi-0.1.0.dev5/phdi/transport/http.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/validation/__init__.py` & `phdi-0.1.0.dev5/phdi/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/validation/validation.py` & `phdi-0.1.0.dev5/phdi/validation/validation.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/phdi/validation/xml_utils.py` & `phdi-0.1.0.dev5/phdi/validation/xml_utils.py`

 * *Files identical despite different names*

### Comparing `phdi-0.1.0.dev4/pyproject.toml` & `phdi-0.1.0.dev5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "phdi"
-version = "0.1.0.dev4"
+version = "v0.1.0.dev5"
 description = "Public health data infrastructure Building Blocks is a library to help public health departments work with their data"
 authors = ["Kenneth Chow <kenneth@skylight.digital>", "Brandon Mader <brandon@skylight.digital>", "Spencer Kathol <spencer@skylight.digital>"]
 homepage = "https://github.com/CDCgov/phdi"
 repository = "https://github.com/CDCgov/phdi"
-documentation = "https://cdcgov.github.io/phdi/v0.1.0-dev/"
+documentation = "https://cdcgov.github.io/phdi"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 smartystreets-python-sdk = "^4.10.6"
 pydantic = "^1.9.0"
 fastapi = "^0.95.0"
```

### Comparing `phdi-0.1.0.dev4/PKG-INFO` & `phdi-0.1.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdi
-Version: 0.1.0.dev4
+Version: 0.1.0.dev5
 Summary: Public health data infrastructure Building Blocks is a library to help public health departments work with their data
 Home-page: https://github.com/CDCgov/phdi
 Author: Kenneth Chow
 Author-email: kenneth@skylight.digital
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -32,15 +32,15 @@
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: pyarrow (>=8.0.0,<9.0.0)
 Requires-Dist: pycountry (>=22.3.5,<23.0.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: rapidfuzz (>=2.13.6,<3.0.0)
 Requires-Dist: smartystreets-python-sdk (>=4.10.6,<5.0.0)
 Requires-Dist: sqlalchemy (>=2.0.0,<3.0.0)
-Project-URL: Documentation, https://cdcgov.github.io/phdi/v0.1.0-dev/
+Project-URL: Documentation, https://cdcgov.github.io/phdi
 Project-URL: Repository, https://github.com/CDCgov/phdi
 Description-Content-Type: text/markdown
 
 # PRIME Public Health Data Infrastructure (PHDI)
 [![Test github badge](https://github.com/CDCgov/phdi/actions/workflows/test.yaml/badge.svg)](https://github.com/CDCgov/phdi/actions/workflows/test.yaml)
 [![codecov](https://codecov.io/gh/CDCgov/phdi/branch/main/graph/badge.svg)](https://codecov.io/gh/CDCgov/phdi)
 - [PRIME Public Health Data Infrastructure](#prime-public-health-data-infrastructure)
```

