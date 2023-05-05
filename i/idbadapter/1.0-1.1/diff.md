# Comparing `tmp/idbadapter-1.0.tar.gz` & `tmp/idbadapter-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.0.tar", last modified: Tue May  2 13:50:04 2023, max compression
+gzip compressed data, was "idbadapter-1.1.tar", last modified: Fri May  5 13:34:12 2023, max compression
```

## Comparing `idbadapter-1.0.tar` & `idbadapter-1.1.tar`

### file list

```diff
@@ -1,7 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 13:50:04.044939 idbadapter-1.0/
--rw-rw-rw-   0        0        0      720 2023-05-02 13:50:04.044939 idbadapter-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-02 13:50:04.044939 idbadapter-1.0/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-05-02 13:48:21.148563 idbadapter-1.0/idbadapter/__init__.py
--rw-rw-rw-   0        0        0     4545 2023-05-02 13:44:17.913622 idbadapter-1.0/idbadapter/schedule_loader.py
--rw-rw-rw-   0        0        0       38 2023-05-02 13:43:37.369920 idbadapter-1.0/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-05-02 13:50:02.665938 idbadapter-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:34:12.482477 idbadapter-1.1/
+-rw-rw-rw-   0        0        0    11558 2023-05-02 13:28:55.000000 idbadapter-1.1/LICENSE
+-rw-rw-rw-   0        0        0      695 2023-05-05 13:34:12.482477 idbadapter-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-05-05 13:33:15.000000 idbadapter-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 13:34:12.469478 idbadapter-1.1/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-05-02 13:48:21.000000 idbadapter-1.1/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0     5820 2023-05-05 13:07:31.000000 idbadapter-1.1/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:34:12.481480 idbadapter-1.1/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      695 2023-05-05 13:34:12.000000 idbadapter-1.1/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-05 13:34:12.000000 idbadapter-1.1/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 13:34:12.000000 idbadapter-1.1/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-05 13:34:12.000000 idbadapter-1.1/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-05 13:34:12.000000 idbadapter-1.1/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 13:34:12.484477 idbadapter-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-05-05 13:34:09.000000 idbadapter-1.1/setup.py
```

### Comparing `idbadapter-1.0/idbadapter/schedule_loader.py` & `idbadapter-1.1/idbadapter/schedule_loader.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             raise Exception("empty list of schedule ids")
         self.ceil_limit = ceil_limit
         self.objects = schedule_ids
         
         return self
         
     def from_works_or_resources(self, works_list: list[int], resource_list: list[int] = [], ceil_limit: int=1_000):
-        """method for getting schedukes pivots from list of works or resources ids
+        """method for getting schedules pivots from list of works or resources ids
 
         Args:
             works_list (list[int]): list of works ids
             resource_list (list, optional): list of resources ids. Defaults to [].
             ceil_limit (_type_, optional): limit of records in one dataframe. Defaults to 10_000.
         """
         if len(works_list) == 0:
@@ -42,14 +42,43 @@
         self.ceil_limit = ceil_limit
         self.works_list = works_list
         self.resource_list = resource_list
         self.objects = list({*self._get_objects_by_resource(), *self._get_objects_by_works()})
 
         return self
     
+    def from_names(self, works: list[str], resources: list[str] = [], ceil_limit: int = 1_000):
+        """method for getting schedules by works names list
+
+        Args:
+            work_name_list (list[str]): lists of basic works names 
+            ceil_limit (int, optional): limit of records in one dataframe. Defaults to 1_000.
+        """
+        if len(works) == 0:
+            raise Exception("Empty works list")
+        self.ceil_limit = ceil_limit
+        self.works_list = self._get_works_ids_by_names(works)
+        self.resource_list = self._get_resource_ids_by_names(resources)
+        
+        self.objects = list({*self._get_objects_by_resource(), *self._get_objects_by_works()})
+        
+        return self
+           
+    def _get_works_ids_by_names(self, work_name_list):
+        data = json.dumps(work_name_list)
+        response = self.session.post(urllib.parse.urljoin(self.url, "work/get_basic_works_ids"), data=data)
+
+        return response.json()
+    
+    def _get_resource_ids_by_names(self, resource_names_list):
+        data = json.dumps(resource_names_list)
+        response = self.session.post(urllib.parse.urljoin(self.url, "resource/get_basic_resouce_ids"), data=data)
+        
+        return response.json()
+    
     def _get_objects_by_resource(self):
         if len(self.resource_list) == 0:
             return []
         data = json.dumps(self.resource_list)
         response = self.session.post(urllib.parse.urljoin(self.url, "resource/schedule_ids"), data=data)
 
         return response.json()
@@ -96,15 +125,14 @@
         df = pd.DataFrame(resources)
         
         return df
     
     def __next__(self):
         try:
             works_df = self._select_works_from_db()
-
             if len(works_df) == self.ceil_limit:
                 self.start_date = works_df.date.max()
                 works_df = works_df[works_df.date != self.start_date]
                 res_df = self._select_resources_from_db(works_df["date"].min(), works_df["date"].max())    
             else:
                 res_df = self._select_resources_from_db(works_df["date"].min(), works_df["date"].max())  
                 self.index += 1
```

### Comparing `idbadapter-1.0/setup.py` & `idbadapter-1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
-version = '1.0'
+version = '1.1'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.0',
+      version='1.1',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```

