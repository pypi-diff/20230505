# Comparing `tmp/padacioso-0.1.3a1.tar.gz` & `tmp/padacioso-0.1.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "padacioso-0.1.3a1.tar", last modified: Wed May  3 00:36:25 2023, max compression
+gzip compressed data, was "padacioso-0.1.3a2.tar", last modified: Fri May  5 00:51:03 2023, max compression
```

## Comparing `padacioso-0.1.3a1.tar` & `padacioso-0.1.3a2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:36:25.811584 padacioso-0.1.3a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-03 00:36:21.000000 padacioso-0.1.3a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-03 00:36:25.811584 padacioso-0.1.3a1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:36:25.811584 padacioso-0.1.3a1/padacioso/
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-05-03 00:36:21.000000 padacioso-0.1.3a1/padacioso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-03 00:36:21.000000 padacioso-0.1.3a1/padacioso/bracket_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-03 00:36:21.000000 padacioso-0.1.3a1/padacioso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:36:25.811584 padacioso-0.1.3a1/padacioso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-03 00:36:25.000000 padacioso-0.1.3a1/padacioso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-03 00:36:25.000000 padacioso-0.1.3a1/padacioso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 00:36:25.000000 padacioso-0.1.3a1/padacioso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 00:36:25.000000 padacioso-0.1.3a1/padacioso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-03 00:36:25.000000 padacioso-0.1.3a1/padacioso.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 00:36:25.811584 padacioso-0.1.3a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-03 00:36:21.000000 padacioso-0.1.3a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:36:25.811584 padacioso-0.1.3a1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-05-03 00:36:21.000000 padacioso-0.1.3a1/test/test_padacioso.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:51:03.849751 padacioso-0.1.3a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-05 00:50:59.000000 padacioso-0.1.3a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-05 00:51:03.849751 padacioso-0.1.3a2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:51:03.845751 padacioso-0.1.3a2/padacioso/
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-05 00:50:59.000000 padacioso-0.1.3a2/padacioso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-05 00:50:59.000000 padacioso-0.1.3a2/padacioso/bracket_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-05 00:50:59.000000 padacioso-0.1.3a2/padacioso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:51:03.849751 padacioso-0.1.3a2/padacioso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-05 00:51:03.000000 padacioso-0.1.3a2/padacioso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-05 00:51:03.000000 padacioso-0.1.3a2/padacioso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:51:03.000000 padacioso-0.1.3a2/padacioso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 00:51:03.000000 padacioso-0.1.3a2/padacioso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 00:51:03.000000 padacioso-0.1.3a2/padacioso.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 00:51:03.849751 padacioso-0.1.3a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-05 00:50:59.000000 padacioso-0.1.3a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:51:03.849751 padacioso-0.1.3a2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-05-05 00:50:59.000000 padacioso-0.1.3a2/test/test_padacioso.py
```

### Comparing `padacioso-0.1.3a1/LICENSE.md` & `padacioso-0.1.3a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `padacioso-0.1.3a1/padacioso/__init__.py` & `padacioso-0.1.3a2/padacioso/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import simplematch
-import logging
+
 from padacioso.bracket_expansion import expand_parentheses, clean_braces
-LOG = logging.getLogger('padacioso')
+
+try:
+    from ovos_utils.log import LOG
+except ImportError:
+    import logging
+    LOG = logging.getLogger('padacioso')
 
 
 class IntentContainer:
     def __init__(self, fuzz=False):
         self.intent_samples, self.entity_samples = {}, {}
         self.intents, self.entities = {}, {}
         self.fuzz = fuzz
@@ -50,61 +55,57 @@
                 penalty = 0
                 if "*" in r:
                     # penalize wildcards
                     penalty = 0.15
 
                 entities = simplematch.match(r, query, case_sensitive=True)
                 if entities is not None:
-                    for k in set(entities.keys()):
-                        v = entities.pop(k)
-                        k = k.lower()
-                        entities[k] = v
+                    for k, v in entities.items():
                         if k not in self.entity_samples:
                             # penalize unregistered entities
-                            penalty += 0.1
+                            penalty += 0.04
                         elif str(v) not in self.entity_samples[k]:
-                            # penalize unknown samples
-                            penalty += 0.05
+                            # penalize parsed entity value not in samples
+                            penalty += 0.1
                     yield {"entities": entities or {},
                            "conf": 1 - penalty,
                            "name": intent_name}
                     break
 
                 entities = simplematch.match(r, query, case_sensitive=False)
                 if entities is not None:
                     # penalize case mismatch
                     penalty += 0.05
-                    for k in set(entities.keys()):
-                        v = entities.pop(k)
-                        k = k.lower()
-                        entities[k] = v
+                    for k, v in entities.items():
                         if k not in self.entity_samples:
                             # penalize unregistered entities
-                            penalty += 0.1
-                        elif str(v) not in self.entity_samples[k]:
-                            # penalize unknown samples
                             penalty += 0.05
+                        elif str(v) not in self.entity_samples[k]:
+                            # penalize parsed entity value not in samples
+                            penalty += 0.1
                     yield {"entities": entities or {},
                            "conf": 1 - penalty,
                            "name": intent_name}
                     break
 
                 if self.fuzz:
                     penalty += 0.25
                     for f in self._get_fuzzed(r):
-                        entities = simplematch.match(f, query, case_sensitive=False)
+                        entities = simplematch.match(f, query,
+                                                     case_sensitive=False)
                         if entities is not None:
-                            for k in set(entities.keys()):
-                                v = entities.pop(k)
-                                k = k.lower()
-                                entities[k] = v
                             yield {"entities": entities or {},
                                    "conf": 1 - penalty,
                                    "name": intent_name}
                             break
 
     def calc_intent(self, query):
-        return max(
+        match = max(
             self.calc_intents(query),
             key=lambda x: x["conf"],
             default={'name': None, 'entities': {}}
         )
+        for entity in set(match['entities'].keys()):
+            entities = match['entities'].pop(entity)
+            match['entities'][entity.lower()] = entities
+        LOG.debug(match)
+        return match
```

