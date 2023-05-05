# Comparing `tmp/pyBibX-2.9.3.tar.gz` & `tmp/pyBibX-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyBibX-2.9.3.tar", last modified: Sun Apr 16 01:59:37 2023, max compression
+gzip compressed data, was "dist\pyBibX-2.9.4.tar", last modified: Fri May  5 20:48:44 2023, max compression
```

## Comparing `pyBibX-2.9.3.tar` & `pyBibX-2.9.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 01:59:37.000000 pyBibX-2.9.3/
--rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-2.9.3/LICENSE
--rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-2.9.3/MANIFEST.in
--rw-rw-rw-   0        0        0     9131 2023-04-16 01:59:37.000000 pyBibX-2.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     8694 2023-04-10 01:54:14.000000 pyBibX-2.9.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 01:59:37.000000 pyBibX-2.9.3/pyBibX/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.3/pyBibX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 01:59:37.000000 pyBibX-2.9.3/pyBibX/base/
--rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-2.9.3/pyBibX/base/__init__.py
--rw-rw-rw-   0        0        0   263628 2023-04-16 01:55:01.000000 pyBibX-2.9.3/pyBibX/base/pbx.py
-drwxrwxrwx   0        0        0        0 2023-04-16 01:59:37.000000 pyBibX-2.9.3/pyBibX/base/stws/
--rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.3/pyBibX/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 01:59:37.000000 pyBibX-2.9.3/pyBibX.egg-info/
--rw-rw-rw-   0        0        0     9131 2023-04-16 01:59:36.000000 pyBibX-2.9.3/pyBibX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1047 2023-04-16 01:59:36.000000 pyBibX-2.9.3/pyBibX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 01:59:36.000000 pyBibX-2.9.3/pyBibX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      210 2023-04-16 01:59:36.000000 pyBibX-2.9.3/pyBibX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-16 01:59:36.000000 pyBibX-2.9.3/pyBibX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-16 01:59:36.000000 pyBibX-2.9.3/pyBibX.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-16 01:59:37.000000 pyBibX-2.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1082 2023-04-16 01:58:53.000000 pyBibX-2.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:48:44.000000 pyBibX-2.9.4/
+-rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-2.9.4/LICENSE
+-rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-2.9.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     9127 2023-05-05 20:48:44.000000 pyBibX-2.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8690 2023-05-02 21:59:33.000000 pyBibX-2.9.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 20:48:44.000000 pyBibX-2.9.4/pyBibX/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.4/pyBibX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:48:44.000000 pyBibX-2.9.4/pyBibX/base/
+-rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-2.9.4/pyBibX/base/__init__.py
+-rw-rw-rw-   0        0        0   263868 2023-05-05 20:47:14.000000 pyBibX-2.9.4/pyBibX/base/pbx.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:48:44.000000 pyBibX-2.9.4/pyBibX/base/stws/
+-rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.4/pyBibX/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 20:48:44.000000 pyBibX-2.9.4/pyBibX.egg-info/
+-rw-rw-rw-   0        0        0     9127 2023-05-05 20:48:43.000000 pyBibX-2.9.4/pyBibX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1047 2023-05-05 20:48:43.000000 pyBibX-2.9.4/pyBibX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 20:48:43.000000 pyBibX-2.9.4/pyBibX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      210 2023-05-05 20:48:43.000000 pyBibX-2.9.4/pyBibX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 20:48:43.000000 pyBibX-2.9.4/pyBibX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-05 20:48:43.000000 pyBibX-2.9.4/pyBibX.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-05-05 20:48:44.000000 pyBibX-2.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1082 2023-05-05 20:48:21.000000 pyBibX-2.9.4/setup.py
```

### Comparing `pyBibX-2.9.3/LICENSE` & `pyBibX-2.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/PKG-INFO` & `pyBibX-2.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 2.9.3
+Version: 2.9.4
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -86,15 +86,15 @@
 
 * Bibliometrix (https://www.bibliometrix.org/home/)
 - a) Github: https://github.com/massimoaria/bibliometrix
 - b) Paper: ARIA, M.; CUCCURULLO, C. (2017). Bibliometrix: An R-tool for Comprehensive Science Mapping Analysis. Journal of informetrics, 11(4), 959-975. doi: https://doi.org/10.1016/j.joi.2017.08.007
 
 * chatGPT (https://chat.openai.com/chat)
 - a) Github: https://github.com/openai
