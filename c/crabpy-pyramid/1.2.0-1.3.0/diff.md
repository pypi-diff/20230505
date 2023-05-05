# Comparing `tmp/crabpy_pyramid-1.2.0.tar.gz` & `tmp/crabpy_pyramid-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crabpy_pyramid-1.2.0.tar", last modified: Thu Apr 13 13:30:20 2023, max compression
+gzip compressed data, was "crabpy_pyramid-1.3.0.tar", last modified: Fri May  5 13:21:56 2023, max compression
```

## Comparing `crabpy_pyramid-1.2.0.tar` & `crabpy_pyramid-1.3.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:20.924411 crabpy_pyramid-1.2.0/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4343 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/CHANGES.rst
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/LICENSE
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/MANIFEST.in
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6373 2023-04-13 13:30:20.924411 crabpy_pyramid-1.2.0/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1326 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/README.rst
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:20.920411 crabpy_pyramid-1.2.0/crabpy_pyramid/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    11550 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/__init__.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:20.924411 crabpy_pyramid-1.2.0/crabpy_pyramid/renderers/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/renderers/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6556 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/renderers/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3726 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/renderers/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    15765 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/renderers/crab.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:20.924411 crabpy_pyramid-1.2.0/crabpy_pyramid/routes/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/routes/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3458 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/routes/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1901 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/routes/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4825 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/routes/crab.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2735 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/utils.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:20.924411 crabpy_pyramid-1.2.0/crabpy_pyramid/views/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/views/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    12175 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/views/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     5610 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/views/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    13969 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/crabpy_pyramid/views/crab.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:20.924411 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6373 2023-04-13 13:30:20.000000 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      804 2023-04-13 13:30:20.000000 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/SOURCES.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 13:30:20.000000 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/dependency_links.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       47 2023-04-13 13:30:20.000000 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/entry_points.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 13:30:20.000000 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/not-zip-safe
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       42 2023-04-13 13:30:20.000000 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/requires.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       15 2023-04-13 13:30:20.000000 crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/top_level.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      173 2023-04-13 13:30:20.924411 crabpy_pyramid-1.2.0/setup.cfg
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1484 2023-04-13 13:30:11.000000 crabpy_pyramid-1.2.0/setup.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-05 13:21:56.532286 crabpy_pyramid-1.3.0/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4460 2023-05-05 13:21:30.000000 crabpy_pyramid-1.3.0/CHANGES.rst
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/LICENSE
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/MANIFEST.in
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6490 2023-05-05 13:21:56.532286 crabpy_pyramid-1.3.0/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1326 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/README.rst
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-05 13:21:56.528286 crabpy_pyramid-1.3.0/crabpy_pyramid/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    11605 2023-05-05 13:21:30.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/__init__.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-05 13:21:56.532286 crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6711 2023-05-05 13:21:30.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3726 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    15765 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/crab.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-05 13:21:56.532286 crabpy_pyramid-1.3.0/crabpy_pyramid/routes/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/routes/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3498 2023-05-05 13:21:30.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/routes/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1901 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/routes/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4825 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/routes/crab.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2735 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/utils.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-05 13:21:56.532286 crabpy_pyramid-1.3.0/crabpy_pyramid/views/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/views/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    11435 2023-05-05 13:21:30.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/views/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     5610 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/views/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    13969 2023-04-13 13:30:11.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/views/crab.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      599 2023-05-05 13:21:30.000000 crabpy_pyramid-1.3.0/crabpy_pyramid/views/exceptions.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-05 13:21:56.532286 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6490 2023-05-05 13:21:56.000000 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      839 2023-05-05 13:21:56.000000 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/SOURCES.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-05-05 13:21:56.000000 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/dependency_links.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       47 2023-05-05 13:21:56.000000 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/entry_points.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 13:30:20.000000 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/not-zip-safe
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       42 2023-05-05 13:21:56.000000 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/requires.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       15 2023-05-05 13:21:56.000000 crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/top_level.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      173 2023-05-05 13:21:56.532286 crabpy_pyramid-1.3.0/setup.cfg
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1484 2023-05-05 13:21:30.000000 crabpy_pyramid-1.3.0/setup.py
```

### Comparing `crabpy_pyramid-1.2.0/CHANGES.rst` & `crabpy_pyramid-1.3.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+1.3.0 (05-05-2023)
+------------------
+
+- Lijst gemeenten statisch maken (#173)
+- Exception handlig aanpassen (#175)
+
 1.2.0 (13-04-2023)
 ------------------
 
 - Drop python < 3.8 support
 - Adressenregister implementeren (#165)
 
 1.1.0 (30-03-2023)
```

### Comparing `crabpy_pyramid-1.2.0/LICENSE` & `crabpy_pyramid-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.2.0/PKG-INFO` & `crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: crabpy_pyramid
-Version: 1.2.0
+Name: crabpy-pyramid
+Version: 1.3.0
 Summary: Bindings for the CRABpy webservices and the Pyramid framework.
 Home-page: http://github.com/OnroerendErfgoed/crabpy_pyramid
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Keywords: web wsgi pyramid CRAB CAPAKEY AGIV
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,20 @@
     # activate your virtual env
     $ pip install sphinx sphinxcontrib-httpdomain
     $ python setup.py develop
     $ cd docs
     $ make html
 
 
+1.3.0 (05-05-2023)
+------------------
+
+- Lijst gemeenten statisch maken (#173)
+- Exception handlig aanpassen (#175)
+
 1.2.0 (13-04-2023)
 ------------------
 
 - Drop python < 3.8 support
 - Adressenregister implementeren (#165)
 
 1.1.0 (30-03-2023)
```

### Comparing `crabpy_pyramid-1.2.0/README.rst` & `crabpy_pyramid-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.2.0/crabpy_pyramid/__init__.py` & `crabpy_pyramid-1.3.0/crabpy_pyramid/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,14 +330,15 @@
         config.add_renderer('adresreg_listjson', adresreg_json_list_renderer)
         config.add_renderer('adresreg_itemjson', adresreg_json_item_renderer)
         _build_adressenregister(config.registry, adresreg_settings)
         config.add_directive('get_adressenregister', get_adressenregister)
         config.add_request_method(get_adressenregister, 'adressenregister_gateway')
         config.include('crabpy_pyramid.routes.adressenregister')
         config.scan('crabpy_pyramid.views.adressenregister')
+        config.scan("crabpy_pyramid.views.exceptions")
 
 
 def main(global_config, **settings):
     """
      This function returns a Pyramid WSGI application.
     """
     config = Configurator(settings=settings)
```

### Comparing `crabpy_pyramid-1.2.0/crabpy_pyramid/renderers/adressenregister.py` & `crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/adressenregister.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-import crabpy
 import pycountry
 from crabpy.gateway import adressenregister
 from pyramid.renderers import JSON
 
 json_list_renderer = JSON()
 json_item_renderer = JSON()
 
 
 def list_gewesten_adapter(obj, request):
     """
     Adapter for rendering a list of
     :class:`crabpy.gateway.adressenregister.Gewest` to json.
     """
-    return {"id": obj.id, "naam": obj.naam}
+    return {"id": obj.id, "naam": obj.naam, "niscode": obj.niscode}
 
 
 def list_provincie_adapter(obj, request):
     """
     Adapter for rendering a list of
     :class:`crabpy.gateway.adressenregister.Provincie` to json.
     """
     return {
         "niscode": obj.niscode,
         "naam": obj.naam,
         "gewest": {
-            "id": obj.gewest,
+            "id": obj.gewest_niscode,
         },
     }
 
 
 def list_deelgemeente_adapter(obj, request):
     """
     Adapter for rendering a list of
@@ -42,15 +41,19 @@
 
 
 def list_gemeente_adapter(obj, request):
     """
     Adapter for rendering a list of
     :class:`crabpy.gateway.adressenregister.Gemeenten` to json.
     """
-    return {"niscode": obj.niscode, "naam": obj.naam, "uri": obj.uri}
+    return {
+        "niscode": obj.niscode,
+        "naam": obj.naam(),
+        "provincie": {"niscode": obj.provincie_niscode}
+    }
 
 
 def list_straten_adapter(obj, request):
     """
     Adapter for rendering a list of
     :class:`crabpy.gateway.adresregister.Straat` to json.
     """
@@ -114,14 +117,15 @@
 def item_gewest_adapter(obj, request):
     """
     Adapter for rendering an object of
     :class:`crabpy.gateway.adressenregister.Gewest` to json.
     """
     return {
         "id": obj.id,
+        "niscode": obj.niscode,
         "naam": obj.naam,
         "centroid": obj.centroid,
         "bounding_box": obj.bounding_box,
     }
 
 
 def item_provincie_adapter(obj, request):
@@ -129,30 +133,29 @@
     Adapter for rendering a object of
     :class:`crabpy.gateway.adressenregister.Provincie` to json.
     """
     return {
         "niscode": obj.niscode,
         "naam": obj.naam,
         "gewest": {
-            "id": obj.gewest,
+            "niscode": obj.gewest_niscode,
         },
     }
 
 
 def item_gemeente_adapter(obj, request):
     """
     Adapter for rendering an object of
     :class:`crabpy.gateway.adressenregister.Gemeente` to json.
     """
     return {
         "niscode": obj.niscode,
-        "uri": obj.uri,
         "naam": obj.naam(),
-        "taal": obj.taal,
-        "status": obj.status,
+        "provincie": {"niscode": obj.provincie_niscode},
+        "gewest": {"niscode": obj.gewest.niscode}
     }
 
 
 def item_deelgemeente_adapter(obj, request):
     """
     Adapter for rendering a object of
     :class:`crabpy.gateway.adressenregister.Deelgemeente` to json.
```

### Comparing `crabpy_pyramid-1.2.0/crabpy_pyramid/renderers/capakey.py` & `crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.2.0/crabpy_pyramid/renderers/crab.py` & `crabpy_pyramid-1.3.0/crabpy_pyramid/renderers/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.2.0/crabpy_pyramid/routes/adressenregister.py` & `crabpy_pyramid-1.3.0/crabpy_pyramid/routes/adressenregister.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,53 +3,53 @@
 
 def includeme(config):
     crabpy_pyramid.add_route(
         config, "adressenregister_list_gewesten", "/adressenregister/gewesten"
     )
     crabpy_pyramid.add_route(
         config,
-        "adressenregister_get_gewest_by_id",
-        "/adressenregister/gewesten/{gewest_id}",
+        "adressenregister_get_gewest_by_niscode",
+        "/adressenregister/gewesten/{gewest_niscode}",
     )
 
     crabpy_pyramid.add_route(
         config,
         "adressenregister_list_provincies",
-        "/adressenregister/gewesten/{gewest_id}/provincies",
+        "/adressenregister/gewesten/{gewest_niscode}/provincies",
     )
     crabpy_pyramid.add_route(
         config,
         "adressenregister_get_provincie",
-        "/adressenregister/provincies/{provincie_id}",
+        "/adressenregister/provincies/{provincie_niscode}",
     )
     crabpy_pyramid.add_route(
         config,
         "adressenregister_list_deelgemeenten",
-        "/adressenregister/gewesten/{gewest_id}/deelgemeenten",
+        "/adressenregister/gewesten/{gewest_niscode}/deelgemeenten",
     )
     crabpy_pyramid.add_route(
         config,
         "adressenregister_list_deelgemeenten_by_gemeente",
         "/adressenregister/gemeenten/{niscode}/deelgemeenten",
     )
     crabpy_pyramid.add_route(
         config,
         "adressenregister_get_deelgemeente_by_id",
-        "/adressenregister/deelgemeenten/{deelgemeente_id}",
+        "/adressenregister/deelgemeenten/{deelgemeente_niscode}",
     )
 
     crabpy_pyramid.add_route(
         config,
         "adressenregister_list_gemeenten_by_provincie",
-        "/adressenregister/provincies/{provincie_id}/gemeenten",
+        "/adressenregister/provincies/{provincie_niscode}/gemeenten",
     )
     crabpy_pyramid.add_route(
         config,
         "list_gemeenten_adressenregister",
-        "/adressenregister/gewesten/{gewest_id}/gemeenten",
+        "/adressenregister/gewesten/{gewest_niscode}/gemeenten",
     )
 
     crabpy_pyramid.add_route(
         config, "get_gemeente_adressenregister", "/adressenregister/gemeenten/{niscode}"
     )
 
     crabpy_pyramid.add_route(
```

### Comparing `crabpy_pyramid-1.2.0/crabpy_pyramid/routes/capakey.py` & `crabpy_pyramid-1.3.0/crabpy_pyramid/routes/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.2.0/crabpy_pyramid/routes/crab.py` & `crabpy_pyramid-1.3.0/crabpy_pyramid/routes/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.2.0/crabpy_pyramid/utils.py` & `crabpy_pyramid-1.3.0/crabpy_pyramid/utils.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.2.0/crabpy_pyramid/views/adressenregister.py` & `crabpy_pyramid-1.3.0/crabpy_pyramid/views/crab.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,349 +1,429 @@
+# -*- coding: utf-8 -*-
+"""
+Views for CRAB services
+
+.. versionadded:: 0.1.0
+"""
 import logging
 
 import pycountry
-from crabpy.client import AdressenRegisterClientException
 from crabpy.gateway.exception import GatewayResourceNotFoundException
 from pyramid.httpexceptions import HTTPNotFound
 from pyramid.view import view_config
 
 from crabpy_pyramid.utils import range_return
 from crabpy_pyramid.utils import set_http_caching
 
 log = logging.getLogger(__name__)
 
 
 @view_config(
-    route_name="adressenregister_list_gewesten",
-    renderer="adresreg_listjson",
-    accept="application/json",
+    route_name='list_gewesten',
+    renderer='crab_listjson', accept='application/json'
 )
 def list_gewesten(request):
-    request = set_http_caching(request, "adressenregister", "long")
-    Gateway = request.adressenregister_gateway()
-    gewesten = Gateway.list_gewesten()
+    request = set_http_caching(request, 'crab', 'permanent')
+    Gateway = request.crab_gateway()
+    sort = request.params.get('sort', 1)
+    gewesten = Gateway.list_gewesten(sort)
     return range_return(request, gewesten)
 
 
 @view_config(
-    route_name="adressenregister_get_gewest_by_id",
-    renderer="adresreg_itemjson",
-    accept="application/json",
+    route_name='get_gewest_by_id',
+    renderer='crab_itemjson', accept='application/json'
 )
 def get_gewest_by_id(request):
-    request = set_http_caching(request, "adressenregister", "long")
-    Gateway = request.adressenregister_gateway()
-    gewest_id = int(request.matchdict.get("gewest_id"))
+    request = set_http_caching(request, 'crab', 'permanent')
+    Gateway = request.crab_gateway()
+    gewest_id = int(request.matchdict.get('gewest_id'))
     try:
         return Gateway.get_gewest_by_id(gewest_id)
     except GatewayResourceNotFoundException:
         return HTTPNotFound()
 
 
 @view_config(
-    route_name="adressenregister_list_provincies",
-    renderer="adresreg_listjson",
-    accept="application/json",
+    route_name='list_provincies',
+    renderer='crab_listjson', accept='application/json'
 )
 def list_provincies(request):
-    request = set_http_caching(request, "adressenregister", "permanent")
-    Gateway = request.adressenregister_gateway()
-    gewest_id = int(request.matchdict.get("gewest_id"))
+    request = set_http_caching(request, 'crab', 'permanent')
+    Gateway = request.crab_gateway()
+    gewest_id = int(request.matchdict.get('gewest_id'))
     provincies = Gateway.list_provincies(gewest_id)
     return range_return(request, provincies)
 
 
 @view_config(
-    route_name="adressenregister_get_provincie",
-    renderer="adresreg_itemjson",
-    accept="application/json",
+    route_name='get_provincie',
+    renderer='crab_itemjson', accept='application/json'
 )
 def get_provincie(request):
-    request = set_http_caching(request, "adressenregister", "permanent")
-    Gateway = request.adressenregister_gateway()
-    provincie_id = int(request.matchdict.get("provincie_id"))
-    provincie = Gateway.get_provincie_by_id(provincie_id)
-    if provincie:
-        return provincie
-    else:
+    request = set_http_caching(request, 'crab', 'permanent')
+    Gateway = request.crab_gateway()
+    provincie_id = int(request.matchdict.get('provincie_id'))
+    try:
+        return Gateway.get_provincie_by_id(provincie_id)
+    except GatewayResourceNotFoundException:
         return HTTPNotFound()
 
 
 @view_config(
-    route_name="adressenregister_list_deelgemeenten",
-    renderer="adresreg_listjson",
-    accept="application/json",
+    route_name='list_gemeenten_by_provincie',
+    renderer='crab_listjson', accept='application/json'
+)
+def list_gemeenten_by_provincie(request):
+    request = set_http_caching(request, 'crab', 'long')
+    Gateway = request.crab_gateway()
+    provincie_id = int(request.matchdict.get('provincie_id'))
+    gemeenten = Gateway.list_gemeenten_by_provincie(provincie_id)
+    return range_return(request, gemeenten)
+
+
+@view_config(
+    route_name='list_gemeenten_crab',
+    renderer='crab_listjson', accept='application/json'
+)
+def list_gemeenten_crab(request):
+    request = set_http_caching(request, 'crab', 'permanent')
+    Gateway = request.crab_gateway()
+    sort = request.params.get('sort', 'niscode')
+    sort_map = {'id': 1, 'naam': 2, 'niscode': 6}
+    sort = sort_map.get(sort, 6)
+    gewest_id = request.matchdict.get('gewest_id')
+    gemeenten = Gateway.list_gemeenten(gewest_id, sort)
+    return range_return(request, gemeenten)
+
+
+@view_config(
+    route_name='get_gemeente_crab',
+    renderer='crab_itemjson', accept='application/json'
+)
+def get_gemeente_crab(request):
+    request = set_http_caching(request, 'crab', 'long')
+    Gateway = request.crab_gateway()
+    gemeente_id = request.matchdict.get('gemeente_id')
+    if len(gemeente_id) == 5:
+        try:
+            return Gateway.get_gemeente_by_niscode(gemeente_id)
+        except GatewayResourceNotFoundException:
+            return HTTPNotFound()
+    else:
+        try:
+            return Gateway.get_gemeente_by_id(gemeente_id)
+        except GatewayResourceNotFoundException:
+            return HTTPNotFound()
+
+
+@view_config(
+    route_name='list_deelgemeenten',
+    renderer='crab_listjson', accept='application/json'
 )
 def list_deelgemeenten(request):
-    request = set_http_caching(request, "adressenregister", "permanent")
-    Gateway = request.adressenregister_gateway()
-    gewest_id = int(request.matchdict.get("gewest_id"))
+    Gateway = request.crab_gateway()
+    gewest_id = int(request.matchdict.get('gewest_id'))
     if gewest_id != 2:
         return HTTPNotFound()
     deelgemeenten = Gateway.list_deelgemeenten(gewest_id)
     return range_return(request, deelgemeenten)
 
 
 @view_config(
-    route_name="adressenregister_list_deelgemeenten_by_gemeente",
-    renderer="adresreg_listjson",
-    accept="application/json",
+    route_name='list_deelgemeenten_by_gemeente',
+    renderer='crab_listjson', accept='application/json'
 )
 def list_deelgemeenten_by_gemeente(request):
-    request = set_http_caching(request, "adressenregister", "permanent")
-    Gateway = request.adressenregister_gateway()
-    gemeente_id = request.matchdict.get("niscode")
-    try:
-        gemeente = Gateway.get_gemeente_by_niscode(gemeente_id)
-    except (GatewayResourceNotFoundException, AdressenRegisterClientException):
-        return HTTPNotFound()
+    request = set_http_caching(request, 'crab', 'permanent')
+    Gateway = request.crab_gateway()
+    gemeente_id = request.matchdict.get('gemeente_id')
+    if len(gemeente_id) == 5:
+        try:
+            gemeente = Gateway.get_gemeente_by_niscode(gemeente_id)
+        except GatewayResourceNotFoundException:
+            return HTTPNotFound()
+    else:
+        try:
+            gemeente = Gateway.get_gemeente_by_id(gemeente_id)
+        except GatewayResourceNotFoundException:
+            return HTTPNotFound()
     deelgemeenten = Gateway.list_deelgemeenten_by_gemeente(gemeente)
     return range_return(request, deelgemeenten)
 
 
 @view_config(
-    route_name="adressenregister_get_deelgemeente_by_id",
-    renderer="adresreg_itemjson",
-    accept="application/json",
+    route_name='get_deelgemeente_by_id',
+    renderer='crab_itemjson', accept='application/json'
 )
 def get_deelgemeente_by_id(request):
-    request = set_http_caching(request, "adressenregister", "permanent")
-    Gateway = request.adressenregister_gateway()
-    deelgemeente_id = request.matchdict.get("deelgemeente_id")
+    request = set_http_caching(request, 'crab', 'permanent')
+    Gateway = request.crab_gateway()
+    deelgemeente_id = request.matchdict.get('deelgemeente_id')
     try:
         return Gateway.get_deelgemeente_by_id(deelgemeente_id)
-    except (GatewayResourceNotFoundException, AdressenRegisterClientException):
+    except GatewayResourceNotFoundException:
         return HTTPNotFound()
 
 
 @view_config(
-    route_name="adressenregister_list_gemeenten_by_provincie",
-    renderer="adresreg_listjson",
-    accept="application/json",
+    route_name='list_straten',
+    renderer='crab_listjson', accept='application/json'
 )
-def list_gemeenten_by_provincie(request):
-    request = set_http_caching(request, "adressenregister", "long")
-    Gateway = request.adressenregister_gateway()
-    provincie_id = int(request.matchdict.get("provincie_id"))
-    try:
-        gemeenten = Gateway.list_gemeenten_by_provincie(provincie_id)
-    except (GatewayResourceNotFoundException, AdressenRegisterClientException):
-        return HTTPNotFound()
-    return range_return(request, gemeenten)
+def list_straten(request):
+    request = set_http_caching(request, 'crab', 'long')
+    Gateway = request.crab_gateway()
+    gemeente_id = request.matchdict.get('gemeente_id')
+    if len(gemeente_id) == 5:
+        gemeente_id = Gateway.get_gemeente_by_niscode(gemeente_id)
+    straten = Gateway.list_straten(gemeente_id)
+    return range_return(request, straten)
 
 
 @view_config(
-    route_name="list_gemeenten_adressenregister",
-    renderer="adresreg_listjson",
-    accept="application/json",
-)
-def list_gemeenten_adressenregister(request):
-    request = set_http_caching(request, "adressenregister", "long")
-    Gateway = request.adressenregister_gateway()
-    gewest_id = request.matchdict.get("gewest_id")
+    route_name='get_straat_by_id',
+    renderer='crab_itemjson', accept='application/json'
+)
+def get_straat_by_id(request):
+    request = set_http_caching(request, 'crab', 'long')
+    Gateway = request.crab_gateway()
+    straat_id = request.matchdict.get('straat_id')
     try:
-        gemeenten = Gateway.list_gemeenten(gewest_id)
-    except (GatewayResourceNotFoundException, AdressenRegisterClientException):
+        return Gateway.get_straat_by_id(straat_id)
+    except GatewayResourceNotFoundException:
         return HTTPNotFound()
-    return range_return(request, gemeenten)
 
 
 @view_config(
-    route_name="get_gemeente_adressenregister",
-    renderer="adresreg_itemjson",
-    accept="application/json",
+    route_name='list_huisnummers',
+    renderer='crab_listjson', accept='application/json'
 )
-def get_gemeente_adressenregister(request):
-    request = set_http_caching(request, "adressenregister", "long")
-    Gateway = request.adressenregister_gateway()
-    gemeente_id = request.matchdict.get("niscode")
-    try:
-        return Gateway.get_gemeente_by_niscode(gemeente_id)
-    except (GatewayResourceNotFoundException, AdressenRegisterClientException):
-        return HTTPNotFound()
+def list_huisnummers(request):
+    request = set_http_caching(request, 'crab', 'short')
+    Gateway = request.crab_gateway()
+    straat_id = request.matchdict.get('straat_id')
+    sort = request.params.get('sort', 1)
+    huisnummers = Gateway.list_huisnummers_by_straat(straat_id, sort)
+    return range_return(request, huisnummers)
 
 
 @view_config(
-    route_name="adressenregister_list_straten",
-    renderer="adresreg_listjson",
-    accept="application/json",
+    route_name='get_huisnummer_by_straat_and_label',
+    renderer='crab_itemjson', accept='application/json'
 )
-def list_straten(request):
-    request = set_http_caching(request, "adressenregister", "short")
-    Gateway = request.adressenregister_gateway()
-    gemeente_id = request.matchdict.get("niscode")
+def get_huisnummer_by_straat_and_label(request):
+    request = set_http_caching(request, 'crab', 'short')
+    Gateway = request.crab_gateway()
+    straat_id = request.matchdict.get('straat_id')
+    huisnummer = request.matchdict.get('huisnummer_label')
     try:
-        straten = Gateway.list_straten(gemeente_id)
-    except (GatewayResourceNotFoundException, AdressenRegisterClientException):
+        return Gateway.get_huisnummer_by_nummer_and_straat(huisnummer, straat_id)
+    except GatewayResourceNotFoundException:
         return HTTPNotFound()
-    return range_return(request, straten)
 
 
 @view_config(
-    route_name="adressenregister_get_straat_by_id",
-    renderer="adresreg_itemjson",
-    accept="application/json",
+    route_name='get_huisnummer_by_id',
+    renderer='crab_itemjson', accept='application/json'
 )
-def get_straat_by_id(request):
-    request = set_http_caching(request, "adressenregister", "short")
-    Gateway = request.adressenregister_gateway()
-    straat_id = request.matchdict.get("straat_id")
+def get_huisnummer_by_id(request):
+    request = set_http_caching(request, 'crab', 'short')
+    Gateway = request.crab_gateway()
+    huisnummer_id = request.matchdict.get('huisnummer_id')
     try:
-        return Gateway.get_straat_by_id(straat_id)
-    except (GatewayResourceNotFoundException, AdressenRegisterClientException):
+        return Gateway.get_huisnummer_by_id(huisnummer_id)
+    except GatewayResourceNotFoundException:
         return HTTPNotFound()
 
 
 @view_config(
-    route_name="adressenregister_list_adressen",
-    renderer="adresreg_listjson",
-    accept="application/json",
+    route_name='list_percelen',
+    renderer='crab_listjson', accept='application/json'
 )
-def list_adressen_by_straat(request):
-    request = set_http_caching(request, "adressenregister", "short")
-    Gateway = request.adressenregister_gateway()
-    straat_id = request.matchdict.get("straat_id")
-    try:
-        straten = Gateway.list_adressen_with_params(straatnaamObjectId=straat_id)
-    except (GatewayResourceNotFoundException, AdressenRegisterClientException):
-        return HTTPNotFound()
-    return range_return(request, straten)
+def list_percelen(request):
+    request = set_http_caching(request, 'crab', 'short')
+    Gateway = request.crab_gateway()
+    huisnummer_id = request.matchdict.get('huisnummer_id')
+    percelen = Gateway.list_percelen_by_huisnummer(huisnummer_id)
+    return range_return(request, percelen)
 
 
 @view_config(
-    route_name="adressenregister_get_adres_by_straat_and_huisnummer",
-    renderer="adresreg_listjson",
-    accept="application/json",
+    route_name='get_perceel_by_id',
+    renderer='crab_itemjson', accept='application/json'
 )
-def adressenregister_get_adres_by_straat_huisnummer(request):
-    request = set_http_caching(request, "adressenregister", "short")
-    Gateway = request.adressenregister_gateway()
-    straat_id = request.matchdict.get("straat_id")
-    huisnummer = request.matchdict.get("huisnummer")
+def get_perceel_by_id(request):
+    request = set_http_caching(request, 'crab', 'short')
+    Gateway = request.crab_gateway()
+    perceel_id = request.matchdict.get('perceel_id1') + '/' + request.matchdict.get('perceel_id2')
     try:
-        adressen = Gateway.list_adressen_with_params(
-            straatnaamObjectId=straat_id, huisnummer=huisnummer
-        )
-    except (GatewayResourceNotFoundException, AdressenRegisterClientException):
+        return Gateway.get_perceel_by_id(perceel_id)
+    except GatewayResourceNotFoundException:
         return HTTPNotFound()
-    return range_return(request, adressen)
 
 
 @view_config(
-    route_name="adressenregister_get_adres_by_straat_and_huisnummer_and_busnummer",
-    renderer="adresreg_listjson",
-    accept="application/json",
+    route_name='list_huisnummers_by_perceel',
+    renderer='crab_listjson', accept='application/json'
 )
-def adressenregister_get_adres_by_straat_huisnummer_busnummer(request):
-    request = set_http_caching(request, "adressenregister", "short")
-    Gateway = request.adressenregister_gateway()
-    straat_id = request.matchdict.get("straat_id")
-    huisnummer = request.matchdict.get("huisnummer")
-    busnummer = request.matchdict.get("busnummer")
+def list_huisnummers_by_perceel(request):
+    request = set_http_caching(request, 'crab', 'short')
+    Gateway = request.crab_gateway()
+    perceel_id = request.matchdict.get('perceel_id1') + '/' + request.matchdict.get('perceel_id2')
+    sort = request.params.get('sort', 1)
     try:
-        adressen = Gateway.list_adressen_with_params(
-            straatnaamObjectId=straat_id, huisnummer=huisnummer, busnummer=busnummer
-        )
-    except (GatewayResourceNotFoundException, AdressenRegisterClientException):
+        perceel = Gateway.get_perceel_by_id(perceel_id)
+        return Gateway.list_huisnummers_by_perceel(perceel, sort)
+    except GatewayResourceNotFoundException:
         return HTTPNotFound()
-    return range_return(request, adressen)
 
 
 @view_config(
-    route_name="adressenregister_get_adres_by_id",
-    renderer="adresreg_itemjson",
-    accept="application/json",
+    route_name='list_gebouwen',
+    renderer='crab_listjson', accept='application/json'
 )
-def adressenregister_get_adres_by_id(request):
-    request = set_http_caching(request, "adressenregister", "long")
-    Gateway = request.adressenregister_gateway()
-    adres_id = request.matchdict.get("adres_id")
-    try:
-        return Gateway.get_adres_by_id(adres_id)
-    except (GatewayResourceNotFoundException, AdressenRegisterClientException):
-        return HTTPNotFound()
+def list_gebouwen(request):
+    request = set_http_caching(request, 'crab', 'short')
+    Gateway = request.crab_gateway()
+    huisnummer_id = request.matchdict.get('huisnummer_id')
+    gebouwen = Gateway.list_gebouwen_by_huisnummer(huisnummer_id)
+    return range_return(request, gebouwen)
 
 
 @view_config(
-    route_name="adressenregister_list_percelen_by_adres",
-    renderer="adresreg_listjson",
-    accept="application/json",
+    route_name='get_gebouw_by_id',
+    renderer='crab_itemjson', accept='application/json'
 )
-def adressenregister_list_percelen_by_adres(request):
-    request = set_http_caching(request, "adressenregister", "short")
-    Gateway = request.adressenregister_gateway()
-    adres_id = request.matchdict.get("adres_id")
+def get_gebouw_by_id(request):
+    request = set_http_caching(request, 'crab', 'short')
+    Gateway = request.crab_gateway()
+    gebouw_id = request.matchdict.get('gebouw_id')
     try:
-        adressen = Gateway.list_percelen_with_params(adresObjectId=adres_id)
-    except (GatewayResourceNotFoundException, AdressenRegisterClientException):
+        return Gateway.get_gebouw_by_id(gebouw_id)
+    except GatewayResourceNotFoundException:
         return HTTPNotFound()
-    return range_return(request, adressen)
 
 
 @view_config(
-    route_name="adressenregister_get_perceel_by_id",
-    renderer="adresreg_itemjson",
-    accept="application/json",
+    route_name='get_wegobject',
+    renderer='crab_itemjson', accept='application/json'
 )
-def adressenregister_get_perceel_by_id(request):
-    request = set_http_caching(request, "adressenregister", "short")
-    Gateway = request.adressenregister_gateway()
-    perceel_id = request.matchdict.get("perceel_id")
+def get_wegobject(request):
+    request = set_http_caching(request, 'crab', 'short')
+    Gateway = request.crab_gateway()
+    wegobject_id = request.matchdict.get('wegobject_id')
     try:
-        return Gateway.get_perceel_by_id(perceel_id=perceel_id)
-    except (GatewayResourceNotFoundException, AdressenRegisterClientException):
+        return Gateway.get_wegobject_by_id(wegobject_id)
+    except GatewayResourceNotFoundException:
         return HTTPNotFound()
 
 
 @view_config(
-    route_name="adressenregister_list_postinfo_by_gemeente",
-    renderer="adresreg_listjson",
-    accept="application/json",
+    route_name='list_subadressen',
+    renderer='crab_listjson', accept='application/json'
 )
-def adressenregister_list_postinfo_by_gemeente(request):
-    request = set_http_caching(request, "adressenregister", "long")
-    Gateway = request.adressenregister_gateway()
-    gemeente_naam = request.matchdict.get("gemeente_naam")
+def list_subadressen(request):
+    request = set_http_caching(request, 'crab', 'short')
+    Gateway = request.crab_gateway()
+    huisnummer_id = request.matchdict.get('huisnummer_id')
+    subadressen = Gateway.list_subadressen_by_huisnummer(huisnummer_id)
+    return range_return(request, subadressen)
+
+
+@view_config(
+    route_name='get_subadres_by_id',
+    renderer='crab_itemjson', accept='application/json'
+)
+def get_subadres_by_id(request):
+    request = set_http_caching(request, 'crab', 'short')
+    Gateway = request.crab_gateway()
+    subadres_id = request.matchdict.get('subadres_id')
     try:
-        adressen = Gateway.get_postinfo_by_gemeentenaam(gemeente_naam)
-    except (GatewayResourceNotFoundException, AdressenRegisterClientException):
+        return Gateway.get_subadres_by_id(subadres_id)
+    except GatewayResourceNotFoundException:
         return HTTPNotFound()
-    return range_return(request, adressen)
 
 
 @view_config(
-    route_name="adressenregister_get_postinfo_by_postcode",
-    renderer="adresreg_itemjson",
-    accept="application/json",
+    route_name='list_postkantons_by_gemeente',
+    renderer='crab_listjson', accept='application/json'
+)
+def list_postkantons_by_gemeente(request):
+    request = set_http_caching(request, 'crab', 'long')
+    Gateway = request.crab_gateway()
+    gemeente_id = request.matchdict.get('gemeente_id')
+    postkantons = Gateway.list_postkantons_by_gemeente(gemeente_id)
+    return range_return(request, postkantons)
+
+
+@view_config(
+    route_name='list_adresposities_by_huisnummer',
+    renderer='crab_listjson', accept='application/json'
+)
+def list_adresposities_by_huisnummer(request):
+    request = set_http_caching(request, 'crab', 'short')
+    Gateway = request.crab_gateway()
+    huisnummer_id = request.matchdict.get('huisnummer_id')
+    adresposities = Gateway.list_adresposities_by_huisnummer(huisnummer_id)
+    return range_return(request, adresposities)
+
+
+@view_config(
+    route_name='list_adresposities_by_subadres',
+    renderer='crab_listjson', accept='application/json'
 )
-def adressenregister_get_postinfo_by_postcode(request):
-    request = set_http_caching(request, "adressenregister", "long")
-    Gateway = request.adressenregister_gateway()
-    postcode = request.matchdict.get("postcode")
+def list_adresposities_by_subadres(request):
+    request = set_http_caching(request, 'crab', 'short')
+    Gateway = request.crab_gateway()
+    subadres_id = request.matchdict.get('subadres_id')
+    adresposities = Gateway.list_adresposities_by_subadres(subadres_id)
+    return range_return(request, adresposities)
+
+
+@view_config(
+    route_name='get_adrespositie_by_id',
+    renderer='crab_itemjson', accept='application/json'
+)
+def get_adrespositie_by_id(request):
+    request = set_http_caching(request, 'crab', 'short')
+    Gateway = request.crab_gateway()
+    adrespositie_id = request.matchdict.get('adrespositie_id')
     try:
-        return Gateway.get_postinfo_by_id(postcode)
-    except (GatewayResourceNotFoundException, AdressenRegisterClientException):
+        return Gateway.get_adrespositie_by_id(adrespositie_id)
+    except GatewayResourceNotFoundException:
         return HTTPNotFound()
 
 
 @view_config(
-    route_name="adressenregister_list_landen",
-    renderer="adresreg_listjson",
-    accept="application/json",
+    route_name='list_landen',
+    renderer='crab_listjson', accept='application/json'
 )
 def list_landen(request):
-    set_http_caching(request, "adressenregister", "permanent")
+    request = set_http_caching(request, 'crab', 'permanent')
     return list(pycountry.countries)
 
 
 @view_config(
-    route_name="adressenregister_get_land_by_id",
-    renderer="adresreg_itemjson",
-    accept="application/json",
+    route_name='get_land_by_id',
+    renderer='crab_itemjson', accept='application/json'
 )
 def get_land_by_id(request):
-    request = set_http_caching(request, "adressenregister", "permanent")
-    land_id = request.matchdict.get("land_id")
+    request = set_http_caching(request, 'crab', 'permanent')
+    land_id = request.matchdict.get('land_id')
     land = pycountry.countries.get(alpha_2=land_id)
     if land is None:
         return HTTPNotFound()
     return land
+
+
+@view_config(
+    route_name='get_postkanton_by_huisnummer',
+    renderer='crab_itemjson', accept='application/json'
+)
+def get_postkanton_by_huisnummer(request):
+    request = set_http_caching(request, 'crab', 'short')
+    Gateway = request.crab_gateway()
+    huisnummer_id = request.matchdict.get('huisnummer_id')
+    try:
+        return Gateway.get_postkanton_by_huisnummer(huisnummer_id)
+    except GatewayResourceNotFoundException:
+        return HTTPNotFound()
```

### Comparing `crabpy_pyramid-1.2.0/crabpy_pyramid/views/capakey.py` & `crabpy_pyramid-1.3.0/crabpy_pyramid/views/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/PKG-INFO` & `crabpy_pyramid-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: crabpy-pyramid
-Version: 1.2.0
+Name: crabpy_pyramid
+Version: 1.3.0
 Summary: Bindings for the CRABpy webservices and the Pyramid framework.
 Home-page: http://github.com/OnroerendErfgoed/crabpy_pyramid
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Keywords: web wsgi pyramid CRAB CAPAKEY AGIV
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,20 @@
     # activate your virtual env
     $ pip install sphinx sphinxcontrib-httpdomain
     $ python setup.py develop
     $ cd docs
     $ make html
 
 
+1.3.0 (05-05-2023)
+------------------
+
+- Lijst gemeenten statisch maken (#173)
+- Exception handlig aanpassen (#175)
+
 1.2.0 (13-04-2023)
 ------------------
 
 - Drop python < 3.8 support
 - Adressenregister implementeren (#165)
 
 1.1.0 (30-03-2023)
```

### Comparing `crabpy_pyramid-1.2.0/crabpy_pyramid.egg-info/SOURCES.txt` & `crabpy_pyramid-1.3.0/crabpy_pyramid.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 crabpy_pyramid/routes/__init__.py
 crabpy_pyramid/routes/adressenregister.py
 crabpy_pyramid/routes/capakey.py
 crabpy_pyramid/routes/crab.py
 crabpy_pyramid/views/__init__.py
 crabpy_pyramid/views/adressenregister.py
 crabpy_pyramid/views/capakey.py
-crabpy_pyramid/views/crab.py
+crabpy_pyramid/views/crab.py
+crabpy_pyramid/views/exceptions.py
```

### Comparing `crabpy_pyramid-1.2.0/setup.py` & `crabpy_pyramid-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'coverage',
     'webtest'
 ]
 
 testing_extras = tests_requires + []
 
 setup(name='crabpy_pyramid',
-      version='1.2.0',
+      version='1.3.0',
       description='Bindings for the CRABpy webservices and the Pyramid framework.',
       long_description=README + '\n\n' + CHANGES,
       classifiers=[
         'Development Status :: 5 - Production/Stable',
         "Programming Language :: Python",
         'Programming Language :: Python :: 3.8',
         "Framework :: Pyramid",
```

