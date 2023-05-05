# Comparing `tmp/lsaBGC-1.35.tar.gz` & `tmp/lsaBGC-1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsaBGC-1.35.tar", last modified: Mon Apr 17 05:52:22 2023, max compression
+gzip compressed data, was "lsaBGC-1.36.tar", last modified: Fri May  5 05:28:22 2023, max compression
```

## Comparing `lsaBGC-1.35.tar` & `lsaBGC-1.36.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-04-17 05:52:22.381701 lsaBGC-1.35/
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     1517 2023-04-16 22:46:02.000000 lsaBGC-1.35/LICENSE
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)      398 2023-04-17 05:52:22.381701 lsaBGC-1.35/PKG-INFO
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     6494 2023-04-16 22:46:02.000000 lsaBGC-1.35/README.md
-drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-04-17 05:52:22.377701 lsaBGC-1.35/bin/
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     8651 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-Cluster.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    10729 2023-04-17 03:41:01.000000 lsaBGC-1.35/bin/lsaBGC-ComprehenSeeIve.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    13310 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-DiscoVary.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    10541 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-Divergence.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    14738 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-Expansion.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    15751 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-MIBiGMapper.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    12808 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-PopGene.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    37287 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-Ready.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     7734 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-Refiner.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    11168 2023-04-16 22:46:02.000000 lsaBGC-1.35/bin/lsaBGC-See.py
-drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-04-17 05:52:22.377701 lsaBGC-1.35/lsaBGC/
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-04-16 22:46:02.000000 lsaBGC-1.35/lsaBGC/__init__.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    14437 2023-04-16 22:46:02.000000 lsaBGC-1.35/lsaBGC/processing.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)   105402 2023-04-17 04:47:50.000000 lsaBGC-1.35/lsaBGC/util.py
-drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-04-17 05:52:22.377701 lsaBGC-1.35/lsaBGC.egg-info/
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)      398 2023-04-17 05:52:22.000000 lsaBGC-1.35/lsaBGC.egg-info/PKG-INFO
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     1050 2023-04-17 05:52:22.000000 lsaBGC-1.35/lsaBGC.egg-info/SOURCES.txt
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)        1 2023-04-17 05:52:22.000000 lsaBGC-1.35/lsaBGC.egg-info/dependency_links.txt
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)        1 2023-04-17 05:52:22.000000 lsaBGC-1.35/lsaBGC.egg-info/not-zip-safe
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)        7 2023-04-17 05:52:22.000000 lsaBGC-1.35/lsaBGC.egg-info/top_level.txt
-drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-04-17 05:52:22.381701 lsaBGC-1.35/scripts/
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    23594 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/GSeeF.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     7624 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/compareBGCtoGenomeCodonUsage.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     2984 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/createPickleOfSampleAnnotationListingFile.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     6276 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/listAllBGCGenbanksInDirectory.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    10399 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/listAllGenomesInDirectory.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    16757 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/popSizeAndSampleSelector.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     7962 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/processAndReformatNCBIGenbanks.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     8298 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/readifyAdditionalGenomes.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     7465 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/runProdigalAndMakeProperGenbank.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     5055 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/setup_annotation_dbs.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     3185 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/setup_bigscape.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     3447 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/simpleProteinExtraction.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    12818 2023-04-16 22:46:02.000000 lsaBGC-1.35/scripts/visualize_BGC-Ome.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)       38 2023-04-17 05:52:22.381701 lsaBGC-1.35/setup.cfg
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     1797 2023-04-17 01:52:56.000000 lsaBGC-1.35/setup.py
-drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-04-17 05:52:22.381701 lsaBGC-1.35/workflows/
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    40240 2023-04-17 05:19:18.000000 lsaBGC-1.35/workflows/lsaBGC-AutoAnalyze.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    18332 2023-04-17 03:23:33.000000 lsaBGC-1.35/workflows/lsaBGC-AutoExpansion.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    44237 2023-04-17 03:32:24.000000 lsaBGC-1.35/workflows/lsaBGC-Easy.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    38073 2023-04-17 03:32:24.000000 lsaBGC-1.35/workflows/lsaBGC-Euk-Easy.py
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-05-05 05:28:22.739867 lsaBGC-1.36/
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     1517 2023-05-05 00:57:38.000000 lsaBGC-1.36/LICENSE
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)      398 2023-05-05 05:28:22.739867 lsaBGC-1.36/PKG-INFO
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     6494 2023-05-05 00:57:38.000000 lsaBGC-1.36/README.md
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-05-05 05:28:22.735867 lsaBGC-1.36/bin/
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     8651 2023-05-05 00:57:38.000000 lsaBGC-1.36/bin/lsaBGC-Cluster.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    10729 2023-05-05 00:57:38.000000 lsaBGC-1.36/bin/lsaBGC-ComprehenSeeIve.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    13310 2023-05-05 00:57:38.000000 lsaBGC-1.36/bin/lsaBGC-DiscoVary.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    10541 2023-05-05 00:57:38.000000 lsaBGC-1.36/bin/lsaBGC-Divergence.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    14738 2023-05-05 00:57:38.000000 lsaBGC-1.36/bin/lsaBGC-Expansion.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    15751 2023-05-05 00:57:38.000000 lsaBGC-1.36/bin/lsaBGC-MIBiGMapper.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    12808 2023-05-05 00:57:38.000000 lsaBGC-1.36/bin/lsaBGC-PopGene.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    37287 2023-05-05 00:57:38.000000 lsaBGC-1.36/bin/lsaBGC-Ready.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     7734 2023-05-05 00:57:38.000000 lsaBGC-1.36/bin/lsaBGC-Refiner.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    11168 2023-05-05 00:57:38.000000 lsaBGC-1.36/bin/lsaBGC-See.py
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-05-05 05:28:22.735867 lsaBGC-1.36/lsaBGC/
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-05-05 00:57:38.000000 lsaBGC-1.36/lsaBGC/__init__.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    14437 2023-05-05 00:57:38.000000 lsaBGC-1.36/lsaBGC/processing.py
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)   105757 2023-05-05 03:45:58.000000 lsaBGC-1.36/lsaBGC/util.py
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-05-05 05:28:22.739867 lsaBGC-1.36/lsaBGC.egg-info/
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)      398 2023-05-05 05:28:22.000000 lsaBGC-1.36/lsaBGC.egg-info/PKG-INFO
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     1050 2023-05-05 05:28:22.000000 lsaBGC-1.36/lsaBGC.egg-info/SOURCES.txt
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)        1 2023-05-05 05:28:22.000000 lsaBGC-1.36/lsaBGC.egg-info/dependency_links.txt
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)        1 2023-05-05 05:20:09.000000 lsaBGC-1.36/lsaBGC.egg-info/not-zip-safe
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)        7 2023-05-05 05:28:22.000000 lsaBGC-1.36/lsaBGC.egg-info/top_level.txt
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-05-05 05:28:22.739867 lsaBGC-1.36/scripts/
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    23732 2023-05-05 03:24:51.000000 lsaBGC-1.36/scripts/GSeeF.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     7624 2023-05-05 00:57:38.000000 lsaBGC-1.36/scripts/compareBGCtoGenomeCodonUsage.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     2984 2023-05-05 00:57:38.000000 lsaBGC-1.36/scripts/createPickleOfSampleAnnotationListingFile.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     6276 2023-05-05 00:57:38.000000 lsaBGC-1.36/scripts/listAllBGCGenbanksInDirectory.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    10399 2023-05-05 00:57:38.000000 lsaBGC-1.36/scripts/listAllGenomesInDirectory.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    16757 2023-05-05 00:57:38.000000 lsaBGC-1.36/scripts/popSizeAndSampleSelector.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     7962 2023-05-05 00:57:38.000000 lsaBGC-1.36/scripts/processAndReformatNCBIGenbanks.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     8298 2023-05-05 00:57:38.000000 lsaBGC-1.36/scripts/readifyAdditionalGenomes.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     7465 2023-05-05 00:57:38.000000 lsaBGC-1.36/scripts/runProdigalAndMakeProperGenbank.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     6838 2023-05-05 05:03:17.000000 lsaBGC-1.36/scripts/setup_annotation_dbs.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     3185 2023-05-05 00:57:38.000000 lsaBGC-1.36/scripts/setup_bigscape.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     3447 2023-05-05 00:57:38.000000 lsaBGC-1.36/scripts/simpleProteinExtraction.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    12818 2023-05-05 00:57:38.000000 lsaBGC-1.36/scripts/visualize_BGC-Ome.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)       38 2023-05-05 05:28:22.739867 lsaBGC-1.36/setup.cfg
+-rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     1798 2023-05-05 01:01:45.000000 lsaBGC-1.36/setup.py
+drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-05-05 05:28:22.739867 lsaBGC-1.36/workflows/
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    40240 2023-05-05 00:57:38.000000 lsaBGC-1.36/workflows/lsaBGC-AutoAnalyze.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    21428 2023-05-05 04:09:13.000000 lsaBGC-1.36/workflows/lsaBGC-AutoExpansion.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    45983 2023-05-05 03:43:34.000000 lsaBGC-1.36/workflows/lsaBGC-Easy.py
+-rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    40099 2023-05-05 05:03:17.000000 lsaBGC-1.36/workflows/lsaBGC-Euk-Easy.py
```

### Comparing `lsaBGC-1.35/LICENSE` & `lsaBGC-1.36/LICENSE`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/README.md` & `lsaBGC-1.36/README.md`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/bin/lsaBGC-Cluster.py` & `lsaBGC-1.36/bin/lsaBGC-Cluster.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/bin/lsaBGC-ComprehenSeeIve.py` & `lsaBGC-1.36/bin/lsaBGC-ComprehenSeeIve.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/bin/lsaBGC-DiscoVary.py` & `lsaBGC-1.36/bin/lsaBGC-DiscoVary.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/bin/lsaBGC-Divergence.py` & `lsaBGC-1.36/bin/lsaBGC-Divergence.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/bin/lsaBGC-Expansion.py` & `lsaBGC-1.36/bin/lsaBGC-Expansion.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/bin/lsaBGC-MIBiGMapper.py` & `lsaBGC-1.36/bin/lsaBGC-MIBiGMapper.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/bin/lsaBGC-PopGene.py` & `lsaBGC-1.36/bin/lsaBGC-PopGene.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/bin/lsaBGC-Ready.py` & `lsaBGC-1.36/bin/lsaBGC-Ready.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/bin/lsaBGC-Refiner.py` & `lsaBGC-1.36/bin/lsaBGC-Refiner.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/bin/lsaBGC-See.py` & `lsaBGC-1.36/bin/lsaBGC-See.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/lsaBGC/processing.py` & `lsaBGC-1.36/lsaBGC/processing.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/lsaBGC/util.py` & `lsaBGC-1.36/lsaBGC/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1543,88 +1543,94 @@
 								  pgap_hmm_file,
 								  kofam_pro_list, pgap_inf_list, logObject, cpus=1):
 	sample_protein_annotations = defaultdict(lambda: defaultdict(lambda: "hypothetical protein"))
 	try:
 		ko_score_cutoffs = {}
 		ko_score_types = {}
 		ko_descriptions = defaultdict(lambda: "NA")
