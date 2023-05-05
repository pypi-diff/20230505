# Comparing `tmp/api-console-solver-0.0.8.tar.gz` & `tmp/api-console-solver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\api-console-solver-0.0.8.tar", last modified: Sat Mar 11 20:27:14 2023, max compression
+gzip compressed data, was "dist\api-console-solver-0.0.9.tar", last modified: Fri Mar 17 13:20:39 2023, max compression
```

## Comparing `api-console-solver-0.0.8.tar` & `api-console-solver-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-11 20:27:14.481997 api-console-solver-0.0.8/
--rw-rw-rw-   0        0        0     3970 2023-03-11 20:27:14.480438 api-console-solver-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2602 2023-03-11 13:06:49.000000 api-console-solver-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-11 20:27:14.450158 api-console-solver-0.0.8/Solver/
--rw-rw-rw-   0        0        0        0 2022-06-23 22:06:41.000000 api-console-solver-0.0.8/Solver/__init__.py
--rw-rw-rw-   0        0        0    10531 2023-03-11 20:26:57.000000 api-console-solver-0.0.8/Solver/api_console.py
-drwxrwxrwx   0        0        0        0 2023-03-11 20:27:14.478694 api-console-solver-0.0.8/api_console_solver.egg-info/
--rw-rw-rw-   0        0        0     3970 2023-03-11 20:27:14.000000 api-console-solver-0.0.8/api_console_solver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-03-11 20:27:14.000000 api-console-solver-0.0.8/api_console_solver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-11 20:27:14.000000 api-console-solver-0.0.8/api_console_solver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-11 20:27:14.000000 api-console-solver-0.0.8/api_console_solver.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-11 20:27:14.000000 api-console-solver-0.0.8/api_console_solver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-11 20:27:14.481997 api-console-solver-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      500 2023-03-11 20:25:36.000000 api-console-solver-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-17 13:20:39.921599 api-console-solver-0.0.9/
+-rw-rw-rw-   0        0        0     3970 2023-03-17 13:20:39.918425 api-console-solver-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2602 2023-03-11 13:06:49.000000 api-console-solver-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-17 13:20:39.908712 api-console-solver-0.0.9/Solver/
+-rw-rw-rw-   0        0        0        0 2022-06-23 22:06:41.000000 api-console-solver-0.0.9/Solver/__init__.py
+-rw-rw-rw-   0        0        0    10523 2023-03-17 13:17:56.000000 api-console-solver-0.0.9/Solver/api_console.py
+drwxrwxrwx   0        0        0        0 2023-03-17 13:20:39.916758 api-console-solver-0.0.9/api_console_solver.egg-info/
+-rw-rw-rw-   0        0        0     3970 2023-03-17 13:20:39.000000 api-console-solver-0.0.9/api_console_solver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-03-17 13:20:39.000000 api-console-solver-0.0.9/api_console_solver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-17 13:20:39.000000 api-console-solver-0.0.9/api_console_solver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-03-17 13:20:39.000000 api-console-solver-0.0.9/api_console_solver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-03-17 13:20:39.000000 api-console-solver-0.0.9/api_console_solver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-17 13:20:39.922607 api-console-solver-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      500 2023-03-17 13:20:00.000000 api-console-solver-0.0.9/setup.py
```

### Comparing `api-console-solver-0.0.8/PKG-INFO` & `api-console-solver-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-console-solver
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrapper oficial da Plataforma Solver
 Home-page: UNKNOWN
 Author: Wesley Romualdo da Silva
 Author-email: romualdo@solvedigital.com.br
 License: MIT License
 Description: # Material de apoio
```

### Comparing `api-console-solver-0.0.8/README.md` & `api-console-solver-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `api-console-solver-0.0.8/Solver/api_console.py` & `api-console-solver-0.0.9/Solver/api_console.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
     def __init__(self, url =''):
         self.url = 'https://consoleapi-dsv.api.zello.services'
         if url != '':
             self.url = url
         self.headers = {'Authorization': 'Bearer ','Content-Type': 'application/json'}
 
-    def gera_token_acesso(self, config):
-        self.config = self.get_automacao_by_id_json(config['executor'])
+    def gera_token_acesso(self, executor):
+        self.config = self.get_automacao_by_id_json(executor)
         
         if 'detail' in self.config:
             return self.config['detail']
 
         self.nome_executor = self.config['tx_nome']
         self.config['tx_json'] = self.config['tx_json'].replace("'",'"')
         self.config = json.loads(self.config['tx_json'])
```

### Comparing `api-console-solver-0.0.8/api_console_solver.egg-info/PKG-INFO` & `api-console-solver-0.0.9/api_console_solver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api-console-solver
-Version: 0.0.8
+Version: 0.0.9
 Summary: Wrapper oficial da Plataforma Solver
 Home-page: UNKNOWN
 Author: Wesley Romualdo da Silva
 Author-email: romualdo@solvedigital.com.br
 License: MIT License
 Description: # Material de apoio
```