### Comparing `padacioso-0.1.3a1/padacioso/bracket_expansion.py` & `padacioso-0.1.3a2/padacioso/bracket_expansion.py`

 * *Files identical despite different names*

### Comparing `padacioso-0.1.3a1/setup.py` & `padacioso-0.1.3a2/setup.py`

 * *Files identical despite different names*

### Comparing `padacioso-0.1.3a1/test/test_padacioso.py` & `padacioso-0.1.3a2/test/test_padacioso.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,23 +45,23 @@
         self.assertEqual(container.calc_intent('hello')['name'], 'hello')
         self.assertEqual(container.calc_intent('bye')['name'], None)
         self.assertEqual(container.calc_intent('buy milk'), {
             'name': 'buy', 'entities': {'item': 'milk'},  "conf": 1
         })
         self.assertEqual(container.calc_intent('buy beer'), {
             'name': 'buy', 'entities': {'item': 'beer'},
-            "conf": 0.95  # unseen entity example
+            "conf": 0.9  # unseen entity example
         })
         self.assertEqual(container.calc_intent('eat some bananas'), {
             'name': 'eat', 'entities': {'fruit': 'bananas'},
-            "conf": 0.9  # unregistered entity
+            "conf": 0.96  # unregistered entity
         })
         self.assertEqual(container.calc_intent("drive me to the store"), {
             'name': 'drive', 'entities': {'place': 'the store'},
-            'conf': 0.9
+            'conf': 0.96
         })
 
     def test_case(self):
         container = IntentContainer()
         container.add_intent('test', ['Testing cAPitalizAtion'])
         self.assertEqual(
             container.calc_intent('Testing cAPitalizAtion')['conf'], 1.0)
@@ -69,15 +69,15 @@
             container.calc_intent('teStiNg CapitalIzation')['conf'], 0.95)
 
     def test_multiple_entities(self):
         container = IntentContainer()
         container.add_intent('test3', ['I see {Thing} (in|on) {place}'])
         self.assertEqual(
             container.calc_intent('I see a bin in there'),
-            {'conf': 0.8,  # unregistered entity * 2
+            {'conf': 0.92,  # unregistered entity * 2
              'entities': {'place': 'there', 'thing': 'a bin'},
              'name': 'test3'}
         )
 
     def test_wildcards(self):
         container = IntentContainer()
         container.add_intent('test', ['say *'])
@@ -87,39 +87,39 @@
              'entities': {}, 'name': 'test'})
 
     def test_typed_entities(self):
         container = IntentContainer()
         container.add_intent('test_int', ['* number {number:int}'])
         self.assertEqual(
             container.calc_intent('i want nuMBer 3'),
-            {'conf': 0.7,  # wildcard + unregistered entity + bad case
+            {'conf': 0.75,  # wildcard + unregistered entity + bad case
              'entities': {'number': 3}, 'name': 'test_int'})
         self.assertEqual(
             container.calc_intent('i want number 3'),
-            {'conf': 0.75,  # wildcard + unregistered entity
+            {'conf': 0.81,  # wildcard + unregistered entity
              'entities': {'number': 3}, 'name': 'test_int'})
 
         container.add_entity("number", ["1", "2", "3", "4", "5"])
         self.assertEqual(
             container.calc_intent('i want number 10'),
-            {'conf': 0.8,  # wildcard + unseen entity example
+            {'conf': 0.75,  # wildcard + unseen entity example
              'entities': {'number': 10}, 'name': 'test_int'})
         self.assertEqual(
             container.calc_intent('i want number 3'),
             {'conf': 0.85,  # wildcard + registered entity sample
              'entities': {'number': 3}, 'name': 'test_int'})
         self.assertEqual(
             container.calc_intent('i want numBeR 3'),
             {'conf': 0.8,  # wildcard + registered entity sample + bad case
              'entities': {'number': 3}, 'name': 'test_int'})
 
         container.add_intent('test_float', ['* float {number:float}'])
         self.assertEqual(
             container.calc_intent('i want float 3'),
-            {'conf': 0.8,   # wildcard + unseen entity example
+            {'conf': 0.75,   # wildcard + unseen entity example
              'entities': {'number': 3.0}, 'name': 'test_float'})
 
     def test_no_fuzz(self):
         container = IntentContainer(fuzz=False)
         container.add_intent('test', ['this is a test',
                                       'test the intent',
                                       'execute test'])
```