-		with open(kofam_pro_list) as okpl:
-			for i, line in enumerate(okpl):
-				if i == 0: continue
-				line = line.strip()
-				ls = line.split('\t')
-				ko = ls[0]
-				if ls[1] == '-': continue
-				score_cutoff = float(ls[1])
-				profile_type = ls[2]
-				description = ls[-1]
-				ko_score_cutoffs[ko] = score_cutoff
-				ko_score_types[ko] = profile_type
+		pgap_descriptions = defaultdict(lambda: "NA")
+		if kofam_pro_list != None and kofam_hmm_file != None:
+			with open(kofam_pro_list) as okpl:
+				for i, line in enumerate(okpl):
+					if i == 0: continue
+					line = line.strip()
+					ls = line.split('\t')
+					ko = ls[0]
+					if ls[1] == '-': continue
+					score_cutoff = float(ls[1])
+					profile_type = ls[2]
+					description = ls[-1]
+					ko_score_cutoffs[ko] = score_cutoff
+					ko_score_types[ko] = profile_type
 				ko_descriptions[ko] = description
 
-		pgap_descriptions = defaultdict(lambda: "NA")
-		with open(pgap_inf_list) as opil:
-			for i, line in enumerate(opil):
-				if i == 0: continue
-				line = line.strip()
-				ls = line.split('\t')
-				label = ls[2]
-				description = ls[10]
-				pgap_descriptions[label] = description
+		if pgap_inf_list != None and pgap_hmm_file != None:
+			with open(pgap_inf_list) as opil:
+				for i, line in enumerate(opil):
+					if i == 0: continue
+					line = line.strip()
+					ls = line.split('\t')
+					label = ls[2]
+					description = ls[10]
+					pgap_descriptions[label] = description
 
 		hmmsearch_cmds = []
 		for f in os.listdir(bgc_prot_directory):
 			sample = f.split('.faa')[0]
 			prot_file = bgc_prot_directory + f
 			ko_annot_result = annot_directory + sample + '.ko.txt'
 			pgap_annot_result = annot_directory + sample + '.pgap.txt'
-			hmmsearch_ko_cmd = ['hmmsearch', '--cpu', '2', '--tblout', ko_annot_result, kofam_hmm_file,
-								prot_file, logObject]
-			hmmsearch_pgap_cmd = ['hmmsearch', '--cpu', '2', '--tblout', pgap_annot_result, pgap_hmm_file,
-								  prot_file, logObject]
-			hmmsearch_cmds.append(hmmsearch_ko_cmd)
-			hmmsearch_cmds.append(hmmsearch_pgap_cmd)
+			if kofam_pro_list != None and kofam_hmm_file != None:
+				hmmsearch_ko_cmd = ['hmmsearch', '--cpu', '2', '--tblout', ko_annot_result, kofam_hmm_file,
+									prot_file, logObject]
+				hmmsearch_cmds.append(hmmsearch_ko_cmd)
+			if pgap_inf_list != None and pgap_hmm_file != None:
+				hmmsearch_pgap_cmd = ['hmmsearch', '--cpu', '2', '--tblout', pgap_annot_result, pgap_hmm_file,
+									  prot_file, logObject]
+				hmmsearch_cmds.append(hmmsearch_pgap_cmd)
 
 		p = multiprocessing.Pool(math.floor(cpus / 2))
 		p.map(multiProcess, hmmsearch_cmds)
 		p.close()
 
 		for sample in sample_bgc_proteins:
 			ko_annot_result = annot_directory + sample + '.ko.txt'
 			pgap_annot_result = annot_directory + sample + '.pgap.txt'
 			hits_per_prot = defaultdict(list)
 
-			with open(ko_annot_result) as orf:
-				for line in orf:
-					if line.startswith("#"): continue
-					line = line.strip()
-					ls = line.split()
-					ko = ls[2]
-					prot_id = ls[0]
-					full_eval = float(ls[4])
-					full_score = float(ls[5])
-					dom_score = float(ls[8])
-					if ko in ko_score_types:
-						if ko_score_types[ko] == 'full' and full_score >= ko_score_cutoffs[ko]:
-							hits_per_prot[prot_id].append(['ko', ko, -full_score, full_eval])
-						elif ko_score_types[ko] == 'domain' and dom_score >= ko_score_cutoffs[ko]:
-							hits_per_prot[prot_id].append(['ko', ko, -dom_score, full_eval])
-					if full_eval < 1e-10:
-						hits_per_prot[prot_id].append(['ko', ko, 1E10, full_eval])
-
-			with open(pgap_annot_result) as orf:
-				for line in orf:
-					if line.startswith("#"): continue
-					line = line.strip()
-					ls = line.split()
-					pgap = ls[2]
-					prot_id = ls[0]
-					full_eval = float(ls[4])
-					if full_eval < 1e-10:
-						hits_per_prot[prot_id].append(['pgap', pgap, 1E10, full_eval])
+			if os.path.isfile(ko_annot_result):
+				with open(ko_annot_result) as orf:
+					for line in orf:
+						if line.startswith("#"): continue
+						line = line.strip()
+						ls = line.split()
+						ko = ls[2]
+						prot_id = ls[0]
+						full_eval = float(ls[4])
+						full_score = float(ls[5])
+						dom_score = float(ls[8])
+						if ko in ko_score_types:
+							if ko_score_types[ko] == 'full' and full_score >= ko_score_cutoffs[ko]:
+								hits_per_prot[prot_id].append(['ko', ko, -full_score, full_eval])
+							elif ko_score_types[ko] == 'domain' and dom_score >= ko_score_cutoffs[ko]:
+								hits_per_prot[prot_id].append(['ko', ko, -dom_score, full_eval])
+						if full_eval < 1e-10:
+							hits_per_prot[prot_id].append(['ko', ko, 1E10, full_eval])
+
+			if os.path.isfile(pgap_annot_result):
+				with open(pgap_annot_result) as orf:
+					for line in orf:
+						if line.startswith("#"): continue
+						line = line.strip()
+						ls = line.split()
+						pgap = ls[2]
+						prot_id = ls[0]
+						full_eval = float(ls[4])
+						if full_eval < 1e-10:
+							hits_per_prot[prot_id].append(['pgap', pgap, 1E10, full_eval])
 
 			best_hits = defaultdict(lambda: 'hypothetical protein')
 			for pi in hits_per_prot:
 				for i, hit in enumerate(sorted(hits_per_prot[pi], key=lambda h: (h[2], h[3]), reverse=False)):
 					if i == 0:
 						conf = ' (High Confidence)'
 						if hit[2] == 1E10 and hit[0] == 'ko':
