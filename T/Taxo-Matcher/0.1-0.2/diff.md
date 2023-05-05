# Comparing `tmp/Taxo-Matcher-0.1.tar.gz` & `tmp/Taxo-Matcher-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Taxo-Matcher-0.1.tar", last modified: Tue Apr 18 00:54:30 2023, max compression
+gzip compressed data, was "Taxo-Matcher-0.2.tar", last modified: Fri May  5 19:11:05 2023, max compression
```

## Comparing `Taxo-Matcher-0.1.tar` & `Taxo-Matcher-0.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 lswhiteh (315696) users      (100)        0 2023-04-18 00:54:30.047226 Taxo-Matcher-0.1/
--rw-r--r--   0 lswhiteh (315696) users      (100)     1073 2023-02-27 20:27:38.000000 Taxo-Matcher-0.1/LICENSE
--rw-r--r--   0 lswhiteh (315696) users      (100)     3006 2023-04-18 00:54:30.048205 Taxo-Matcher-0.1/PKG-INFO
--rw-r--r--   0 lswhiteh (315696) users      (100)     2407 2023-02-27 20:49:42.000000 Taxo-Matcher-0.1/README.md
-drwxr-xr-x   0 lswhiteh (315696) users      (100)        0 2023-04-18 00:54:30.031178 Taxo-Matcher-0.1/Taxo_Matcher.egg-info/
--rw-r--r--   0 lswhiteh (315696) users      (100)     3006 2023-04-18 00:54:29.000000 Taxo-Matcher-0.1/Taxo_Matcher.egg-info/PKG-INFO
--rw-r--r--   0 lswhiteh (315696) users      (100)      387 2023-04-18 00:54:29.000000 Taxo-Matcher-0.1/Taxo_Matcher.egg-info/SOURCES.txt
--rw-r--r--   0 lswhiteh (315696) users      (100)        1 2023-04-18 00:54:29.000000 Taxo-Matcher-0.1/Taxo_Matcher.egg-info/dependency_links.txt
--rw-r--r--   0 lswhiteh (315696) users      (100)       61 2023-04-18 00:54:29.000000 Taxo-Matcher-0.1/Taxo_Matcher.egg-info/entry_points.txt
--rw-r--r--   0 lswhiteh (315696) users      (100)       22 2023-04-18 00:54:29.000000 Taxo-Matcher-0.1/Taxo_Matcher.egg-info/requires.txt
--rw-r--r--   0 lswhiteh (315696) users      (100)       12 2023-04-18 00:54:29.000000 Taxo-Matcher-0.1/Taxo_Matcher.egg-info/top_level.txt
--rw-r--r--   0 lswhiteh (315696) users      (100)      756 2023-04-18 00:54:30.051210 Taxo-Matcher-0.1/setup.cfg
--rw-r--r--   0 lswhiteh (315696) users      (100)      225 2023-04-18 00:01:46.000000 Taxo-Matcher-0.1/setup.py
-drwxr-xr-x   0 lswhiteh (315696) users      (100)        0 2023-04-18 00:54:30.045196 Taxo-Matcher-0.1/taxomatcher/
--rw-r--r--   0 lswhiteh (315696) users      (100)        0 2023-04-18 00:04:07.000000 Taxo-Matcher-0.1/taxomatcher/__init__.py
--rw-r--r--   0 lswhiteh (315696) users      (100)        0 2023-04-18 00:04:02.000000 Taxo-Matcher-0.1/taxomatcher/__main__.py
--rw-r--r--   0 lswhiteh (315696) users      (100)     4979 2023-04-18 00:16:31.000000 Taxo-Matcher-0.1/taxomatcher/entrez_matcher.py
--rw-r--r--   0 lswhiteh (315696) users      (100)     2089 2023-04-18 00:07:14.000000 Taxo-Matcher-0.1/taxomatcher/gbif_matcher.py
--rw-r--r--   0 lswhiteh (315696) users      (100)      615 2023-04-18 00:54:14.000000 Taxo-Matcher-0.1/taxomatcher/taxomatcher.py
+drwxr-xr-x   0 lswhiteh (315696) users      (100)        0 2023-05-05 19:11:05.394436 Taxo-Matcher-0.2/
+-rw-r--r--   0 lswhiteh (315696) users      (100)     1073 2023-02-27 20:27:38.000000 Taxo-Matcher-0.2/LICENSE
+-rw-r--r--   0 lswhiteh (315696) users      (100)     3016 2023-05-05 19:11:05.395435 Taxo-Matcher-0.2/PKG-INFO
+-rw-r--r--   0 lswhiteh (315696) users      (100)     2417 2023-04-18 00:59:52.000000 Taxo-Matcher-0.2/README.md
+drwxr-xr-x   0 lswhiteh (315696) users      (100)        0 2023-05-05 19:11:05.378450 Taxo-Matcher-0.2/Taxo_Matcher.egg-info/
+-rw-r--r--   0 lswhiteh (315696) users      (100)     3016 2023-05-05 19:11:05.000000 Taxo-Matcher-0.2/Taxo_Matcher.egg-info/PKG-INFO
+-rw-r--r--   0 lswhiteh (315696) users      (100)      435 2023-05-05 19:11:05.000000 Taxo-Matcher-0.2/Taxo_Matcher.egg-info/SOURCES.txt
+-rw-r--r--   0 lswhiteh (315696) users      (100)        1 2023-05-05 19:11:05.000000 Taxo-Matcher-0.2/Taxo_Matcher.egg-info/dependency_links.txt
+-rw-r--r--   0 lswhiteh (315696) users      (100)       61 2023-05-05 19:11:05.000000 Taxo-Matcher-0.2/Taxo_Matcher.egg-info/entry_points.txt
+-rw-r--r--   0 lswhiteh (315696) users      (100)       29 2023-05-05 19:11:05.000000 Taxo-Matcher-0.2/Taxo_Matcher.egg-info/requires.txt
+-rw-r--r--   0 lswhiteh (315696) users      (100)       12 2023-05-05 19:11:05.000000 Taxo-Matcher-0.2/Taxo_Matcher.egg-info/top_level.txt
+-rw-r--r--   0 lswhiteh (315696) users      (100)      764 2023-05-05 19:11:05.397443 Taxo-Matcher-0.2/setup.cfg
+-rw-r--r--   0 lswhiteh (315696) users      (100)      225 2023-04-18 00:01:46.000000 Taxo-Matcher-0.2/setup.py
+drwxr-xr-x   0 lswhiteh (315696) users      (100)        0 2023-05-05 19:11:05.392440 Taxo-Matcher-0.2/taxomatcher/
+-rw-r--r--   0 lswhiteh (315696) users      (100)        0 2023-04-18 00:04:07.000000 Taxo-Matcher-0.2/taxomatcher/__init__.py
+-rw-r--r--   0 lswhiteh (315696) users      (100)        0 2023-04-18 00:04:02.000000 Taxo-Matcher-0.2/taxomatcher/__main__.py
+-rw-r--r--   0 lswhiteh (315696) users      (100)     5041 2023-05-05 18:45:49.000000 Taxo-Matcher-0.2/taxomatcher/entrez_matcher.py
+-rw-r--r--   0 lswhiteh (315696) users      (100)     2158 2023-05-05 18:42:21.000000 Taxo-Matcher-0.2/taxomatcher/gbif_matcher.py
+-rw-r--r--   0 lswhiteh (315696) users      (100)     4965 2023-05-02 19:22:14.000000 Taxo-Matcher-0.2/taxomatcher/gui.py
+-rw-r--r--   0 lswhiteh (315696) users      (100)     2192 2023-05-05 18:41:32.000000 Taxo-Matcher-0.2/taxomatcher/taxomatcher.py
+-rw-r--r--   0 lswhiteh (315696) users      (100)      629 2023-05-05 19:03:13.000000 Taxo-Matcher-0.2/taxomatcher/trait_matcher.py
```

### Comparing `Taxo-Matcher-0.1/LICENSE` & `Taxo-Matcher-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Taxo-Matcher-0.1/PKG-INFO` & `Taxo-Matcher-0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Taxo-Matcher
-Version: 0.1
+Version: 0.2
 Summary: A tool for parsing and extracting taxon synonyms.
 Home-page: https://github.com/Lswhiteh/taxo-matcher
 Author: Logan Whitehouse
 Author-email: lswhiteh@unc.edu
 License: MIT
 Project-URL: Issues, https://github.com/Lswhiteh/taxo-matcher/issues
 Project-URL: GitHub, https://github.com/Lswhiteh/taxo-matcher
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Taxomatcher
-Python module to query the NCBI Taxonomy database for synonym names of target species.
+Python modules to query the GFIB or NCBI Taxonomy databases for synonym names of target species.
 
 ## Installation
 Required packages:
 - Biopython
 - pygbif
 
 To use conda:
