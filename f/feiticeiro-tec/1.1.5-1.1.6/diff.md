# Comparing `tmp/feiticeiro_tec-1.1.5.tar.gz` & `tmp/feiticeiro_tec-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feiticeiro_tec-1.1.5.tar", last modified: Mon May  1 03:33:20 2023, max compression
+gzip compressed data, was "feiticeiro_tec-1.1.6.tar", last modified: Fri May  5 05:55:51 2023, max compression
```

## Comparing `feiticeiro_tec-1.1.5.tar` & `feiticeiro_tec-1.1.6.tar`

### file list

```diff
@@ -1,37 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:33:20.338828 feiticeiro_tec-1.1.5/
--rw-r--r--   0 root         (0) root         (0)     3699 2023-05-01 03:33:20.338828 feiticeiro_tec-1.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3332 2023-04-29 06:54:41.000000 feiticeiro_tec-1.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:33:20.338828 feiticeiro_tec-1.1.5/feiticeiro_tec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 03:10:34.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-04-29 05:32:12.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:33:20.338828 feiticeiro_tec-1.1.5/feiticeiro_tec/api/
--rw-r--r--   0 root         (0) root         (0)      223 2023-05-01 03:20:40.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:33:20.338828 feiticeiro_tec-1.1.5/feiticeiro_tec/api/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 01:50:18.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/api/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2525 2023-05-01 02:41:14.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/api/utils/forms.py
--rw-r--r--   0 root         (0) root         (0)     2980 2023-05-01 03:04:05.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/api/utils/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:33:20.338828 feiticeiro_tec-1.1.5/feiticeiro_tec/api/v1/
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-01 02:27:59.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/api/v1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:33:20.338828 feiticeiro_tec-1.1.5/feiticeiro_tec/api/v1/usuario/
--rw-r--r--   0 root         (0) root         (0)      789 2023-05-01 03:32:16.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/api/v1/usuario/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:33:20.338828 feiticeiro_tec-1.1.5/feiticeiro_tec/create/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 03:44:01.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/create/__init__.py
--rw-r--r--   0 root         (0) root         (0)      324 2023-04-29 04:38:50.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/create/app.py
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-29 05:30:31.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/create/env.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-04-29 04:07:25.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/create/model.py
--rw-r--r--   0 root         (0) root         (0)     1049 2023-04-29 04:21:28.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/create/namespace.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-05-01 03:11:51.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/create/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:33:20.338828 feiticeiro_tec-1.1.5/feiticeiro_tec/database/
--rw-r--r--   0 root         (0) root         (0)      323 2023-04-29 04:46:18.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/database/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:33:20.338828 feiticeiro_tec-1.1.5/feiticeiro_tec/database/models/
--rw-r--r--   0 root         (0) root         (0)       51 2023-05-01 03:18:28.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/database/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-05-01 03:18:46.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/database/models/base.py
--rw-r--r--   0 root         (0) root         (0)      612 2023-05-01 03:16:32.000000 feiticeiro_tec-1.1.5/feiticeiro_tec/database/models/usuario.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-01 03:33:20.338828 feiticeiro_tec-1.1.5/feiticeiro_tec.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3699 2023-05-01 03:33:20.000000 feiticeiro_tec-1.1.5/feiticeiro_tec.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      829 2023-05-01 03:33:20.000000 feiticeiro_tec-1.1.5/feiticeiro_tec.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-01 03:33:20.000000 feiticeiro_tec-1.1.5/feiticeiro_tec.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-01 03:33:20.000000 feiticeiro_tec-1.1.5/feiticeiro_tec.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      249 2023-05-01 03:33:20.000000 feiticeiro_tec-1.1.5/feiticeiro_tec.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-01 03:33:20.338828 feiticeiro_tec-1.1.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1063 2023-05-01 03:32:38.000000 feiticeiro_tec-1.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:55:51.660192 feiticeiro_tec-1.1.6/
+-rw-r--r--   0 root         (0) root         (0)     4401 2023-05-05 05:55:51.660192 feiticeiro_tec-1.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4034 2023-05-05 05:53:21.000000 feiticeiro_tec-1.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:55:51.656192 feiticeiro_tec-1.1.6/feiticeiro_tec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 03:10:34.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-04-29 05:32:12.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:55:51.656192 feiticeiro_tec-1.1.6/feiticeiro_tec/api/
+-rw-r--r--   0 root         (0) root         (0)      223 2023-05-01 03:59:17.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:55:51.656192 feiticeiro_tec-1.1.6/feiticeiro_tec/api/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 03:33:54.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/api/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3266 2023-05-05 05:53:21.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/api/utils/forms.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2023-05-05 05:53:21.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/api/utils/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:55:51.656192 feiticeiro_tec-1.1.6/feiticeiro_tec/api/v1/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-05 05:53:21.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/api/v1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:55:51.656192 feiticeiro_tec-1.1.6/feiticeiro_tec/api/v1/permissions/
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-05-05 05:53:21.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/api/v1/permissions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      275 2023-05-05 05:53:21.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/api/v1/permissions/form.py
+-rw-r--r--   0 root         (0) root         (0)      172 2023-05-05 05:53:21.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/api/v1/permissions/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:55:51.656192 feiticeiro_tec-1.1.6/feiticeiro_tec/api/v1/usuarios/
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-05-05 05:53:21.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/api/v1/usuarios/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      293 2023-05-05 05:53:21.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/api/v1/usuarios/forms.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-05-05 05:53:21.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/api/v1/usuarios/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:55:51.660192 feiticeiro_tec-1.1.6/feiticeiro_tec/create/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 03:44:01.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/create/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      324 2023-04-29 04:38:50.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/create/app.py
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-29 05:30:31.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/create/env.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-04-29 04:07:25.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/create/model.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-04-29 04:21:28.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/create/namespace.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-05-05 05:53:21.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/create/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:55:51.660192 feiticeiro_tec-1.1.6/feiticeiro_tec/database/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-04-29 04:46:18.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/database/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:55:51.660192 feiticeiro_tec-1.1.6/feiticeiro_tec/database/models/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-05-05 05:53:21.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/database/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-05-05 05:53:21.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/database/models/base.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2023-05-05 05:53:21.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/database/models/permission.py
+-rw-r--r--   0 root         (0) root         (0)      612 2023-05-05 05:08:36.000000 feiticeiro_tec-1.1.6/feiticeiro_tec/database/models/usuario.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:55:51.656192 feiticeiro_tec-1.1.6/feiticeiro_tec.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4401 2023-05-05 05:55:51.000000 feiticeiro_tec-1.1.6/feiticeiro_tec.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-05-05 05:55:51.000000 feiticeiro_tec-1.1.6/feiticeiro_tec.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 05:55:51.000000 feiticeiro_tec-1.1.6/feiticeiro_tec.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-05 05:55:51.000000 feiticeiro_tec-1.1.6/feiticeiro_tec.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      284 2023-05-05 05:55:51.000000 feiticeiro_tec-1.1.6/feiticeiro_tec.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 05:55:51.660192 feiticeiro_tec-1.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-05 05:55:46.000000 feiticeiro_tec-1.1.6/setup.py
```

### Comparing `feiticeiro_tec-1.1.5/PKG-INFO` & `feiticeiro_tec-1.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feiticeiro_tec
-Version: 1.1.5
+Version: 1.1.6
 Summary: Extenção flask para aumento de agilidade no processo de criação de projeto.
 Home-page: https://github.com/feiticeiro-tec/feiticeiro-tec
 Author: Silvio Henrique Cruz Da Silva
 Author-email: silviohenriquecruzdasilva@gmail.com
 License: BSD3
 Keywords: Pacote
 Description-Content-Type: text/markdown