```

### Comparing `lsaBGC-1.35/lsaBGC.egg-info/SOURCES.txt` & `lsaBGC-1.36/lsaBGC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/scripts/GSeeF.py` & `lsaBGC-1.36/scripts/GSeeF.py`

 * *Files 2% similar despite different names*

```diff
@@ -408,15 +408,18 @@
 	logObject.info('\n---------------------\nStep 5\n---------------------\nGenerating final static PDF visualization and iTol track file.')
 	sys.stdout.write('---------------------\nStep 5\n---------------------\nGenerating final static PDF visualization and iTol track file.\n')
 
 	gSeefScript = lsaBGC_main_directory + 'lsaBGC/Rscripts/gSeef.R'
 	resulting_png = final_results_dir + 'Phylogenetic_Heatmap.png'
 	label_resulting_png = final_results_dir + 'Annotation_Legend.png'
 	gseef_cmd = ['Rscript', gSeefScript, rooted_species_tree_file, gseef_track_file, resulting_png, label_resulting_png]
-	runCmdViaSubprocess(gseef_cmd, logObject, check_files=[resulting_png, label_resulting_png])
+	# check files should be: resulting_png, label_resulting_png
+	# but plots are not essential so taking out requirement in case
+	# R environment broken in conda environment.
+	runCmdViaSubprocess(gseef_cmd, logObject, check_files=[])
 
 	# Close logging object and exit
 	logObject.info('GSeeF completed! Check out the major results in the folder: %s' % final_results_dir)
 	sys.stdout.write('GSeeF completed! Check out the major results in the folder:\n%s\n' % final_results_dir)
 	util.closeLoggerObject(logObject)
 	sys.exit(0)
```

### Comparing `lsaBGC-1.35/scripts/compareBGCtoGenomeCodonUsage.py` & `lsaBGC-1.36/scripts/compareBGCtoGenomeCodonUsage.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/scripts/createPickleOfSampleAnnotationListingFile.py` & `lsaBGC-1.36/scripts/createPickleOfSampleAnnotationListingFile.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/scripts/listAllBGCGenbanksInDirectory.py` & `lsaBGC-1.36/scripts/listAllBGCGenbanksInDirectory.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/scripts/listAllGenomesInDirectory.py` & `lsaBGC-1.36/scripts/listAllGenomesInDirectory.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/scripts/popSizeAndSampleSelector.py` & `lsaBGC-1.36/scripts/popSizeAndSampleSelector.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/scripts/processAndReformatNCBIGenbanks.py` & `lsaBGC-1.36/scripts/processAndReformatNCBIGenbanks.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/scripts/readifyAdditionalGenomes.py` & `lsaBGC-1.36/scripts/readifyAdditionalGenomes.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/scripts/runProdigalAndMakeProperGenbank.py` & `lsaBGC-1.36/scripts/runProdigalAndMakeProperGenbank.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/scripts/setup_bigscape.py` & `lsaBGC-1.36/scripts/setup_bigscape.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/scripts/simpleProteinExtraction.py` & `lsaBGC-1.36/scripts/simpleProteinExtraction.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/scripts/visualize_BGC-Ome.py` & `lsaBGC-1.36/scripts/visualize_BGC-Ome.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/setup.py` & `lsaBGC-1.36/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='lsaBGC',
-      version='1.35',
+      version='1.36',
       description='Suite for comparative genomic, population genetics and evolutionary analysis, as well as metagenomic mining of micro-evolutionary novelty in BGCs all in the context of a single lineage of interest.',
       url='http://github.com/Kalan-Lab/lsaBGC/',
       author='Rauf Salamzade',
       author_email='salamzader@gmail.com',
       license='BSD-3',
       packages=['lsaBGC'],
       scripts=['scripts/setup_annotation_dbs.py',
@@ -31,8 +31,8 @@
                'bin/lsaBGC-ComprehenSeeIve.py',
                'bin/lsaBGC-PopGene.py', 
                'bin/lsaBGC-Refiner.py', 
                'bin/lsaBGC-Expansion.py', 
                'bin/lsaBGC-Divergence.py', 
                'bin/lsaBGC-DiscoVary.py',
                'bin/lsaBGC-MIBiGMapper.py'],
-      zip_safe=False)
+      zip_safe=False)
```

### Comparing `lsaBGC-1.35/workflows/lsaBGC-AutoAnalyze.py` & `lsaBGC-1.36/workflows/lsaBGC-AutoAnalyze.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.35/workflows/lsaBGC-AutoExpansion.py` & `lsaBGC-1.36/workflows/lsaBGC-AutoExpansion.py`

 * *Files 22% similar despite different names*

```diff
@@ -60,19 +60,27 @@
 
 	Program to run lsaBGC-Expansion on each GCF, resolve conflicts across GCFs, and then consolidate result files when
 	overlapping BGC predictions for different GCFs exist.
 	""", formatter_class=argparse.RawTextHelpFormatter)
 
 	parser.add_argument('-g', '--gcf_listing_dir', help='Directory with GCF listing files.', required=True)
 	parser.add_argument('-m', '--orthofinder_matrix', help="OrthoFinder homolog group by sample matrix.", required=True)
-	parser.add_argument('-l', '--initial_listing', type=str, help="Path to tab delimited text file for samples with three columns: (1) sample\nname (2) Prokka generated Genbank file (*.gbk), and (3) Prokka generated predicted-proteome file\n(*.faa). Please remove troublesome characters in the sample name.", required=True)
-	parser.add_argument('-e', '--expansion_listing', help="Path to tab delimited file listing: (1) sample name (2) path to Prokka Genbank and\n(3) path to Prokka predicted proteome. This file is produced by\nlsaBGC-AutoProcess.py.", required=True)
+	parser.add_argument('-l', '--initial_listing', type=str, help="Path to tab delimited text file for samples with three columns: (1) sample\nname (2) path to genome-wide full Genbank file (*.gbk) with CDS features, and (3) path to genome-wide proteome file\n(*.faa). Please remove troublesome characters in the sample name.", required=True)
+	parser.add_argument('-e', '--expansion_listing', help="Path to tab delimited file listing: (1) sample name (2) path to\ngenome-wide full Genbank file and (3) path to genome-wide\npredicted proteome.", required=True)
 	parser.add_argument('-o', '--output_directory', help="Parent output/workspace directory.", required=True)
 	parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO)\n[Default is antiSMASH].', default='antiSMASH', required=False)
 	parser.add_argument('-q', '--quick_mode', action='store_true', help='Whether to run lsaBGC-Expansion in quick mode?', required=False, default=False)
+	parser.add_argument('-ms', '--min_segment_size', type=float, help="The minimum number of homolog groups (>3) needed to report discrete\nsegments of the GCF. Ignored if GCF specific or functionally core (e.g. harboring key domain for\ndetection of BGC) homolog group is found in segment [Default is 5].", required=False, default=5)
+	parser.add_argument('-mcs', '--min_segment_core_size', type=float, help="The minimum number of core (to the known instances of the GCF) homololog groups needed\nto report discrete segments of the GCF [Default is 3].", required=False, default=3)
+	parser.add_argument('-sct', '--syntenic_correlation_threshold', type=float, help="The minimum syntenic correlation needed to at least one known\nGCF instance to report segment [Default is 0.8].", required=False, default=0.8)
+	parser.add_argument('-tg', '--transition_from_gcf_to_gcf', type=float, help="GCF to GCF state transition probability for HMM. Should be between\n0.0 and 1.0 [Default is 0.9].", required=False, default=0.9)
+	parser.add_argument('-tb', '--transition_from_bg_to_bg', type=float, help="Background to background state transition probability for HMM. Should be\nbetween 0.0 and 1.0 [Default is 0.9].", required=False, default=0.9)
+	parser.add_argument('-no', '--no_orthogroup_matrix', action='store_true', help="Avoid writing the updated OrthoFinder matrix at the end.", required=False, default=False)
+	parser.add_argument('-w', '--loose_mode', action='store_true', help="Remove requirement for proto-core/rule-based homolog group being detected in\na single neighborhood for GCF to be reported as present.", required=False, default=False)
+	parser.add_argument('-ap', '--all_primary', action='store_true', help='Treat all known GCF instances as primary (use if BGC Genbanks\nwere not processed through lsaBGC-Ready).', required=False, default=False)
 	parser.add_argument('-z', '--pickle_expansion_annotation_data', help="Pickle file with serialization of annotation data in the expansion listing file.", required=False, default=None)
 	parser.add_argument('-ph', '--protocore_homologs', help="File with manual listings of proto-core homolog groups.\nThis should be provided as 2 column tab-delmited file: (1) GCF id and\n(2) space delmited listing of homolog groups.", required=False, default=None)
 	parser.add_argument('-c', '--cpus', type=int, help="Total number of CPUs to use [Default is 1].", required=False, default=1)
 
 	args = parser.parse_args()
 	return args
 
@@ -108,14 +116,22 @@
 	"""
 
 	cpus = myargs.cpus
 	bgc_prediction_software = myargs.bgc_prediction_software.upper()
 	quick_mode = myargs.quick_mode
 	pickle_expansion_annotation_data_file = myargs.pickle_expansion_annotation_data
 	protocore_homologs_file = myargs.protocore_homologs
