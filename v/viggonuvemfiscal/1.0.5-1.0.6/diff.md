# Comparing `tmp/viggonuvemfiscal-1.0.5.tar.gz` & `tmp/viggonuvemfiscal-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggonuvemfiscal-1.0.5.tar", last modified: Wed Apr 19 13:20:06 2023, max compression
+gzip compressed data, was "viggonuvemfiscal-1.0.6.tar", last modified: Fri May  5 19:26:33 2023, max compression
```

## Comparing `viggonuvemfiscal-1.0.5.tar` & `viggonuvemfiscal-1.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:20:06.185099 viggonuvemfiscal-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-19 13:20:06.185099 viggonuvemfiscal-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:20:06.185099 viggonuvemfiscal-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:20:06.181099 viggonuvemfiscal-1.0.5/viggonuvemfiscal/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:20:06.181099 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:20:06.181099 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:20:06.181099 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:20:06.185099 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:20:06.181099 viggonuvemfiscal-1.0.5/viggonuvemfiscal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-19 13:20:06.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-19 13:20:06.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:20:06.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-19 13:20:06.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 13:20:06.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:26:33.372335 viggonuvemfiscal-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-05 19:26:33.372335 viggonuvemfiscal-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:26:33.372335 viggonuvemfiscal-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:26:33.368335 viggonuvemfiscal-1.0.6/viggonuvemfiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:26:33.368335 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:26:33.368335 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:26:33.372335 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:26:33.372335 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-05 19:25:41.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:26:33.368335 viggonuvemfiscal-1.0.6/viggonuvemfiscal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-05 19:26:33.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-05 19:26:33.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:26:33.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-05 19:26:33.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 19:26:33.000000 viggonuvemfiscal-1.0.6/viggonuvemfiscal.egg-info/top_level.txt
```

### Comparing `viggonuvemfiscal-1.0.5/viggonuvemfiscal/__init__.py` & `viggonuvemfiscal-1.0.6/viggonuvemfiscal/__init__.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.5/viggonuvemfiscal/resources.py` & `viggonuvemfiscal-1.0.6/viggonuvemfiscal/resources.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py` & `viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-import requests
-import os
-import flask
-from vex.subsystem.aplicacao.tabela_preco.resource import TabelaPreco
 from viggocore.common.subsystem import operation, manager
-from viggocore.common import exception, utils
+from viggocore.common import exception
 
 
 class Create(operation.Create):
 
     def pre(self, session, **kwargs):
         configuracao_nuvem_fiscals = self.manager.list()
         if len(configuracao_nuvem_fiscals) > 0:
@@ -17,15 +13,15 @@
 
 
 class Manager(manager.Manager):
 
     def __init__(self, driver):
         super(Manager, self).__init__(driver)
         self.create = Create(self)
-    
+
     def get_configuracao_nuvem_fiscal(self):
         configs = self.list()
         if len(configs) == 0:
             raise exception.NotFound(
                 'Nenhuma configuração da Nuvem Fiscal cadastrada, por favor ' +
                 'cadastre uma para usar a api.')
         return configs[0]
```

### Comparing `viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py` & `viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py` & `viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py` & `viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,32 +17,33 @@
 
     # funções em comum
     def get_authorization(self):
         authorization = os.getenv('NUVEM_FISCAL_AUTHORIZATION', None)
         if authorization is None:
             raise exception.PreconditionFailed(
                 'NUVEM_FISCAL_AUTHORIZATION é obrigatório!')
-        return  {'Authorization': authorization}
-    
+        return {'Authorization': authorization}
+
     def get_cpf_cnpj(self, **kwargs):
         cpf_cnpj = kwargs.get('cpf_cnpj', None)
         if cpf_cnpj is None:
             raise exception.BadRequest('O campo cpf_cnpj é obrigatório.')
         return cpf_cnpj
 
     def get_nfe_id(self, **kwargs):
         nfe_id = kwargs.get('nfe_id', None)
         if nfe_id is None:
             raise exception.BadRequest('O campo nfe_id é obrigatório.')
         return nfe_id
-    
+
     def get_endpoint(self, resource):
         return self.BASE_URL_HOMO + resource
 
-    def executar_requisicao(self, method, endpoint, params={}, json={}, headers={}):
+    def executar_requisicao(
+       self, method, endpoint, params={}, json={}, headers={}):
         headers.update(self.get_authorization())
         if method == 'GET':
             return requests.get(
                 endpoint, params=params, json=json, headers=headers)
         elif method == 'POST':
             return requests.post(
                 endpoint, params=params, json=json, headers=headers)
@@ -50,15 +51,15 @@
             return requests.put(
                 endpoint, params=params, json=json, headers=headers)
         elif method == 'DELETE':
             return requests.delete(endpoint)
         else:
             raise exception.OperationBadRequest(
                 'Método de requisição não permitido.')
-    
+
     def montar_response_dict(self, response):
         try:
             response_dict = json.loads(response.text)
         except Exception:
             response_dict = {'error': response.text}
 
         return response_dict
@@ -334,15 +335,15 @@
                                   status=exc.status)
 
         response_dict = self.montar_response_dict(response)
 
         return flask.Response(response=utils.to_json(response_dict),
                               status=response.status_code,
                               mimetype="application/json")
-    
+
     def baixar_xml_cancelamento_nfe(self):
         filters = self._filters_parse()
         filters = self._filters_cleanup(filters)
 
         try:
             filters = self._parse_list_options(filters)
             nfe_id = self.get_nfe_id(**filters)
@@ -359,19 +360,19 @@
                               mimetype="application/json")
 
     def cancelar_nfe_autorizada(self):
         data = flask.request.get_json()
 
         try:
             nfe_id = self.get_nfe_id(**data)
