# Comparing `tmp/mongogettersetter-1.3.4.tar.gz` & `tmp/mongogettersetter-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongogettersetter-1.3.4.tar", last modified: Fri May  5 15:50:06 2023, max compression
+gzip compressed data, was "mongogettersetter-1.3.5.tar", last modified: Fri May  5 20:28:42 2023, max compression
```

## Comparing `mongogettersetter-1.3.4.tar` & `mongogettersetter-1.3.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-05 15:50:05.997540 mongogettersetter-1.3.4/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-05 15:50:05.997540 mongogettersetter-1.3.4/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29274 2023-04-12 16:07:24.000000 mongogettersetter-1.3.4/README.md
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-05 15:50:05.997540 mongogettersetter-1.3.4/mongogettersetter/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    24973 2023-05-05 15:47:50.000000 mongogettersetter-1.3.4/mongogettersetter/__init__.py
-drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-05 15:50:05.997540 mongogettersetter-1.3.4/mongogettersetter.egg-info/
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-05 15:50:05.000000 mongogettersetter-1.3.4/mongogettersetter.egg-info/PKG-INFO
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-05 15:50:05.000000 mongogettersetter-1.3.4/mongogettersetter.egg-info/SOURCES.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-05 15:50:05.000000 mongogettersetter-1.3.4/mongogettersetter.egg-info/dependency_links.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-05 15:50:05.000000 mongogettersetter-1.3.4/mongogettersetter.egg-info/requires.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-05 15:50:05.000000 mongogettersetter-1.3.4/mongogettersetter.egg-info/top_level.txt
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-05 15:50:05.997540 mongogettersetter-1.3.4/setup.cfg
--rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-05-05 15:41:57.000000 mongogettersetter-1.3.4/setup.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-05 20:28:42.582710 mongogettersetter-1.3.5/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-05 20:28:42.582710 mongogettersetter-1.3.5/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29274 2023-04-12 16:07:24.000000 mongogettersetter-1.3.5/README.md
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-05 20:28:42.582710 mongogettersetter-1.3.5/mongogettersetter/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    24990 2023-05-05 20:23:21.000000 mongogettersetter-1.3.5/mongogettersetter/__init__.py
+drwxrwxr-x   0 sibidharan  (1000) sibidharan  (1000)        0 2023-05-05 20:28:42.582710 mongogettersetter-1.3.5/mongogettersetter.egg-info/
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)    29871 2023-05-05 20:28:42.000000 mongogettersetter-1.3.5/mongogettersetter.egg-info/PKG-INFO
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      252 2023-05-05 20:28:42.000000 mongogettersetter-1.3.5/mongogettersetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        1 2023-05-05 20:28:42.000000 mongogettersetter-1.3.5/mongogettersetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)        8 2023-05-05 20:28:42.000000 mongogettersetter-1.3.5/mongogettersetter.egg-info/requires.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       18 2023-05-05 20:28:42.000000 mongogettersetter-1.3.5/mongogettersetter.egg-info/top_level.txt
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)       38 2023-05-05 20:28:42.582710 mongogettersetter-1.3.5/setup.cfg
+-rw-rw-r--   0 sibidharan  (1000) sibidharan  (1000)      879 2023-05-05 20:28:33.000000 mongogettersetter-1.3.5/setup.py
```

### Comparing `mongogettersetter-1.3.4/PKG-INFO` & `mongogettersetter-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.3.4
+Version: 1.3.5
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
```

### Comparing `mongogettersetter-1.3.4/README.md` & `mongogettersetter-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mongogettersetter-1.3.4/mongogettersetter/__init__.py` & `mongogettersetter-1.3.5/mongogettersetter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,231 +1,187 @@
-# import sys
 import json
+from .MongoDataWrapper import MongoDataWrapper
+from .MongoDictWrapper import MongoDictWrapper
 
-# sys.(64)setrecursionlimit
 
+class MongoGetterSetter(type):
 
