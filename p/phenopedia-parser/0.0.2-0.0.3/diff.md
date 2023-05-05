# Comparing `tmp/phenopedia-parser-0.0.2.tar.gz` & `tmp/phenopedia-parser-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenopedia-parser-0.0.2.tar", last modified: Tue Apr 19 01:33:32 2022, max compression
+gzip compressed data, was "phenopedia-parser-0.0.3.tar", last modified: Fri May  5 16:00:11 2023, max compression
```

## Comparing `phenopedia-parser-0.0.2.tar` & `phenopedia-parser-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2022-04-19 01:33:32.632868 phenopedia-parser-0.0.2/
--rw-r--r--   0 spaethju   (501) staff       (20)     1070 2022-04-18 20:45:47.000000 phenopedia-parser-0.0.2/LICENSE
--rw-r--r--   0 spaethju   (501) staff       (20)      877 2022-04-19 01:33:32.632926 phenopedia-parser-0.0.2/PKG-INFO
--rw-r--r--   0 spaethju   (501) staff       (20)      299 2022-04-18 21:12:54.000000 phenopedia-parser-0.0.2/README.md
--rw-r--r--   0 spaethju   (501) staff       (20)      121 2022-04-18 20:54:41.000000 phenopedia-parser-0.0.2/pyproject.toml
--rw-r--r--   0 spaethju   (501) staff       (20)      666 2022-04-19 01:33:32.633208 phenopedia-parser-0.0.2/setup.cfg
-drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2022-04-19 01:33:32.631629 phenopedia-parser-0.0.2/src/
-drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2022-04-19 01:33:32.632340 phenopedia-parser-0.0.2/src/phenopedia_parser/
--rw-r--r--   0 spaethju   (501) staff       (20)     1702 2022-04-19 01:31:05.000000 phenopedia-parser-0.0.2/src/phenopedia_parser/PhenopediaParser.py
--rw-r--r--   0 spaethju   (501) staff       (20)        0 2022-04-18 19:08:47.000000 phenopedia-parser-0.0.2/src/phenopedia_parser/__init__.py
-drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2022-04-19 01:33:32.632771 phenopedia-parser-0.0.2/src/phenopedia_parser.egg-info/
--rw-r--r--   0 spaethju   (501) staff       (20)      877 2022-04-19 01:33:32.000000 phenopedia-parser-0.0.2/src/phenopedia_parser.egg-info/PKG-INFO
--rw-r--r--   0 spaethju   (501) staff       (20)      298 2022-04-19 01:33:32.000000 phenopedia-parser-0.0.2/src/phenopedia_parser.egg-info/SOURCES.txt
--rw-r--r--   0 spaethju   (501) staff       (20)        1 2022-04-19 01:33:32.000000 phenopedia-parser-0.0.2/src/phenopedia_parser.egg-info/dependency_links.txt
--rw-r--r--   0 spaethju   (501) staff       (20)       18 2022-04-19 01:33:32.000000 phenopedia-parser-0.0.2/src/phenopedia_parser.egg-info/top_level.txt
+drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2023-05-05 16:00:11.320902 phenopedia-parser-0.0.3/
+-rw-r--r--   0 spaethju   (501) staff       (20)     1070 2023-05-05 14:22:29.000000 phenopedia-parser-0.0.3/LICENSE
+-rw-r--r--   0 spaethju   (501) staff       (20)     1321 2023-05-05 16:00:11.320980 phenopedia-parser-0.0.3/PKG-INFO
+-rw-r--r--   0 spaethju   (501) staff       (20)      780 2023-05-05 14:22:29.000000 phenopedia-parser-0.0.3/README.md
+-rw-r--r--   0 spaethju   (501) staff       (20)      121 2023-05-05 14:22:29.000000 phenopedia-parser-0.0.3/pyproject.toml
+-rw-r--r--   0 spaethju   (501) staff       (20)      666 2023-05-05 16:00:11.321298 phenopedia-parser-0.0.3/setup.cfg
+drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2023-05-05 16:00:11.318984 phenopedia-parser-0.0.3/src/
+drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2023-05-05 16:00:11.320133 phenopedia-parser-0.0.3/src/phenopedia_parser/
+-rw-r--r--   0 spaethju   (501) staff       (20)     1607 2023-05-05 15:50:40.000000 phenopedia-parser-0.0.3/src/phenopedia_parser/PhenopediaParser.py
+-rw-r--r--   0 spaethju   (501) staff       (20)        0 2023-05-05 14:22:29.000000 phenopedia-parser-0.0.3/src/phenopedia_parser/__init__.py
+drwxr-xr-x   0 spaethju   (501) staff       (20)        0 2023-05-05 16:00:11.320771 phenopedia-parser-0.0.3/src/phenopedia_parser.egg-info/
+-rw-r--r--   0 spaethju   (501) staff       (20)     1321 2023-05-05 16:00:11.000000 phenopedia-parser-0.0.3/src/phenopedia_parser.egg-info/PKG-INFO
+-rw-r--r--   0 spaethju   (501) staff       (20)      298 2023-05-05 16:00:11.000000 phenopedia-parser-0.0.3/src/phenopedia_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 spaethju   (501) staff       (20)        1 2023-05-05 16:00:11.000000 phenopedia-parser-0.0.3/src/phenopedia_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 spaethju   (501) staff       (20)       18 2023-05-05 16:00:11.000000 phenopedia-parser-0.0.3/src/phenopedia_parser.egg-info/top_level.txt
```

### Comparing `phenopedia-parser-0.0.2/LICENSE` & `phenopedia-parser-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `phenopedia-parser-0.0.2/PKG-INFO` & `phenopedia-parser-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: phenopedia-parser
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package to parse phenopedia data
 Home-page: https://github.com/julianspaeth/PhenopediaParser
 Author: Julian Späth
 Author-email: spaethju@posteo.de
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/julianspaeth/PhenopediaParser/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PhenopediaParser
 
+A python API for parsing [Phenopedia](https://phgkb.cdc.gov/PHGKB/startPagePhenoPedia.action "Phenopedia's Homepage"). 
+
+"Phenopedia provides a disease-centered view of genetic association studies summarized in the online Human Genome Epidemiology (HuGE) encyclopedia. Users can switch to a gene-centered view (Genopedia) or to other HuGE Tools."
+
+
 ## Getting Started
 
 ### Install
 
 ```pip install phenopedia_parser```
 
 ### Usage
 
 ```
