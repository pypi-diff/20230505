# Comparing `tmp/litspy-0.0.6-py3-none-any.whl.zip` & `tmp/litspy-0.0.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 66533 bytes, number of entries: 16
+Zip file size: 66574 bytes, number of entries: 16
 -rwxrwxrwx  2.0 unx        0 b- defN 20-Oct-02 10:02 litspy/__init__.py
--rwxrwxrwx  2.0 unx    27988 b- defN 22-Nov-10 10:41 litspy/__main__.py
+-rwxrwxrwx  2.0 unx    27990 b- defN 23-May-05 10:53 litspy/__main__.py
 -rwxrwxrwx  2.0 unx     1375 b- defN 20-Oct-02 10:02 litspy/alternative_characters.py
 -rwxrwxrwx  2.0 unx     7081 b- defN 22-May-09 18:40 litspy/anatomy_qualifiers.py
 -rwxrwxrwx  2.0 unx    14831 b- defN 20-Oct-02 10:02 litspy/create_html.py
 -rwxrwxrwx  2.0 unx    63403 b- defN 23-Mar-15 10:35 litspy/epmc_query.py
--rwxrwxrwx  2.0 unx    39521 b- defN 22-Nov-10 10:41 litspy/get_synonyms.py
+-rwxrwxrwx  2.0 unx    39576 b- defN 23-May-05 11:05 litspy/get_synonyms.py
 -rwxrwxrwx  2.0 unx    26367 b- defN 22-Nov-10 10:27 litspy/input_args.py
 -rwxrwxrwx  2.0 unx     6378 b- defN 22-Jan-19 10:47 litspy/logger.py
 -rwxrwxrwx  2.0 unx    14533 b- defN 22-May-09 08:41 litspy/noisy_phrases.py
--rwxrwxrwx  2.0 unx    27988 b- defN 22-Nov-10 10:41 litspy-0.0.6.data/scripts/__main__.py
--rwxrwxrwx  2.0 unx     1075 b- defN 23-Mar-15 10:46 litspy-0.0.6.dist-info/LICENCE.txt
--rwxrwxrwx  2.0 unx     8387 b- defN 23-Mar-15 10:46 litspy-0.0.6.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Mar-15 10:46 litspy-0.0.6.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        7 b- defN 23-Mar-15 10:46 litspy-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1270 b- defN 23-Mar-15 10:46 litspy-0.0.6.dist-info/RECORD
-16 files, 240296 bytes uncompressed, 64469 bytes compressed:  73.2%
+-rwxrwxrwx  2.0 unx    27990 b- defN 23-May-05 10:53 litspy-0.0.6.1.data/scripts/__main__.py
+-rwxrwxrwx  2.0 unx     1075 b- defN 23-May-05 11:28 litspy-0.0.6.1.dist-info/LICENCE.txt
+-rwxrwxrwx  2.0 unx     8389 b- defN 23-May-05 11:28 litspy-0.0.6.1.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-May-05 11:28 litspy-0.0.6.1.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        7 b- defN 23-May-05 11:28 litspy-0.0.6.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1282 b- defN 23-May-05 11:28 litspy-0.0.6.1.dist-info/RECORD
+16 files, 240369 bytes uncompressed, 64486 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -24,26 +24,26 @@
 
 Filename: litspy/logger.py
 Comment: 
 
 Filename: litspy/noisy_phrases.py
 Comment: 
 
-Filename: litspy-0.0.6.data/scripts/__main__.py
+Filename: litspy-0.0.6.1.data/scripts/__main__.py
 Comment: 
 
-Filename: litspy-0.0.6.dist-info/LICENCE.txt
+Filename: litspy-0.0.6.1.dist-info/LICENCE.txt
 Comment: 
 
-Filename: litspy-0.0.6.dist-info/METADATA
+Filename: litspy-0.0.6.1.dist-info/METADATA
 Comment: 
 
-Filename: litspy-0.0.6.dist-info/WHEEL
+Filename: litspy-0.0.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: litspy-0.0.6.dist-info/top_level.txt
+Filename: litspy-0.0.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: litspy-0.0.6.dist-info/RECORD
+Filename: litspy-0.0.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## litspy/__main__.py

```diff
@@ -250,16 +250,16 @@
             df['TaxID'] = self.args.tax_id
             df['Keyword'] = self.args.kwds
 
         # clean the data
         self.logger.info("Processing submitted genes to remove clone-based gene names and gene map locations")
         df.drop_duplicates(inplace=True)  # remove duplicate rows
 
-        clone_name_df = df[df['UniProtID'].str.match(r"[A-Z]{2,}\d{6}\.\d")]
-        map_name_df = df[df['UniProtID'].str.match(r"\d{1,2}[pq]\d+\.?\d*")]
+        clone_name_df = df[df['UniProtID'].str.match(r"0[A-Z]{2,}\d{6}\.\d")]
+        map_name_df = df[df['UniProtID'].str.match(r"Z\d{1,2}[pq]\d+\.?\d*")]
         dirty_df = pandas.concat([clone_name_df, map_name_df])
 
         df.drop(dirty_df.index, inplace=True)
 
         self.logger.info(f"Done processing submitted genes. {len(dirty_df)} removed.")
 
         if not dirty_df.empty:
```

## litspy/get_synonyms.py

```diff
@@ -762,16 +762,17 @@
         """
         process the query result to obtain a list of synonyms
         :param res: result object from querying Uniprot
         :return: list of syns
         """
         gene_syns_found = False
 
-        # process the retrieved text in to a list of gene synonyms
+        # process the retrieved text into a list of gene synonyms
         gene_syns = res.text.replace("Gene names", "")
+        gene_syns = res.text.replace("Gene Names", "")
         gene_syns = gene_syns.strip()
         if gene_syns == "":
             gene_syns = [self.gene_id]
         else:
             gene_syns = re.split(r"[\n ]", gene_syns)
             self.logger.info(f"{threading.current_thread().name}: Uniprot synonyms {gene_syns} "
                              f"found for {self.gene_id}")
```

