# Comparing `tmp/redis_elastic-0.3.4.tar.gz` & `tmp/redis_elastic-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_elastic-0.3.4.tar", last modified: Thu May  4 17:01:25 2023, max compression
+gzip compressed data, was "redis_elastic-1.0.0.tar", last modified: Thu May  4 22:58:52 2023, max compression
```

## Comparing `redis_elastic-0.3.4.tar` & `redis_elastic-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 17:01:25.617388 redis_elastic-0.3.4/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3224 2023-05-04 17:01:25.617388 redis_elastic-0.3.4/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2801 2023-05-04 16:55:29.000000 redis_elastic-0.3.4/README.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 17:01:25.617388 redis_elastic-0.3.4/Warehouse/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-02 22:29:25.000000 redis_elastic-0.3.4/Warehouse/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4774 2023-05-02 22:59:48.000000 redis_elastic-0.3.4/Warehouse/redis_elastic.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 17:01:25.617388 redis_elastic-0.3.4/redis_elastic.egg-info/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3224 2023-05-04 17:01:25.000000 redis_elastic-0.3.4/redis_elastic.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      251 2023-05-04 17:01:25.000000 redis_elastic-0.3.4/redis_elastic.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-04 17:01:25.000000 redis_elastic-0.3.4/redis_elastic.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       71 2023-05-04 17:01:25.000000 redis_elastic-0.3.4/redis_elastic.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       10 2023-05-04 17:01:25.000000 redis_elastic-0.3.4/redis_elastic.egg-info/top_level.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-04 17:01:25.617388 redis_elastic-0.3.4/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      865 2023-05-04 17:00:44.000000 redis_elastic-0.3.4/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 22:58:52.383008 redis_elastic-1.0.0/
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 22:58:52.383008 redis_elastic-1.0.0/Develop/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-04 19:00:06.000000 redis_elastic-1.0.0/Develop/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2682 2023-04-27 18:32:13.000000 redis_elastic-1.0.0/Develop/extract.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1323 2023-05-04 22:53:19.000000 redis_elastic-1.0.0/Develop/tools.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3120 2023-05-04 22:58:52.383008 redis_elastic-1.0.0/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2697 2023-05-04 22:51:13.000000 redis_elastic-1.0.0/README.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 22:58:52.383008 redis_elastic-1.0.0/Warehouse/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2023-05-02 22:29:25.000000 redis_elastic-1.0.0/Warehouse/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4988 2023-05-04 22:48:21.000000 redis_elastic-1.0.0/Warehouse/redis_elastic.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-05-04 22:58:52.383008 redis_elastic-1.0.0/redis_elastic.egg-info/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3120 2023-05-04 22:58:52.000000 redis_elastic-1.0.0/redis_elastic.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      307 2023-05-04 22:58:52.000000 redis_elastic-1.0.0/redis_elastic.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-05-04 22:58:52.000000 redis_elastic-1.0.0/redis_elastic.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       71 2023-05-04 22:58:52.000000 redis_elastic-1.0.0/redis_elastic.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       18 2023-05-04 22:58:52.000000 redis_elastic-1.0.0/redis_elastic.egg-info/top_level.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-05-04 22:58:52.387008 redis_elastic-1.0.0/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      876 2023-05-04 22:54:12.000000 redis_elastic-1.0.0/setup.py
```

### Comparing `redis_elastic-0.3.4/PKG-INFO` & `redis_elastic-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: redis_elastic
-Version: 0.3.4
+Version: 1.0.0
 Summary: Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch
 Home-page: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE
 Download-URL: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE/tarball/01
 Author: Carlos Garcia Garcia
 Author-email: carlos.garcia1.gr1@icloud.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # Redis ElasticSearch
 
 ![](https://i.imgur.com/sEkqRr3.png)
 
-version 0.3.3 (Stable release)
+version 1.0.0 (Stable release)
 
 ## Summary
 
 This Python code uses various libraries to connect to and manipulate data in different databases. Specifically, it imports the ast, psycopg2, functools, redis, threading, time, json, and pandas libraries, as well as the Elasticsearch and bulk modules of the elasticsearch library.
 
 The Settings_redis_elastic class uses the connection parameters to a Redis server and an Elasticsearch server to create methods that allow you to get data from a PostgreSQL database and send it to an Elasticsearch index through Redis.
 
@@ -49,15 +49,15 @@
 }
 
 list_fields = ['id', 'name', 'code']
 
 query = """Select rp.id,rp.name,rp.code from res_partner rp"""
 
 my_object = Settings_redis_elastic("localhost", "6379", "http://localhost:9200")
