# Comparing `tmp/mongogettersetter-1.3.3.tar.gz` & `tmp/mongogettersetter-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongogettersetter-1.3.3.tar", last modified: Wed Apr 12 16:07:35 2023, max compression
+gzip compressed data, was "mongogettersetter-1.3.4.tar", last modified: Fri May  5 15:50:06 2023, max compression
```

## Comparing `mongogettersetter-1.3.3.tar` & `mongogettersetter-1.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 16:07:35.558649 mongogettersetter-1.3.3/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-04-12 16:07:35.558649 mongogettersetter-1.3.3/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29274 2023-04-12 16:07:24.000000 mongogettersetter-1.3.3/README.md
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 16:07:35.558649 mongogettersetter-1.3.3/mongogettersetter/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    24177 2023-04-12 12:58:33.000000 mongogettersetter-1.3.3/mongogettersetter/__init__.py
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-04-12 16:07:35.558649 mongogettersetter-1.3.3/mongogettersetter.egg-info/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-04-12 16:07:35.000000 mongogettersetter-1.3.3/mongogettersetter.egg-info/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-04-12 16:07:35.000000 mongogettersetter-1.3.3/mongogettersetter.egg-info/SOURCES.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-04-12 16:07:35.000000 mongogettersetter-1.3.3/mongogettersetter.egg-info/dependency_links.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-04-12 16:07:35.000000 mongogettersetter-1.3.3/mongogettersetter.egg-info/requires.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-04-12 16:07:35.000000 mongogettersetter-1.3.3/mongogettersetter.egg-info/top_level.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-04-12 16:07:35.558649 mongogettersetter-1.3.3/setup.cfg
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-04-12 16:07:31.000000 mongogettersetter-1.3.3/setup.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-05 15:50:05.997540 mongogettersetter-1.3.4/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-05 15:50:05.997540 mongogettersetter-1.3.4/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29274 2023-04-12 16:07:24.000000 mongogettersetter-1.3.4/README.md
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-05 15:50:05.997540 mongogettersetter-1.3.4/mongogettersetter/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    24973 2023-05-05 15:47:50.000000 mongogettersetter-1.3.4/mongogettersetter/__init__.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-05 15:50:05.997540 mongogettersetter-1.3.4/mongogettersetter.egg-info/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-05 15:50:05.000000 mongogettersetter-1.3.4/mongogettersetter.egg-info/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-05 15:50:05.000000 mongogettersetter-1.3.4/mongogettersetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-05 15:50:05.000000 mongogettersetter-1.3.4/mongogettersetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-05 15:50:05.000000 mongogettersetter-1.3.4/mongogettersetter.egg-info/requires.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-05 15:50:05.000000 mongogettersetter-1.3.4/mongogettersetter.egg-info/top_level.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-05 15:50:05.997540 mongogettersetter-1.3.4/setup.cfg
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-05-05 15:41:57.000000 mongogettersetter-1.3.4/setup.py
```

### Comparing `mongogettersetter-1.3.3/PKG-INFO` & `mongogettersetter-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.3.3
+Version: 1.3.4
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
```

### Comparing `mongogettersetter-1.3.3/README.md` & `mongogettersetter-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mongogettersetter-1.3.3/mongogettersetter/__init__.py` & `mongogettersetter-1.3.4/mongogettersetter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         )
 
     def get(self, _key=None, default=None):
         """
         Get the value of the key from the dictionary. If the key is not present, return the default value.
         """
         if _key is None:
-            return self
+            return dict(self)
         if _key in self:
             return self[_key]
         else:
             return default
 
     def pop(self, _key, default=None):
         """
@@ -202,14 +202,15 @@
     """
 
     def __init__(self, _key, _collection, _filter_query):
         self._filter_query = _filter_query
         self._collection = _collection
         self._key = _key[0]
         self._keys = _key
+        
 
     def get(self, _key=None):
         """
         Get the original representation of the document as it exists without MongoGetterSetter Wrappers.
                 If no arguments are passed, then return the whole data.
                 If _key is passed, it will return the specific value w.r.t the key.
 
@@ -611,21 +612,38 @@
         `PyMongoGetterSetter` is a class that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
         """
 
         def __getattr__(self, _key):
             """
             Return the value of the key in the array/string/object
             """
-            return MongoDataWrapper([_key], self._collection, self._filter_query)
+            data = self._collection.find_one(self._filter_query)
+            if _key in data and isinstance(data[_key], dict):
+                dictwrapper = MongoDictWrapper(data[_key])
+                dictwrapper.prepare(
+                    [_key], self._collection, self._filter_query
+                )
+                return dictwrapper
+            else:
+                return MongoDataWrapper([_key], self._collection, self._filter_query)
 
         def __getitem__(self, _key):
             """
             Return the value of the key in the array/string/object
             """
-            return MongoDataWrapper([_key], self._collection, self._filter_query)
+            #TODO: make sure the filter query runs only once
+            data = self._collection.find_one(self._filter_query)
+            if _key in data and isinstance(data[_key], dict):
+                dictwrapper = MongoDictWrapper(data)
+                dictwrapper.prepare(
+                    [_key], self._collection, self._filter_query
+                )
+                return dictwrapper
+            else:
+                return MongoDataWrapper([_key], self._collection, self._filter_query)
 
         def __setattr__(self, _key, value):
             """
             Set the value of the key in the array/string/object
             """
             _filter_query = self._filter_query
             self._collection.update_one(_filter_query, {"$set": {_key: value}})
```

### Comparing `mongogettersetter-1.3.3/mongogettersetter.egg-info/PKG-INFO` & `mongogettersetter-1.3.4/mongogettersetter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.3.3
+Version: 1.3.4
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
```

### Comparing `mongogettersetter-1.3.3/setup.py` & `mongogettersetter-1.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setup(
     name='mongogettersetter',
-    version='1.3.3',
+    version='1.3.4',
     author='Sibidharan',
     author_email='sibi@selfmade.ninja',
     description='A clean realtime way to handle MongoDB documents in Pythonic way',
     packages=find_packages(),
     url='https://git.selfmade.ninja/sibidharan/pymongogettersetter',
     install_requires=['pymongo'],
     long_description=long_description,
```

