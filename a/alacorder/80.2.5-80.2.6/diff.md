# Comparing `tmp/alacorder-80.2.5.tar.gz` & `tmp/alacorder-80.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.2.5.tar", max compression
+gzip compressed data, was "alacorder-80.2.6.tar", max compression
```

## Comparing `alacorder-80.2.5.tar` & `alacorder-80.2.6.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.2.5/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.2.5/README.md
--rw-r--r--   0        0        0      697 2023-05-05 14:51:55.941968 alacorder-80.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.2.5/src/alacorder/__init__.py
--rw-r--r--   0        0        0   216932 2023-05-05 14:51:33.966359 alacorder-80.2.5/src/alacorder/__main__.py
--rw-r--r--   0        0        0   216932 2023-05-05 14:51:18.624013 alacorder-80.2.5/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.2.6/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.2.6/README.md
+-rw-r--r--   0        0        0      697 2023-05-05 15:34:46.288301 alacorder-80.2.6/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-05 15:35:05.911439 alacorder-80.2.6/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.2.6/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   219831 2023-05-05 15:35:57.869401 alacorder-80.2.6/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   219831 2023-05-05 15:35:47.118259 alacorder-80.2.6/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.2.6/PKG-INFO
```

### Comparing `alacorder-80.2.5/LICENSE` & `alacorder-80.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.2.5/README.md` & `alacorder-80.2.6/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.2.5/pyproject.toml` & `alacorder-80.2.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.2.5"
+version = "80.2.6"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.2.5/src/alacorder/__main__.py` & `alacorder-80.2.6/src/alacorder/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.2.5"
+version = "80.2.6"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -36,14 +36,15 @@
 pl.Config.set_tbl_hide_column_data_types(True)
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 FNAME = f"{name} {version}"
 FSHORT_NAME = f"{name} {'.'.join(version.split('.')[0:-1])}"
 
 prt = print
 
+
 def plog(*msg, cf=None):
     global prt
     if len(msg) == 1:
         msg = msg[0]
         if isinstance(cf, dict):
             try:
                 if cf["LOG"] == True:
@@ -63,14 +64,15 @@
                 except:
                     prt(m)
             elif cf == None:
                 prt(m)
             elif type(cf) == bool and cf:
                 prt(m)
 
+
 print = plog
 
 
 def dlog(*msg, cf=None):
     if type(cf) == bool:
         if cf:
             for m in msg:
@@ -132,14 +134,15 @@
     write(a, cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-MA", True)
     return a
 
+
 def multi(cf):
     """
     Start multitable collection using configuration object `cf`.
     """
     start = time.time()
     df = read(cf)
     print("Parsing case info...", cf=cf)
@@ -454,15 +457,14 @@
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CONVSUM-COMPLETE", True)
     return conv
 
 
-
 #   #   #   #         CONFIGURATION & I/O        #   #   #   #
 
 
 def set(
     inputs,
     outputs=None,
     count=0,
@@ -1111,27 +1113,29 @@
                 x[4].replace("\n", " ") for x in pg.get_text(option="blocks")
             )
         except:
             pass
     text = re.sub(r"(<image\:.+?>)", "", text).strip()
     return text
 
+
 def extract_text_pg_one(path) -> str:
     """
     From path, return text of first page of PDF as string (PyMuPdf engine required!)
     """
     try:
         doc = fitz.open(path)
     except:
         return ""
     text = " \n ".join(
-                x[4].replace("\n", " ") for x in doc[0].get_text(option="blocks")
-            )
+        x[4].replace("\n", " ") for x in doc[0].get_text(option="blocks")
+    )
     return text
 