-- b) Paper: ECOFFET, A. (2023). GPT-4 Technical Report. arXiv. doi: https://doi.org/10.48550/arXiv.2303.08774
+- b) Paper: OPENAI. (2023). GPT-4 Technical Report. arXiv. doi: https://doi.org/10.48550/arXiv.2303.08774
 
 * Metaknowledge (http://www.networkslab.org/metaknowledge)
 - a) Github: https://github.com/UWNETLAB/metaknowledge
 - b) Paper: McILROY-YOUNG, R.; McLEVEY, J.; ANDERSON, J. (2015). Metaknowledge: Open Source Software for Social Networks, Bibliometrics, and Sociology of Knowledge Research.
 
 * SentenceTransformers (https://www.sbert.net/)
 - a) Github: https://github.com/UKPLab/sentence-transformers
```

### Comparing `pyBibX-2.9.3/README.md` & `pyBibX-2.9.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 * Bibliometrix (https://www.bibliometrix.org/home/)
 - a) Github: https://github.com/massimoaria/bibliometrix
 - b) Paper: ARIA, M.; CUCCURULLO, C. (2017). Bibliometrix: An R-tool for Comprehensive Science Mapping Analysis. Journal of informetrics, 11(4), 959-975. doi: https://doi.org/10.1016/j.joi.2017.08.007
 
 * chatGPT (https://chat.openai.com/chat)
 - a) Github: https://github.com/openai
-- b) Paper: ECOFFET, A. (2023). GPT-4 Technical Report. arXiv. doi: https://doi.org/10.48550/arXiv.2303.08774
+- b) Paper: OPENAI. (2023). GPT-4 Technical Report. arXiv. doi: https://doi.org/10.48550/arXiv.2303.08774
 
 * Metaknowledge (http://www.networkslab.org/metaknowledge)
 - a) Github: https://github.com/UWNETLAB/metaknowledge
 - b) Paper: McILROY-YOUNG, R.; McLEVEY, J.; ANDERSON, J. (2015). Metaknowledge: Open Source Software for Social Networks, Bibliometrics, and Sociology of Knowledge Research.
 
 * SentenceTransformers (https://www.sbert.net/)
 - a) Github: https://github.com/UKPLab/sentence-transformers
```

### Comparing `pyBibX-2.9.3/pyBibX/base/pbx.py` & `pyBibX-2.9.4/pyBibX/base/pbx.py`

 * *Files 0% similar despite different names*

```diff
@@ -778,45 +778,45 @@
             rgba = 'black'
         return rgba
     
     #############################################################################
     
     # Function: EDA .bib docs
     def eda_bib(self):
-        report         = []
+        report = []
         report.append(['Timespan', str(self.date_str)+'-'+str(self.date_end)])
         report.append(['Total Number of Countries', len(self.u_ctr)])
         report.append(['Total Number of Institutions', len(self.u_uni)])
         report.append(['Total Number of Sources', len(self.u_jou)])
         report.append(['Total Number of References', len(self.u_ref)])
         report.append(['Total Number of Languages', len(self.u_lan)])
         for i in range(0, len(self.u_lan)):
             report.append(['--'+self.u_lan[i]+' (# of docs)', self.lan_count[i]])
         report.append(['-//-', '-//-'])
         report.append(['Total Number of Documents', self.data.shape[0]])
         for i in range(0, self.doc_types.shape[0]):
             report.append(['--'+self.doc_types.index[i], self.doc_types[i]])
         report.append(['Average Documents per Author',self. av_doc_aut])
-        report.append(['Average Documents per Institution', round(sum(self.uni_count)/len(self.uni_count), 2)])
-        report.append(['Average Documents per Source', round(sum(self.jou_count)/len(self.jou_count), 2)])
+        report.append(['Average Documents per Institution', round(sum(self.uni_count)/len(self.uni_count), 2) if len(self.uni_count) > 0 else 0])
+        report.append(['Average Documents per Source', round(sum(self.jou_count)/len(self.jou_count), 2) if len(self.jou_count) > 0 else 0])
         report.append(['Average Documents per Year', self.av_d_year])
         report.append(['-//-', '-//-'])
         report.append(['Total Number of Authors', len(self.u_aut)])
         report.append(['Total Number of Authors Keywords', len(self.u_auk)])
         report.append(['Total Number of Authors Keywords Plus', len(self.u_kid)])
         report.append(['Total Single-Authored Documents', self.aut_single])
         report.append(['Total Multi-Authored Documents', len(self.aut_multi)])
         report.append(['Average Collaboration Index', self.dy_c_year.iloc[-1, -1]])
         report.append(['Max H-Index', max(self.aut_h)])
         report.append(['-//-', '-//-'])
         report.append(['Total Number of Citations', sum(self.citation)])
