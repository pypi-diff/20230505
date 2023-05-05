# Comparing `tmp/rpa_cooperativa-1.0.51.tar.gz` & `tmp/rpa_cooperativa-1.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.51.tar", last modified: Wed May  3 11:39:17 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.52.tar", last modified: Fri May  5 16:58:58 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.51.tar` & `rpa_cooperativa-1.0.52.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 11:39:17.606253 rpa_cooperativa-1.0.51/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.51/LICENSE
--rw-rw-rw-   0        0        0     6670 2023-05-03 11:39:17.598061 rpa_cooperativa-1.0.51/PKG-INFO
--rw-rw-rw-   0        0        0     5525 2023-05-03 11:36:32.000000 rpa_cooperativa-1.0.51/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 11:39:17.350176 rpa_cooperativa-1.0.51/rpa_coop/
--rw-rw-rw-   0        0        0      568 2023-05-02 17:34:09.000000 rpa_cooperativa-1.0.51/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:39:17.515048 rpa_cooperativa-1.0.51/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.51/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.51/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.51/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.51/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.51/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.51/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.51/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.51/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.51/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.51/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.51/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    80396 2023-05-03 11:33:25.000000 rpa_cooperativa-1.0.51/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-05-03 11:39:17.583741 rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6670 2023-05-03 11:39:16.000000 rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-05-03 11:39:16.000000 rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 11:39:16.000000 rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-03 11:39:16.000000 rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      559 2023-05-03 11:39:16.000000 rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-03 11:39:16.000000 rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 11:39:17.608327 rpa_cooperativa-1.0.51/setup.cfg
--rw-rw-rw-   0        0        0     2323 2023-05-03 11:36:40.000000 rpa_cooperativa-1.0.51/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:58:58.924408 rpa_cooperativa-1.0.52/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.52/LICENSE
+-rw-rw-rw-   0        0        0     6670 2023-05-05 16:58:58.918832 rpa_cooperativa-1.0.52/PKG-INFO
+-rw-rw-rw-   0        0        0     5525 2023-05-03 11:36:32.000000 rpa_cooperativa-1.0.52/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 16:58:58.632903 rpa_cooperativa-1.0.52/rpa_coop/
+-rw-rw-rw-   0        0        0      568 2023-05-02 17:34:09.000000 rpa_cooperativa-1.0.52/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:58:58.845824 rpa_cooperativa-1.0.52/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.52/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.52/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.52/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.52/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.52/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.52/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.52/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.52/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.52/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.52/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.52/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    80588 2023-05-05 15:04:34.000000 rpa_cooperativa-1.0.52/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:58:58.906430 rpa_cooperativa-1.0.52/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6670 2023-05-05 16:58:57.000000 rpa_cooperativa-1.0.52/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-05-05 16:58:57.000000 rpa_cooperativa-1.0.52/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 16:58:57.000000 rpa_cooperativa-1.0.52/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-05 16:58:57.000000 rpa_cooperativa-1.0.52/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      559 2023-05-05 16:58:57.000000 rpa_cooperativa-1.0.52/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 16:58:57.000000 rpa_cooperativa-1.0.52/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 16:58:58.925612 rpa_cooperativa-1.0.52/setup.cfg
+-rw-rw-rw-   0        0        0     2325 2023-05-05 15:04:41.000000 rpa_cooperativa-1.0.52/setup.py
```

### Comparing `rpa_cooperativa-1.0.51/LICENSE` & `rpa_cooperativa-1.0.52/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.51/PKG-INFO` & `rpa_cooperativa-1.0.52/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.51
+Version: 1.0.52
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.51/README.md` & `rpa_cooperativa-1.0.52/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.51/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.52/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.51/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.52/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.51/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.52/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.51/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.52/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.51/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.52/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.51/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.52/rpa_coop/rpa_coop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1148,27 +1148,27 @@
         # Selecionar o MENU SIAT
         posicao = 0
         pasta_imagens = user_site_packages +  '\\rpa_coop\\img\\'
                    
         
         if 'SACG' in str(siat_siac_sacg).upper():
             try:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_branco.png')
+                posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_branco.png', confidence=0.9, grayscale=True)
             except:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_verde.png')
+                posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_verde.png', confidence=0.9, grayscale=True)
         elif 'SIAT' in str(siat_siac_sacg).upper():
             try:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'siat_amarelo.png')
+                posicao = self.p.locateOnScreen(pasta_imagens + 'siat_amarelo.png', confidence=0.9, grayscale=True)
             except:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'siat_branco.png')
+                posicao = self.p.locateOnScreen(pasta_imagens + 'siat_branco.png', confidence=0.9, grayscale=True)
         elif 'SIAC' in str(siat_siac_sacg).upper():
             try:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'siac_branco.png')
+                posicao = self.p.locateOnScreen(pasta_imagens + 'siac_branco.png', confidence=0.9, grayscale=True)
             except:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'siac_amarelo.png')
+                posicao = self.p.locateOnScreen(pasta_imagens + 'siac_amarelo.png', confidence=0.9, grayscale=True)
         time.sleep(1)
         self.p.click(posicao)
         print('selecionou o menu: siat, siac, sacg')
         time.sleep(3)
         
         if transacional:
             self.p.moveTo(janela.left + 48, janela.top + 165)
@@ -1246,30 +1246,30 @@
             self.p.sleep(1)
             self.p.typewrite(letras[6])
             self.p.sleep(1)
         else:
             print('ops funcao entende apenas 2, 3, 4, 5, 6 ou 7 letras')
             
                 
-    def get_text(self, ini_linha=22, fim_linha=632, topo1=407, topo2=407):
+    def get_text(self, ini_linha=22, fim_linha=632, topo1=410, topo2=415):
         time.sleep(1)
         janela = self.p.getWindowsWithTitle('teoff-exe')[0]
         time.sleep(1)
         janela.activate()
         self.p.moveTo(janela.left + ini_linha, janela.top + topo1)
         self.p.sleep(1)
-        self.p.dragTo(janela.left + fim_linha, janela.top + topo2, 0.8, button='left')
+        self.p.dragTo(janela.left + fim_linha, janela.top + topo2, 1.5, button='left')
         self.p.moveTo(janela.left + ini_linha, janela.top + topo2)
         self.p.rightClick()
         capturado = self.pyperclip.paste()
         print(f'texto capturado:{capturado}')
         return capturado            
             
             
-    def exist_text(self, texto_esperado, max_tentativas=7, segundos_entre_tentativas=3, ini_linha=22, fim_linha=632, topo1=407, topo2=407, continua_seerro=False):
+    def exist_text(self, texto_esperado, max_tentativas=7, segundos_entre_tentativas=3, ini_linha=22, fim_linha=632, topo1=412, topo2=412, continua_seerro=False):
         time.sleep(1)
         self.pyperclip.copy('')
         tentativas = 0
         time.sleep(1)
         captura = self.get_text(ini_linha, fim_linha, topo1, topo2)
         resultado = True
         while not texto_esperado in captura and tentativas < max_tentativas:
```

### Comparing `rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.52/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.51
+Version: 1.0.52
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.52/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.52/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.51/setup.py` & `rpa_cooperativa-1.0.52/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import setuptools
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
+
 setup(
     name="rpa_cooperativa",
-    version="1.0.51",
+    version="1.0.52",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