@@ -56,43 +56,71 @@
 ```
 server
 ├── __init__.py
 ├── api
 │   ├── __init__.py
 │   └── v1
 │       ├── __init__.py
-│       └── usuario
-│           └── __init__.py
+|       ├── permissions
+|       |   ├── __init__.py
+|       |   ├── forms.py
+|       |   └── serializers.py
+|       |
+│       └── usuarios
+│           ├── __init__.py
+|           ├── forms.py
+|           └── serializers.py
+|
 └── database
     ├── __init__.py
     └── models
         ├── __init__.py
+        ├── usuario.py
+        ├── permission.py
         └── base.py
 ```
+> Criando permissoes de rotas
+```bash
+flask create_permissions
+```
+> Esse comando deve ser executado toda vez que ouver uma alteracao nas rotas
+
+
 > Criando um novo endpoint/namespace
 ```bash
 python -m feiticeiro_tec create_namespace
 Qual a Versão? v1
-Qual o Nome Do NameSpace? empresa
+Qual o Nome Do NameSpace? empresas
 Deseja Criar o Model? (S/n) [enter]
 Qual o Nome Do Model? empresa
 ```
 ```
 server
 ├── __init__.py
 ├── api
 │   ├── __init__.py
 │   └── v1
 │       ├── __init__.py
-│       ├── empresa
-│       │   └── __init__.py
-│       └── usuario
-│           └── __init__.py
+|       ├── permissions
+│       |   ├── __init__.py
+|       |   ├── forms.py
+|       |   └── serializers.py
+|       |
+│       ├── usuarios
+│       |   ├── __init__.py
+|       |   ├── forms.py
+|       |   └── serializers.py
+|       |
+|       └── empresas
+|           └── __init__.py
+|
 └── database
     ├── __init__.py
     └── models
         ├── __init__.py
+        ├── usuario.py
+        ├── permission.py
         ├── base.py
         └── empresa.py
 ```
 
 Pronto agora é so fazer as importações e começar a codar.