+	min_segment_size = myargs.min_segment_size
+	min_segment_core_size = myargs.min_segment_core_size
+	syntenic_correlation_threshold = myargs.syntenic_correlation_threshold
+	transition_from_gcf_to_gcf = myargs.transition_from_gcf_to_gcf
+	transition_from_bg_to_bg = myargs.transition_from_bg_to_bg
+	no_orthogroup_matrix = myargs.no_orthogroup_matrix
+	loose_mode = myargs.loose_mode
+	all_primary = myargs.all_primary
 
 	try:
 		assert (bgc_prediction_software in set(['ANTISMASH', 'DEEPBGC', 'GECCO']))
 	except:
 		raise RuntimeError('BGC prediction software option is not a valid option.')
 
 	if pickle_expansion_annotation_data_file != None:
@@ -139,21 +155,27 @@
 
 	# Step 0: Log input arguments and update reference and query FASTA files.
 	logObject.info("Saving parameters for easier determination of results' provenance in the future.")
 	parameters_file = outdir + 'Parameter_Inputs.txt'
 	parameter_values = [gcf_listing_dir, initial_listing_file,
 						expansion_listing_file, original_orthofinder_matrix_file, outdir,
 						pickle_expansion_annotation_data_file, quick_mode, bgc_prediction_software,
-						protocore_homologs_file, cpus]
+						protocore_homologs_file, min_segment_size, min_segment_core_size,
+						syntenic_correlation_threshold, transition_from_gcf_to_gcf, transition_from_bg_to_bg,
+						no_orthogroup_matrix, loose_mode, all_primary, cpus]
 	parameter_names = ["GCF Listings Directory", "Listing File of Prokka Annotation Files for Initial Set of Samples",
 					   "Listing File of Prokka Annotation Files for Expansion/Additional Set of Samples",
 					   "OrthoFinder Homolog Matrix", "Output Directory",
 					   "Pickle File with Annotation Data in Expansion Listing for Quick Loading",
 					   "Run in Quick Mode?", "BGC Prediction Software", "ProtoCore-Like Homolog Group Specifications",
-					   "CPUs"]
+					   "Minimum Segment Size", "Minimum Core Segment Size", "Syntenic Correlation Threshold",
+					   "Transition probability from GCF state to GCF state",
+					   "Transition probability from Background to Background",
+					   "Avoid Orthogroup Matrix Construction for Individual GCF", "Loose Mode",
+					   "All Primary", "CPUs"]
 	util.logParametersToFile(parameters_file, parameter_names, parameter_values)
 	logObject.info("Done saving parameters!")
 
 	# parse manual proto-core homolog group specifications if provided
 	protocore_hgs = None
 	if protocore_homologs_file != None:
 		protocore_hgs = {}
@@ -200,21 +222,32 @@
 
 		# Run lsaBGC-Expansion.py for GCF
 		### TODO add additional options in expansion to auto-expansion
 		gcf_exp_outdir = exp_outdir + gcf_id + '/'
 		if not os.path.isdir(gcf_exp_outdir):
 			cmd = ['lsaBGC-Expansion.py', '-g', gcf_listing_file, '-m', orthofinder_matrix_file, '-l',
 				   initial_listing_file, '-p', bgc_prediction_software, '-e', expansion_listing_file,
-				   '-o', gcf_exp_outdir, '-i', gcf_id, '-c', str(cpus)]
+				   '-o', gcf_exp_outdir, '-i', gcf_id, '-ms', min_segment_size, '-mcs', min_segment_core_size,
+				   '-sct', syntenic_correlation_threshold, '-tg', transition_from_bg_to_bg,
+				   '-tb', transition_from_bg_to_bg, '-c', cpus]
+			cmd = [str(cmd_piece) for cmd_piece in cmd]
+
 			if quick_mode:
 				cmd += ['-q']
 			if pickle_expansion_annotation_data_file:
 				cmd += ['-z', pickle_expansion_annotation_data_file]
 			if protocore_hgs != None:
 				cmd += ['-ph', '"' + protocore_hgs[gcf_id] + '"']
+			if no_orthogroup_matrix:
+				cmd += ['-no']
+			if loose_mode:
+				cmd += ['-w']
+			if all_primary:
+				cmd += ['-ap']
+
 			try:
 				util.run_cmd(cmd, logObject, stderr=sys.stderr, stdout=sys.stdout)
 			except:
 				logObject.warning("lsaBGC-Expansion.py was unsuccessful, skipping over GCF %s" % gcf_id)
 				sys.stderr.write("lsaBGC-Expansion.py was unsuccessful, skipping over GCF %s\n" % gcf_id)
 				continue
 		try:
