# Comparing `tmp/pondpond-1.3.1.tar.gz` & `tmp/pondpond-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pondpond-1.3.1.tar", last modified: Wed Apr 12 02:33:26 2023, max compression
+gzip compressed data, was "pondpond-1.3.2.tar", last modified: Fri May  5 06:12:54 2023, max compression
```

## Comparing `pondpond-1.3.1.tar` & `pondpond-1.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11358 2022-08-06 06:58:54.027681 pondpond-1.3.1/LICENSE
--rw-r--r--   0        0        0     5842 2023-04-12 02:03:28.409629 pondpond-1.3.1/README.md
--rw-r--r--   0        0        0      750 2023-03-28 02:08:30.764284 pondpond-1.3.1/pond/__init__.py
--rw-r--r--   0        0        0     3213 2023-04-11 08:25:05.994200 pondpond-1.3.1/pond/count_min_sketch.py
--rw-r--r--   0        0        0    14879 2023-04-12 02:20:45.045119 pondpond-1.3.1/pond/pond_class.py
--rw-r--r--   0        0        0     1116 2022-11-08 07:16:32.733609 pondpond-1.3.1/pond/pooled_object.py
--rw-r--r--   0        0        0     1309 2022-11-08 06:30:28.188665 pondpond-1.3.1/pond/pooled_object_factory.py
--rw-r--r--   0        0        0        0 2022-10-18 06:53:42.469389 pondpond-1.3.1/pond/py.typed
--rw-r--r--   0        0        0        0 2023-04-12 02:21:20.185473 pondpond-1.3.1/pond-stubs/__init__.pyi
--rw-r--r--   0        0        0      402 2023-04-12 02:21:20.185878 pondpond-1.3.1/pond-stubs/count_min_sketch.pyi
--rw-r--r--   0        0        0     2070 2023-04-12 02:21:20.185714 pondpond-1.3.1/pond-stubs/pond_class.pyi
--rw-r--r--   0        0        0      247 2023-04-12 02:21:20.186188 pondpond-1.3.1/pond-stubs/pooled_object.pyi
--rw-r--r--   0        0        0      678 2023-04-12 02:21:20.186037 pondpond-1.3.1/pond-stubs/pooled_object_factory.pyi
--rw-r--r--   0        0        0     1223 2023-04-12 02:03:40.888842 pondpond-1.3.1/pyproject.toml
--rw-r--r--   0        0        0       37 2022-08-02 09:08:23.046400 pondpond-1.3.1/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2022-08-02 09:08:23.046470 pondpond-1.3.1/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2022-08-02 09:08:23.046298 pondpond-1.3.1/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2022-08-02 09:08:23.046548 pondpond-1.3.1/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-08-02 09:08:23.046645 pondpond-1.3.1/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2022-08-02 08:15:47.024533 pondpond-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0     1033 2023-04-11 07:34:01.539120 pondpond-1.3.1/tests/draw.py
--rw-r--r--   0        0        0     1374 2023-04-11 06:56:38.551526 pondpond-1.3.1/tests/test_aysnc_pond.py
--rw-r--r--   0        0        0     1168 2023-04-11 08:37:53.522729 pondpond-1.3.1/tests/test_cprofile.py
--rw-r--r--   0        0        0     4926 2023-04-11 09:20:34.424503 pondpond-1.3.1/tests/test_pond.py
--rw-r--r--   0        0        0     6231 1970-01-01 00:00:00.000000 pondpond-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-08-06 06:58:54.027681 pondpond-1.3.2/LICENSE
+-rw-r--r--   0        0        0     5842 2023-05-05 06:08:53.742668 pondpond-1.3.2/README.md
+-rw-r--r--   0        0        0      750 2023-03-28 02:08:30.764284 pondpond-1.3.2/pond/__init__.py
+-rw-r--r--   0        0        0     3213 2023-04-11 08:25:05.994200 pondpond-1.3.2/pond/count_min_sketch.py
+-rw-r--r--   0        0        0    14879 2023-05-05 06:08:53.763756 pondpond-1.3.2/pond/pond_class.py
+-rw-r--r--   0        0        0     1116 2022-11-08 07:16:32.733609 pondpond-1.3.2/pond/pooled_object.py
+-rw-r--r--   0        0        0     1309 2023-05-05 06:08:53.769064 pondpond-1.3.2/pond/pooled_object_factory.py
+-rw-r--r--   0        0        0        0 2022-10-18 06:53:42.469389 pondpond-1.3.2/pond/py.typed
+-rw-r--r--   0        0        0        0 2023-05-05 06:09:53.293716 pondpond-1.3.2/pond-stubs/__init__.pyi
+-rw-r--r--   0        0        0      402 2023-05-05 06:09:53.294090 pondpond-1.3.2/pond-stubs/count_min_sketch.pyi
+-rw-r--r--   0        0        0     2070 2023-05-05 06:09:53.293927 pondpond-1.3.2/pond-stubs/pond_class.pyi
+-rw-r--r--   0        0        0      247 2023-05-05 06:09:53.294452 pondpond-1.3.2/pond-stubs/pooled_object.pyi
+-rw-r--r--   0        0        0      678 2023-05-05 06:09:53.294285 pondpond-1.3.2/pond-stubs/pooled_object_factory.pyi
+-rw-r--r--   0        0        0     1223 2023-05-05 06:09:15.901247 pondpond-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0       37 2022-08-02 09:08:23.046400 pondpond-1.3.2/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2022-08-02 09:08:23.046470 pondpond-1.3.2/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2022-08-02 09:08:23.046298 pondpond-1.3.2/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2022-08-02 09:08:23.046548 pondpond-1.3.2/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-08-02 09:08:23.046645 pondpond-1.3.2/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2022-08-02 08:15:47.024533 pondpond-1.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     1033 2023-04-11 07:34:01.539120 pondpond-1.3.2/tests/draw.py
+-rw-r--r--   0        0        0     1374 2023-05-05 06:08:53.742705 pondpond-1.3.2/tests/test_aysnc_pond.py
+-rw-r--r--   0        0        0     1156 2023-05-05 06:12:49.671857 pondpond-1.3.2/tests/test_cprofile.py
+-rw-r--r--   0        0        0     4926 2023-05-05 06:08:53.742686 pondpond-1.3.2/tests/test_pond.py
+-rw-r--r--   0        0        0     6231 1970-01-01 00:00:00.000000 pondpond-1.3.2/PKG-INFO
```

### Comparing `pondpond-1.3.1/LICENSE` & `pondpond-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pondpond-1.3.1/README.md` & `pondpond-1.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 ```python
 class Dog:
     name: str
     validate_result:bool = True
 
 
 class PooledDogFactory(PooledObjectFactory):
-    def creatInstantce(self) -> PooledObject:
+    def createInstance(self) -> PooledObject:
         dog = Dog()
         dog.name = "puppy"
         return PooledObject(dog)
 
     def destroy(self, pooled_object: PooledObject):
         del pooled_object
```