```

### Comparing `Taxo-Matcher-0.1/README.md` & `Taxo-Matcher-0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Taxomatcher
-Python module to query the NCBI Taxonomy database for synonym names of target species.
+Python modules to query the GFIB or NCBI Taxonomy databases for synonym names of target species.
 
 ## Installation
 Required packages:
 - Biopython
 - pygbif
 
 To use conda:
```

### Comparing `Taxo-Matcher-0.1/Taxo_Matcher.egg-info/PKG-INFO` & `Taxo-Matcher-0.2/Taxo_Matcher.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Taxo-Matcher
-Version: 0.1
+Version: 0.2
 Summary: A tool for parsing and extracting taxon synonyms.
 Home-page: https://github.com/Lswhiteh/taxo-matcher
 Author: Logan Whitehouse
 Author-email: lswhiteh@unc.edu
 License: MIT
 Project-URL: Issues, https://github.com/Lswhiteh/taxo-matcher/issues
 Project-URL: GitHub, https://github.com/Lswhiteh/taxo-matcher
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Taxomatcher
-Python module to query the NCBI Taxonomy database for synonym names of target species.
+Python modules to query the GFIB or NCBI Taxonomy databases for synonym names of target species.
 
 ## Installation
 Required packages:
 - Biopython
 - pygbif
 
 To use conda:
