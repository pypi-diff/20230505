# Comparing `tmp/naver-db-0.0.5.post4.tar.gz` & `tmp/naver-db-0.0.5.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naver-db-0.0.5.post4.tar", last modified: Wed Aug 31 22:56:04 2022, max compression
+gzip compressed data, was "naver-db-0.0.5.post5.tar", last modified: Fri May  5 21:22:12 2023, max compression
```

## Comparing `naver-db-0.0.5.post4.tar` & `naver-db-0.0.5.post5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-08-31 22:56:04.535959 naver-db-0.0.5.post4/
--rw-rw-rw-   0        0        0      451 2022-08-31 22:56:04.535959 naver-db-0.0.5.post4/PKG-INFO
--rw-rw-rw-   0        0        0        6 2021-09-28 19:46:20.000000 naver-db-0.0.5.post4/README.md
-drwxrwxrwx   0        0        0        0 2022-08-31 22:56:04.517415 naver-db-0.0.5.post4/naver_db/
--rw-rw-rw-   0        0        0      554 2022-07-20 20:10:32.000000 naver-db-0.0.5.post4/naver_db/__init__.py
--rw-rw-rw-   0        0        0    15077 2022-08-31 22:54:33.000000 naver-db-0.0.5.post4/naver_db/persistence.py
-drwxrwxrwx   0        0        0        0 2022-08-31 22:56:04.525957 naver-db-0.0.5.post4/naver_db.egg-info/
--rw-rw-rw-   0        0        0      451 2022-08-31 22:56:04.000000 naver-db-0.0.5.post4/naver_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2022-08-31 22:56:04.000000 naver-db-0.0.5.post4/naver_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-31 22:56:04.000000 naver-db-0.0.5.post4/naver_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2022-08-31 22:56:04.000000 naver-db-0.0.5.post4/naver_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-08-31 22:56:04.000000 naver-db-0.0.5.post4/naver_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-31 22:56:04.535959 naver-db-0.0.5.post4/setup.cfg
--rw-rw-rw-   0        0        0      768 2022-08-31 22:54:57.000000 naver-db-0.0.5.post4/setup.py
-drwxrwxrwx   0        0        0        0 2022-08-31 22:56:04.534957 naver-db-0.0.5.post4/test/
--rw-rw-rw-   0        0        0      194 2021-10-18 15:36:17.000000 naver-db-0.0.5.post4/test/__init__.py
--rw-rw-rw-   0        0        0      139 2021-10-19 14:00:31.000000 naver-db-0.0.5.post4/test/naver_getprops.py
--rw-rw-rw-   0        0        0      263 2021-10-19 15:13:38.000000 naver-db-0.0.5.post4/test/naver_nextval.py
--rw-rw-rw-   0        0        0      138 2021-10-19 14:00:03.000000 naver-db-0.0.5.post4/test/naver_param.py
--rw-rw-rw-   0        0        0      178 2021-10-19 14:02:35.000000 naver-db-0.0.5.post4/test/naver_query.py
--rw-rw-rw-   0        0        0      145 2021-10-19 15:17:09.000000 naver-db-0.0.5.post4/test/naver_userpermission.py
--rw-rw-rw-   0        0        0      487 2021-10-19 15:36:07.000000 naver-db-0.0.5.post4/test/naver_write.py
--rw-rw-rw-   0        0        0      381 2021-10-19 15:37:53.000000 naver-db-0.0.5.post4/test/naver_writelog.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:22:12.210700 naver-db-0.0.5.post5/
+-rw-rw-rw-   0        0        0      412 2023-05-05 21:22:12.210700 naver-db-0.0.5.post5/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 21:22:12.179930 naver-db-0.0.5.post5/naver_db/
+-rw-rw-rw-   0        0        0      554 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/naver_db/__init__.py
+-rw-rw-rw-   0        0        0    15142 2023-05-05 21:18:26.000000 naver-db-0.0.5.post5/naver_db/persistence.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:22:12.194904 naver-db-0.0.5.post5/naver_db.egg-info/
+-rw-rw-rw-   0        0        0      412 2023-05-05 21:22:12.000000 naver-db-0.0.5.post5/naver_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-05-05 21:22:12.000000 naver-db-0.0.5.post5/naver_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 21:22:12.000000 naver-db-0.0.5.post5/naver_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-05 21:22:12.000000 naver-db-0.0.5.post5/naver_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-05 21:22:12.000000 naver-db-0.0.5.post5/naver_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 21:22:12.210700 naver-db-0.0.5.post5/setup.cfg
+-rw-rw-rw-   0        0        0      768 2023-05-05 21:18:58.000000 naver-db-0.0.5.post5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:22:12.210700 naver-db-0.0.5.post5/test/
+-rw-rw-rw-   0        0        0      194 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/__init__.py
+-rw-rw-rw-   0        0        0      139 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/naver_getprops.py
+-rw-rw-rw-   0        0        0      263 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/naver_nextval.py
+-rw-rw-rw-   0        0        0      138 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/naver_param.py
+-rw-rw-rw-   0        0        0      178 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/naver_query.py
+-rw-rw-rw-   0        0        0      145 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/naver_userpermission.py
+-rw-rw-rw-   0        0        0      487 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/naver_write.py
+-rw-rw-rw-   0        0        0      381 2023-04-18 00:04:52.000000 naver-db-0.0.5.post5/test/naver_writelog.py
```

### Comparing `naver-db-0.0.5.post4/naver_db/__init__.py` & `naver-db-0.0.5.post5/naver_db/__init__.py`

 * *Files identical despite different names*

### Comparing `naver-db-0.0.5.post4/naver_db/persistence.py` & `naver-db-0.0.5.post5/naver_db/persistence.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         self.config = config
         self.mySession = [1, 1]
         self.redis = redis.Redis(
             host=config.core.myVariables.get("REDIS_HOST"),
             port=config.core.myVariables.get("REDIS_PORT"))
         if(config.core.myVariables.get("REDIS_PASSWORD")is not None):
             self.redis = redis.Redis(
+            username=config.core.myVariables.get("REDIS_USER"),
             host=config.core.myVariables.get("REDIS_HOST"),
             port=config.core.myVariables.get("REDIS_PORT"),
             password=config.core.myVariables.get("REDIS_PASSWORD")
             )
 
     def _sql(self, rawSql):
         """Método para ejecutar una consulta SQL
```

### Comparing `naver-db-0.0.5.post4/setup.py` & `naver-db-0.0.5.post5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='naver-db',
-    version='0.0.5-4',
+    version='0.0.5-5',
     packages=setuptools.find_packages(),
     author="Jose Cuevas",
     author_email="jose.cuevas.cv@gmail.com",
     description="A DB Persistence Ancestor Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jacr6/naver-db",
```