### Comparing `pondpond-1.3.1/pond/__init__.py` & `pondpond-1.3.2/pond/__init__.py`

 * *Files identical despite different names*

### Comparing `pondpond-1.3.1/pond/count_min_sketch.py` & `pondpond-1.3.2/pond/count_min_sketch.py`

 * *Files identical despite different names*

### Comparing `pondpond-1.3.1/pond/pond_class.py` & `pondpond-1.3.2/pond/pond_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             name = factory.factory_name()
         assert factory is not None
         if self.__pooled_object_tree.__contains__(name):
             raise ValueError("The factoryClass existed in the PooledObjectTree!")
         self.__class_dict[name] = factory
         self.__pooled_object_tree[name] = deque(maxlen=factory.pooled_maxsize)
         for i in range(factory.pooled_maxsize):
-            instance = self.__class_dict[name].creatInstantce()
+            instance = self.__class_dict[name].createInstance()
             if instance is None:
                 raise ValueError("The instance must not be null!")
             self.__pooled_object_tree[name].appendleft(instance)
 
     def borrow(
         self, factory: Optional[PooledObjectFactory] = None, name: Optional[str] = None
     ) -> PooledObject:
@@ -131,20 +131,20 @@
         with self.__sync_lock:
             if not name:
                 assert factory is not None
                 name = factory.factory_name()
             if self.is_empty(name=name):
                 if self.__time_between_eviction_runs > -1:
                     self.counter.add(name)
-                return self.__class_dict[name].creatInstantce()
+                return self.__class_dict[name].createInstance()
             pooled_object = self.__pooled_object_tree[name].pop()
             while not self.__class_dict[name].validate(pooled_object):
                 self.__clear_one_object(pooled_object, name=name)
                 if self.is_empty(name=name):