```

### Comparing `Taxo-Matcher-0.1/setup.cfg` & `Taxo-Matcher-0.2/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Taxo-Matcher
-version = 0.1
+version = 0.2
 author = Logan Whitehouse
 author_email = lswhiteh@unc.edu
 description = A tool for parsing and extracting taxon synonyms.
 url = https://github.com/Lswhiteh/taxo-matcher
 project_urls = 
 	Issues = https://github.com/Lswhiteh/taxo-matcher/issues
 	GitHub = https://github.com/Lswhiteh/taxo-matcher
@@ -21,14 +21,15 @@
 python_requires = >=3.6
 include_package_data = True
 packages = taxomatcher
 install_requires = 
 	biopython
 	tqdm
 	pygbif
+	pandas
 
 [options.entry_points]
 console_scripts = 
 	taxomatcher = taxomatcher.taxomatcher:main
 
 [egg_info]
 tag_build =
```

### Comparing `Taxo-Matcher-0.1/taxomatcher/entrez_matcher.py` & `Taxo-Matcher-0.2/taxomatcher/entrez_matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 - https://biopython.org/docs/1.76/api/Bio.Entrez.html
 - https://www.ncbi.nlm.nih.gov/books/NBK25497/
 - https://www.ncbi.nlm.nih.gov/books/NBK25500/
 
 Logan Whitehouse - lswhiteh@unc.edu
 """
 import argparse
+import os
 
 from tqdm import tqdm
 from Bio import Entrez
 
-
 def get_ua():
     ap = argparse.ArgumentParser()
     ap.add_argument("-e", "--email", dest="email", required=True)
     ap.add_argument(
         "-c",
         "--csv",
         dest="input_csv",
@@ -95,18 +95,19 @@
                 sp_list.extend(_line)
                 target_list.append(line.strip().split(",")[0])
                 idx_list.extend([idx] * len(_line))
 
     return sp_list, target_list, idx_list
 
 
-def main(ua):
-    Entrez.email = ua.email
+def main(input_csv, outfile, user_email):
+    Entrez.email = user_email
+    os.makedirs(os.path.dirname(outfile), exist_ok=True)
 
-    sp_list, target_list, idx_list = read_csv(ua.input_csv)
+    sp_list, target_list, idx_list = read_csv(input_csv)
     cleaned_sp_list = [i.replace("_", " ") for i in sp_list]
 
     name_res = []
     pass_list = []
     fail_list = []
     tax_ids = []
     for idx, sp_str in tqdm(
@@ -154,17 +155,17 @@
             if s in n:
                 n.remove(s)
                 n.insert(0, s)
 
     max_len = max([len(i) for i in name_res])
     eq_headers = ["Tree_Sp_Name"] + [f"Eq_{i}" for i in range(max_len - 1)]
 
-    with open(f"output/multi_taxomatcher_output.tsv", "w") as ofile:
+    with open(outfile, "w") as ofile:
         ofile.write("\t".join(eq_headers) + "\n")
         for names in name_res:
             ofile.write("\t".join(names) + "\n")
 
-    with open("output/multi_taxomatcher_fails.tsv", "w") as failfile:
+    with open(f"{outfile.split('.')[0]}_fails.csv", "w") as failfile:
         for i in set(fail_list):
             failfile.write(i.replace(" ", "_") + "\n")
 
     print("[INFO] Done")
```

### Comparing `Taxo-Matcher-0.1/taxomatcher/gbif_matcher.py` & `Taxo-Matcher-0.2/taxomatcher/gbif_matcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Logan Whitehouse - lswhiteh@unc.edu
 """
 import argparse
 import multiprocessing as mp
 from tqdm import tqdm
 from pygbif import species