+
 def append_archive(inpath="", outpath="", cf=None):
     """
     Append the contents of one archive to another.
 
     Args:
         inpath (str): Input archive
         outpath (str): Output archive
@@ -1171,51 +1175,68 @@
 
     if window:
         window.write_event_value("COMPLETE-AA", True)
     write(out, path=outpath, overwrite=True)
     return out
 
 
-
 def rename_pdfs(cf):
     if isinstance(cf, dict):
         q = cf["QUEUE"]
     elif isinstance(cf, pl.dataframe.frame.DataFrame):
         if "Path" in cf.columns:
             q = cf.select("Path").to_series().to_list()
             cf = {"LOG": False}
     else:
         q = cf
         cf = {"LOG": False}
-    if cf["LOG"]:
+    if cf["LOG"] and not cf["WINDOW"]:
+        print("Renaming cases...")
         for path in tqdm(q):
             text = extract_text_pg_one(path)
             try:
                 cnum = (
                     re.search(r"County: (\d\d)", str(text)).group(1)
                     + "-"
                     + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
                 )
             except:
                 cnum = os.path.split(path)[1]
             newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
             os.rename(path, newpath)
-    else:
+    elif not cf["LOG"]:
         for path in q:
             text = extract_text_pg_one(path)
             try:
                 cnum = (
                     re.search(r"County: (\d\d)", str(text)).group(1)
                     + "-"
                     + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
                 )
             except:
                 cnum = os.path.split(path)[1]
             newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
             os.rename(path, newpath)
+    elif cf["LOG"] and cf["WINDOW"]:
+        print("Renaming cases...")
+        cf["WINDOW"].write_event_value("PROGRESS_TOTAL", len(q))
+        for i, path in enumerate(q):
+            text = [extract_text_pg_one(path)]
+            try:
+                cnum = (
+                    re.search(r"County: (\d\d)", str(text)).group(1)
+                    + "-"
+                    + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
+                )
+            except:
+                cnum = os.path.split(path)[1]
+            newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
+            os.rename(path, newpath)
+            cf["WINDOW"].write_event_value("PROGRESS", i + 1)
+        cf["WINDOW"].write_event_value("RN-COMPLETE", True)
 
 
 def make_pairs_template(df, debug=False):
     if isinstance(df, str):
         df = read(df)
     names = df.with_columns(
         [
@@ -1620,15 +1641,15 @@
             .str.replace(r"\:", "")
             .str.strip()
             .alias("Alias"),
             pl.col("AllPagesText")
             .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
             .str.replace(r"[^\d/]", "")  # _all
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("DOB"),
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
                     pl.lit("-"),
@@ -1637,28 +1658,34 @@
             ).alias("CaseNumber"),
             pl.col("AllPagesText")
             .str.extract(r"(Phone: )(.+)", group_index=2)
             .str.replace_all(r"[^0-9]", "")
             .str.slice(0, 10)
             .str.replace(r"(.{3}0000000)", "")  # _all
             .alias("RE_Phone"),
-            pl.col("AllPagesText").str.extract(r"(B|W|H|A)/(?:F|M)").cast(pl.Categorical).alias("Race"),
-            pl.col("AllPagesText").str.extract(r"(?:B|W|H|A)/(F|M)").cast(pl.Categorical).alias("Sex"),
+            pl.col("AllPagesText")
+            .str.extract(r"(B|W|H|A)/(?:F|M)")
+            .cast(pl.Categorical)
+            .alias("Race"),
+            pl.col("AllPagesText")
+            .str.extract(r"(?:B|W|H|A)/(F|M)")
+            .cast(pl.Categorical)
+            .alias("Sex"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Address 1:)(.+)(?:Phone)*?", group_index=1)
             .str.replace(r"(Phone.+)", "")
             .str.strip()
             .alias("Address1"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Address 2:)(.+)")
             .str.strip()
             .alias("Address2"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Zip: )(.+)", group_index=1)
-            .str.replace(r'[A-Za-z\:\s]+','')
+            .str.replace(r"[A-Za-z\:\s]+", "")
             .str.strip()
             .alias("ZipCode"),
             pl.col("AllPagesText")
             .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=1)
             .str.strip()
             .alias("City"),
             pl.col("AllPagesText")
@@ -1680,65 +1707,64 @@
             .alias("D999RAW"),
             pl.col("AllPagesText")
             .str.extract_all(r"(\w{2}\d{12})")
             .arr.join("/")
             .alias("RelatedCases"),
             pl.col("AllPagesText")
             .str.extract(r"Filing Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("FilingDate"),
             pl.col("AllPagesText")
             .str.extract(r"Case Initiation Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("CaseInitiationDate"),
             pl.col("AllPagesText")
             .str.extract(r"Arrest Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("ArrestDate"),
             pl.col("AllPagesText")
             .str.extract(r"Offense Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("OffenseDate"),
             pl.col("AllPagesText")
             .str.extract(r"Indictment Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("IndictmentDate"),
             pl.col("AllPagesText")
             .str.extract(r"Youthful Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("YouthfulDate"),
             pl.col("AllPagesText")
             .str.extract(r"AL Institutional Service Num: ([^\na-z])")
             .str.strip()
             .alias("ALInstitutionalServiceNum"),
             pl.col("AllPagesText")
             .str.extract(r"Alacourt\.com (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("Retrieved"),
             pl.col("AllPagesText")
             .str.extract(
                 r"Court Action: (BOUND|GUILTY PLEA|WAIVED TO GJ|DISMISSED|TIME LAPSED|NOL PROSS|CONVICTED|INDICTED|DISMISSED|FORFEITURE|TRANSFER|REMANDED|WAIVED|ACQUITTED|WITHDRAWN|PETITION|PRETRIAL|COND\. FORF\.)"
             )
             .alias("CourtAction"),
             pl.col("AllPagesText")
             .str.extract(r"Court Action Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("CourtActionDate"),
             pl.col("AllPagesText")
             .str.extract(r"Charge: ([A-Z\.0-9\-\s]+)")
             .str.rstrip("C")
             .str.strip()
             .alias("Description"),
             pl.col("AllPagesText")
             .str.extract(r"Jury Demand: ([A-Z]+)")
             .cast(pl.Categorical)
             .alias("JuryDemand"),
-            pl.col("AllPagesText").str.extract(
-                r"Inpatient Treatment Ordered: ([YES|NO]?)"
-            )
+            pl.col("AllPagesText")
+            .str.extract(r"Inpatient Treatment Ordered: ([YES|NO]?)")
             .cast(pl.Categorical)
             .alias("InpatientTreatmentOrdered"),
             pl.col("AllPagesText")
             .str.extract(r"Trial Type: ([A-Z]+)")
             .str.replace(r"[S|N]$", "")
             .str.strip()
             .cast(pl.Categorical)
@@ -1834,20 +1860,20 @@
             .str.replace(r"(Enforcement|Party)", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("Country"),
             pl.col("AllPagesText")
             .str.extract(r"(\d\d?/\d\d?/\d\d\d\d) Warrant Issuance Date:")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("WarrantIssuanceDate"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Action Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("WarrantActionDate"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Issuance Status: (\w+)")
             .str.replace(r"Description", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("WarrantIssuanceStatus"),
@@ -1881,38 +1907,39 @@
             .str.extract(r"([\d\.]+) Bond Amount:")
             .cast(pl.Float64, strict=False)
             .alias("BondAmt"),
             pl.col("AllPagesText")
             .str.extract(r"Bond Company: ([A-Z0-9]+)")
             .str.rstrip("S")
             .alias("BondCompany"),
-            pl.col("AllPagesText").str.extract(r"Surety Code: ([A-Z0-9]{4})")
+            pl.col("AllPagesText")
+            .str.extract(r"Surety Code: ([A-Z0-9]{4})")
             .alias("SuretyCode"),
-            pl.col("AllPagesText").str.extract(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            pl.col("AllPagesText")
+            .str.extract(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("BondReleaseDate"),
-            pl.col("AllPagesText").str.extract(
-                r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)"
-            )
-            .str.to_date('%m/%d/%Y', strict=False)
+            pl.col("AllPagesText")
+            .str.extract(r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("FailedToAppearDate"),
             pl.col("AllPagesText")
             .str.extract(
                 r"Bondsman Process Issuance: ([^\n]*?) Bondsman Process Return:"
             )
             .str.strip()
             .alias("BondsmanProcessIssuance"),
             pl.col("AllPagesText")
             .str.extract(r"Bondsman Process Return: (.*?) Number of Subponeas")
             .str.strip()
             .alias("BondsmanProcessReturn"),
             pl.col("AllPagesText")
             .str.extract(r"([\n\s/\d]*?) Appeal Court:")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("AppealDate"),
             pl.col("AllPagesText")
             .str.extract(r"([A-Z\-\s]+) Appeal Case Number")
             .str.strip()
             .cast(pl.Categorical)
             .alias("AppealCourt"),
             pl.col("AllPagesText")
@@ -1927,34 +1954,34 @@
             .str.rstrip("O")
             .str.strip()
             .cast(pl.Categorical)
             .alias("AppealToDesc"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal Status: ([A-Z\-\s]+)")
             .str.rstrip("A")
-            .str.replace_all(r'\n','')
+            .str.replace_all(r"\n", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("AppealStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal To: (\w*) Appeal")
             .str.strip()
             .cast(pl.Categorical)
             .alias("AppealTo"),
             pl.col("AllPagesText")
             .str.extract(r"LowerCourt Appeal Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.replace_all(r"[\n\s:\-]", "")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("LowerCourtAppealDate"),
             pl.col("AllPagesText")
             .str.extract(r"Disposition Date Of Appeal: (\d\d?/\d\d?/\d\d\d\d)")
             .str.replace_all(r"[\n\s:\-]", "")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("DispositionDateOfAppeal"),
             pl.col("AllPagesText")
             .str.extract(r"Disposition Type Of Appeal: [^A-Za-z]+")
             .str.replace_all(r"[\n\s:\-]", "")
             .str.strip()
             .alias("DispositionTypeOfAppeal"),
             pl.col("AllPagesText")
@@ -1966,53 +1993,56 @@
             pl.col("AllPagesText")
             .str.extract(r"Updated By: (\w{3})")
             .str.strip()
             .alias("AdminUpdatedBy"),
             pl.col("AllPagesText")
             .str.extract(r"Transfer to Admin Doc Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("TransferToAdminDocDate"),
             pl.col("AllPagesText")
             .str.extract(r"Transfer Desc: ([A-Z\s]{0,15} \d\d?/\d\d?/\d\d\d\d)")
             .str.replace_all(r"(Transfer Desc:)", "")
             .str.strip()
             .alias("TransferDesc"),
             pl.col("AllPagesText")
             .str.extract(r"Date Trial Began but No Verdict \(TBNV1\): ([^\n]+)")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("TBNV1"),
             pl.col("AllPagesText")
             .str.extract(r"Date Trial Began but No Verdict \(TBNV2\): ([^\n]+)")
             .str.replace(r"Financial", "")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("TBNV2"),
             pl.col("AllPagesText")
             .str.extract(r"TurnOver Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("TurnOverDate"),
             pl.col("AllPagesText")
             .str.extract(r"TurnOver Amt\: \$(\d+\.\d\d)")
             .cast(pl.Float64, strict=False)
             .alias("TurnOverAmt"),
             pl.col("AllPagesText")
             .str.extract(r"Frequency Amt\: \$(\d+\.\d\d)")
             .cast(pl.Float64, strict=False)
             .alias("FrequencyAmt"),
             pl.col("AllPagesText")
             .str.extract(r"Due Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("DueDate"),
             pl.col("AllPagesText")
             .str.extract(r"Last Paid Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("LastPaidDate"),
-            pl.col("AllPagesText").str.extract(r"Payor\: ([A-Z0-9]{4})").cast(pl.Categorical).alias("Payor"),
+            pl.col("AllPagesText")
+            .str.extract(r"Payor\: ([A-Z0-9]{4})")
+            .cast(pl.Categorical)
+            .alias("Payor"),
             pl.col("AllPagesText")
             .str.extract(r"Enforcement Status\: ([A-Z\:,\s]+)")
             .str.replace_all(r"\s+", " ")
             .str.replace(r" F$", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("EnforcementStatus"),
@@ -2028,51 +2058,51 @@
             pl.col("AllPagesText")
             .str.extract(r"PreTrial\: (YES|NO)")
             .cast(pl.Categorical)
             .alias("PreTrial"),
             pl.col("AllPagesText")
             .str.extract(r"PreTrail Date\: (.+)PreTrial")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("PreTrialDate"),
             pl.col("AllPagesText")
             .str.extract(r"PreTrial Terms\: (YES|NO)")
             .cast(pl.Categorical)
             .alias("PreTrialTerms"),
             pl.col("AllPagesText")
             .str.extract(r"Pre Terms Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("PreTermsDate"),
             pl.col("AllPagesText")
             .str.extract(r"Delinquent\: (YES|NO)")
             .cast(pl.Categorical)
             .alias("Delinquent"),
             pl.col("AllPagesText")
             .str.extract(r"Delinquent Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("DelinquentDate"),
             pl.col("AllPagesText")
             .str.extract(r"DA Mailer\: (YES|NO)")
             .cast(pl.Categorical)
             .alias("DAMailer"),
             pl.col("AllPagesText")
             .str.extract(r"DA Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("DAMailerDate"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Mailer\: (YES|NO)")
             .cast(pl.Categorical)
             .alias("WarrantMailer"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("WarrantMailerDate"),
             pl.col("AllPagesText")
             .str.extract(r"Last Update\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("EnforcementLastUpdate"),
             pl.col("AllPagesText")
             .str.extract(r"Updated By\: ([A-Z]{3})")
             .alias("EnforcementUpdatedBy"),
         ]
     )
     cases = cases.with_columns(
@@ -2256,15 +2286,15 @@
         ]
     )
     fh = fh.explode("FinancialHistory")
     fh = fh.with_columns(
         [
             pl.col("FinancialHistory")
             .str.extract(r"(\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("TransactionDate"),
             pl.col("FinancialHistory")
             .str.extract(r"(RECEIPT|CREDIT)")
             .alias("Description"),
             pl.col("FinancialHistory")
             .str.extract(r"(\$\d+\.\d\d)")
             .str.replace(r"\$", "")
@@ -2509,20 +2539,22 @@
             )
             .str.strip()
             .str.replace(r",$", "")
             .str.replace(r"\s+", " ")
             .alias("ChargesSummary")
         ]
     )
-    charges = charges.with_columns([
-        pl.col("CourtActionDate").str.to_date('%m/%d/%Y', strict=False),
-        pl.col("Category").cast(pl.Categorical),
-        pl.col("TypeDescription").cast(pl.Categorical),
-        pl.col("CourtAction").cast(pl.Categorical)
-        ])
+    charges = charges.with_columns(
+        [
+            pl.col("CourtActionDate").str.to_date("%m/%d/%Y", strict=False),
+            pl.col("Category").cast(pl.Categorical),
+            pl.col("TypeDescription").cast(pl.Categorical),
+            pl.col("CourtAction").cast(pl.Categorical),
+        ]
+    )
     charges = charges.select(
         "Name",
         "CaseNumber",
         "Num",
         "Code",
         "Cite",
         "Description",
@@ -2849,143 +2881,147 @@
         [
             pl.col("CaseNumber"),
             pl.col("Sentence")
             .str.extract(r"Sentence\s(\d)\s")
             .cast(pl.Int64, strict=False)
             .alias("Number"),
             pl.col("Sentence")
-            .str.extract(r"Last Update\:\s(\d\d?/\d\d?/\d\d\d\d)\sUpdated By\: [A-Z]{3}")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.extract(
+                r"Last Update\:\s(\d\d?/\d\d?/\d\d\d\d)\sUpdated By\: [A-Z]{3}"
+            )
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("LastUpdate"),
             pl.col("Sentence")
-            .str.extract(r"Last Update\:\s\d\d?/\d\d?/\d\d\d\d\sUpdated By\: ([A-Z]{3})")
+            .str.extract(
+                r"Last Update\:\s\d\d?/\d\d?/\d\d\d\d\sUpdated By\: ([A-Z]{3})"
+            )
             .alias("UpdatedBy"),
             pl.col("Sentence")
             .str.extract(r"Probation Revoke\:(.+?) (Sentence|License)")
-            .str.replace(r'Sentence.*','')
-            .str.replace(r'License.+','')
+            .str.replace(r"Sentence.*", "")
+            .str.replace(r"License.+", "")
             .str.strip()
             .alias("ProbationRevoke"),
             pl.col("Sentence")
             .str.extract(r"License Susp Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
             .alias("LicenseSuspPeriod"),
             pl.col("Sentence")
             .str.extract(r"Days\.\s*(\d+ Years, \d+ Months, \d+ Days\.)\s+")
-            .alias("JailCreditPeriod"), 
+            .alias("JailCreditPeriod"),
             pl.col("Sentence")
             .str.extract(r"Probation Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
             .alias("ProbationPeriod"),
             pl.col("Sentence")
             .str.extract(r"Sentence Provisions\: ([YN])")
             .cast(pl.Categorical)
             .alias("Provisions"),
             pl.col("Sentence")
             .str.extract(r"Requrements Completed\: (YES|NO)")
             .cast(pl.Categorical)
             .alias("RequirementsCompleted"),
             pl.col("Sentence")
             .str.extract(r"Sentence Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("SentenceDate"),
             pl.col("Sentence")
             .str.extract(r"Sentence Start Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("StartDate"),
             pl.col("Sentence")
             .str.extract(r"Sentence End Date\: .{0,40}? (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("EndDate"),
             pl.col("Sentence")
             .str.extract(r"Jail Fee\:(.+?)Costs")
             .str.replace(r"[A-Z]-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("JailFee"),
             pl.col("Sentence")
             .str.extract(r"Costs\: (.+?)Fine\:")
-            .str.replace(r'Fine.+','')
+            .str.replace(r"Fine.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("Costs"),
             # pl.col("Sentence")
-            # .str.extract(r"Fine\:(.+?)Crime Victims") 
+            # .str.extract(r"Fine\:(.+?)Crime Victims")
             # .str.strip()
             # .alias("Fine"),
             # pl.col("Sentence")
             # .str.extract(r"Crime Victims Fee\:(.+?)Monetary")
             # .str.strip()
             # .alias("CrimeVictimsFee"),
             pl.col("Sentence")
-            .str.extract(r"Municipal Court\:(.+?)Fine Suspended") ## NONE
+            .str.extract(r"Municipal Court\:(.+?)Fine Suspended")  ## NONE
             .str.replace(r"X-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("MunicipalCourt"),
             # pl.col("Sentence")
-            # .str.extract(r"Fine Suspended\: (.+?)Immigration Fine") 
+            # .str.extract(r"Fine Suspended\: (.+?)Immigration Fine")
             # .str.strip()
-            # .alias("FineSuspended"), 
+            # .alias("FineSuspended"),
             pl.col("Sentence")
             .str.extract(r"Immigration Fine\: (.+?)Fine")
-            .str.replace(r'X\-\$','')
+            .str.replace(r"X\-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("ImmigrationFine"),
             pl.col("Sentence")
             .str.extract(r"Fine Imposed\: (.+?) Alias Warrant")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("FineImposed"),
             # pl.col("Sentence")
-            # .str.extract(r"Drug Docket Fees\: (.+?)Prelim Hearing") 
+            # .str.extract(r"Drug Docket Fees\: (.+?)Prelim Hearing")
             # .str.replace(r'Prelim Hearing.+','')
             # .str.strip()
             # .alias("DrugDocketFees"),
             pl.col("Sentence")
             .str.extract(r"Prelim Hearing\:(.+?)Amt Over Minimum CVF")
-            .str.replace(r'Amt.+','') 
+            .str.replace(r"Amt.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("PrelimHearing"),
             pl.col("Sentence")
             .str.extract(r"Amt Over Minimum CVF\: (.+?) WC Fee DA")
             .str.replace_all(r"[A-Z\s]|\-|\$", "")
             .cast(pl.Float64, strict=False)
             .alias("AmtOverMinimumCVF"),
             # pl.col("Sentence")
-            # .str.extract(r"WC Fee DA\: (.+?)Removal Bill") 
+            # .str.extract(r"WC Fee DA\: (.+?)Removal Bill")
             # .str.strip()
-            # .alias("WCFeeDA"), 
+            # .alias("WCFeeDA"),
             # pl.col("Sentence")
             # .str.extract(r"Removal Bill\: (.+?)Crime History Fee")
             # .str.strip()
             # .alias("RemovalBill"),
             pl.col("Sentence")
-            .str.extract(r"Crime History Fee\: (.+?) SX10") 
+            .str.extract(r"Crime History Fee\: (.+?) SX10")
             .str.strip()
             .cast(pl.Categorical)
             .alias("CrimeHistoryFee"),
             pl.col("Sentence")
             .str.extract(r"SX10\: (.+?)License Suspension Fee")
             .str.strip()
             .cast(pl.Categorical)
             .alias("SX10"),
             pl.col("Sentence")
             .str.extract(r"License Suspension Fee\: (.+?) WC Fee 85%")
             .str.replace_all(r"[A-Z\s]+", "")
             .cast(pl.Float64, strict=False)
             .alias("LicenseSuspensionFee"),
             pl.col("Sentence")
-            .str.extract(r"WC Fee 85%\: (.+?) Demand Reduction Hearing\:") 
-            .str.replace(r'Demand Reduction Hearing.+','')
+            .str.extract(r"WC Fee 85%\: (.+?) Demand Reduction Hearing\:")
+            .str.replace(r"Demand Reduction Hearing.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("WCFee85"),
             pl.col("Sentence")
-            .str.extract(r"Demand Reduction Hearing\: (.+?)Drug User Fee") 
+            .str.extract(r"Demand Reduction Hearing\: (.+?)Drug User Fee")
             .str.replace_all(r"[A-Z]\-|\s|\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("DemandReductionHearing"),
             pl.col("Sentence")
             .str.extract(r"Drug User Fee\: (.+?) Subpoena")
             .str.strip()
@@ -3018,141 +3054,146 @@
             pl.col("Sentence")
             .str.extract(
                 r"Suspended Confinement Period (\d+ Years, \d+ Months, \d+ Days\.)"
             )
             .alias("SuspendedConfinementPeriod"),
             pl.col("Sentence")
             .str.extract(r"Boot Camp\: (.+?) (Penitentiary|Life Without Parole)")
-            .str.replace(r'Penitentiary.+','')
+            .str.replace(r"Penitentiary.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("BootCamp"),
             pl.col("Sentence")
-            .str.extract(r"Life Without Parole\: (.+?) (Restitution|Death\:)", group_index=1) 
-            .str.replace(r'Death.+','')
-            .str.replace(r'Restitution.+','')
+            .str.extract(
+                r"Life Without Parole\: (.+?) (Restitution|Death\:)", group_index=1
+            )
+            .str.replace(r"Death.+", "")
+            .str.replace(r"Restitution.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("LifeWithoutParole"),
             # pl.col("Sentence")
-            # .str.extract(r"Split\: (.+?) (Concurrent|Confinement)", group_index=1) 
+            # .str.extract(r"Split\: (.+?) (Concurrent|Confinement)", group_index=1)
             # .str.strip()
             # .alias("Split"),
             # pl.col("Sentence")
             # .str.extract(r"Concurrent Sentence\:\s+([A-Z]?)\s")
             # .str.strip()
             # .alias("ConcurrentSentence"),
             # pl.col("Sentence")
-            # .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s") 
+            # .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s")
             # .str.strip()
             # .alias("ConsecutiveSentence"),
             pl.col("Sentence")
             .str.extract(r"Electronic Monitoring\: (.+?) Reverse Split")
             .str.replace_all(r"[-0\s]", "")
             .cast(pl.Categorical)
             .alias("ElectronicMonitoring"),
             pl.col("Sentence")
-            .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)") 
+            .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)")
             .str.replace_all(r"Death\: Life\:", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("ReverseSplit"),
             # pl.col("Sentence")
             # .str.extract(r"Coterminous Sentence\:\s+([A-Z]?)\s")
             # .alias("CoterminousSentence"),
             # pl.col("Sentence").str.extract(r"Death\:\s+(X?)").alias("Death"),
             pl.col("Sentence").str.extract(r"Life\:\s+(X?)").alias("Life"),
             pl.col("Sentence")
             .str.extract(r"Chain Gang\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("ChainGang"),
-            pl.col("Sentence").str.extract(r"Jail\:\s+([0-9]|X?)").cast(pl.Categorical).alias("Jail"),
+            pl.col("Sentence")
+            .str.extract(r"Jail\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
+            .alias("Jail"),
             # pl.col("Sentence")
-            # .str.extract(r"Community Service Hrs\:\s+([0-9]|X?)") 
+            # .str.extract(r"Community Service Hrs\:\s+([0-9]|X?)")
             # .alias("CommunityServiceHrs"),
             pl.col("Sentence")
             .str.extract(r"Jail Diversion\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("JailDiversion"),
             # pl.col("Sentence")
-            # .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s") 
+            # .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s")
             # .alias("Alcoholics Anonymous"),
             # pl.col("Sentence")
-            # .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s") 
+            # .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s")
             # .alias("BadCheckSchool"),
             pl.col("Sentence")
             .str.extract(r"Informal Probation\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("InformalProbation"),
             pl.col("Sentence")
-            .str.extract(r"Court Referral Program\:\s+([0-9]|X?)\s") 
+            .str.extract(r"Court Referral Program\:\s+([0-9]|X?)\s")
             .cast(pl.Categorical)
             .alias("CourtReferralProgram"),
             # pl.col("Sentence")
-            # .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s") 
+            # .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s")
             # .alias("CommunityService"),
             # pl.col("Sentence")
-            # .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s") 
+            # .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s")
             # .alias("AlternativeSentencing"),
             # pl.col("Sentence")
-            # .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s") 
+            # .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s")
             # .alias("PreTrialDiversion"),
             pl.col("Sentence")
             .str.extract(r"Dui School\:\s+([0-9A-Z]?)\s")
             .cast(pl.Categorical)
             .alias("DUISchool"),
             # pl.col("Sentence")
-            # .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s") 
+            # .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s")
             # .alias("DefensiveDrivingSchool"),
             # pl.col("Sentence")
-            # .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)") 
+            # .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)")
             # .alias("DocCommunityCorrections"),
             # pl.col("Sentence")
             # .str.extract(r"Jail Community Corrections\:\s+([0-9]|X?)")
             # .alias("JailCommunityCorrections"),
             # pl.col("Sentence")
             # .str.extract(r"Mental Health\:\s+([0-9]|X?)")
             # .alias("MentalHealth"),
             # pl.col("Sentence")
-            # .str.extract(r"Anger Management Program\:\s+([0-9]|X?)") 
+            # .str.extract(r"Anger Management Program\:\s+([0-9]|X?)")
             # .alias("AngerManagementProgram"),
             pl.col("Sentence")
             .str.extract(r"Drug Court\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("DrugCourt"),
             pl.col("Sentence")
             .str.extract(r"Doc Drug Program\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("DocDrugProgram"),
             # pl.col("Sentence")
-            # .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project") 
+            # .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project")
             # .str.strip()
             # .alias("DrugMeasureUnit"),
             pl.col("Sentence")
             .str.extract(r"Drug Near Project\: (.+?)Drugs Near School")
             .str.strip()
             .cast(pl.Categorical)
             .alias("DrugNearProject"),
             pl.col("Sentence")
-            .str.extract(r"Drugs Near School\: (.+?)Habitual Offender") 
-            .str.replace(r'Habitual Offender\:','')
-            .str.replace(r'Sex Offender Community Notification\:','')
-            .str.replace(r'Drug Volume\:','')
-            .str.replace(r'Drug\:','')
-            .str.replace(r'Drug Code\:\s?\d*','')
+            .str.extract(r"Drugs Near School\: (.+?)Habitual Offender")
+            .str.replace(r"Habitual Offender\:", "")
+            .str.replace(r"Sex Offender Community Notification\:", "")
+            .str.replace(r"Drug Volume\:", "")
+            .str.replace(r"Drug\:", "")
+            .str.replace(r"Drug Code\:\s?\d*", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("DrugsNearSchool"),
             pl.col("Sentence")
             .str.extract(r"Habitual Offender\: (.+?)Sex Offender")
             .str.strip()
             .cast(pl.Categorical)
             .alias("HabitualOffender"),
             # pl.col("Sentence")
-            # .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume") 
+            # .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume")
             # .str.replace_all(r"[X\s0-9]", "")
             # .str.replace(r'\.','')
             # .alias("SexOffenderCommunityNotification"),
             pl.col("Sentence")
             .str.extract(r"(\d+\.\d\d)\sDrug Volume\:")
             .cast(pl.Float64, strict=False)
             .alias("DrugVolume"),
@@ -3163,15 +3204,15 @@
             .alias("DrugCode"),
             pl.col("Sentence")
             .str.extract(r"Habitual Offender Number\: (.+?)Victim")
             .str.strip()
             .alias("HabitualOffenderNumber"),
             pl.col("Sentence")
             .str.extract(r"Victim DOB\:\s+(\d?\d?/?\d?\d?/?\d?\d?\d?\d?)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("VictimDOB"),
         ]
     )
     sent = sent.fill_null("")
     return sent
 
 
@@ -4096,14 +4137,51 @@
                 button_color=("white", "black"),
                 pad=(10, 10),
                 disabled_button_color=("grey", "black"),
                 bind_return_key=True,
             )
         ],
     ]  # "TB"
+    rename_layout = [
+        [
+            sg.Text(
+                """Rename case PDFs in directory to\ncase numbers.""",
+                font=HEADER_FONT,
+                pad=(5, 5),
+            )
+        ],
+        [
+            sg.Text(
+                """To rename each PDF case in a directory to its case number, enter the\ndirectory path below and click start. Some devices may require a\nreboot or reindex to reflect updated file names.""",
+                pad=(5, 5),
+            )
+        ],
+        [
+            sg.Text("Directory: "),
+            sg.InputText(
+                tooltip="PDF Directory",
+                size=[30, 10],
+                key="RN-INPUTPATH",
+                focus=True,
+            ),
+            sg.FolderBrowse(
+                button_text="Select Folder", button_color=("white", "black")
+            ),
+        ],
+        [
+            sg.Button(
+                "Rename Cases",
+                key="RN",
+                button_color=("white", "black"),
+                pad=(10, 10),
+                disabled_button_color=("grey", "black"),
+                bind_return_key=True,
+            )
+        ],
+    ]  # "RN"
     about_layout = [
         [
             sg.Text(
                 f"""╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗\n╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ \n╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝\nversion {version}""",
                 font=ASCII_FONT,
                 pad=(5, 5),
             )
@@ -4129,14 +4207,15 @@
         font="Courier",
         layout=[
             [sg.Tab("fetch", layout=fetch_layout, pad=(2, 2))],
             [sg.Tab("archive", layout=archive_layout, pad=(2, 2))],
             [sg.Tab("table", layout=table_layout, pad=(2, 2))],
             [sg.Tab("append", layout=append_layout, pad=(2, 2))],
             [sg.Tab("pair", layout=sum_layout, pad=(2, 2))],
+            [sg.Tab("rename", layout=rename_layout, pad=(2, 2))],
             [sg.Tab("about", layout=about_layout, pad=(2, 2))],
         ],
     )
     layout = [
         [sg.Text(FSHORT_NAME, font=LOGO_FONT, pad=(5, 5))],
         [tabs],
         [
@@ -4186,22 +4265,24 @@
         elif "ERROR" in event:
             window["AA"].update(disabled=False)
             window["SQ"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["SUM"].update(disabled=False)
+            window["RN"].update(disabled=False)
         elif "COMPLETE" in event:
             print("Alacorder completed the task.")
             window["AA"].update(disabled=False)
             window["SQ"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["SUM"].update(disabled=False)
+            window["RN"].update(disabled=False)
             window["PROGRESS"].update(current_count=0, max=100)
             sg.popup("Alacorder completed the task.")
             continue
         elif event == "NEWQUERY":
             if window["SQ-INPUTPATH"].get() == "":
                 sg.popup(
                     "To create empty query template, enter file output path (extension must be .xlsx) in Input Path, then press the New Query button to try again."
@@ -4373,14 +4454,27 @@
                     daemon=True,
                 ).start()
                 continue
             except:
                 print("Check configuration and try again.")
                 window["AA"].update(disabled=False)
                 continue
+        elif event == "RN":
+            if window["RN-INPUTPATH"].get() == "":
+                sg.popup("Enter directory path and try again.")
+                continue
+            else:
+                cf = set(window["RN-INPUTPATH"].get(), log=True, window=window)
+                window["RN"].update(disabled=True)
+                thread = threading.Thread(
+                    target=rename_pdfs,
+                    args=[cf],
+                    daemon=True,
+                ).start()
+                continue
         else:
             pass
 
 
 #   #   #   #       COMMAND LINE INTERFACE     #   #   #   #
```

### Comparing `alacorder-80.2.5/src/alacorder/alac.py` & `alacorder-80.2.6/src/alacorder/alac.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.2.5"
+version = "80.2.6"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -36,14 +36,15 @@
 pl.Config.set_tbl_hide_column_data_types(True)
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 FNAME = f"{name} {version}"
 FSHORT_NAME = f"{name} {'.'.join(version.split('.')[0:-1])}"
 
 prt = print
 
+
 def plog(*msg, cf=None):
     global prt
     if len(msg) == 1:
         msg = msg[0]
         if isinstance(cf, dict):
             try:
                 if cf["LOG"] == True:
@@ -63,14 +64,15 @@
                 except:
                     prt(m)
             elif cf == None:
                 prt(m)
             elif type(cf) == bool and cf:
                 prt(m)
 
+
 print = plog
 
 
 def dlog(*msg, cf=None):
     if type(cf) == bool:
         if cf:
             for m in msg:
@@ -132,14 +134,15 @@
     write(a, cf=cf)
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("COMPLETE-MA", True)
     return a
 
+
 def multi(cf):
     """
     Start multitable collection using configuration object `cf`.
     """
     start = time.time()
     df = read(cf)
     print("Parsing case info...", cf=cf)
@@ -454,15 +457,14 @@
     elapsed = math.floor(time.time() - start)
     print(f"Completed in {elapsed} seconds.", cf=cf)
     if cf["WINDOW"]:
         cf["WINDOW"].write_event_value("CONVSUM-COMPLETE", True)
     return conv
 
 
-
 #   #   #   #         CONFIGURATION & I/O        #   #   #   #
 
 
 def set(
     inputs,
     outputs=None,
     count=0,
@@ -1111,27 +1113,29 @@
                 x[4].replace("\n", " ") for x in pg.get_text(option="blocks")
             )
         except:
             pass
     text = re.sub(r"(<image\:.+?>)", "", text).strip()
     return text
 
+
 def extract_text_pg_one(path) -> str:
     """
     From path, return text of first page of PDF as string (PyMuPdf engine required!)
     """
     try:
         doc = fitz.open(path)
     except:
         return ""
     text = " \n ".join(
-                x[4].replace("\n", " ") for x in doc[0].get_text(option="blocks")
-            )
+        x[4].replace("\n", " ") for x in doc[0].get_text(option="blocks")
+    )
     return text
 
+
 def append_archive(inpath="", outpath="", cf=None):
     """
     Append the contents of one archive to another.
 
     Args:
         inpath (str): Input archive
         outpath (str): Output archive