-class MongoDictWrapper(dict):
     """
-    MongoDictWrapper is a wrapper around the dictionary object to provide the functionality of updating the database when the dictionary is updated. It is used to wrap the dictionary object in the MongoGetterSetter class. It is not meant to be used directly.
+    `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
     """
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def prepare(self, _key, _collection, _filter_query):
+    def __call__(cls, *args, **kwargs):
         """
-        Prepare the MongoDictWrapper object to be used. This method is called by the MongoGetterSetter class when the object is created.
+        Return a new instance of the class
         """
 
-        self._filter_query = _filter_query
-        self._collection = _collection
-        self._key = _key[0]
-        self._keys = _key
-        # path = '.'.join(str(v) for v in self._keys)
-        # print(f"__prepare__ you are at: {path}")
+        instance = super().__call__(*args, **kwargs)
+        instance.__class__ = type(
+            "PyMongoGetterSetter",
+            (cls,), 
+            {
+                "__getattr__": cls.PyMongoGetterSetter.__getattr__,
+                "__getitem__": cls.PyMongoGetterSetter.__getitem__,
+                "__setattr__": cls.PyMongoGetterSetter.__setattr__,
+                "__setitem__": cls.PyMongoGetterSetter.__setitem__,
+                "__contains__": cls.PyMongoGetterSetter.__contains__,
+                "__str__": cls.PyMongoGetterSetter.__str__,
+                "__repr__": cls.PyMongoGetterSetter.__repr__,
+                "__delattr__": cls.PyMongoGetterSetter.__delattr__,
+                "__delitem__": cls.PyMongoGetterSetter.__delitem__,
+                "delete": cls.PyMongoGetterSetter.delete,
+                "set": cls.PyMongoGetterSetter.set,
+                "get": cls.PyMongoGetterSetter.get,
+            },
+        )
+        return instance
 
-    def __setattr__(self, _key, value):
-        _key = str(_key)
-        """
-        Set the value of the key in the dictionary and update the database.
-        """
-        if _key in ["_filter_query", "_collection", "_key", "_keys"]:
-            self.__dict__[_key] = value
-        else:
-            # Call the parent __setitem__ method to actually set the value in the dictionary
-            path = ".".join(str(v) for v in self._keys)
-            # Execute your function here
-            # # print(f"Dictionary updated: {path}.{_key}={value}")
-            update = {"$set": {"{}.{}".format(path, _key): value}}
-            result = self._collection.update_one(self._filter_query, update)
-            nested_dict = self._collection.find_one(self._filter_query)
-            for k in self._keys:
-                nested_dict = nested_dict[k]
-            # print(f"__setitem__ {str(nested_dict)}")
-            super().update(nested_dict)
+    class PyMongoGetterSetter:
 
-    def __getattr__(self, _key):
         """
-        Get the value of the key in the dictionary.
+        `PyMongoGetterSetter` is a class that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
         """
-        _key = str(_key)
-        if _key in self.__dict__:
-            return self.__dict__[_key]
-        else:
-            path = ".".join(str(v) for v in self._keys)
-            # print(f"__getitem__ you are at: {path}")
-            nested_dict = self._collection.find_one(self._filter_query)
-            for k in self._keys:
-                nested_dict = nested_dict[k]
-            super().update(nested_dict)
-            # print(f"__getitem__ {str(nested_dict)}")
-            if isinstance(nested_dict[_key], dict):
-                dictwrapper = MongoDictWrapper(nested_dict[_key])
+
+        def __getattr__(self, _key):
+            """
+            Return the value of the key in the array/string/object
+            """
+            data = self._collection.find_one(self._filter_query)
+            if _key in data and isinstance(data[_key], dict):
+                dictwrapper = MongoDictWrapper(data[_key])
                 dictwrapper.prepare(
-                    self._keys + [_key], self._collection, self._filter_query
+                    [_key], self._collection, self._filter_query
                 )
                 return dictwrapper