-                    pooled_object = self.__class_dict[name].creatInstantce()
+                    pooled_object = self.__class_dict[name].createInstance()
                 else:
                     pooled_object = self.__pooled_object_tree[name].pop()
             if self.__time_between_eviction_runs > -1:
                 self.counter.add(name)
             return pooled_object.update_brrow_time()
 
     def recycle(
```

### Comparing `pondpond-1.3.1/pond/pooled_object.py` & `pondpond-1.3.2/pond/pooled_object.py`

 * *Files identical despite different names*

### Comparing `pondpond-1.3.1/pond/pooled_object_factory.py` & `pondpond-1.3.2/pond/pooled_object_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class PooledObjectFactory(metaclass=abc.ABCMeta):
     def __init__(self, pooled_maxsize: int = 8, least_one: bool = False) -> None:
         self.pooled_maxsize = pooled_maxsize
         self.least_one = least_one
 
     @abc.abstractmethod
-    def creatInstantce(self) -> PooledObject:
+    def createInstance(self) -> PooledObject:
         pass
 
     @abc.abstractmethod
     def destroy(self, pooled_object: PooledObject) -> None:
         pass
 
     @abc.abstractmethod
```

### Comparing `pondpond-1.3.1/pond-stubs/pond_class.pyi` & `pondpond-1.3.2/pond-stubs/pond_class.pyi`

 * *Files identical despite different names*

### Comparing `pondpond-1.3.1/pond-stubs/pooled_object_factory.pyi` & `pondpond-1.3.2/pond-stubs/pooled_object_factory.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from _typeshed import Incomplete
 
 class PooledObjectFactory(metaclass=abc.ABCMeta):
     pooled_maxsize: Incomplete
     least_one: Incomplete
     def __init__(self, pooled_maxsize: int = ..., least_one: bool = ...) -> None: ...
     @abc.abstractmethod
-    def creatInstantce(self) -> PooledObject: ...
+    def createInstance(self) -> PooledObject: ...
     @abc.abstractmethod
     def destroy(self, pooled_object: PooledObject) -> None: ...
     @abc.abstractmethod
     def reset(self, pooled_object: PooledObject) -> PooledObject: ...
     @abc.abstractmethod
     def validate(self, pooled_object: PooledObject) -> bool: ...
     def factory_name(self) -> str: ...
```

### Comparing `pondpond-1.3.1/pyproject.toml` & `pondpond-1.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 dependencies = [
     "madoka>=0.7.1",
 ]
 description = "Pond is a high performance object-pooling library for Python."
 name = "pondpond"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "1.3.1"
+version = "1.3.2"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Blog = "https://qin.news"
 "Bug Tracker" = "https://github.com/t-baby/pond/issues"
```

### Comparing `pondpond-1.3.1/tests/draw.py` & `pondpond-1.3.2/tests/draw.py`

 * *Files identical despite different names*

### Comparing `pondpond-1.3.1/tests/test_aysnc_pond.py` & `pondpond-1.3.2/tests/test_aysnc_pond.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class Dog:
     name: str
     validate_result: bool = True
 
 
 class PooledDogFactory(PooledObjectFactory):
-    def creatInstantce(self) -> PooledObject:
+    def createInstance(self) -> PooledObject:
         dog = Dog()
         dog.name = "puppy"
         return PooledObject(dog)
 
     def destroy(self, pooled_object: PooledObject) -> None:
         del pooled_object
```

### Comparing `pondpond-1.3.1/tests/test_cprofile.py` & `pondpond-1.3.2/tests/test_cprofile.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class Dog:
     name: str
     validate_result: bool = True
 
 
 class PooledDogFactory(PooledObjectFactory):
-    def creatInstantce(self) -> PooledObject:
+    def createInstance(self) -> PooledObject:
         dog = Dog()
         dog.name = "puppy"
         return PooledObject(dog)
 
     def destroy(self, pooled_object: PooledObject) -> None:
         del pooled_object
 
@@ -39,8 +39,8 @@
 pond.register(factory)
 T1 = time.perf_counter()
 for i in range(100000):
     pooled_object: PooledObject = pond.borrow(factory)
     dog: Dog = pooled_object.use()
     pond.recycle(pooled_object, factory)
 T2 = time.perf_counter()
-print("程序运行时间:%s毫秒" % ((T2 - T1) * 1000))
+print("Run time: %s ms" % ((T2 - T1) * 1000))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pondpond-1.3.1/tests/test_pond.py` & `pondpond-1.3.2/tests/test_pond.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class Dog:
     name: str
     validate_result: bool = True
 
 
 class PooledDogFactory(PooledObjectFactory):
-    def creatInstantce(self) -> PooledObject:
+    def createInstance(self) -> PooledObject:
         dog = Dog()
         dog.name = "puppy"
         return PooledObject(dog)
 
     def destroy(self, pooled_object: PooledObject) -> None:
         del pooled_object
```

### Comparing `pondpond-1.3.1/PKG-INFO` & `pondpond-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pondpond
-Version: 1.3.1
+Version: 1.3.2
 Summary: Pond is a high performance object-pooling library for Python.
 Author-email: Andy Qin <dr.qin@protonmail.com>
 Requires-Python: >=3.8
 Project-URL: Blog, https://qin.news
 Project-URL: Bug Tracker, https://github.com/t-baby/pond/issues
 Project-URL: Homepage, https://github.com/t-baby/pond
 Description-Content-Type: text/markdown
@@ -52,15 +52,15 @@
 ```python
 class Dog:
     name: str
     validate_result:bool = True
 
 
 class PooledDogFactory(PooledObjectFactory):
-    def creatInstantce(self) -> PooledObject:
+    def createInstance(self) -> PooledObject:
         dog = Dog()
         dog.name = "puppy"
         return PooledObject(dog)
 
     def destroy(self, pooled_object: PooledObject):
         del pooled_object
```