@@ -1171,51 +1175,68 @@
 
     if window:
         window.write_event_value("COMPLETE-AA", True)
     write(out, path=outpath, overwrite=True)
     return out
 
 
-
 def rename_pdfs(cf):
     if isinstance(cf, dict):
         q = cf["QUEUE"]
     elif isinstance(cf, pl.dataframe.frame.DataFrame):
         if "Path" in cf.columns:
             q = cf.select("Path").to_series().to_list()
             cf = {"LOG": False}
     else:
         q = cf
         cf = {"LOG": False}
-    if cf["LOG"]:
+    if cf["LOG"] and not cf["WINDOW"]:
+        print("Renaming cases...")
         for path in tqdm(q):
             text = extract_text_pg_one(path)
             try:
                 cnum = (
                     re.search(r"County: (\d\d)", str(text)).group(1)
                     + "-"
                     + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
                 )
             except:
                 cnum = os.path.split(path)[1]
             newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
             os.rename(path, newpath)
-    else:
+    elif not cf["LOG"]:
         for path in q:
             text = extract_text_pg_one(path)
             try:
                 cnum = (
                     re.search(r"County: (\d\d)", str(text)).group(1)
                     + "-"
                     + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
                 )
             except:
                 cnum = os.path.split(path)[1]
             newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
             os.rename(path, newpath)