-            elif isinstance(nested_dict[_key], list):
-                datawrapper = MongoDataWrapper(
-                    self._keys + [_key], self._collection, self._filter_query
-                )
-                return datawrapper
             else:
-                return nested_dict[_key]
-
-    def __getitem__(self, _key):
-        _key = str(_key)
-        """
-        Get the value of the key in the dictionary.
-        """
-        path = ".".join(str(v) for v in self._keys)
-        # print(f"__getitem__ you are at: {path}")
-        nested_dict = self._collection.find_one(self._filter_query)
-        for k in self._keys:
-            nested_dict = nested_dict[k]
-        super().update(nested_dict)
-        # print(f"__getitem__ {str(nested_dict)}")
-        if isinstance(nested_dict[_key], dict):
-            dictwrapper = MongoDictWrapper(nested_dict[_key])
-            dictwrapper.prepare(
-                self._keys + [_key], self._collection, self._filter_query
-            )
-            return dictwrapper
-        elif isinstance(nested_dict[_key], list):
-            datawrapper = MongoDataWrapper(
-                self._keys + [_key], self._collection, self._filter_query
-            )
-            return datawrapper
-        else:
-            return nested_dict[_key]
-
-    def __setitem__(self, _key, value):
-        _key = str(_key)
-        """
-        Set the value of the key in the dictionary and update the database.
-        """
-        # Call the parent __setitem__ method to actually set the value in the dictionary
-        path = ".".join(str(v) for v in self._keys)
-        # Execute your function here
-        # # print(f"Dictionary updated: {path}.{_key}={value}")
-        update = {"$set": {"{}.{}".format(path, _key): value}}
-        result = self._collection.update_one(self._filter_query, update)
-        nested_dict = self._collection.find_one(self._filter_query)
-        for k in self._keys:
-            nested_dict = nested_dict[k]
-        # print(f"__setitem__ {str(nested_dict)}")
-        super().update(nested_dict)
-
-    def __delitem__(self, _key):
-        _key = str(_key)
-        """
-        Delete the item from the dictionary and update the database.
-        """
-        super().__delitem__(_key)
-        path = ".".join(str(v) for v in self._keys)
-        self._collection.update_one(
-            self._filter_query, {"$unset": {path + "." + _key: ""}}
-        )
-
-    def __delattr_(self, _key):
-        _key = str(_key)
-        """
-        Delete the item from the dictionary and update the database.
-        """
-        super().__delitem__(_key)
-        path = ".".join(str(v) for v in self._keys)
-        self._collection.update_one(
-            self._filter_query, {"$unset": {path + "." + _key: ""}}
-        )
-    
-    def delete(self):
-        """
-        Delete the nested object from the MongoDB Document using $unset
-        """
-        
-        path = ".".join(str(v) for v in self._keys)
-        self._collection.update_one(
-            self._filter_query, {"$unset": {path: ""}}
-        )
+                return MongoDataWrapper(data, [_key], self._collection, self._filter_query)
 
-    def get(self, _key=None, default=None):
-        """
-        Get the value of the key from the dictionary. If the key is not present, return the default value.
-        """
-        if _key is None:
-            return dict(self)
-        if _key in self:
-            return self[_key]
-        else:
-            return default
+        def __getitem__(self, _key):
+            """
+            Return the value of the key in the array/string/object
+            """
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
 
-    def pop(self, _key, default=None):
-        """
-        Pop the value of the key from the dictionary and update the database. If the key is not present, return the default value.
-        """
+        def __setattr__(self, _key, value):
+            """
+            Set the value of the key in the array/string/object
+            """
+            _filter_query = self._filter_query
+            self._collection.update_one(_filter_query, {"$set": {_key: value}})
 
-        value = super().pop(_key, default)
-        path = ".".join(str(v) for v in self._keys)
-        self._collection.update_one(
-            self._filter_query, {"$unset": {path + "." + _key: ""}}
-        )
-        return value
+        def __setitem__(self, _key, value):
+            """
+            Set the value of the key in the array/string/object
+            """
+            _filter_query = self._filter_query
+            self._collection.update_one(_filter_query, {"$set": {_key: value}})
 