```

### Comparing `feiticeiro_tec-1.1.5/README.md` & `feiticeiro_tec-1.1.6/feiticeiro_tec.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: feiticeiro-tec
+Version: 1.1.6
+Summary: Extenção flask para aumento de agilidade no processo de criação de projeto.
+Home-page: https://github.com/feiticeiro-tec/feiticeiro-tec
+Author: Silvio Henrique Cruz Da Silva
+Author-email: silviohenriquecruzdasilva@gmail.com
+License: BSD3
+Keywords: Pacote
+Description-Content-Type: text/markdown
+
 # Ola meu nome é Silvio Henrique
 
 Boas-vindas ao meu mundo, no meu repositório principal,
 esse o repositório do meu módulo de gerador passivo Flask,
 o objetivo é automatizar alguns processos, e gerir melhor os meus projetos
 como, por exemplo, um padrão de arquitetura, que seja fácil de implementar
 novos recursos sem muitos esforços.
@@ -45,43 +56,71 @@
 ```
 server
 ├── __init__.py
 ├── api
 │   ├── __init__.py
 │   └── v1
 │       ├── __init__.py
-│       └── usuario
-│           └── __init__.py
+|       ├── permissions
+|       |   ├── __init__.py
+|       |   ├── forms.py
+|       |   └── serializers.py
+|       |
+│       └── usuarios
+│           ├── __init__.py
+|           ├── forms.py
+|           └── serializers.py
+|
 └── database
     ├── __init__.py
     └── models
         ├── __init__.py
+        ├── usuario.py
+        ├── permission.py
         └── base.py
 ```
+> Criando permissoes de rotas
+```bash
+flask create_permissions
+```
+> Esse comando deve ser executado toda vez que ouver uma alteracao nas rotas
+
+
 > Criando um novo endpoint/namespace
 ```bash
 python -m feiticeiro_tec create_namespace
 Qual a Versão? v1
-Qual o Nome Do NameSpace? empresa
+Qual o Nome Do NameSpace? empresas
 Deseja Criar o Model? (S/n) [enter]
 Qual o Nome Do Model? empresa
 ```
 ```
 server
 ├── __init__.py
 ├── api
 │   ├── __init__.py
 │   └── v1
 │       ├── __init__.py
-│       ├── empresa
-│       │   └── __init__.py
-│       └── usuario
-│           └── __init__.py
+|       ├── permissions
+│       |   ├── __init__.py
+|       |   ├── forms.py
+|       |   └── serializers.py
+|       |
+│       ├── usuarios
+│       |   ├── __init__.py
+|       |   ├── forms.py
+|       |   └── serializers.py
+|       |
+|       └── empresas
+|           └── __init__.py
+|
 └── database
     ├── __init__.py
     └── models
         ├── __init__.py
+        ├── usuario.py
+        ├── permission.py
         ├── base.py
         └── empresa.py
 ```
 
 Pronto agora é so fazer as importações e começar a codar.