-my_object.fusion(query, "_test", "test", 10, 20, postgres, list_fields)
+my_object.fusion(query, "_test", "test", 10, 20, postgres)
 ``` 
 
 ## Documentation
 
 1. The first step is to create an object, and connect redis and elasticsearch
 
 ```python
@@ -75,20 +75,18 @@
  
  - time_redis : The time the SQL query is saved to Redis
  
  - time_elastic : It is the timeout from Redis to elasticsearch,
  **Recommendation:** It should be bigger than <<time_redis>>
  
  - database : It is the connection to the database, it must be a dictionary
- 
- - fields : **Important**, Field names must be the same as the SQL query headers
 
 
 Position in the method **fusion**
 
 ```python
-my_object.fusion(query, redis_name , elasticsearch_name, time_redis, time_elastic, database, fields)
+my_object.fusion(query, redis_name , elasticsearch_name, time_redis, time_elastic, database)
 ```
```

### Comparing `redis_elastic-0.3.4/README.md` & `redis_elastic-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Redis ElasticSearch
 
 ![](https://i.imgur.com/sEkqRr3.png)
 
-version 0.3.3 (Stable release)
+version 1.0.0 (Stable release)
 
 ## Summary
 
 This Python code uses various libraries to connect to and manipulate data in different databases. Specifically, it imports the ast, psycopg2, functools, redis, threading, time, json, and pandas libraries, as well as the Elasticsearch and bulk modules of the elasticsearch library.
 
 The Settings_redis_elastic class uses the connection parameters to a Redis server and an Elasticsearch server to create methods that allow you to get data from a PostgreSQL database and send it to an Elasticsearch index through Redis.
 
@@ -38,15 +38,15 @@
 }
 
 list_fields = ['id', 'name', 'code']
 
 query = """Select rp.id,rp.name,rp.code from res_partner rp"""
 
 my_object = Settings_redis_elastic("localhost", "6379", "http://localhost:9200")
-my_object.fusion(query, "_test", "test", 10, 20, postgres, list_fields)
+my_object.fusion(query, "_test", "test", 10, 20, postgres)
 ``` 
 
 ## Documentation
 
 1. The first step is to create an object, and connect redis and elasticsearch
 
 ```python
@@ -64,20 +64,18 @@
  
  - time_redis : The time the SQL query is saved to Redis
  
  - time_elastic : It is the timeout from Redis to elasticsearch,
  **Recommendation:** It should be bigger than <<time_redis>>
  
  - database : It is the connection to the database, it must be a dictionary
- 
- - fields : **Important**, Field names must be the same as the SQL query headers
 
 
 Position in the method **fusion**
 
 ```python
-my_object.fusion(query, redis_name , elasticsearch_name, time_redis, time_elastic, database, fields)
+my_object.fusion(query, redis_name , elasticsearch_name, time_redis, time_elastic, database)
 ```
```

### Comparing `redis_elastic-0.3.4/Warehouse/redis_elastic.py` & `redis_elastic-1.0.0/Warehouse/redis_elastic.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 class Settings_redis_elastic:
     def __init__(self, ip_redis, port_redis, url_elasticsearch):
         self.ip_redis = ip_redis
         self.port_redis = port_redis
         self.url_elasticsearch = url_elasticsearch
 
-    def fusion(self, query, redis_name, elasticsearch_name, time_redis, time_elastic, database, source):
+    def fusion(self, query, redis_name, elasticsearch_name, time_redis, time_elastic, database):
         # Creamos un cliente de Redis
         redis_client = redis.Redis(host=self.ip_redis, port=self.port_redis)
 
         # Decorador para cachear resultados de la función en Redis
         def cache_function_results(function):
             @functools.wraps(function)
             def wrapper(*args, **kwargs):
                 # Generamos la clave del caché
                 cache_key = f"{function.__name__}{redis_name}:{args}:{kwargs.items()}"
-                print(cache_key)
+                print("Key in Redis {}".format(cache_key))
                 # Intentamos obtener el resultado del caché
                 cached_result = redis_client.get(cache_key)
 
                 # Si existe el resultado en caché, lo devolvemos
                 if cached_result is not None:
                     return pd.read_json(cached_result)
 
@@ -65,15 +65,15 @@
         @cache_function_results
         def cached_query_dates():
             return query_dates()
 
         def update_cache():
             while True:
                 # Obtener la versión actual del caché