## Comparing `litspy-0.0.6.data/scripts/__main__.py` & `litspy-0.0.6.1.data/scripts/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,16 +250,16 @@
             df['TaxID'] = self.args.tax_id
             df['Keyword'] = self.args.kwds
 
         # clean the data
         self.logger.info("Processing submitted genes to remove clone-based gene names and gene map locations")
         df.drop_duplicates(inplace=True)  # remove duplicate rows
 
-        clone_name_df = df[df['UniProtID'].str.match(r"[A-Z]{2,}\d{6}\.\d")]
-        map_name_df = df[df['UniProtID'].str.match(r"\d{1,2}[pq]\d+\.?\d*")]
+        clone_name_df = df[df['UniProtID'].str.match(r"0[A-Z]{2,}\d{6}\.\d")]
+        map_name_df = df[df['UniProtID'].str.match(r"Z\d{1,2}[pq]\d+\.?\d*")]
         dirty_df = pandas.concat([clone_name_df, map_name_df])
 
         df.drop(dirty_df.index, inplace=True)
 
         self.logger.info(f"Done processing submitted genes. {len(dirty_df)} removed.")
 
         if not dirty_df.empty:
```

## Comparing `litspy-0.0.6.dist-info/LICENCE.txt` & `litspy-0.0.6.1.dist-info/LICENCE.txt`

 * *Files identical despite different names*

## Comparing `litspy-0.0.6.dist-info/METADATA` & `litspy-0.0.6.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litspy
-Version: 0.0.6
+Version: 0.0.6.1
 Summary: Searches through all titles and abstracts available in Europe PMC for co-occurrence of supplied terms (and their synonyms where available), and produces summaries of the search results.
 Home-page: https://github.com/ec339/litspy/tree/master/litspy
 Author: Emma Croot
 Author-email: ec339@le.ac.uk
 License: LICENCE.txt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

## Comparing `litspy-0.0.6.dist-info/RECORD` & `litspy-0.0.6.1.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 litspy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-litspy/__main__.py,sha256=n_wYVHxszet7DlHkkkxp7EZ8Zr5JisWBwvsqatAWDjU,27988
+litspy/__main__.py,sha256=dLsxANup0Ctzn6siH2KKVApgha1Rj21DgXf1xoOnBMg,27990
 litspy/alternative_characters.py,sha256=5uOpbkt-SYJtDTs5WiRlCvVcKJ02KbWWA4-P9STcats,1375
 litspy/anatomy_qualifiers.py,sha256=oe4DRGTY_0DYooHJZRxwGSfGckaMcuqY5GchxTAD62A,7081
 litspy/create_html.py,sha256=19ZAhyPOTTXLo62Kl6pROpKA7cKy6FS3fb1BSlNvB6I,14831
 litspy/epmc_query.py,sha256=byV3YgJhkT49l7GVKGhBRbT9j-1Eh_svU4ixtVBFJYE,63403
-litspy/get_synonyms.py,sha256=6Ldv9ZShzZmENHsgKy4s0yq_tT0-XjFpaCnEFMDKgSU,39521
+litspy/get_synonyms.py,sha256=3sNznqoHxaGKQ9-_WngwsI-7PW98qwkA0obIVGeNH5Y,39576
 litspy/input_args.py,sha256=N8dy18R-nVgDc2PpT97Qwco_4ahEvgOqOOqO3dJYpjI,26367
 litspy/logger.py,sha256=v32aNM9lnbOxtzjyM4J07LtzMwVl2afSOWFG_oQpy50,6378
 litspy/noisy_phrases.py,sha256=iAXZ0Ua5Kk-dGAIUHV4pVPGxQhN-DvC4TnFtJZj8Y0A,14533
-litspy-0.0.6.data/scripts/__main__.py,sha256=n_wYVHxszet7DlHkkkxp7EZ8Zr5JisWBwvsqatAWDjU,27988
-litspy-0.0.6.dist-info/LICENCE.txt,sha256=zIaHx_rOy10zxmbwXnKXFgbrb-riKXRBw4geirfI-L8,1075
-litspy-0.0.6.dist-info/METADATA,sha256=ciXXDun-d28PoEItF52lsFMsQLFyljiwk7onD52Msok,8387
-litspy-0.0.6.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-litspy-0.0.6.dist-info/top_level.txt,sha256=qbUYsaYmsG4yhMMC8IK0tuR1bnhCzbxkqZyx4UCD76w,7
-litspy-0.0.6.dist-info/RECORD,,
+litspy-0.0.6.1.data/scripts/__main__.py,sha256=dLsxANup0Ctzn6siH2KKVApgha1Rj21DgXf1xoOnBMg,27990
+litspy-0.0.6.1.dist-info/LICENCE.txt,sha256=zIaHx_rOy10zxmbwXnKXFgbrb-riKXRBw4geirfI-L8,1075
+litspy-0.0.6.1.dist-info/METADATA,sha256=scrQUcpD2IuT8ALQxkJvG_ZrJu6zMDyuCtfIOc9W3F8,8389
+litspy-0.0.6.1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+litspy-0.0.6.1.dist-info/top_level.txt,sha256=qbUYsaYmsG4yhMMC8IK0tuR1bnhCzbxkqZyx4UCD76w,7
+litspy-0.0.6.1.dist-info/RECORD,,
```