+    elif cf["LOG"] and cf["WINDOW"]:
+        print("Renaming cases...")
+        cf["WINDOW"].write_event_value("PROGRESS_TOTAL", len(q))
+        for i, path in enumerate(q):
+            text = [extract_text_pg_one(path)]
+            try:
+                cnum = (
+                    re.search(r"County: (\d\d)", str(text)).group(1)
+                    + "-"
+                    + re.search(r"(\w{2}\-\d{4}-\d{6}\.\d{2})", str(text)).group()
+                )
+            except:
+                cnum = os.path.split(path)[1]
+            newpath = f"{os.path.split(path)[0]}/{cnum}.pdf"
+            os.rename(path, newpath)
+            cf["WINDOW"].write_event_value("PROGRESS", i + 1)
+        cf["WINDOW"].write_event_value("RN-COMPLETE", True)
 
 
 def make_pairs_template(df, debug=False):
     if isinstance(df, str):
         df = read(df)
     names = df.with_columns(
         [
@@ -1620,15 +1641,15 @@
             .str.replace(r"\:", "")
             .str.strip()
             .alias("Alias"),
             pl.col("AllPagesText")
             .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
             .str.replace(r"[^\d/]", "")  # _all
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("DOB"),
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
                     pl.lit("-"),
@@ -1637,28 +1658,34 @@
             ).alias("CaseNumber"),
             pl.col("AllPagesText")
             .str.extract(r"(Phone: )(.+)", group_index=2)
             .str.replace_all(r"[^0-9]", "")
             .str.slice(0, 10)
             .str.replace(r"(.{3}0000000)", "")  # _all
             .alias("RE_Phone"),
-            pl.col("AllPagesText").str.extract(r"(B|W|H|A)/(?:F|M)").cast(pl.Categorical).alias("Race"),
-            pl.col("AllPagesText").str.extract(r"(?:B|W|H|A)/(F|M)").cast(pl.Categorical).alias("Sex"),
+            pl.col("AllPagesText")
+            .str.extract(r"(B|W|H|A)/(?:F|M)")
+            .cast(pl.Categorical)
+            .alias("Race"),
+            pl.col("AllPagesText")
+            .str.extract(r"(?:B|W|H|A)/(F|M)")
+            .cast(pl.Categorical)
+            .alias("Sex"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Address 1:)(.+)(?:Phone)*?", group_index=1)
             .str.replace(r"(Phone.+)", "")
             .str.strip()
             .alias("Address1"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Address 2:)(.+)")
             .str.strip()
             .alias("Address2"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Zip: )(.+)", group_index=1)
-            .str.replace(r'[A-Za-z\:\s]+','')
+            .str.replace(r"[A-Za-z\:\s]+", "")
             .str.strip()
             .alias("ZipCode"),
             pl.col("AllPagesText")
             .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=1)
             .str.strip()
             .alias("City"),
             pl.col("AllPagesText")