```

### Comparing `lsaBGC-1.35/workflows/lsaBGC-Easy.py` & `lsaBGC-1.36/workflows/lsaBGC-Easy.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,53 +96,54 @@
  	*******************************************************************************************************************
 	""", formatter_class=argparse.RawTextHelpFormatter)
 
 	parser.add_argument('-n', '--taxa_name', help='Name of the taxa of interest as listed in GTDB. If there is a space in the\nname, please surround by quotes.', required=True)
 	parser.add_argument('-g', '--user_genomes_directory', help='A directory with additional genomes, e.g. those recently sequenced by the\nuser, belonging to the taxa. Accepted formats include FASTA.\nAccepted suffices include: .fna, .fa, .fasta.', required=False, default=None)
 	parser.add_argument('-o', '--output_directory', help='Parent output/workspace directory.', required=True)
 	parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO). GECCO is\nautomatic, but for the other two, lsaBGC-Easy will produce a task-file which you will need to run in a\nseperate environment with antiSMASH or DeepBGC installed, then rerun lsaBGC-Easy.py using the\noriginal command [Default is GECCO].', default='gecco', required=False)
-	parser.add_argument('-x', '--ignore_limits', action='store_true', help="Ignore limitations on number of genomes allowed.\nE.g. allow for analyses of taxa with more than 2000 genomes available and more than 100 genomes\nafter dereplication. Not recommend, be cautious!!! Also note,\nyou can always delete \"Dereplicated_Set_of_Genomes.txt\" in the results directory and redo\ndereplication with different threshold.")
+	parser.add_argument('-x', '--ignore_limits', action='store_true', help="Ignore limitations on number of genomes allowed.\nE.g. allow for analyses of taxa with more than 2000 genomes available before dereplication and more than 100 genomes\nafter dereplication. Not recommend, be cautious!!! Also note,\nyou can always delete \"Dereplicated_Set_of_Genomes.txt\" in the results directory and redo\ndereplication with different threshold.")
 	parser.add_argument('-gtm', '--gtotree_model', help="SCG model for secondary GToTree analysis and what would be used for dereplication. [Default is \"Bacteria\"].", default='Bacteria', required=False)
 	parser.add_argument('-iib', '--include_incomplete_bgcs', action='store_true', help="Whether to account for incomplete BGCs (those near contig edges) prior to clustering.", default=False, required=False)
 	parser.add_argument('-b', '--use_bigscape', action='store_true', help="Use BiG-SCAPE for BGC clustering into GCFs instead of lsaBGC-Cluster. Recommended if\nyou want to include incomplete BGCs for clustering and are using antiSMASH.", required=False, default=False)
+	parser.add_argument('-bo', '--bigscape_options', action='store_true', help="Options for BiG-SCAPE clustering of BGCs if requested (should be surrounded by quotes). [Default is \"--hybrids-off --include_singletons\"].", required=False, default="--hybrids-off --include_singletons")
 	parser.add_argument('-lci', '--lsabgc_cluster_inflation', type=float, help='Value for MCL inflation parameter to use in lsaBGC-Cluster [Default is 4.0].', required=False, default=4.0)
 	parser.add_argument('-lcj', '--lsabgc_cluster_jaccard', type=float, help='Minimal Jaccard Index cutoff to regard two BGCs as potentially homologous\nin lsaBGC-Cluster [Default is 20.0].', required=False, default=20.0)
 	parser.add_argument('-lcr', '--lsabgc_cluster_synteny', type=float, help='Minimal absolute correlation coefficient to measure syntenic similarity and\nregard two BGCs as potentially homologous in lsaBGC-Cluster [Default is 0.7].', required=False, default=0.7)
 	parser.add_argument('-pae', '--perform_auto_expansion', action='store_true', help="Perform lsaBGC-AutoExpansion.py to find missing pieces of BGCs due to assembly\nfragmentation. Will increase sensitivity at the potential cost of false positives, recommended for\ntaxa with <10 BGCs per genome or more constrained lineages/species. For genus-wide analyses,\nespecially of BGC-rich organisms, please use expansion manually and assess lsaBGC-See reports\nto filter false positives.", required=False, default=False)
 	parser.add_argument('-sd', '--skip_dereplication', action='store_true', help="Whether to skip dereplication based on GToTree alignments of SCGs - not\nrecommended and can cause issues if there are a lot of\ngenomes for the taxa of interest.", default=False, required=False)
 	parser.add_argument('-dt', '--dereplicate_threshold', type=float, help="Amino acid similarity threshold of SCGs for considering\ntwo genomes as redundant [Default is 0.999].", default=0.999, required=False)
 	parser.add_argument('-pt', '--population_threshold', type=float, help="Amino acid similarity threshold of SCGs for considering\ntwo genomes as belonging to the same population [Default is 0.99].", default=0.99, required=False)
 	parser.add_argument('-py', '--use_pyrodigal', action='store_true', help='Use pyrodigal instead of prodigal.', required=False, default=False)
 	parser.add_argument('-om', '--orthofinder_mode', help="Method for running OrthoFinder2. (Options: Genome_Wide, BGC_Only).\nBGC_Only is experimental but much faster and should work especially well for\ntaxa with many BGCs [Default is Genome_Wide].", default='Genome_Wide', required=False)
 	parser.add_argument('-mc', '--run_coarse_orthofinder', action='store_true', help='Use coarse clustering of homolog groups in OrthoFinder instead of more\nresolute hierarchical determined homolog groups. There are some advantages to coarse\nOGs, including their construction being deterministic.', required=False, default=False)
 	parser.add_argument('-c', '--cpus', type=int, help="Total number of CPUs to use [Default is 4].", required=False, default=4)
-	parser.add_argument('-a', '--antismash_prediction_cpus', type=int, help="Number of CPUs to specify for each antiSMASH command in\ntask file [Default is 4].", required=False, default=4)
-
+	parser.add_argument('-ao', '--antismash_options', help="Options for antiSMASH prediction analysis (should be surrounded by quotes). [Default is \"--genefinding-tool none --cpus 4\"]", required=False, default="--genefinding-tool none --cpus 4")
 	args = parser.parse_args()
 	return args
 
 
 def lsaBGC_Easy():
 	myargs = create_parser()
 
 	taxa_name = myargs.taxa_name.strip('"').strip()
 	outdir = os.path.abspath(myargs.output_directory) + '/'
 	cpus = myargs.cpus
-	bgc_prediction_cpus = myargs.antismash_prediction_cpus
+	antismash_options = myargs.antismash_options
 	user_genomes_directory = myargs.user_genomes_directory
 	bgc_prediction_software = myargs.bgc_prediction_software.upper()
 	gtotree_model = myargs.gtotree_model
 	skip_dereplication_flag = myargs.skip_dereplication
 	include_incomplete_bgcs_flag = myargs.include_incomplete_bgcs
 	perform_auto_expansion_flag = myargs.perform_auto_expansion
 	dereplicate_threshold = myargs.dereplicate_threshold
 	population_threshold = myargs.population_threshold
 	run_coarse_orthofinder = myargs.run_coarse_orthofinder
 	orthofinder_mode = myargs.orthofinder_mode.upper()
 	use_bigscape_flag = myargs.use_bigscape
+	bigscape_options = myargs.bigscape_options
 	ignore_limits_flag = myargs.ignore_limits
 	use_pyrodigal = myargs.use_pyrodigal
 	lsabgc_cluster_inflation = myargs.lsabgc_cluster_inflation
 	lsabgc_cluster_jaccard = myargs.lsabgc_cluster_jaccard
 	lsabgc_cluster_synteny = myargs.lsabgc_cluster_synteny
 
 	try:
@@ -201,15 +202,15 @@
 	genbank_accession_listing_file = outdir + 'NCBI_Genbank_Accession_Listing.txt'
 	sys.stdout.write(
 		"--------------------\nStep 1\n--------------------\nBeginning by assessing which genomic assemblies are available for the taxa %s in GTDB and NCBI's Genbank db\n" % taxa_name)
 	logObject.info(
 		"\n--------------------\nStep 1\n--------------------\nBeginning by assessing which genomic assemblies are available for the taxa %s in GTDB and NCBI's Genbank db" % taxa_name)
 	if not os.path.isfile(genbank_accession_listing_file):
 		genbank_accession_listing_handle = open(genbank_accession_listing_file, 'w')
-		with gzip.open(lsaBGC_main_directory + 'db/GTDB_R207_Information.txt.gz', 'rt') as ogtdb:
+		with gzip.open(lsaBGC_main_directory + 'db/GTDB_R214_Information.txt.gz', 'rt') as ogtdb:
 			for line in ogtdb:
 				line = line.strip('\n')
 				ls = line.split('\t')
 				if ls[0] == 'none': continue
 				if len(taxa_name.split()) == 1:
 					if ls[1] == taxa_name:
 						genbank_accession_listing_handle.write(ls[0] + '\n')
@@ -218,15 +219,15 @@
 						genbank_accession_listing_handle.write(ls[0] + '\n')
 		genbank_accession_listing_handle.close()
 
 	ogalf = open(genbank_accession_listing_file)
 	accession_count = len(ogalf.readlines())
 	ogalf.close()
 
-	if (accession_count >= 2000 or accession_count < 10) and (not ignore_limits_flag):
+	if (accession_count > 2000) and (not ignore_limits_flag) and (not (accession_count < 10 and os.path.isdir(user_genomes_directory))):
 		logObject.error(
 			"Currently not recommended to use lsaBGC-Easy for taxa with > 2000 genomes or < 10 genomes. In the future this will likely be updated to be a warning, but would rather not risk harming your server!")
 		sys.stderr.write(
 			"Currently not recommended to use lsaBGC-Easy for taxa with > 2000 genomes or < 10 genomes.\nIn the future this will likely be updated to be a warning, but would rather not risk harming your computer/server!\n")
 		sys.stderr.write(
 			'Exiting now, but you can move past this if you feel comfortable and are willing to wait for longer processing times using the -x flag.\n')
 		sys.exit(1)
@@ -242,23 +243,14 @@
 			of = open(genome_listing_file, 'w')
 			of.close()
 
 	oglf = open(genome_listing_file)
 	genome_count = len(oglf.readlines())
 	oglf.close()
 
-	if (genome_count >= 2000 or genome_count < 10) and (not ignore_limits_flag):
-		logObject.error(
-			"Currently not recommended to use lsaBGC-Easy for taxa with > 2000 genomes or < 10 genomes. In the future this will likely be updated to be a warning, but would rather not risk harming your server!")
-		sys.stderr.write(
-			"Currently not recommended to use lsaBGC-Easy for taxa with > 2000 genomes or < 10 genomes.\nIn the future this will likely be updated to be a warning, but would rather not risk harming your computer/server!\n")
-		sys.stderr.write(
-			'Exiting now, but you can move past this if you feel comfortable and are willing to wait for longer processing times using the -x flag.\n')
-		sys.exit(1)
-
 	# Step 2: Download all genomes in FASTA format & prodigal gene calling
 	genomes_directory = outdir + 'genbank/'
 	all_genomes_listing_file = outdir + 'All_Genomes_Listing.txt'
 	uncompress_dir = outdir + 'Uncompressed_Genomes/'
 	if not os.path.isfile(all_genomes_listing_file):
 		if genome_count != 0:
 			ngd_real_cmd = ['ncbi-genome-download', '--formats', 'fasta', '--retries', '2', '--section',
@@ -281,14 +273,22 @@
 		oaglf = open(all_genomes_listing_file)
 		genome_included_count = len(oaglf.readlines())
 		oaglf.close()
 		if genome_included_count <= 2:
 			logObject.error('Fewer than 3 genomes downloaded / provided. Exiting as more genomes are needed.')
 			sys.stderr.write('Fewer than 3 genomes downloaded / provided. Exiting as more genomes are needed.\n')
 			sys.exit(1)
+		elif (genome_included_count > 2000 or genome_included_count < 10) and not ignore_limits_flag:
+			logObject.error(
+				"Currently not recommended to use lsaBGC-Easy for taxa with > 2000 genomes or < 10 genomes. In the future this will likely be updated to be a warning, but would rather not risk harming your server!")
+			sys.stderr.write(
+				"Currently not recommended to use lsaBGC-Easy for taxa with > 2000 genomes or < 10 genomes.\nIn the future this will likely be updated to be a warning, but would rather not risk harming your computer/server!\n")
+			sys.stderr.write(
+				'Exiting now, but you can move past this if you feel comfortable and are willing to wait for longer processing times using the -x flag.\n')
+			sys.exit(1)
 		else:
 			logObject.info('Great, we found or downloaded %d genomes belonging to the taxa!' % (genome_included_count))
 			sys.stdout.write(
 				'Great, we found or downloaded %d genomes belonging to the taxa!\n' % (genome_included_count))
 
 	prodigal_results_directory = outdir + 'Prodigal_and_Processing_Results/'
 	all_proteomes_listing_file = outdir + 'All_Proteomes_Listing.txt'
@@ -346,16 +346,26 @@
 	expected_similarities_file = outdir + 'GToTree_Expected_Similarities.txt'
 	logObject.info(
 		'\n--------------------\nStep 3\n--------------------\nBeginning construction of species tree using GToTree.')
 	sys.stdout.write(
 		'--------------------\nStep 3\n--------------------\nBeginning construction of species tree using GToTree.\n')
 	if not os.path.isfile(species_tree_file) or not os.path.isfile(expected_similarities_file):
 		os.system('rm -rf %s' % gtotree_outdir)
-		gtotree_cmd = ['GToTree', '-A', all_proteomes_listing_file, '-H', gtotree_model, '-n', '4', '-j',
-					   str(parallel_jobs_4cpu), '-M', '4', '-o', gtotree_outdir]
+
+		actino_hmm_file = lsaBGC_main_directory + '/db/Actinobacteria.hmm'
+		bacteria_hmm_file = lsaBGC_main_directory + '/db/Bacteria.hmm'
+		universal_hmm_file = lsaBGC_main_directory + '/db/Universal_et_al_Hug.hmm'
+
+		gtotree_model_arg = gtotree_model
+		if gtotree_model == 'Actinobacteria' and os.path.isfile(actino_hmm_file): gtotree_model_arg =  actino_hmm_file
+		elif gtotree_model == 'Bacteria' and os.path.isfile(bacteria_hmm_file): gtotree_model_arg = bacteria_hmm_file
+		elif gtotree_model == 'Universal_et_al_Hug' and os.path.isfile(universal_hmm_file): gtotree_model_arg = universal_hmm_file
+
+		gtotree_cmd = ['GToTree', '-A', all_proteomes_listing_file, '-H', gtotree_model_arg, '-n', str(max([cpus, 4])),
+					   '-j', str(parallel_jobs_4cpu), '-M', str(max([cpus, 4])), '-o', gtotree_outdir]
 		runCmdViaSubprocess(gtotree_cmd, logObject, check_files=[species_tree_file])
 
 		protein_msa_file = gtotree_outdir + 'Aligned_SCGs.faa'
 		pair_seq_matching = util.determineSeqSimProteinAlignment(protein_msa_file)
 		expected_sim_handle = open(expected_similarities_file, 'w')
 		for s1 in pair_seq_matching:
 			for s2 in pair_seq_matching:
@@ -482,20 +492,23 @@
 			'Found prior determined population/clade inference and sample listing files. Using them instead of reassessing them.\n')
 
 	count_of_dereplicated_sample_set = 0
 	with open(samples_to_keep_file) as oskf:
 		for line in oskf:
 			count_of_dereplicated_sample_set += 1
 	if (count_of_dereplicated_sample_set > 100) and (not ignore_limits_flag):
-		logObject.error(
-			"Currently not recommended to use lsaBGC-Easy for taxa with > 100 genomes after dereplication. In the future this will likely be updated to be a warning, but would rather not risk harming your computer/server!")
-		sys.stderr.write(
-			"Currently not recommended to use lsaBGC-Easy for taxa with > 100 genomes\nafter dereplication. In the future this will likely be updated\nto be a warning, but would rather not risk harming\nyour computer/server!")
-		sys.stderr.write(
-			'Exiting now, but you can move past this if you feel comfortable and are willing to wait for longer processing times using the -x flag.\n')
+		logObject.error("Currently not recommended to use lsaBGC-Easy for taxa with > 100 genomes after dereplication. In the future this will likely be updated to be a warning, but would rather not risk harming your computer/server!")
+		sys.stderr.write("Currently not recommended to use lsaBGC-Easy for taxa with > 100 genomes\nafter dereplication. In the future this will likely be updated\nto be a warning, but would rather not risk harming\nyour computer/server!")
+		sys.stderr.write("Exiting now, but you can move past this if you feel comfortable and are willing to wait for longer processing times using the -x flag.\n")
+		sys.exit(1)
+	elif (count_of_dereplicated_sample_set > 300):
+		logObject.error("You have >300 genomes after dereplication and probably don't want to continue - OrthoFinder will need to perform a lot of pairwise comparisons... over 90K! You can reperform dereplication using more stringent thresholds to get fewer genomes.")
+		sys.stderr.write("You have >300 genomes after dereplication and probably don't want to continue - OrthoFinder will need to perform a lot of pairwise comparisons... over 90K! You can reperform dereplication using more stringent thresholds to get fewer genomes.\n")
+		sys.stderr.write("Exiting now, if you really must get past this and feel comfortable - you can edit this program.\n")
+		sys.exit(1)
 	else:
 		logObject.info(
 			"After dereplication (if performed) there are %d samples/genomes being considered." % count_of_dereplicated_sample_set)
 		sys.stdout.write(
 			"After dereplication (if performed) there are %d samples/genomes being considered.\n" % count_of_dereplicated_sample_set)
 
 	checkUlimitSettings(count_of_dereplicated_sample_set, logObject)
@@ -522,17 +535,16 @@
 					gecco_cmd = ['gecco', 'run', '-j', '4', '-o', primary_bgc_pred_directory + s + '/', '-g',
 								 all_genome_listings_fna[s]]
 					if not include_incomplete_bgcs_flag:
 						gecco_cmd += ['-E', '10']
 					gecco_cmd += [logObject]
 					primary_bgc_pred_cmds.append(gecco_cmd)
 				if bgc_prediction_software == 'ANTISMASH':
-					antismash_cmd = ['antismash', '--output-dir', primary_bgc_pred_directory + s + '/', '-c',
-									 str(bgc_prediction_cpus), '--genefinding-tool', 'none', '--output-basename', s,
-									 all_genome_listings_gbk[s]]
+					antismash_cmd = ['antismash', '--output-dir', primary_bgc_pred_directory + s + '/',
+									 antismash_options, '--output-basename', s, all_genome_listings_gbk[s]]
 					primary_bgc_pred_cmds.append(antismash_cmd)
 				elif bgc_prediction_software == 'DEEPBGC':
 					deepbgc_cmd = ['deepbgc', 'pipeline', '--output', primary_bgc_pred_directory + s + '/',
 								   all_genome_listings_fna[s]]
 					primary_bgc_pred_cmds.append(deepbgc_cmd)
 		primary_genomes_listing_handle.close()
 
@@ -584,15 +596,15 @@
 	bigscape_listing_file = lsaBGC_main_directory + 'external_tools/bigscape_location.txt'
 	bigscape_prog_location, pfam_directory = [None] * 2
 	if os.path.isfile(bigscape_listing_file):
 		bigscape_prog_location, pfam_directory = open(bigscape_listing_file).readlines()[0].strip().split('\t')
 	bigscape_results_dir = outdir + 'BiG_SCAPE_Clustering_Results/'
 	if use_bigscape_flag and not os.path.isdir(bigscape_results_dir) and os.path.isfile(bigscape_prog_location):
 		bigscape_cmd = ['python', bigscape_prog_location, '-i', primary_bgc_pred_directory, '-o', bigscape_results_dir,
-						'-c', str(cpus), '--include_singletons', '--pfam_dir', pfam_directory]
+						'-c', str(cpus), '--pfam_dir', pfam_directory, bigscape_options]
 		runCmdViaSubprocess(bigscape_cmd, logObject, check_directories=[bigscape_results_dir])
 		try:
 			assert (os.path.isdir(bigscape_results_dir + 'network_files/'))
 		except:
 			logObject.error("Something unexpected in BiG-SCAPE processing occurred.")
 			sys.stderr.write("Something unexpected in BiG-SCAPE processing occurred.\n")
 			exit(1)
@@ -670,15 +682,15 @@
 								  '-mb', '-m', exp_orthogroups_matrix_file, '-s', species_tree_file, '-w',
 								  expected_similarities_file, '-k', samples_to_keep_file, '-c', str(cpus), '-o',
 								  lsabgc_autoanalyze_dir, '-p', bgc_prediction_software, '-u', population_file,
 								  '-ogm', orthogroups_matrix_file]
 		runCmdViaSubprocess(lsabgc_autoanalyze_cmd, logObject, check_directories=[lsabgc_autoanalyze_results_dir])
 
 
-	# Step 8: Run lsaBGC-AutoAnalyze.py
+	# Step 8: Run GSeeF.py
 	logObject.info('\n--------------------\nStep 8\n--------------------\nBeginning GSeeF analysis.')
 	sys.stdout.write('--------------------\nStep 8\n--------------------\nBeginning GSeeF analysis.')
 
 	gseef_results_dir = outdir + 'GSeeF_Results/'
 	gseef_final_results_dir = gseef_results_dir + 'Final_Results/'
 	if not os.path.isdir(gseef_results_dir):
 		os.system('rm -rf %s' % gseef_results_dir)
```

### Comparing `lsaBGC-1.35/workflows/lsaBGC-Euk-Easy.py` & `lsaBGC-1.36/workflows/lsaBGC-Euk-Easy.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,48 +85,50 @@
 		- Step 7: Run lsaBGC-AutoAnalyze.py
 		- Step 8: Run GSeeF.py
 	*******************************************************************************************************************
 	""", formatter_class=argparse.RawTextHelpFormatter)
 
 	parser.add_argument('-g', '--genomes_directory', help='A directory with additional genomes, e.g. those recently sequenced by the\nuser, belonging to the taxa. Must be full GenBanks with gene-calling already performed and\nCDS features available.', required=True)
 	parser.add_argument('-o', '--output_directory', help='Parent output/workspace directory.', required=True)