-                cached_version = redis_client.get(f"query_version{redis_name}")
+                cached_version = redis_client.get(f"query_version{redis_name}").decode("utf8")
 
                 # Obtener la versión actual de la consulta en la base de datos
                 db_version = str(query_dates().values)
 
                 # Si la versión en la base de datos es diferente a la versión en caché,
                 # actualizar el caché y la versión en caché
                 if cached_version != db_version:
@@ -101,20 +101,23 @@
                 df = pd.DataFrame.from_dict(data)
 
             return df
 
         def elastic_indexation():
             client = Elasticsearch(self.url_elasticsearch)
 
+            # Obtiene la variable de columnas de la función query dates
+            get_list_columns = query_dates().columns.tolist()
+            print(get_list_columns)
             docs = []
             for i, row in redis_dates().iterrows():
                 doc = {
                     '_index': elasticsearch_name,
                     '_id': i,
-                    '_source': {field: row[field] for field in source}
+                    '_source': {field: row[field] for field in get_list_columns}
                 }
                 docs.append(doc)
 
             # Indexar documentos en Elasticsearch
             bulk(client, docs)
             client.close()
```

### Comparing `redis_elastic-0.3.4/redis_elastic.egg-info/PKG-INFO` & `redis_elastic-1.0.0/redis_elastic.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: redis-elastic
-Version: 0.3.4
+Version: 1.0.0
 Summary: Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch
 Home-page: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE
 Download-URL: https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE/tarball/01
 Author: Carlos Garcia Garcia
 Author-email: carlos.garcia1.gr1@icloud.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # Redis ElasticSearch
 
 ![](https://i.imgur.com/sEkqRr3.png)
 
-version 0.3.3 (Stable release)
+version 1.0.0 (Stable release)
 
 ## Summary
 
 This Python code uses various libraries to connect to and manipulate data in different databases. Specifically, it imports the ast, psycopg2, functools, redis, threading, time, json, and pandas libraries, as well as the Elasticsearch and bulk modules of the elasticsearch library.
 
 The Settings_redis_elastic class uses the connection parameters to a Redis server and an Elasticsearch server to create methods that allow you to get data from a PostgreSQL database and send it to an Elasticsearch index through Redis.
 
@@ -49,15 +49,15 @@
 }
 
 list_fields = ['id', 'name', 'code']
 
 query = """Select rp.id,rp.name,rp.code from res_partner rp"""
 
 my_object = Settings_redis_elastic("localhost", "6379", "http://localhost:9200")
-my_object.fusion(query, "_test", "test", 10, 20, postgres, list_fields)
+my_object.fusion(query, "_test", "test", 10, 20, postgres)
 ``` 
 
 ## Documentation
 
 1. The first step is to create an object, and connect redis and elasticsearch
 
 ```python
@@ -75,20 +75,18 @@
  
  - time_redis : The time the SQL query is saved to Redis
  
  - time_elastic : It is the timeout from Redis to elasticsearch,
  **Recommendation:** It should be bigger than <<time_redis>>
  
  - database : It is the connection to the database, it must be a dictionary
- 
- - fields : **Important**, Field names must be the same as the SQL query headers
 
 
 Position in the method **fusion**
 
 ```python
-my_object.fusion(query, redis_name , elasticsearch_name, time_redis, time_elastic, database, fields)
+my_object.fusion(query, redis_name , elasticsearch_name, time_redis, time_elastic, database)
 ```
```

### Comparing `redis_elastic-0.3.4/setup.py` & `redis_elastic-1.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 readme = open("./README.md", "r")
 
 setup(
     name="redis_elastic",
-    version="0.3.4",
+    version="1.0.0",
     description="Crea una conexión de una base de datos postgres lo gurda en cache y en elasticsearch",
     install_requires=[
         "setuptools",
         "psycopg2",
         "psycopg2-binary",
         "redis",
         "elasticsearch==7.13.4",
@@ -19,10 +19,10 @@
     author="Carlos Garcia Garcia",
     author_email="carlos.garcia1.gr1@icloud.com",
     # REPOSITORIO GIT
     url="https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE",
     download_url='https://github.com/CarlosRaloy/ETL_ELASTIC_REDIS_MORE/tarball/01',
     kwargs=['redis', 'elasticsearch', 'warehouse'],
     license='MIT',
-    packages=["Warehouse"],
+    packages=["Warehouse", "Develop"],
     include_package_data=True
 )
```