-            url = self.get_endpoint('/nfe/{nfe_id}/cancelamento')
+            url = self.get_endpoint(f'/nfe/{nfe_id}/cancelamento')
             data.pop('nfe_id')
             response = self.executar_requisicao('POST', url, json=data)
         except exception.ViggoCoreException as exc:
             return flask.Response(response=exc.message,
                                   status=exc.status)
 
         response_dict = self.montar_response_dict(response)
 
         return flask.Response(response=utils.to_json(response_dict),
                               status=response.status_code,
-                              mimetype="application/json")
+                              mimetype="application/json")
```

### Comparing `viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py` & `viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import json
 import requests
-import os
-import flask
-from vex.subsystem.aplicacao.tabela_preco.resource import TabelaPreco
 from viggocore.common.subsystem import operation, manager
 from viggocore.common import exception, utils
 
 
 class CadastrarEmpresa(operation.Create):
 
     def pre(self, session, **kwargs):
         return True
-    
+
     def do(self, session, **kwargs):
         url = self.manager.get_endpoint('/empresas')
         return self.manager.executar_requisicao('POST', url, json=kwargs)
 
 
 class ListarEmpresas(operation.List):
 
@@ -46,14 +43,15 @@
 class ConsultarCerticado(operation.List):
 
     def do(self, session, **kwargs):
         cpf_cnpj = self.manager.get_cpf_cnpj(**kwargs)
         url = self.manager.get_endpoint(f'/empresas/{cpf_cnpj}/certificado')
         return self.manager.executar_requisicao('GET', url)
 
+
 class CadastrarCertificado(operation.Update):
 
     def pre(self, session, **kwargs):
         return True
 
     def do(self, session, **kwargs):
         cpf_cnpj = self.manager.get_cpf_cnpj(**kwargs)
@@ -130,15 +128,23 @@
         return self.manager.executar_requisicao('GET', url)
 
 
 class BaixarXmlNfe(operation.List):
 
     def do(self, session, **kwargs):
         nfe_id = self.manager.get_nfe_id(**kwargs)
-        url = self.manager.get_endpoint(f'/nfe/{nfe_id}/xml')
+        url = self.manager.get_endpoint(f'/nfe/{nfe_id}/xml/nota')
+        return self.manager.executar_requisicao('GET', url)
+
+
+class BaixarPdfDanfeNfe(operation.List):
+
+    def do(self, session, **kwargs):
+        nfe_id = self.manager.get_nfe_id(**kwargs)
+        url = self.manager.get_endpoint(f'/nfe/{nfe_id}/pdf')
         return self.manager.executar_requisicao('GET', url)
 
 
 class ConsultarCancelamentoNfe(operation.List):
 
     def do(self, session, **kwargs):
         nfe_id = self.manager.get_nfe_id(**kwargs)
@@ -158,14 +164,21 @@
     def do(self, session, **kwargs):
         nfe_id = self.manager.get_nfe_id(**kwargs)
         url = self.manager.get_endpoint(f'/nfe/{nfe_id}/cancelamento')
         kwargs.pop('nfe_id')
         return self.manager.executar_requisicao('POST', url, json=kwargs)
 
 
+class InutilizarSeqNumNfe(operation.List):
+
+    def do(self, session, **kwargs):
+        url = self.manager.get_endpoint('/nfe/inutilizacoes')
+        return self.manager.executar_requisicao('POST', url, json=kwargs)
+
+
 class Manager(manager.Manager):
     # BASE_URL_PROD = 'https://api.nuvemfiscal.com.br'
     BASE_URL_HOMO = 'https://api.sandbox.nuvemfiscal.com.br'
 
     def __init__(self, driver):
         super(Manager, self).__init__(driver)
         self.cadastrar_empresa = CadastrarEmpresa(self)
@@ -179,17 +192,19 @@
         self.alterar_configuracao_nfe = AlterarConfiguracaoNfe(self)
         self.emitir_nfe = EmitirNfe(self)
         self.listar_nfe = ListarNfe(self)
         self.consulta_status_do_servico_na_sefaz_autorizadora = \
             ConsultaStatusDoServicoNaSefazAutorizadora(self)
         self.consultar_nfe = ConsultarNfe(self)
         self.baixar_xml_nfe = BaixarXmlNfe(self)
+        self.baixar_pdf_danfe_nfe = BaixarPdfDanfeNfe(self)
         self.consultar_cancelamento_nfe = ConsultarCancelamentoNfe(self)
         self.baixar_xml_cancelamento_nfe = BaixarXmlCancelamentoNfe(self)
         self.cancelar_nfe_autorizada = CancelarNfeAutorizada(self)
+        self.inutilizar_seq_num_nfe = InutilizarSeqNumNfe(self)
 
     def get_authorization(self):
         config = self.api.configuracao_nuvem_fiscals().\
             get_configuracao_nuvem_fiscal()
         data = {'Authorization': config.authorization}
 
         endpoint = self.get_endpoint('/empresas')
@@ -251,14 +266,14 @@
             return requests.put(
                 endpoint, params=params, json=json, headers=headers, data=data)
         elif method == 'DELETE':
             return requests.delete(endpoint)
         else:
             raise exception.OperationBadRequest(
                 'Método de requisição não permitido.')
-    
+
     def montar_response_dict(self, response):
         try:
             response_dict = json.loads(response.text)
         except Exception:
             response_dict = {'error': response.text}
         return response_dict
```

### Comparing `viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py` & `viggonuvemfiscal-1.0.6/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.5/viggonuvemfiscal.egg-info/SOURCES.txt` & `viggonuvemfiscal-1.0.6/viggonuvemfiscal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