-	parser.add_argument('-x', '--ignore_limits', action='store_true', help="Ignore limitations on number of genomes allowed.\nE.g. allow for analyses of taxa with more than 2000 genomes available and more than 100 genomes\nafter dereplication. Not recommend, be cautious!!! Also note,\nyou can always delete \"Dereplicated_Set_of_Genomes.txt\" in the results directory and redo\ndereplication with different threshold.")
+	parser.add_argument('-x', '--ignore_limits', action='store_true', help="Ignore limitations on number of genomes allowed.\nE.g. allow for analyses of taxa with more than 2000 genomes available before dereplication and more than 100 genomes\nafter dereplication. Not recommend, be cautious!!! Also note,\nyou can always delete \"Dereplicated_Set_of_Genomes.txt\" in the results directory and redo\ndereplication with different threshold.")
 	parser.add_argument('-iib', '--include_incomplete_bgcs', action='store_true', help="Whether to account for incomplete BGCs prior to clustering -\nnot recommended.", default=False, required=False)
 	parser.add_argument('-b', '--use_bigscape', action='store_true', help="Use BiG-SCAPE for BGC clustering into GCFs instead of lsaBGC-Cluster.\nRecommended if you want to include incomplete BGCs for clustering and are using\nantiSMASH.", required=False, default=False)