-        report.append(['Average Citations per Author', round(sum(self.citation)/len(self.u_aut), 2)])
-        report.append(['Average Citations per Institution', round(sum(self.citation)/len(self.u_uni), 2)])
+        report.append(['Average Citations per Author', round(sum(self.citation)/len(self.u_aut), 2) if len(self.u_aut) > 0 else 0])
+        report.append(['Average Citations per Institution', round(sum(self.citation)/len(self.u_uni), 2) if len(self.u_uni) > 0 else 0])
         report.append(['Average Citations per Document', self.av_c_doc])
-        report.append(['Average Citations per Source', round(sum(self.jou_cit)/len(self.jou_cit), 2)])
+        report.append(['Average Citations per Source', round(sum(self.jou_cit)/len(self.jou_cit), 2) if len(self.jou_cit) > 0 else 0])
         report.append(['-//-', '-//-'])
         self.ask_gpt_rt = pd.DataFrame(report, columns = ['Main Information', 'Results'])
         report_df       = pd.DataFrame(report, columns = ['Main Information', 'Results'])
         return report_df
 
     ##############################################################################
 
@@ -2244,45 +2244,24 @@
     # Function: Text Pre-Processing
     def clear_text(self, corpus, stop_words = ['en'], lowercase = True, rmv_accents = True, rmv_special_chars = True, rmv_numbers = True, rmv_custom_words = [], verbose = False):
         sw_full = []
         # Lower Case
         if (lowercase == True):
             if (verbose == True):
                 print('Lower Case: Working...')
-            corpus = [str(x).lower() for x in  corpus]
+            corpus = [str(x).lower().replace("’","'") for x in  corpus]
             if (verbose == True):
                 print('Lower Case: Done!')
-        # Replace Accents 
-        if (rmv_accents == True):
-            if (verbose == True):
-                print('Removing Accents: Working...')
-            for i in range(0, len(corpus)):
-                text = corpus[i]
-                try:
-                    text = unicode(text, 'utf-8')
-                except NameError: 
-                    pass
-                text      = unicodedata.normalize('NFD', text).encode('ascii', 'ignore').decode('utf-8')
-                corpus[i] = str(text)
-            if (verbose == True):
-                print('Removing Accents: Done!')
         # Remove Punctuation & Special Characters
         if (rmv_special_chars == True):
             if (verbose == True):
                 print('Removing Special Characters: Working...')
-            corpus = [re.sub(r"[^a-zA-Z0-9]+", ' ', i) for i in corpus]
+            corpus = [re.sub(r"[^a-zA-Z0-9']+", ' ', i) for i in corpus]
             if (verbose == True):
                 print('Removing Special Characters: Done!')
-        # Remove Numbers
-        if (rmv_numbers == True):
-            if (verbose == True):
-                print('Removing Numbers: Working...')
-            corpus = [re.sub('[0-9]', ' ', i) for i in corpus] 
-            if (verbose == True):
-                print('Removing Numbers: Done!')
         # Remove Stopwords
         if (len(stop_words) > 0):
             for sw_ in stop_words: 
                 if   (sw_ == 'ar' or sw_ == 'ara'):
                     f_file = pkg_resources.open_text(stws, 'Stopwords-Arabic.txt', encoding = 'utf8')
                     #f_file = open('../pyBibX/Stopwords-Arabic.txt', 'r',        encoding = 'utf8')
                 elif (sw_ == 'bn' or sw_ == 'ben'):
@@ -2343,32 +2322,53 @@
                 sw      = f_lines.split('\n')
                 sw      = list(filter(None, sw))
                 sw_full.extend(sw)
             if (verbose == True):
                 print('Removing Stopwords: Working...')
             for i in range(0, len(corpus)):
                text      = corpus[i].split()