```

### Comparing `feiticeiro_tec-1.1.5/feiticeiro_tec/__main__.py` & `feiticeiro_tec-1.1.6/feiticeiro_tec/__main__.py`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.1.5/feiticeiro_tec/api/utils/forms.py` & `feiticeiro_tec-1.1.6/feiticeiro_tec/api/utils/forms.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from flask_restx import ValidationError
 from validate_docbr import CPF, CNPJ
 import re
 
 
 def number_required(value):
-    if not re.match(r'^[0-9]+', value):
+    if not re.search(r'[0-9]', value):
         raise ValidationError('Conter um numero é obrigatório')
     return value
 
 
 def lower_case_required(value):
-    if not re.match(r'^[a-z]+', value):
+    if not re.search(r'[a-z]', value):
         raise ValidationError('Conter uma letra minuscula é obrigatório')
     return value
 
 
 def upper_case_required(value):
-    if not re.match(r'^[A-Z]+', value):
+    if not re.search(r'[A-Z]', value):
         raise ValidationError('Conter uma letra maiuscula é obrigatório')
     return value
 
 
 def special_character_required(value):
-    if not re.match(r'^[!@#$%&*()_+=-]+', value):
+    if not re.search(r'[!@#$%&*()_+=-]', value):
         raise ValidationError('Conter um caracter especial é obrigatório')
     return value
 
 
 def length_required(value):
     if len(value) < 8:
         raise ValidationError('Conter no minimo 8 caracteres é obrigatório')
@@ -95,7 +95,36 @@
 
 def unique_fields_validate(field, query, field_name):
     def inner(value):
         if query.filter(field == value).first():
             raise ValidationError(f'{field_name} já cadastrado')
         return value
     return inner
+
+
+def password_validate(value):
+    number_required(value)
+    lower_case_required(value)
+    upper_case_required(value)
+    special_character_required(value)
+    length_required(value)
+    return value
+
+
+def boolean_validate(value):
+    error = ValidationError(
+        'Valor deve ser [True,False,"true", "false", 1, 0,"1", "0"]')
+    if isinstance(value, bool):
+        return value
+
+    elif isinstance(value, str):
+        value = value.lower()
+        if value not in ('true', 'false', '1', '0'):
+            raise error
+        return True if value == 'true' or value == '1' else False
+
+    elif isinstance(value, int):
+        if value not in (1, 0):
+            raise error
+        return True if value == 1 else False
+
+    raise error
```

### Comparing `feiticeiro_tec-1.1.5/feiticeiro_tec/api/utils/serializers.py` & `feiticeiro_tec-1.1.6/feiticeiro_tec/api/utils/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     'update_time': fields.DateTime(
         required=True,
         description='Data de atualização do registro',),
     'is_delete': fields.Boolean(
         required=True,
         description='Se o registro foi deletado ou não',
     ),
-    'is_ativo': fields.Boolean(
+    'is_active': fields.Boolean(
         required=True,
         description='Se o registro está ativo ou não',
     )
 }
 
 base_endereco_serializer = {
     'endereco': fields.String(
@@ -114,7 +114,13 @@
     )
 }
 
 base_empresa_plus_serializer = {
     **base_empresa_serializer,
     **base_endereco_serializer
 }
+
+base_permission_serializer = {
+    **base_serializer,
+    'endpoint': fields.String,
+    'method': fields.String,
+}
```

### Comparing `feiticeiro_tec-1.1.5/feiticeiro_tec/api/v1/usuario/__init__.py` & `feiticeiro_tec-1.1.6/feiticeiro_tec/api/v1/usuarios/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 from flask_restx import Resource
 from server.api import api
 from server.database.models import Usuario