-from phenopedia_parser.phenopedia_parser import PhenopediaParser
+from phenopedia_parser import PhenopediaParser
 
 pheno_dataframe = PhenopediaParser.parse(search_term='lung', dataframe=True)
 print(pheno_dataframe)
 ```
 
 ### License
 MIT License
 
+### Support
+[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/julianspaeth)
```

### Comparing `phenopedia-parser-0.0.2/setup.cfg` & `phenopedia-parser-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phenopedia-parser
-version = 0.0.2
+version = 0.0.3
 author = Julian Späth
 author_email = spaethju@posteo.de
 description = A python package to parse phenopedia data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/julianspaeth/PhenopediaParser
 project_urls =
```

### Comparing `phenopedia-parser-0.0.2/src/phenopedia_parser/PhenopediaParser.py` & `phenopedia-parser-0.0.3/src/phenopedia_parser/PhenopediaParser.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,43 @@
+import urllib
+
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
 
 cdc_url = 'https://phgkb.cdc.gov'
 search_term = 'lung'
 headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) '
                   'AppleWebKit/537.36 '
                   '(KHTML, like Gecko) '
                   'Chrome/39.0.2171.95 Safari/537.36'}
 
 
 def parse(search_term: str, dataframe=True):
+    search_term = search_term.strip().replace(" ", "+")
     url = f'{cdc_url}/PHGKB/phenoPedia.action?firstQuery={search_term}' \
           f'&typeSubmit=Go&typeOption=disease&check=n&which=1'
     html_text = requests.get(url, headers=headers).text
     soup = BeautifulSoup(html_text, features="lxml")
     links = soup.find_all('a')
     diseases = {}
     for link in links:
         href = str(link.get('href'))
         if href.startswith('/PHGKB/phenoPedia.action?firstQuery='):
             diseases[link.getText()] = cdc_url + href
 
-    genes = {}
+    genes = []
     for disease in diseases.keys():
         html_text = requests.get(diseases[disease]).text
         soup = BeautifulSoup(html_text, features="lxml")
-        urls = soup.find_all('a')
-        for gene in urls:
-            url = str(gene.get('href'))
-            if 'geneID' in url and '/PHGKB/huGEPedia.action' in url:
-                geneID = url.split('=')[1].split('&')[0]
-            elif 'searchSummary' in url and geneID is not None:
-                n_pubs = gene.getText().replace('\r\n\t\t\t', '')
-                genes[geneID] = [disease, n_pubs]
-                geneID = None
+        gene_entries = soup.find_all('tr')
+        for gene_entry in gene_entries:
+            td_elements = gene_entry.find_all('td')
+            if len(td_elements) == 3 and td_elements[0].text.strip() != 'Associated Gene':
+                genes.append([td_elements[0].text.strip(), disease, td_elements[1].text.strip(), td_elements[2].text.strip()])
 
     if dataframe:
-        df = pd.DataFrame.from_dict(genes, orient='index').reset_index()
-        rename_map = {'index': 'gene', 0: 'disease', 1: 'n_publications'}
-        return df.rename(rename_map, axis='columns')
+        df = pd.DataFrame(genes, columns=['gene', 'disease', 'n_publications', 'n_meta_analyses'])
+        return df
 
     return genes
```

### Comparing `phenopedia-parser-0.0.2/src/phenopedia_parser.egg-info/PKG-INFO` & `phenopedia-parser-0.0.3/src/phenopedia_parser.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 Metadata-Version: 2.1
 Name: phenopedia-parser
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package to parse phenopedia data
 Home-page: https://github.com/julianspaeth/PhenopediaParser
 Author: Julian Späth
 Author-email: spaethju@posteo.de
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/julianspaeth/PhenopediaParser/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PhenopediaParser
 
+A python API for parsing [Phenopedia](https://phgkb.cdc.gov/PHGKB/startPagePhenoPedia.action "Phenopedia's Homepage"). 
+
+"Phenopedia provides a disease-centered view of genetic association studies summarized in the online Human Genome Epidemiology (HuGE) encyclopedia. Users can switch to a gene-centered view (Genopedia) or to other HuGE Tools."
+
+
 ## Getting Started
 
 ### Install
 
 ```pip install phenopedia_parser```
 
 ### Usage
 
 ```
-from phenopedia_parser.phenopedia_parser import PhenopediaParser
+from phenopedia_parser import PhenopediaParser
 
 pheno_dataframe = PhenopediaParser.parse(search_term='lung', dataframe=True)
 print(pheno_dataframe)
 ```
 
 ### License
 MIT License
 
+### Support
+[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/julianspaeth)
```