-    def update(self, other):
-        """
-        Update the dictionary with the other dictionary and update the database.
-        """
+        def __contains__(self, _key):
+            """
+            Return the value of the key in the array/string/object
+            """
+            return self._collection.find_one({_key: {"$exists": True}})
 
-        super().update(other)
-        d = dict(self)
-        other.update(d)
-        path = ".".join(str(v) for v in self._keys)
-        update = {"$set": {path: other}}
-        self._collection.update_one(self._filter_query, update, upsert=True)
+        def __str__(self):
+            """
+            Return the string representation of the array/string/object
+            """
+            _filter_query = self._filter_query
+            doc = self._collection.find_one(_filter_query)
+            return json.dumps(doc, indent=4, default=str)
 
-    def clear(self):
-        """
-        Clear the dictionary and update the database.
-        """
+        def __repr__(self):
+            """
+            Return the string representation of the array/string/object
+            """
+            _filter_query = self._filter_query
+            return str(self._collection.find_one(_filter_query))
 
-        # print("__clear__ ")
-        path = ".".join(str(v) for v in self._keys)
-        update = {"$set": {path: {}}}
-        self._collection.update_one(self._filter_query, update)
-        super().clear()
+        def __delattr__(self, name):
+            """
+            Delete the key in the array/string/object using del keyword
+            """
+            # print(f"___delattr___ name = {name}")
+            self._collection.update_one(self._filter_query, {"$unset": {name: ""}})
 
+        def __delitem__(self, name):
+            """
+            Delete the key in the array/string/object using del keyword
+            """
+            # print(f"___delattr___ name = {name}")
+            self._collection.update_one(self._filter_query, {"$unset": {name: ""}})
+            
+        def delete(self):
+            """
+            Delete object from the MongoDB Collection using $unset
+            """
+            # print(f"deleting {self._id}")
+            self._collection.delete_one(self._filter_query)
+            
+        
+        def __eq__(self, other):
+            """
+            Return True if the two objects are equal
+            """
+            return repr(self) == repr(other)
+        
+        def __ne__(self, other):
+            """
+            Return True if the two objects are not equal
+            """
+            return repr(self) != repr(other)
+        
+        def set(self, data):
+            """
+            Set the document in the MongoDB Collection
+            """
+            self._collection.update_one(self._filter_query, {"$set": data})
+            
+        def get(self):
+            """
+            Get the document from the MongoDB Collection
+            """
+            return self._collection.find_one(self._filter_query)
+            
 
 class MongoDataWrapper:
 
     """
     `MongoDataWrapper` is a subscriptable class, which wraps MongoDB document datatypes to provide MongoDB Array/List Operations over a simple, straightforward API to perform various operations on the MongoDB collection. Check the list of methods for the allowed operations.
     """
 
-    def __init__(self, _key, _collection, _filter_query):
+    def __init__(self, data, _key, _collection, _filter_query):
+        self._data = data
         self._filter_query = _filter_query
         self._collection = _collection
         self._key = _key[0]
         self._keys = _key
-        
 
     def get(self, _key=None):
         """
         Get the original representation of the document as it exists without MongoGetterSetter Wrappers.
                 If no arguments are passed, then return the whole data.
                 If _key is passed, it will return the specific value w.r.t the key.
 
                 Args:
                     _key (any|None, optional):  Defaults to None.
 
                 Returns:
                     any: Original Data without Wrapper
 
         """
-
         nested_dict = self._collection.find_one(self._filter_query)
         for k in self._keys:
             nested_dict = nested_dict[k]
         if _key is None:
             return nested_dict
         else:
             return nested_dict[_key]
@@ -420,55 +376,55 @@
         return len(self.get())
 
     def __str__(self):
         """
         Return the string representation of the array/string/object
         """
 