+from .forms import usuario_form
+from .serializers import usuario_serializer
 
 np_usuario = api.namespace(
-    'usuario', description='Operações relacionadas a usuários')
+    'usuarios',
+    description='Operações relacionadas a usuários',
+    path='/v1/usuarios'
+)
 
 
 class UsuarioResource(Resource):
+
+    @np_usuario.expect(usuario_form)
+    @np_usuario.marshal_with(usuario_serializer, code=201)
     def post(self):
+        data = usuario_form.parse_args()
         user = Usuario()
-        user.insert_cadastro()
+        user.insert_cadastro(**data)
         user.add()
         user.save()
-        return user
+        return user, 201
 
     def get(self, id=None):
         ...
 
     def patch(self, id):
         ...
```

### Comparing `feiticeiro_tec-1.1.5/feiticeiro_tec/create/namespace.py` & `feiticeiro_tec-1.1.6/feiticeiro_tec/create/namespace.py`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.1.5/feiticeiro_tec/database/models/base.py` & `feiticeiro_tec-1.1.6/feiticeiro_tec/database/models/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class Base():
     id = Column(String(36), primary_key=True,
                 default=lambda: str(uuid.uuid4()))
     create_time = Column(DateTime, default=datetime.now, nullable=False)
     update_time = Column(DateTime, default=datetime.now,
                          onupdate=datetime.now, nullable=False)
     is_delete = Column(Boolean, default=False, nullable=False)
-    is_ativo = Column(Boolean, default=True, nullable=False)
+    is_active = Column(Boolean, default=True, nullable=False)
 
     def add(self):
         logger.debug('Adicionando {} ao Banco de Dados'.format(self))
         db.session.add(self)
 
     def save(self):
         logger.debug('Salvando {} no Banco de Dados'.format(self))
```

### Comparing `feiticeiro_tec-1.1.5/feiticeiro_tec/database/models/usuario.py` & `feiticeiro_tec-1.1.6/feiticeiro_tec/database/models/usuario.py`

 * *Files identical despite different names*

### Comparing `feiticeiro_tec-1.1.5/feiticeiro_tec.egg-info/SOURCES.txt` & `feiticeiro_tec-1.1.6/feiticeiro_tec.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -8,18 +8,24 @@
 feiticeiro_tec.egg-info/requires.txt
 feiticeiro_tec.egg-info/top_level.txt
 feiticeiro_tec/api/__init__.py
 feiticeiro_tec/api/utils/__init__.py
 feiticeiro_tec/api/utils/forms.py
 feiticeiro_tec/api/utils/serializers.py
 feiticeiro_tec/api/v1/__init__.py
-feiticeiro_tec/api/v1/usuario/__init__.py
+feiticeiro_tec/api/v1/permissions/__init__.py
+feiticeiro_tec/api/v1/permissions/form.py
+feiticeiro_tec/api/v1/permissions/serializers.py
+feiticeiro_tec/api/v1/usuarios/__init__.py
+feiticeiro_tec/api/v1/usuarios/forms.py
+feiticeiro_tec/api/v1/usuarios/serializers.py
 feiticeiro_tec/create/__init__.py
 feiticeiro_tec/create/app.py
 feiticeiro_tec/create/env.py
 feiticeiro_tec/create/model.py
 feiticeiro_tec/create/namespace.py
 feiticeiro_tec/create/server.py
 feiticeiro_tec/database/__init__.py
 feiticeiro_tec/database/models/__init__.py
 feiticeiro_tec/database/models/base.py
+feiticeiro_tec/database/models/permission.py
 feiticeiro_tec/database/models/usuario.py
```

### Comparing `feiticeiro_tec-1.1.5/setup.py` & `feiticeiro_tec-1.1.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(
     name='feiticeiro_tec',
-    version='1.1.5',
+    version='1.1.6',
     url='https://github.com/feiticeiro-tec/feiticeiro-tec',
     license='BSD3',
     author='Silvio Henrique Cruz Da Silva',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='silviohenriquecruzdasilva@gmail.com',
     keywords='Pacote',
```