-
+import os
 
 def read_csv(csvfile):
     target_list = []
     with open(csvfile, "r") as ifile:
         for line in ifile.readlines():
             if "Tree_Sp_Name" in line:
                 continue
@@ -52,31 +52,31 @@
         synonyms.insert(0, sp)
         synonyms.append(curr_name)
     else:
         synonyms = [sp]
 
     return synonyms
 
-
-def main(ua):
-    sp_list = read_csv(ua.input_csv)
+def main(input_csv, outfile, threads):
+    sp_list = read_csv(input_csv)
     cleaned_sp_list = [i.replace("_", " ") for i in sp_list]
 
-    with mp.Pool(ua.threads) as p:
+    with mp.Pool(threads) as p:
         synonyms = list(
             tqdm(
                 p.imap(worker, cleaned_sp_list, chunksize=4),
                 desc="[INFO] Fetching GBIF information",
                 total=len(cleaned_sp_list),
             )
         )
 
     max_len = max([len(i) for i in synonyms])
     eq_headers = (
         ["Tree_Sp_Name"] + [f"Eq_{i}" for i in range(max_len - 1)] + ["Curr_Name"]
     )
+    
+    os.makedirs(os.path.dirname(outfile), exist_ok=True)
 
-    with open(f"output/gbif_output.tsv", "w") as ofile:
+    with open(outfile, "w") as ofile:
         ofile.write("\t".join(eq_headers) + "\n")
         for names in synonyms:
-            ofile.write("\t".join([i.replace(" ", "_") for i in names]) + "\n")
-
+            ofile.write("\t".join([i.replace(" ", "_") for i in names]) + "\n")
```