-        nested_dict = self._collection.find_one(self._filter_query)
+        nested_dict = self._data
         for k in self._keys:
             nested_dict = nested_dict[k]
         return json.dumps(nested_dict, indent=4, default=str)
 
     def __repr__(self):
         """
         Return the string representation of the array/string/object
         """
 
-        nested_dict = self._collection.find_one(self._filter_query)
+        nested_dict = self._data
         for k in self._keys:
             nested_dict = nested_dict[k]
         return str(nested_dict)
 
     def __int__(self):
         """
         Return the integer representation of the array/string/object
         """
 
-        nested_dict = self._collection.find_one(self._filter_query)
+        nested_dict = self._data
         for k in self._keys:
             nested_dict = nested_dict[k]
         return int(nested_dict)
 
     def __float__(self):
         """
         Return the float representation of the array/string/object
         """
 
-        nested_dict = self._collection.find_one(self._filter_query)
+        nested_dict = self._data
         for k in self._keys:
             nested_dict = nested_dict[k]
         return float(nested_dict)
 
     def __bool__(self):
         """
         Return the boolean representation of the array/string/object
         """
 
-        nested_dict = self._collection.find_one(self._filter_query)
+        nested_dict = self._data
         for k in self._keys:
             nested_dict = nested_dict[k]
         return bool(nested_dict)
 
     def __getitem__(self, _key):
         """
         Return the value of the key in the array/string/object
@@ -480,15 +436,15 @@
             dictwrapper = MongoDictWrapper(data)
             dictwrapper.prepare(
                 self._keys + [_key], self._collection, self._filter_query
             )
             return dictwrapper
         elif isinstance(data, list):
             datawrapper = MongoDataWrapper(
-                self._keys + [_key], self._collection, self._filter_query
+                data, self._keys + [_key], self._collection, self._filter_query
             )
             return datawrapper
         else:
             return data
 
     def __getattr__(self, _key):
         """
@@ -499,31 +455,31 @@
             return self.__dict__[_key]
         else:
             data = self.get(_key)
             # return data[_key]
             if isinstance(data, dict):
                 dictwrapper = MongoDictWrapper(data)
                 dictwrapper.prepare(
-                    self._keys + [_key], self._collection, self._filter_query
+                    data, self._keys + [_key], self._collection, self._filter_query
                 )
                 return dictwrapper
             elif isinstance(data, list):
                 datawrapper = MongoDataWrapper(
-                    self._keys + [_key], self._collection, self._filter_query
+                    data, self._keys + [_key], self._collection, self._filter_query
                 )
                 return datawrapper
             else:
                 return data
 
     def __setattr__(self, _key, value):
         """
         Set the value of the key in the array/string/object
         """
         _key = str(_key)
-        if _key in ["_filter_query", "_collection", "_key", "_keys"]:
+        if _key in ["_filter_query", "_collection", "_key", "_keys", "_data"]:
             self.__dict__[_key] = value
         else:
             path = ".".join(str(v) for v in self._keys)
             self._collection.update_one(
                 self._filter_query, {"$set": {path + "." + _key: value}}
             )
             # # print("__setattr__", _key, value)
@@ -570,155 +526,199 @@
         path = ".".join(str(v) for v in self._keys)
         self._collection.update_one(
             self._filter_query, {"$unset": {path: ""}}
         )
         
 
 
-class MongoGetterSetter(type):
-
+class MongoDictWrapper(dict):
     """
-    `MongoGetterSetter` is a metaclass that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
+    MongoDictWrapper is a wrapper around the dictionary object to provide the functionality of updating the database when the dictionary is updated. It is used to wrap the dictionary object in the MongoGetterSetter class. It is not meant to be used directly.
     """
 
-    def __call__(cls, *args, **kwargs):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def prepare(self, _key, _collection, _filter_query):
         """
-        Return a new instance of the class
+        Prepare the MongoDictWrapper object to be used. This method is called by the MongoGetterSetter class when the object is created.
         """
 