+	parser.add_argument('-bo', '--bigscape_options', action='store_true', help="Options for BiG-SCAPE clustering of BGCs if requested (should be surrounded by quotes). [Default is \"--hybrids-off --include_singletons\"].", required=False, default="--hybrids-off --include_singletons")
 	parser.add_argument('-lci', '--lsabgc_cluster_inflation', type=float, help='Value for MCL inflation parameter to use in lsaBGC-Cluster [Default is 4.0].', required=False, default=4.0)
 	parser.add_argument('-lcj', '--lsabgc_cluster_jaccard', type=float, help='Minimal Jaccard Index cutoff to regard two BGCs as potentially homologous\nin lsaBGC-Cluster [Default is 20.0].', required=False, default=20.0)
 	parser.add_argument('-lcr', '--lsabgc_cluster_synteny', type=float, help='Minimal absolute correlation coefficient to measure syntenic similarity and\nregard two BGCs as potentially homologous in lsaBGC-Cluster [Default is 0.7].', required=False, default=0.7)
 	parser.add_argument('-pae', '--perform_auto_expansion', action='store_true', help="Perform lsaBGC-AutoExpansion.py to find missing pieces of BGCs due to assembly\nfragmentation. Will increase sensitivity at the potential cost of false positives, recommended for\ntaxa with <10 BGCs per genome or more constrained lineages/species. For genus-wide analyses,\nespecially of BGC-rich organisms, please use expansion manually and assess lsaBGC-See reports\nto filter false positives.", required=False, default=False)
 	parser.add_argument('-dt', '--dereplicate_threshold', type=float, help="Amino acid similarity threshold of SCGs for considering\ntwo genomes as redundant [Default is 0.999].", default=0.999, required=False)
 	parser.add_argument('-sd', '--skip_dereplication', action='store_true', help="Whether to skip dereplication based on GToTree alignments of SCGs - not\nrecommended and can cause issues if there are a lot of genomes for the taxa\nof interest.", default=False, required=False)
 	parser.add_argument('-pt', '--population_threshold', type=float, help="Amino acid similarity threshold of SCGs for considering\ntwo genomes as belonging to the same population [Default is 0.99].", default=0.99, required=False)
 	parser.add_argument('-om', '--orthofinder_mode', help="Method for running OrthoFinder2. (Options: Genome_Wide, BGC_Only).\nDefault is Genome_Wide (BGC_Only is slightly experimental but much faster and should work\nespecially well for taxa with many BGCs).", default='Genome_Wide', required=False)
 	parser.add_argument('-mc', '--run_coarse_orthofinder', action='store_true', help='Use coarse clustering of homolog groups in OrthoFinder instead\nof more resolute hierarchical determined homolog groups. There are some advantages to\ncoarse OGs, including their construction being deterministic.', required=False, default=False)
 	parser.add_argument('-c', '--cpus', type=int, help="Total number of CPUs to use [Default is 4].", required=False, default=4)
-	parser.add_argument('-a', '--antismash_prediction_cpus', type=int, help="Number of CPUs to specify for each antiSMASH command in\ntask file [Default is 4].", required=False, default=4)
+	parser.add_argument('-ao', '--antismash_options', help="Options for antiSMASH prediction analysis (should be surrounded by quotes). [Default is \"--taxon fungi --genefinding-tool none --cpus 4\"]", required=False, default="--taxon fungi --genefinding-tool none --cpus 4")
 
 	args = parser.parse_args()
 	return args
 
 
 def lsaBGC_Euk_Easy():
 	myargs = create_parser()
 
 	outdir = os.path.abspath(myargs.output_directory) + '/'
 	cpus = myargs.cpus
-	bgc_prediction_cpus = myargs.antismash_prediction_cpus
+	antismash_options = myargs.antismash_options
 	genomes_directory = myargs.genomes_directory
 	skip_dereplication_flag = myargs.skip_dereplication
 	include_incomplete_bgcs_flag = myargs.include_incomplete_bgcs
 	perform_auto_expansion_flag = myargs.perform_auto_expansion
 	dereplicate_threshold = myargs.dereplicate_threshold
 	population_threshold = myargs.population_threshold
 	run_coarse_orthofinder = myargs.run_coarse_orthofinder
 	orthofinder_mode = myargs.orthofinder_mode.upper()
 	use_bigscape_flag = myargs.use_bigscape
+	bigscape_options = myargs.bigscape_options
 	ignore_limits_flag = myargs.ignore_limits
 	lsabgc_cluster_inflation = myargs.lsabgc_cluster_inflation
 	lsabgc_cluster_jaccard = myargs.lsabgc_cluster_jaccard
 	lsabgc_cluster_synteny = myargs.lsabgc_cluster_synteny
 
 	try:
 		assert (orthofinder_mode in set(['GENOME_WIDE', 'BGC_ONLY']))
@@ -205,14 +207,22 @@
 		oaglf = open(all_genomes_listing_file)
 		genome_included_count = len(oaglf.readlines())
 		oaglf.close()
 		if genome_included_count <= 2:
 			logObject.error('Fewer than 3 genomes provided. Exiting as more genomes are needed.')
 			sys.stderr.write('Fewer than 3 genomes provided. Exiting as more genomes are needed.\n')
 			sys.exit(1)