-               text      = [x for x in text if x not in sw_full]
+               text      = [x.replace(' ', '') for x in text if x.replace(' ', '') not in sw_full]
                corpus[i] = ' '.join(text) 
                if (verbose == True):
                    print('Removing Stopwords: ' + str(i + 1) +  ' of ' + str(len(corpus)) )
             if (verbose == True):
                 print('Removing Stopwords: Done!')
         # Remove Custom Words
         if (len(rmv_custom_words) > 0):
             if (verbose == True):
                 print('Removing Custom Words: Working...')
             for i in range(0, len(corpus)):
                text      = corpus[i].split()
-               text      = [x for x in text if x not in rmv_custom_words]
+               text      = [x.replace(' ', '') for x in text if x.replace(' ', '') not in rmv_custom_words]
                corpus[i] = ' '.join(text) 
                if (verbose == True):
                    print('Removing Custom Words: ' + str(i + 1) +  ' of ' + str(len(corpus)) )
             if (verbose == True):
                 print('Removing Custom Word: Done!')
+        # Replace Accents 
+        if (rmv_accents == True):
+            if (verbose == True):
+                print('Removing Accents: Working...')
+            for i in range(0, len(corpus)):
+                text = corpus[i]
+                try:
+                    text = unicode(text, 'utf-8')
+                except NameError: 
+                    pass
+                text      = unicodedata.normalize('NFD', text).encode('ascii', 'ignore').decode('utf-8')
+                corpus[i] = str(text)
+            if (verbose == True):
+                print('Removing Accents: Done!')
+        # Remove Numbers
+        if (rmv_numbers == True):
+            if (verbose == True):
+                print('Removing Numbers: Working...')
+            corpus = [re.sub('[0-9]', ' ', i) for i in corpus] 
+            if (verbose == True):
+                print('Removing Numbers: Done!')
         for i in range(0, len(corpus)):
             corpus[i] = ' '.join(corpus[i].split())
         return corpus
 
     # Function: TF-IDF
     def dtm_tf_idf(self, corpus):
         vectorizer = TfidfVectorizer(norm = 'l2')
```

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Arabic.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Arabic.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Bengali.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Bulgarian.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Czech.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Czech.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-English.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-English.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Finnish.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-French.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-French.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-German.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-German.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Hindi.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Hungarian.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Italian.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Italian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Marathi.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Persian.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Polish.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Portuguese-br.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Romanian.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Russian.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Spanish.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Spanish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX/base/stws/Stopwords-Swedish.txt` & `pyBibX-2.9.4/pyBibX/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/pyBibX.egg-info/PKG-INFO` & `pyBibX-2.9.4/pyBibX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 2.9.3
+Version: 2.9.4
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -86,15 +86,15 @@
 
 * Bibliometrix (https://www.bibliometrix.org/home/)
 - a) Github: https://github.com/massimoaria/bibliometrix
 - b) Paper: ARIA, M.; CUCCURULLO, C. (2017). Bibliometrix: An R-tool for Comprehensive Science Mapping Analysis. Journal of informetrics, 11(4), 959-975. doi: https://doi.org/10.1016/j.joi.2017.08.007
 
 * chatGPT (https://chat.openai.com/chat)
 - a) Github: https://github.com/openai
-- b) Paper: ECOFFET, A. (2023). GPT-4 Technical Report. arXiv. doi: https://doi.org/10.48550/arXiv.2303.08774
+- b) Paper: OPENAI. (2023). GPT-4 Technical Report. arXiv. doi: https://doi.org/10.48550/arXiv.2303.08774
 
 * Metaknowledge (http://www.networkslab.org/metaknowledge)
 - a) Github: https://github.com/UWNETLAB/metaknowledge
 - b) Paper: McILROY-YOUNG, R.; McLEVEY, J.; ANDERSON, J. (2015). Metaknowledge: Open Source Software for Social Networks, Bibliometrics, and Sociology of Knowledge Research.
 
 * SentenceTransformers (https://www.sbert.net/)
 - a) Github: https://github.com/UKPLab/sentence-transformers
```

### Comparing `pyBibX-2.9.3/pyBibX.egg-info/SOURCES.txt` & `pyBibX-2.9.4/pyBibX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.3/setup.py` & `pyBibX-2.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyBibX',
-    version='2.9.3',
+    version='2.9.4',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyBibX',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