-        instance = super().__call__(*args, **kwargs)
-        instance.__class__ = type(
-            "PyMongoGetterSetter",
-            (cls,),
-            {
-                "__getattr__": cls.PyMongoGetterSetter.__getattr__,
-                "__getitem__": cls.PyMongoGetterSetter.__getitem__,
-                "__setattr__": cls.PyMongoGetterSetter.__setattr__,
-                "__setitem__": cls.PyMongoGetterSetter.__setitem__,
-                "__contains__": cls.PyMongoGetterSetter.__contains__,
-                "__str__": cls.PyMongoGetterSetter.__str__,
-                "__repr__": cls.PyMongoGetterSetter.__repr__,
-                "__delattr__": cls.PyMongoGetterSetter.__delattr__,
-                "__delitem__": cls.PyMongoGetterSetter.__delitem__,
-                "delete": cls.PyMongoGetterSetter.delete,
-                "set": cls.PyMongoGetterSetter.set,
-                "get": cls.PyMongoGetterSetter.get,
-            },
-        )
-        return instance
-
-    class PyMongoGetterSetter:
+        self._filter_query = _filter_query
+        self._collection = _collection
+        self._key = _key[0]
+        self._keys = _key
+        # path = '.'.join(str(v) for v in self._keys)
+        # print(f"__prepare__ you are at: {path}")
 
+    def __setattr__(self, _key, value):
+        _key = str(_key)
         """
-        `PyMongoGetterSetter` is a class that provides a convenient getter and setter API for instances of the classes that use it, allowing natural operations in Python objects to easily reflect in MongoDB documents.
+        Set the value of the key in the dictionary and update the database.
         """
+        if _key in ["_filter_query", "_collection", "_key", "_keys"]:
+            self.__dict__[_key] = value
+        else:
+            # Call the parent __setitem__ method to actually set the value in the dictionary
+            path = ".".join(str(v) for v in self._keys)
+            # Execute your function here
+            # # print(f"Dictionary updated: {path}.{_key}={value}")
+            update = {"$set": {"{}.{}".format(path, _key): value}}
+            result = self._collection.update_one(self._filter_query, update)
+            nested_dict = self._collection.find_one(self._filter_query)
+            for k in self._keys:
+                nested_dict = nested_dict[k]
+            # print(f"__setitem__ {str(nested_dict)}")
+            super().update(nested_dict)
 
-        def __getattr__(self, _key):
-            """
-            Return the value of the key in the array/string/object
-            """
-            data = self._collection.find_one(self._filter_query)
-            if _key in data and isinstance(data[_key], dict):
-                dictwrapper = MongoDictWrapper(data[_key])
+    def __getattr__(self, _key):
+        """
+        Get the value of the key in the dictionary.
+        """
+        _key = str(_key)
+        if _key in self.__dict__:
+            return self.__dict__[_key]
+        else:
+            path = ".".join(str(v) for v in self._keys)
+            # print(f"__getitem__ you are at: {path}")
+            original_dict = self._collection.find_one(self._filter_query)
+            nested_dict = original_dict
+            for k in self._keys:
+                nested_dict = nested_dict[k]
+            super().update(nested_dict)
+            # print(f"__getitem__ {str(nested_dict)}")
+            if isinstance(nested_dict[_key], dict):
+                dictwrapper = MongoDictWrapper(nested_dict[_key])
                 dictwrapper.prepare(
-                    [_key], self._collection, self._filter_query
+                    self._keys + [_key], self._collection, self._filter_query
                 )
                 return dictwrapper