+		elif (genome_included_count > 2000 or genome_included_count < 10) and not ignore_limits_flag:
+			logObject.error(
+				"Currently not recommended to use lsaBGC-Easy for taxa with > 2000 genomes or < 10 genomes. In the future this will likely be updated to be a warning, but would rather not risk harming your server!")
+			sys.stderr.write(
+				"Currently not recommended to use lsaBGC-Easy for taxa with > 2000 genomes or < 10 genomes.\nIn the future this will likely be updated to be a warning, but would rather not risk harming your computer/server!\n")
+			sys.stderr.write(
+				'Exiting now, but you can move past this if you feel comfortable and are willing to wait for longer processing times using the -x flag.\n')
+			sys.exit(1)
 		else:
 			logObject.info('Great, we found %d genomes belonging to the taxa!' % (genome_included_count))
 			sys.stdout.write('Great, we found %d genomes belonging to the taxa!\n' % (genome_included_count))
 
 	proteome_directory = outdir + 'Proteomes/'
 	genbank_directory = outdir + 'GenBanks_Genomes/'
 	namemapping_directory = outdir + 'Name_Mapping/'
@@ -277,16 +287,21 @@
 	gtotree_outdir = outdir + 'GToTree_output/'
 	species_tree_file = gtotree_outdir + 'GToTree_output.tre'
 	expected_similarities_file = outdir + 'GToTree_Expected_Similarities.txt'
 	logObject.info('\n--------------------\nStep 3\n--------------------\nBeginning construction of species tree using GToTree.')
 	sys.stdout.write('--------------------\nStep 3\n--------------------\nBeginning construction of species tree using GToTree.\n')
 	if not os.path.isfile(species_tree_file) or not os.path.isfile(expected_similarities_file):
 		os.system('rm -rf %s' % gtotree_outdir)
-		gtotree_cmd = ['GToTree', '-A', all_proteomes_listing_file, '-H', 'Universal_Hug_et_al', '-n', '4', '-j',
-					   str(parallel_jobs_4cpu), '-M', '4', '-o', gtotree_outdir]
+		universal_hmm_file = lsaBGC_main_directory + '/db/Universal_Hug_et_al.hmm'
+
+		gtotree_model_arg = "Universal_Hug_et_al"
+		if os.path.isfile(universal_hmm_file): gtotree_model_arg = universal_hmm_file
+
+		gtotree_cmd = ['GToTree', '-A', all_proteomes_listing_file, '-H', gtotree_model_arg, '-n', str(max([cpus, 4])),
+					   '-j', str(parallel_jobs_4cpu), '-M', str(max([cpus, 4])), '-o', gtotree_outdir]
 		runCmdViaSubprocess(gtotree_cmd, logObject, check_files=[species_tree_file])
 
 		protein_msa_file = gtotree_outdir + 'Aligned_SCGs.faa'
 		pair_seq_matching = util.determineSeqSimProteinAlignment(protein_msa_file)
 		expected_sim_handle = open(expected_similarities_file, 'w')
 		for s1 in pair_seq_matching:
 			for s2 in pair_seq_matching:
@@ -419,14 +434,20 @@
 	if (count_of_dereplicated_sample_set > 100) and (not ignore_limits_flag):
 		logObject.error(
 			"Currently not recommended to use lsaBGC-Easy for taxa with > 100 genomes after dereplication. In the future this will likely be updated to be a warning, but would rather not risk harming your computer/server!")
 		sys.stderr.write(
 			"Currently not recommended to use lsaBGC-Easy for taxa with > 100 genomes\nafter dereplication. In the future this will likely be updated\nto be a warning, but would rather not risk harming\nyour computer/server!")
 		sys.stderr.write(
 			'Exiting now, but you can move past this if you feel comfortable and are willing to wait for longer processing times using the -x flag.\n')
+		sys.exit(1)
+	elif (count_of_dereplicated_sample_set > 300):
+		logObject.error("You have >300 genomes after dereplication and probably don't want to continue - OrthoFinder will need to perform a lot of pairwise comparisons... over 90K! You can reperform dereplication using more stringent thresholds to get fewer genomes.")
+		sys.stderr.write("You have >300 genomes after dereplication and probably don't want to continue - OrthoFinder will need to perform a lot of pairwise comparisons... over 90K! You can reperform dereplication using more stringent thresholds to get fewer genomes.\n")
+		sys.stderr.write("Exiting now, if you really must get past this and feel comfortable - you can edit this program.\n")
+		sys.exit(1)
 	else:
 		logObject.info(
 			"After dereplication (if performed) there are %d samples/genomes being considered." % count_of_dereplicated_sample_set)
 		sys.stdout.write(
 			"After dereplication (if performed) there are %d samples/genomes being considered.\n" % count_of_dereplicated_sample_set)
 
 	checkUlimitSettings(count_of_dereplicated_sample_set, logObject)
@@ -441,16 +462,15 @@
 		primary_genomes_listing_handle = open(primary_genomes_listing_file, 'w')
 		util.setupReadyDirectory([primary_bgc_pred_directory])
 		primary_bgc_pred_cmds = []
 		with open(samples_to_keep_file) as oskf:
 			for s in oskf:
 				s = s.strip()
 				primary_genomes_listing_handle.write(s + '\t' + all_genome_listings_gbk[s] + '\n')
-				antismash_cmd = ['antismash', '--output-dir', primary_bgc_pred_directory + s + '/', '-c',
-								 str(bgc_prediction_cpus), '--taxon', 'fungi', '--genefinding-tool', 'none',
+				antismash_cmd = ['antismash', '--output-dir', primary_bgc_pred_directory + s + '/', antismash_options,
 								 '--output-basename', s, all_genome_listings_gbk[s]]
 				primary_bgc_pred_cmds.append(antismash_cmd)
 		primary_genomes_listing_handle.close()
 
 		cmd_handle = open(cmd_file, 'w')
 		for cmd in primary_bgc_pred_cmds:
 			cmd_handle.write(' '.join(cmd) + '\n')
@@ -485,15 +505,15 @@
 	bigscape_listing_file = lsaBGC_main_directory + 'external_tools/bigscape_location.txt'
 	bigscape_prog_location, pfam_directory = [None] * 2
 	if os.path.isfile(bigscape_listing_file):
 		bigscape_prog_location, pfam_directory = open(bigscape_listing_file).readlines()[0].strip().split('\t')
 	bigscape_results_dir = outdir + 'BiG_SCAPE_Clustering_Results/'
 	if use_bigscape_flag and not os.path.isdir(bigscape_results_dir) and os.path.isfile(bigscape_prog_location):
 		bigscape_cmd = ['python', bigscape_prog_location, '-i', primary_bgc_pred_directory, '-o', bigscape_results_dir,
-						'-c', str(cpus), '--include_singletons', '--pfam_dir', pfam_directory]
+						'-c', str(cpus), '--pfam_dir', pfam_directory, bigscape_options]
 		runCmdViaSubprocess(bigscape_cmd, logObject, check_directories=[bigscape_results_dir])
 		try:
 			assert (os.path.isdir(bigscape_results_dir + 'network_files/'))
 		except:
 			logObject.error("Something unexpected in BiG-SCAPE processing occurred.")
 			sys.stderr.write("Something unexpected in BiG-SCAPE processing occurred.\n")
 			exit(1)
@@ -567,15 +587,15 @@
 								  '-m', exp_orthogroups_matrix_file, '-mb', '-s', species_tree_file, '-w',
 								  expected_similarities_file, '-k', samples_to_keep_file, '-c', str(cpus), '-o',
 								  lsabgc_autoanalyze_dir, '-p', 'antiSMASH', '-u', population_file,
 								  '-ogm', orthogroups_matrix_file]
 		runCmdViaSubprocess(lsabgc_autoanalyze_cmd, logObject, check_directories=[lsabgc_autoanalyze_results_dir])
 
 
-	# Step 8: Run lsaBGC-AutoAnalyze.py
+	# Step 8: Run GSeeF.py
 	logObject.info('\n--------------------\nStep 8\n--------------------\nBeginning GSeeF analysis.')
 	sys.stdout.write('--------------------\nStep 8\n--------------------\nBeginning GSeeF analysis.')
 
 	gseef_results_dir = outdir + 'GSeeF_Results/'
 	gseef_final_results_dir = gseef_results_dir + 'Final_Results/'
 	if not os.path.isdir(gseef_results_dir):
 		os.system('rm -rf %s' % gseef_results_dir)
```