@@ -1680,65 +1707,64 @@
             .alias("D999RAW"),
             pl.col("AllPagesText")
             .str.extract_all(r"(\w{2}\d{12})")
             .arr.join("/")
             .alias("RelatedCases"),
             pl.col("AllPagesText")
             .str.extract(r"Filing Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("FilingDate"),
             pl.col("AllPagesText")
             .str.extract(r"Case Initiation Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("CaseInitiationDate"),
             pl.col("AllPagesText")
             .str.extract(r"Arrest Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("ArrestDate"),
             pl.col("AllPagesText")
             .str.extract(r"Offense Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("OffenseDate"),
             pl.col("AllPagesText")
             .str.extract(r"Indictment Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("IndictmentDate"),
             pl.col("AllPagesText")
             .str.extract(r"Youthful Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("YouthfulDate"),
             pl.col("AllPagesText")
             .str.extract(r"AL Institutional Service Num: ([^\na-z])")
             .str.strip()
             .alias("ALInstitutionalServiceNum"),
             pl.col("AllPagesText")
             .str.extract(r"Alacourt\.com (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("Retrieved"),
             pl.col("AllPagesText")
             .str.extract(
                 r"Court Action: (BOUND|GUILTY PLEA|WAIVED TO GJ|DISMISSED|TIME LAPSED|NOL PROSS|CONVICTED|INDICTED|DISMISSED|FORFEITURE|TRANSFER|REMANDED|WAIVED|ACQUITTED|WITHDRAWN|PETITION|PRETRIAL|COND\. FORF\.)"
             )
             .alias("CourtAction"),
             pl.col("AllPagesText")
             .str.extract(r"Court Action Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("CourtActionDate"),
             pl.col("AllPagesText")
             .str.extract(r"Charge: ([A-Z\.0-9\-\s]+)")
             .str.rstrip("C")
             .str.strip()
             .alias("Description"),
             pl.col("AllPagesText")
             .str.extract(r"Jury Demand: ([A-Z]+)")
             .cast(pl.Categorical)
             .alias("JuryDemand"),
-            pl.col("AllPagesText").str.extract(
-                r"Inpatient Treatment Ordered: ([YES|NO]?)"
-            )
+            pl.col("AllPagesText")
+            .str.extract(r"Inpatient Treatment Ordered: ([YES|NO]?)")
             .cast(pl.Categorical)
             .alias("InpatientTreatmentOrdered"),
             pl.col("AllPagesText")
             .str.extract(r"Trial Type: ([A-Z]+)")
             .str.replace(r"[S|N]$", "")
             .str.strip()
             .cast(pl.Categorical)
@@ -1834,20 +1860,20 @@
             .str.replace(r"(Enforcement|Party)", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("Country"),
             pl.col("AllPagesText")
             .str.extract(r"(\d\d?/\d\d?/\d\d\d\d) Warrant Issuance Date:")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("WarrantIssuanceDate"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Action Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("WarrantActionDate"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Issuance Status: (\w+)")
             .str.replace(r"Description", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("WarrantIssuanceStatus"),
@@ -1881,38 +1907,39 @@
             .str.extract(r"([\d\.]+) Bond Amount:")
             .cast(pl.Float64, strict=False)
             .alias("BondAmt"),
             pl.col("AllPagesText")
             .str.extract(r"Bond Company: ([A-Z0-9]+)")
             .str.rstrip("S")
             .alias("BondCompany"),
-            pl.col("AllPagesText").str.extract(r"Surety Code: ([A-Z0-9]{4})")
+            pl.col("AllPagesText")
+            .str.extract(r"Surety Code: ([A-Z0-9]{4})")
             .alias("SuretyCode"),
-            pl.col("AllPagesText").str.extract(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            pl.col("AllPagesText")
+            .str.extract(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("BondReleaseDate"),
-            pl.col("AllPagesText").str.extract(
-                r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)"
-            )
-            .str.to_date('%m/%d/%Y', strict=False)
+            pl.col("AllPagesText")
+            .str.extract(r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("FailedToAppearDate"),
             pl.col("AllPagesText")
             .str.extract(
                 r"Bondsman Process Issuance: ([^\n]*?) Bondsman Process Return:"
             )
             .str.strip()
             .alias("BondsmanProcessIssuance"),
             pl.col("AllPagesText")
             .str.extract(r"Bondsman Process Return: (.*?) Number of Subponeas")
             .str.strip()
             .alias("BondsmanProcessReturn"),
             pl.col("AllPagesText")
             .str.extract(r"([\n\s/\d]*?) Appeal Court:")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("AppealDate"),
             pl.col("AllPagesText")
             .str.extract(r"([A-Z\-\s]+) Appeal Case Number")
             .str.strip()
             .cast(pl.Categorical)
             .alias("AppealCourt"),
             pl.col("AllPagesText")
@@ -1927,34 +1954,34 @@
             .str.rstrip("O")
             .str.strip()
             .cast(pl.Categorical)
             .alias("AppealToDesc"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal Status: ([A-Z\-\s]+)")
             .str.rstrip("A")
-            .str.replace_all(r'\n','')
+            .str.replace_all(r"\n", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("AppealStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal To: (\w*) Appeal")
             .str.strip()
             .cast(pl.Categorical)
             .alias("AppealTo"),
             pl.col("AllPagesText")
             .str.extract(r"LowerCourt Appeal Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.replace_all(r"[\n\s:\-]", "")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("LowerCourtAppealDate"),
             pl.col("AllPagesText")
             .str.extract(r"Disposition Date Of Appeal: (\d\d?/\d\d?/\d\d\d\d)")
             .str.replace_all(r"[\n\s:\-]", "")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("DispositionDateOfAppeal"),
             pl.col("AllPagesText")
             .str.extract(r"Disposition Type Of Appeal: [^A-Za-z]+")
             .str.replace_all(r"[\n\s:\-]", "")
             .str.strip()
             .alias("DispositionTypeOfAppeal"),
             pl.col("AllPagesText")
@@ -1966,53 +1993,56 @@
             pl.col("AllPagesText")
             .str.extract(r"Updated By: (\w{3})")
             .str.strip()
             .alias("AdminUpdatedBy"),
             pl.col("AllPagesText")
             .str.extract(r"Transfer to Admin Doc Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("TransferToAdminDocDate"),
             pl.col("AllPagesText")
             .str.extract(r"Transfer Desc: ([A-Z\s]{0,15} \d\d?/\d\d?/\d\d\d\d)")
             .str.replace_all(r"(Transfer Desc:)", "")
             .str.strip()
             .alias("TransferDesc"),
             pl.col("AllPagesText")
             .str.extract(r"Date Trial Began but No Verdict \(TBNV1\): ([^\n]+)")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("TBNV1"),
             pl.col("AllPagesText")
             .str.extract(r"Date Trial Began but No Verdict \(TBNV2\): ([^\n]+)")
             .str.replace(r"Financial", "")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("TBNV2"),
             pl.col("AllPagesText")
             .str.extract(r"TurnOver Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("TurnOverDate"),
             pl.col("AllPagesText")
             .str.extract(r"TurnOver Amt\: \$(\d+\.\d\d)")
             .cast(pl.Float64, strict=False)
             .alias("TurnOverAmt"),
             pl.col("AllPagesText")
             .str.extract(r"Frequency Amt\: \$(\d+\.\d\d)")
             .cast(pl.Float64, strict=False)
             .alias("FrequencyAmt"),
             pl.col("AllPagesText")
             .str.extract(r"Due Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("DueDate"),
             pl.col("AllPagesText")
             .str.extract(r"Last Paid Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("LastPaidDate"),
-            pl.col("AllPagesText").str.extract(r"Payor\: ([A-Z0-9]{4})").cast(pl.Categorical).alias("Payor"),
+            pl.col("AllPagesText")
+            .str.extract(r"Payor\: ([A-Z0-9]{4})")
+            .cast(pl.Categorical)
+            .alias("Payor"),
             pl.col("AllPagesText")
             .str.extract(r"Enforcement Status\: ([A-Z\:,\s]+)")
             .str.replace_all(r"\s+", " ")
             .str.replace(r" F$", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("EnforcementStatus"),
@@ -2028,51 +2058,51 @@
             pl.col("AllPagesText")
             .str.extract(r"PreTrial\: (YES|NO)")
             .cast(pl.Categorical)
             .alias("PreTrial"),
             pl.col("AllPagesText")
             .str.extract(r"PreTrail Date\: (.+)PreTrial")
             .str.strip()
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("PreTrialDate"),
             pl.col("AllPagesText")
             .str.extract(r"PreTrial Terms\: (YES|NO)")
             .cast(pl.Categorical)
             .alias("PreTrialTerms"),
             pl.col("AllPagesText")
             .str.extract(r"Pre Terms Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("PreTermsDate"),
             pl.col("AllPagesText")
             .str.extract(r"Delinquent\: (YES|NO)")
             .cast(pl.Categorical)
             .alias("Delinquent"),
             pl.col("AllPagesText")
             .str.extract(r"Delinquent Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("DelinquentDate"),
             pl.col("AllPagesText")
             .str.extract(r"DA Mailer\: (YES|NO)")
             .cast(pl.Categorical)
             .alias("DAMailer"),
             pl.col("AllPagesText")
             .str.extract(r"DA Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("DAMailerDate"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Mailer\: (YES|NO)")
             .cast(pl.Categorical)
             .alias("WarrantMailer"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("WarrantMailerDate"),
             pl.col("AllPagesText")
             .str.extract(r"Last Update\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("EnforcementLastUpdate"),
             pl.col("AllPagesText")
             .str.extract(r"Updated By\: ([A-Z]{3})")
             .alias("EnforcementUpdatedBy"),
         ]
     )
     cases = cases.with_columns(
@@ -2256,15 +2286,15 @@
         ]
     )
     fh = fh.explode("FinancialHistory")
     fh = fh.with_columns(
         [
             pl.col("FinancialHistory")
             .str.extract(r"(\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("TransactionDate"),
             pl.col("FinancialHistory")
             .str.extract(r"(RECEIPT|CREDIT)")
             .alias("Description"),
             pl.col("FinancialHistory")
             .str.extract(r"(\$\d+\.\d\d)")
             .str.replace(r"\$", "")
@@ -2509,20 +2539,22 @@
             )
             .str.strip()
             .str.replace(r",$", "")
             .str.replace(r"\s+", " ")
             .alias("ChargesSummary")
         ]
     )
-    charges = charges.with_columns([
-        pl.col("CourtActionDate").str.to_date('%m/%d/%Y', strict=False),
-        pl.col("Category").cast(pl.Categorical),
-        pl.col("TypeDescription").cast(pl.Categorical),
-        pl.col("CourtAction").cast(pl.Categorical)
-        ])
+    charges = charges.with_columns(
+        [
+            pl.col("CourtActionDate").str.to_date("%m/%d/%Y", strict=False),
+            pl.col("Category").cast(pl.Categorical),
+            pl.col("TypeDescription").cast(pl.Categorical),
+            pl.col("CourtAction").cast(pl.Categorical),
+        ]
+    )
     charges = charges.select(
         "Name",
         "CaseNumber",
         "Num",
         "Code",
         "Cite",
         "Description",
@@ -2849,143 +2881,147 @@
         [
             pl.col("CaseNumber"),
             pl.col("Sentence")
             .str.extract(r"Sentence\s(\d)\s")
             .cast(pl.Int64, strict=False)
             .alias("Number"),
             pl.col("Sentence")
-            .str.extract(r"Last Update\:\s(\d\d?/\d\d?/\d\d\d\d)\sUpdated By\: [A-Z]{3}")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.extract(
+                r"Last Update\:\s(\d\d?/\d\d?/\d\d\d\d)\sUpdated By\: [A-Z]{3}"
+            )
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("LastUpdate"),
             pl.col("Sentence")
-            .str.extract(r"Last Update\:\s\d\d?/\d\d?/\d\d\d\d\sUpdated By\: ([A-Z]{3})")
+            .str.extract(
+                r"Last Update\:\s\d\d?/\d\d?/\d\d\d\d\sUpdated By\: ([A-Z]{3})"
+            )
             .alias("UpdatedBy"),
             pl.col("Sentence")
             .str.extract(r"Probation Revoke\:(.+?) (Sentence|License)")
-            .str.replace(r'Sentence.*','')
-            .str.replace(r'License.+','')
+            .str.replace(r"Sentence.*", "")
+            .str.replace(r"License.+", "")
             .str.strip()
             .alias("ProbationRevoke"),
             pl.col("Sentence")
             .str.extract(r"License Susp Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
             .alias("LicenseSuspPeriod"),
             pl.col("Sentence")
             .str.extract(r"Days\.\s*(\d+ Years, \d+ Months, \d+ Days\.)\s+")
-            .alias("JailCreditPeriod"), 
+            .alias("JailCreditPeriod"),
             pl.col("Sentence")
             .str.extract(r"Probation Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
             .alias("ProbationPeriod"),
             pl.col("Sentence")
             .str.extract(r"Sentence Provisions\: ([YN])")
             .cast(pl.Categorical)
             .alias("Provisions"),
             pl.col("Sentence")
             .str.extract(r"Requrements Completed\: (YES|NO)")
             .cast(pl.Categorical)
             .alias("RequirementsCompleted"),
             pl.col("Sentence")
             .str.extract(r"Sentence Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("SentenceDate"),
             pl.col("Sentence")
             .str.extract(r"Sentence Start Date\: (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("StartDate"),
             pl.col("Sentence")
             .str.extract(r"Sentence End Date\: .{0,40}? (\d\d?/\d\d?/\d\d\d\d)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("EndDate"),
             pl.col("Sentence")
             .str.extract(r"Jail Fee\:(.+?)Costs")
             .str.replace(r"[A-Z]-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("JailFee"),
             pl.col("Sentence")
             .str.extract(r"Costs\: (.+?)Fine\:")
-            .str.replace(r'Fine.+','')
+            .str.replace(r"Fine.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("Costs"),
             # pl.col("Sentence")
-            # .str.extract(r"Fine\:(.+?)Crime Victims") 
+            # .str.extract(r"Fine\:(.+?)Crime Victims")
             # .str.strip()
             # .alias("Fine"),
             # pl.col("Sentence")
             # .str.extract(r"Crime Victims Fee\:(.+?)Monetary")
             # .str.strip()
             # .alias("CrimeVictimsFee"),
             pl.col("Sentence")
-            .str.extract(r"Municipal Court\:(.+?)Fine Suspended") ## NONE
+            .str.extract(r"Municipal Court\:(.+?)Fine Suspended")  ## NONE
             .str.replace(r"X-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("MunicipalCourt"),
             # pl.col("Sentence")
-            # .str.extract(r"Fine Suspended\: (.+?)Immigration Fine") 
+            # .str.extract(r"Fine Suspended\: (.+?)Immigration Fine")
             # .str.strip()
-            # .alias("FineSuspended"), 
+            # .alias("FineSuspended"),
             pl.col("Sentence")
             .str.extract(r"Immigration Fine\: (.+?)Fine")
-            .str.replace(r'X\-\$','')
+            .str.replace(r"X\-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("ImmigrationFine"),
             pl.col("Sentence")
             .str.extract(r"Fine Imposed\: (.+?) Alias Warrant")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("FineImposed"),
             # pl.col("Sentence")
-            # .str.extract(r"Drug Docket Fees\: (.+?)Prelim Hearing") 
+            # .str.extract(r"Drug Docket Fees\: (.+?)Prelim Hearing")
             # .str.replace(r'Prelim Hearing.+','')
             # .str.strip()
             # .alias("DrugDocketFees"),
             pl.col("Sentence")
             .str.extract(r"Prelim Hearing\:(.+?)Amt Over Minimum CVF")
-            .str.replace(r'Amt.+','') 
+            .str.replace(r"Amt.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("PrelimHearing"),
             pl.col("Sentence")
             .str.extract(r"Amt Over Minimum CVF\: (.+?) WC Fee DA")
             .str.replace_all(r"[A-Z\s]|\-|\$", "")
             .cast(pl.Float64, strict=False)
             .alias("AmtOverMinimumCVF"),
             # pl.col("Sentence")
-            # .str.extract(r"WC Fee DA\: (.+?)Removal Bill") 
+            # .str.extract(r"WC Fee DA\: (.+?)Removal Bill")
             # .str.strip()
-            # .alias("WCFeeDA"), 
+            # .alias("WCFeeDA"),
             # pl.col("Sentence")
             # .str.extract(r"Removal Bill\: (.+?)Crime History Fee")
             # .str.strip()
             # .alias("RemovalBill"),
             pl.col("Sentence")
-            .str.extract(r"Crime History Fee\: (.+?) SX10") 
+            .str.extract(r"Crime History Fee\: (.+?) SX10")
             .str.strip()
             .cast(pl.Categorical)
             .alias("CrimeHistoryFee"),
             pl.col("Sentence")
             .str.extract(r"SX10\: (.+?)License Suspension Fee")
             .str.strip()
             .cast(pl.Categorical)
             .alias("SX10"),
             pl.col("Sentence")
             .str.extract(r"License Suspension Fee\: (.+?) WC Fee 85%")
             .str.replace_all(r"[A-Z\s]+", "")
             .cast(pl.Float64, strict=False)
             .alias("LicenseSuspensionFee"),
             pl.col("Sentence")
-            .str.extract(r"WC Fee 85%\: (.+?) Demand Reduction Hearing\:") 
-            .str.replace(r'Demand Reduction Hearing.+','')
+            .str.extract(r"WC Fee 85%\: (.+?) Demand Reduction Hearing\:")
+            .str.replace(r"Demand Reduction Hearing.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("WCFee85"),
             pl.col("Sentence")
-            .str.extract(r"Demand Reduction Hearing\: (.+?)Drug User Fee") 
+            .str.extract(r"Demand Reduction Hearing\: (.+?)Drug User Fee")
             .str.replace_all(r"[A-Z]\-|\s|\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("DemandReductionHearing"),
             pl.col("Sentence")
             .str.extract(r"Drug User Fee\: (.+?) Subpoena")
             .str.strip()
@@ -3018,141 +3054,146 @@
             pl.col("Sentence")
             .str.extract(
                 r"Suspended Confinement Period (\d+ Years, \d+ Months, \d+ Days\.)"
             )
             .alias("SuspendedConfinementPeriod"),
             pl.col("Sentence")
             .str.extract(r"Boot Camp\: (.+?) (Penitentiary|Life Without Parole)")
-            .str.replace(r'Penitentiary.+','')
+            .str.replace(r"Penitentiary.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("BootCamp"),
             pl.col("Sentence")
-            .str.extract(r"Life Without Parole\: (.+?) (Restitution|Death\:)", group_index=1) 
-            .str.replace(r'Death.+','')
-            .str.replace(r'Restitution.+','')
+            .str.extract(
+                r"Life Without Parole\: (.+?) (Restitution|Death\:)", group_index=1
+            )
+            .str.replace(r"Death.+", "")
+            .str.replace(r"Restitution.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("LifeWithoutParole"),
             # pl.col("Sentence")
-            # .str.extract(r"Split\: (.+?) (Concurrent|Confinement)", group_index=1) 
+            # .str.extract(r"Split\: (.+?) (Concurrent|Confinement)", group_index=1)
             # .str.strip()
             # .alias("Split"),
             # pl.col("Sentence")
             # .str.extract(r"Concurrent Sentence\:\s+([A-Z]?)\s")
             # .str.strip()
             # .alias("ConcurrentSentence"),
             # pl.col("Sentence")
-            # .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s") 
+            # .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s")
             # .str.strip()
             # .alias("ConsecutiveSentence"),
             pl.col("Sentence")
             .str.extract(r"Electronic Monitoring\: (.+?) Reverse Split")
             .str.replace_all(r"[-0\s]", "")
             .cast(pl.Categorical)
             .alias("ElectronicMonitoring"),
             pl.col("Sentence")
-            .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)") 
+            .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)")
             .str.replace_all(r"Death\: Life\:", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("ReverseSplit"),
             # pl.col("Sentence")
             # .str.extract(r"Coterminous Sentence\:\s+([A-Z]?)\s")
             # .alias("CoterminousSentence"),
             # pl.col("Sentence").str.extract(r"Death\:\s+(X?)").alias("Death"),
             pl.col("Sentence").str.extract(r"Life\:\s+(X?)").alias("Life"),
             pl.col("Sentence")
             .str.extract(r"Chain Gang\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("ChainGang"),
-            pl.col("Sentence").str.extract(r"Jail\:\s+([0-9]|X?)").cast(pl.Categorical).alias("Jail"),
+            pl.col("Sentence")
+            .str.extract(r"Jail\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
+            .alias("Jail"),
             # pl.col("Sentence")
-            # .str.extract(r"Community Service Hrs\:\s+([0-9]|X?)") 
+            # .str.extract(r"Community Service Hrs\:\s+([0-9]|X?)")
             # .alias("CommunityServiceHrs"),
             pl.col("Sentence")
             .str.extract(r"Jail Diversion\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("JailDiversion"),
             # pl.col("Sentence")
-            # .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s") 
+            # .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s")
             # .alias("Alcoholics Anonymous"),
             # pl.col("Sentence")
-            # .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s") 
+            # .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s")
             # .alias("BadCheckSchool"),
             pl.col("Sentence")
             .str.extract(r"Informal Probation\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("InformalProbation"),
             pl.col("Sentence")
-            .str.extract(r"Court Referral Program\:\s+([0-9]|X?)\s") 
+            .str.extract(r"Court Referral Program\:\s+([0-9]|X?)\s")
             .cast(pl.Categorical)
             .alias("CourtReferralProgram"),
             # pl.col("Sentence")
-            # .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s") 
+            # .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s")
             # .alias("CommunityService"),
             # pl.col("Sentence")
-            # .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s") 
+            # .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s")
             # .alias("AlternativeSentencing"),
             # pl.col("Sentence")
-            # .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s") 
+            # .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s")
             # .alias("PreTrialDiversion"),
             pl.col("Sentence")
             .str.extract(r"Dui School\:\s+([0-9A-Z]?)\s")
             .cast(pl.Categorical)
             .alias("DUISchool"),
             # pl.col("Sentence")
-            # .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s") 
+            # .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s")
             # .alias("DefensiveDrivingSchool"),
             # pl.col("Sentence")
-            # .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)") 
+            # .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)")
             # .alias("DocCommunityCorrections"),
             # pl.col("Sentence")
             # .str.extract(r"Jail Community Corrections\:\s+([0-9]|X?)")
             # .alias("JailCommunityCorrections"),
             # pl.col("Sentence")
             # .str.extract(r"Mental Health\:\s+([0-9]|X?)")
             # .alias("MentalHealth"),
             # pl.col("Sentence")
-            # .str.extract(r"Anger Management Program\:\s+([0-9]|X?)") 
+            # .str.extract(r"Anger Management Program\:\s+([0-9]|X?)")
             # .alias("AngerManagementProgram"),
             pl.col("Sentence")
             .str.extract(r"Drug Court\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("DrugCourt"),
             pl.col("Sentence")
             .str.extract(r"Doc Drug Program\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("DocDrugProgram"),
             # pl.col("Sentence")
-            # .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project") 
+            # .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project")
             # .str.strip()
             # .alias("DrugMeasureUnit"),
             pl.col("Sentence")
             .str.extract(r"Drug Near Project\: (.+?)Drugs Near School")
             .str.strip()
             .cast(pl.Categorical)
             .alias("DrugNearProject"),
             pl.col("Sentence")
-            .str.extract(r"Drugs Near School\: (.+?)Habitual Offender") 
-            .str.replace(r'Habitual Offender\:','')
-            .str.replace(r'Sex Offender Community Notification\:','')
-            .str.replace(r'Drug Volume\:','')
-            .str.replace(r'Drug\:','')
-            .str.replace(r'Drug Code\:\s?\d*','')
+            .str.extract(r"Drugs Near School\: (.+?)Habitual Offender")
+            .str.replace(r"Habitual Offender\:", "")
+            .str.replace(r"Sex Offender Community Notification\:", "")
+            .str.replace(r"Drug Volume\:", "")
+            .str.replace(r"Drug\:", "")
+            .str.replace(r"Drug Code\:\s?\d*", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("DrugsNearSchool"),
             pl.col("Sentence")
             .str.extract(r"Habitual Offender\: (.+?)Sex Offender")
             .str.strip()
             .cast(pl.Categorical)
             .alias("HabitualOffender"),
             # pl.col("Sentence")
-            # .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume") 
+            # .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume")
             # .str.replace_all(r"[X\s0-9]", "")
             # .str.replace(r'\.','')
             # .alias("SexOffenderCommunityNotification"),
             pl.col("Sentence")
             .str.extract(r"(\d+\.\d\d)\sDrug Volume\:")
             .cast(pl.Float64, strict=False)
             .alias("DrugVolume"),
@@ -3163,15 +3204,15 @@
             .alias("DrugCode"),
             pl.col("Sentence")
             .str.extract(r"Habitual Offender Number\: (.+?)Victim")
             .str.strip()
             .alias("HabitualOffenderNumber"),
             pl.col("Sentence")
             .str.extract(r"Victim DOB\:\s+(\d?\d?/?\d?\d?/?\d?\d?\d?\d?)")
-            .str.to_date('%m/%d/%Y', strict=False)
+            .str.to_date("%m/%d/%Y", strict=False)
             .alias("VictimDOB"),
         ]
     )
     sent = sent.fill_null("")
     return sent
 
 
@@ -4096,14 +4137,51 @@
                 button_color=("white", "black"),
                 pad=(10, 10),
                 disabled_button_color=("grey", "black"),
                 bind_return_key=True,
             )
         ],
     ]  # "TB"
+    rename_layout = [
+        [
+            sg.Text(
+                """Rename case PDFs in directory to\ncase numbers.""",
+                font=HEADER_FONT,
+                pad=(5, 5),
+            )
+        ],
+        [
+            sg.Text(
+                """To rename each PDF case in a directory to its case number, enter the\ndirectory path below and click start. Some devices may require a\nreboot or reindex to reflect updated file names.""",
+                pad=(5, 5),
+            )
+        ],
+        [
+            sg.Text("Directory: "),
+            sg.InputText(
+                tooltip="PDF Directory",
+                size=[30, 10],
+                key="RN-INPUTPATH",
+                focus=True,
+            ),
+            sg.FolderBrowse(
+                button_text="Select Folder", button_color=("white", "black")
+            ),
+        ],
+        [
+            sg.Button(
+                "Rename Cases",
+                key="RN",
+                button_color=("white", "black"),
+                pad=(10, 10),
+                disabled_button_color=("grey", "black"),
+                bind_return_key=True,
+            )
+        ],
+    ]  # "RN"
     about_layout = [
         [
             sg.Text(
                 f"""╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗\n╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ \n╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝\nversion {version}""",
                 font=ASCII_FONT,
                 pad=(5, 5),
             )
@@ -4129,14 +4207,15 @@
         font="Courier",
         layout=[
             [sg.Tab("fetch", layout=fetch_layout, pad=(2, 2))],
             [sg.Tab("archive", layout=archive_layout, pad=(2, 2))],
             [sg.Tab("table", layout=table_layout, pad=(2, 2))],
             [sg.Tab("append", layout=append_layout, pad=(2, 2))],
             [sg.Tab("pair", layout=sum_layout, pad=(2, 2))],
+            [sg.Tab("rename", layout=rename_layout, pad=(2, 2))],
             [sg.Tab("about", layout=about_layout, pad=(2, 2))],
         ],
     )
     layout = [
         [sg.Text(FSHORT_NAME, font=LOGO_FONT, pad=(5, 5))],
         [tabs],
         [
@@ -4186,22 +4265,24 @@
         elif "ERROR" in event:
             window["AA"].update(disabled=False)
             window["SQ"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["SUM"].update(disabled=False)
+            window["RN"].update(disabled=False)
         elif "COMPLETE" in event:
             print("Alacorder completed the task.")
             window["AA"].update(disabled=False)
             window["SQ"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["TB"].update(disabled=False)
             window["MA"].update(disabled=False)
             window["SUM"].update(disabled=False)
+            window["RN"].update(disabled=False)
             window["PROGRESS"].update(current_count=0, max=100)
             sg.popup("Alacorder completed the task.")
             continue
         elif event == "NEWQUERY":
             if window["SQ-INPUTPATH"].get() == "":
                 sg.popup(
                     "To create empty query template, enter file output path (extension must be .xlsx) in Input Path, then press the New Query button to try again."
@@ -4373,14 +4454,27 @@
                     daemon=True,
                 ).start()
                 continue
             except:
                 print("Check configuration and try again.")
                 window["AA"].update(disabled=False)
                 continue
+        elif event == "RN":
+            if window["RN-INPUTPATH"].get() == "":
+                sg.popup("Enter directory path and try again.")
+                continue
+            else:
+                cf = set(window["RN-INPUTPATH"].get(), log=True, window=window)
+                window["RN"].update(disabled=True)
+                thread = threading.Thread(
+                    target=rename_pdfs,
+                    args=[cf],
+                    daemon=True,
+                ).start()
+                continue
         else:
             pass
 
 
 #   #   #   #       COMMAND LINE INTERFACE     #   #   #   #
```

### Comparing `alacorder-80.2.5/PKG-INFO` & `alacorder-80.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.2.5
+Version: 80.2.6
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