-            else:
-                return MongoDataWrapper([_key], self._collection, self._filter_query)
-
-        def __getitem__(self, _key):
-            """
-            Return the value of the key in the array/string/object
-            """
-            #TODO: make sure the filter query runs only once
-            data = self._collection.find_one(self._filter_query)
-            if _key in data and isinstance(data[_key], dict):
-                dictwrapper = MongoDictWrapper(data)
-                dictwrapper.prepare(
-                    [_key], self._collection, self._filter_query
+            elif isinstance(nested_dict[_key], list):
+                datawrapper = MongoDataWrapper(
+                    original_dict + [_key], self._collection, self._filter_query
                 )
-                return dictwrapper
+                return datawrapper
             else:
-                return MongoDataWrapper([_key], self._collection, self._filter_query)
+                return nested_dict[_key]
 
-        def __setattr__(self, _key, value):
-            """
-            Set the value of the key in the array/string/object
-            """
-            _filter_query = self._filter_query
-            self._collection.update_one(_filter_query, {"$set": {_key: value}})
+    def __getitem__(self, _key):
+        _key = str(_key)
+        """
+        Get the value of the key in the dictionary.
+        """
+        path = ".".join(str(v) for v in self._keys)
+        # print(f"__getitem__ you are at: {path}")
+        original_dict = self._collection.find_one(self._filter_query)
+        nested_dict = original_dict
+        for k in self._keys:
+            nested_dict = nested_dict[k]
+        super().update(nested_dict)
+        # print(f"__getitem__ {str(nested_dict)}")
+        if isinstance(nested_dict[_key], dict):
+            dictwrapper = MongoDictWrapper(nested_dict[_key])
+            dictwrapper.prepare(
+                self._keys + [_key], self._collection, self._filter_query
+            )
+            return dictwrapper
+        elif isinstance(nested_dict[_key], list):
+            datawrapper = MongoDataWrapper(
+                self._keys + [_key], self._collection, self._filter_query
+            )
+            return datawrapper
+        else:
+            return nested_dict[_key]
 
-        def __setitem__(self, _key, value):
-            """
-            Set the value of the key in the array/string/object
-            """
-            _filter_query = self._filter_query
-            self._collection.update_one(_filter_query, {"$set": {_key: value}})
+    def __setitem__(self, _key, value):
+        _key = str(_key)
+        """
+        Set the value of the key in the dictionary and update the database.
+        """
+        # Call the parent __setitem__ method to actually set the value in the dictionary
+        path = ".".join(str(v) for v in self._keys)
+        # Execute your function here
+        # # print(f"Dictionary updated: {path}.{_key}={value}")
+        update = {"$set": {"{}.{}".format(path, _key): value}}
+        result = self._collection.update_one(self._filter_query, update)
+        nested_dict = self._collection.find_one(self._filter_query)
+        for k in self._keys:
+            nested_dict = nested_dict[k]
+        # print(f"__setitem__ {str(nested_dict)}")
+        super().update(nested_dict)
 
-        def __contains__(self, _key):
-            """
-            Return the value of the key in the array/string/object
-            """
-            return self._collection.find_one({_key: {"$exists": True}})
+    def __delitem__(self, _key):
+        _key = str(_key)
+        """
+        Delete the item from the dictionary and update the database.
+        """
+        super().__delitem__(_key)
+        path = ".".join(str(v) for v in self._keys)
+        self._collection.update_one(
+            self._filter_query, {"$unset": {path + "." + _key: ""}}
+        )
 
-        def __str__(self):
-            """
-            Return the string representation of the array/string/object
-            """
-            _filter_query = self._filter_query
-            doc = self._collection.find_one(_filter_query)
-            return json.dumps(doc, indent=4, default=str)
+    def __delattr_(self, _key):
+        _key = str(_key)
+        """
+        Delete the item from the dictionary and update the database.
+        """
+        super().__delitem__(_key)
+        path = ".".join(str(v) for v in self._keys)
+        self._collection.update_one(
+            self._filter_query, {"$unset": {path + "." + _key: ""}}
+        )
+    
+    def delete(self):
+        """
+        Delete the nested object from the MongoDB Document using $unset
+        """
+        
+        path = ".".join(str(v) for v in self._keys)
+        self._collection.update_one(
+            self._filter_query, {"$unset": {path: ""}}
+        )
 
-        def __repr__(self):
-            """
-            Return the string representation of the array/string/object
-            """
-            _filter_query = self._filter_query
-            return str(self._collection.find_one(_filter_query))
+    def get(self, _key=None, default=None):
+        """
+        Get the value of the key from the dictionary. If the key is not present, return the default value.
+        """
+        if _key is None:
+            return dict(self)
+        if _key in self:
+            return self[_key]
+        else:
+            return default
 
-        def __delattr__(self, name):
-            """
-            Delete the key in the array/string/object using del keyword
-            """
-            # print(f"___delattr___ name = {name}")
-            self._collection.update_one(self._filter_query, {"$unset": {name: ""}})
+    def pop(self, _key, default=None):
+        """
+        Pop the value of the key from the dictionary and update the database. If the key is not present, return the default value.
+        """
+
+        value = super().pop(_key, default)
+        path = ".".join(str(v) for v in self._keys)
+        self._collection.update_one(
+            self._filter_query, {"$unset": {path + "." + _key: ""}}
+        )
+        return value
+
+    def update(self, other):
+        """
+        Update the dictionary with the other dictionary and update the database.
+        """
+
+        super().update(other)
+        d = dict(self)
+        other.update(d)
+        path = ".".join(str(v) for v in self._keys)
+        update = {"$set": {path: other}}
+        self._collection.update_one(self._filter_query, update, upsert=True)
+
+    def clear(self):
+        """
+        Clear the dictionary and update the database.
+        """
+
+        # print("__clear__ ")
+        path = ".".join(str(v) for v in self._keys)
+        update = {"$set": {path: {}}}
+        self._collection.update_one(self._filter_query, update)
+        super().clear()
 
-        def __delitem__(self, name):
-            """
-            Delete the key in the array/string/object using del keyword
-            """
-            # print(f"___delattr___ name = {name}")
-            self._collection.update_one(self._filter_query, {"$unset": {name: ""}})
-            
-        def delete(self):
-            """
-            Delete object from the MongoDB Collection using $unset
-            """
-            # print(f"deleting {self._id}")
-            self._collection.delete_one(self._filter_query)
-            
-        
-        def __eq__(self, other):
-            """
-            Return True if the two objects are equal
-            """
-            return repr(self) == repr(other)
-        
-        def __ne__(self, other):
-            """
-            Return True if the two objects are not equal
-            """
-            return repr(self) != repr(other)
-        
-        def set(self, data):
-            """
-            Set the document in the MongoDB Collection
-            """
-            self._collection.update_one(self._filter_query, {"$set": data})
-            
-        def get(self):
-            """
-            Get the document from the MongoDB Collection
-            """
-            return self._collection.find_one(self._filter_query)
-
```

### Comparing `mongogettersetter-1.3.4/mongogettersetter.egg-info/PKG-INFO` & `mongogettersetter-1.3.5/mongogettersetter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongogettersetter
-Version: 1.3.4
+Version: 1.3.5
 Summary: A clean realtime way to handle MongoDB documents in Pythonic way
 Home-page: https://git.selfmade.ninja/sibidharan/pymongogettersetter
 Author: Sibidharan
 Author-email: sibi@selfmade.ninja
 License: MIT
 Keywords: pymongo mongodb mongo mongogettersetter gettersetter getter setter
 Platform: UNKNOWN
```

### Comparing `mongogettersetter-1.3.4/setup.py` & `mongogettersetter-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setup(
     name='mongogettersetter',
-    version='1.3.4',
+    version='1.3.5',
     author='Sibidharan',
     author_email='sibi@selfmade.ninja',
     description='A clean realtime way to handle MongoDB documents in Pythonic way',
     packages=find_packages(),
     url='https://git.selfmade.ninja/sibidharan/pymongogettersetter',
     install_requires=['pymongo'],
     long_description=long_description,
```

