# Comparing `tmp/alacorder-80.2.4.tar.gz` & `tmp/alacorder-80.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.2.4.tar", max compression
+gzip compressed data, was "alacorder-80.2.5.tar", max compression
```

## Comparing `alacorder-80.2.4.tar` & `alacorder-80.2.5.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.2.4/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.2.4/README.md
--rw-r--r--   0        0        0      697 2023-05-05 01:17:39.033967 alacorder-80.2.4/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-05 01:17:15.209499 alacorder-80.2.4/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.2.4/src/alacorder/__init__.py
--rw-r--r--   0        0        0   213293 2023-05-05 01:17:04.987098 alacorder-80.2.4/src/alacorder/__main__.py
--rw-r--r--   0        0        0   213293 2023-05-05 01:16:42.478686 alacorder-80.2.4/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.2.5/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.2.5/README.md
+-rw-r--r--   0        0        0      697 2023-05-05 14:51:55.941968 alacorder-80.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.2.5/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   216932 2023-05-05 14:51:33.966359 alacorder-80.2.5/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   216932 2023-05-05 14:51:18.624013 alacorder-80.2.5/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.2.5/PKG-INFO
```

### Comparing `alacorder-80.2.4/LICENSE` & `alacorder-80.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.2.4/README.md` & `alacorder-80.2.5/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.2.4/pyproject.toml` & `alacorder-80.2.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.2.4"
+version = "80.2.5"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.2.4/src/alacorder/__main__.py` & `alacorder-80.2.5/src/alacorder/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.2.4"
+version = "80.2.5"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -641,15 +641,15 @@
     support_singletable = (
         True
         if outputext in (".xls", ".xlsx", "none", ".json", ".parquet", ".csv")
         else False
     )
     support_archive = (
         True
-        if outputext in (".xls", ".xlsx", ".csv", ".parquet", ".zip", ".json", "none")
+        if outputext in (".xls", ".xlsx", ".csv", ".parquet", ".json", "none")
         else False
     )
     if force not in (  # raise file extension not supported
         ".xls",
         ".xlsx",
         ".csv",
         ".parquet",
@@ -1620,14 +1620,15 @@
             .str.replace(r"\:", "")
             .str.strip()
             .alias("Alias"),
             pl.col("AllPagesText")
             .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
             .str.replace(r"[^\d/]", "")  # _all
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("DOB"),
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
                     pl.lit("-"),
@@ -1636,16 +1637,16 @@
             ).alias("CaseNumber"),
             pl.col("AllPagesText")
             .str.extract(r"(Phone: )(.+)", group_index=2)
             .str.replace_all(r"[^0-9]", "")
             .str.slice(0, 10)
             .str.replace(r"(.{3}0000000)", "")  # _all
             .alias("RE_Phone"),
-            pl.col("AllPagesText").str.extract(r"(B|W|H|A)/(?:F|M)").alias("Race"),
-            pl.col("AllPagesText").str.extract(r"(?:B|W|H|A)/(F|M)").alias("Sex"),
+            pl.col("AllPagesText").str.extract(r"(B|W|H|A)/(?:F|M)").cast(pl.Categorical).alias("Race"),
+            pl.col("AllPagesText").str.extract(r"(?:B|W|H|A)/(F|M)").cast(pl.Categorical).alias("Sex"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Address 1:)(.+)(?:Phone)*?", group_index=1)
             .str.replace(r"(Phone.+)", "")
             .str.strip()
             .alias("Address1"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Address 2:)(.+)")
@@ -1659,14 +1660,15 @@
             pl.col("AllPagesText")
             .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=1)
             .str.strip()
             .alias("City"),
             pl.col("AllPagesText")
             .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=2)
             .str.strip()
+            .cast(pl.Categorical)
             .alias("State"),
             pl.col("AllPagesText")
             .str.extract(r"(Total:.+\$[^\n]*)")
             .str.replace_all(r"[^0-9|\.|\s|\$]", "")
             .str.extract_all(r"\s\$\d+\.\d{2}")
             .alias("TOTALS"),
             pl.col("AllPagesText")
@@ -1678,62 +1680,72 @@
             .alias("D999RAW"),
             pl.col("AllPagesText")
             .str.extract_all(r"(\w{2}\d{12})")
             .arr.join("/")
             .alias("RelatedCases"),
             pl.col("AllPagesText")
             .str.extract(r"Filing Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("FilingDate"),
             pl.col("AllPagesText")
             .str.extract(r"Case Initiation Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("CaseInitiationDate"),
             pl.col("AllPagesText")
             .str.extract(r"Arrest Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("ArrestDate"),
             pl.col("AllPagesText")
             .str.extract(r"Offense Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("OffenseDate"),
             pl.col("AllPagesText")
             .str.extract(r"Indictment Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("IndictmentDate"),
             pl.col("AllPagesText")
             .str.extract(r"Youthful Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("YouthfulDate"),
             pl.col("AllPagesText")
             .str.extract(r"AL Institutional Service Num: ([^\na-z])")
             .str.strip()
             .alias("ALInstitutionalServiceNum"),
             pl.col("AllPagesText")
             .str.extract(r"Alacourt\.com (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("Retrieved"),
             pl.col("AllPagesText")
             .str.extract(
                 r"Court Action: (BOUND|GUILTY PLEA|WAIVED TO GJ|DISMISSED|TIME LAPSED|NOL PROSS|CONVICTED|INDICTED|DISMISSED|FORFEITURE|TRANSFER|REMANDED|WAIVED|ACQUITTED|WITHDRAWN|PETITION|PRETRIAL|COND\. FORF\.)"
             )
             .alias("CourtAction"),
             pl.col("AllPagesText")
             .str.extract(r"Court Action Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("CourtActionDate"),
             pl.col("AllPagesText")
             .str.extract(r"Charge: ([A-Z\.0-9\-\s]+)")
             .str.rstrip("C")
             .str.strip()
             .alias("Description"),
             pl.col("AllPagesText")
             .str.extract(r"Jury Demand: ([A-Z]+)")
+            .cast(pl.Categorical)
             .alias("JuryDemand"),
             pl.col("AllPagesText").str.extract(
                 r"Inpatient Treatment Ordered: ([YES|NO]?)"
             )
-            # .str.strip()
+            .cast(pl.Categorical)
             .alias("InpatientTreatmentOrdered"),
             pl.col("AllPagesText")
             .str.extract(r"Trial Type: ([A-Z]+)")
             .str.replace(r"[S|N]$", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("TrialType"),
             pl.col("AllPagesText")
             .str.extract(r"Case Number: (\d\d-\w+) County:")
             .str.strip()
             .alias("County"),
             pl.col("AllPagesText")
             .str.extract(r"Judge: ([A-Z\-\.\s]+)")
@@ -1745,24 +1757,26 @@
             .alias("PROBATIONOFFICENUMBERRAW"),
             pl.col("AllPagesText")
             .str.extract(r"Defendant Status: ([A-Z\s]+)")
             .str.rstrip("J")
             .str.replace(r"\n", " ")
             .str.replace(r"\s+", " ")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("DefendantStatus"),
             pl.col("AllPagesText")
             .str.extract(r"([^0-9]+) Arresting Agency Type:")
             .str.replace(r"^\-.+", "")
             .str.replace(r"County\:", "")
             .str.replace(r"Defendant Status\:", "")
             .str.replace(r"Judge\:", "")
             .str.replace(r"Trial Type\:", "")
             .str.replace(r"Probation Office \#\:", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("ArrestingAgencyType"),
             pl.col("AllPagesText")
             .str.extract(r"Arresting Officer: ([A-Z\s]+)")
             .str.replace(r"[\s\n]+[A-Z0-9]$", "")
             .str.strip()
             .alias("ArrestingOfficer"),
             pl.col("AllPagesText")
@@ -1776,17 +1790,19 @@
             .str.strip()
             .cast(pl.Int64, strict=False)
             .alias("PreviousDUIConvictions"),
             pl.col("AllPagesText")
             .str.extract(r"Case Initiation Type: ([A-Z\s]+)")
             .str.rstrip("J")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("CaseInitiationType"),
             pl.col("AllPagesText")
             .str.extract(r"Domestic Violence: ([YES|NO])")
+            .cast(pl.Categorical)
             .alias("DomesticViolence"),
             pl.col("AllPagesText")
             .str.extract(r"Agency ORI: ([A-Z\s]+)")
             .str.rstrip("C")
             .str.replace(r"\n", "")
             .str.replace(r"\s+", " ")
             .str.strip()
@@ -1813,115 +1829,132 @@
             pl.col("AllPagesText")
             .str.extract(r"Eyes/Hair: (\w{3})/(\w{3})", group_index=2)
             .alias("Hair"),
             pl.col("AllPagesText")
             .str.extract(r"Country: (\w*+)")
             .str.replace(r"(Enforcement|Party)", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("Country"),
             pl.col("AllPagesText")
             .str.extract(r"(\d\d?/\d\d?/\d\d\d\d) Warrant Issuance Date:")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("WarrantIssuanceDate"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Action Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("WarrantActionDate"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Issuance Status: (\w+)")
             .str.replace(r"Description", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("WarrantIssuanceStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Action Status: (\w+)")
             .str.replace(r"Description", "")
             .str.strip()
             .alias("WarrantActionStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Location Status: (\w+)")
             .str.replace(r"Description", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("WarrantLocationStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Number Of Warrants: (\d{3}\s\d{3})")
             .str.strip()
             .alias("NumberOfWarrants"),
             pl.col("AllPagesText")
             .str.extract(r"Bond Type: (\w+)")  # +
             .str.replace(r"Bond", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("BondType"),
             pl.col("AllPagesText")
             .str.extract(r"Bond Type Desc: ([A-Z\s]+)")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("BondTypeDesc"),
             pl.col("AllPagesText")
             .str.extract(r"([\d\.]+) Bond Amount:")
             .cast(pl.Float64, strict=False)
             .alias("BondAmt"),
             pl.col("AllPagesText")
             .str.extract(r"Bond Company: ([A-Z0-9]+)")
             .str.rstrip("S")
             .alias("BondCompany"),
             pl.col("AllPagesText").str.extract(r"Surety Code: ([A-Z0-9]{4})")
             .alias("SuretyCode"),
             pl.col("AllPagesText").str.extract(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("BondReleaseDate"),
             pl.col("AllPagesText").str.extract(
                 r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)"
             )
+            .str.to_date('%m/%d/%Y', strict=False)
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
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("AppealDate"),
             pl.col("AllPagesText")
             .str.extract(r"([A-Z\-\s]+) Appeal Case Number")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("AppealCourt"),
             pl.col("AllPagesText")
             .str.extract(r"Orgin Of Appeal: ([A-Z\-\s]+)")
             .str.rstrip("L")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("OriginOfAppeal"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal To Desc: ([A-Z\-\s]+)")
             .str.replace(r"[\s\n]+[A-Z0-9]$", "")
             .str.rstrip("O")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("AppealToDesc"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal Status: ([A-Z\-\s]+)")
             .str.rstrip("A")
             .str.replace_all(r'\n','')
             .str.strip()
+            .cast(pl.Categorical)
             .alias("AppealStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal To: (\w*) Appeal")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("AppealTo"),
             pl.col("AllPagesText")
             .str.extract(r"LowerCourt Appeal Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.replace_all(r"[\n\s:\-]", "")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("LowerCourtAppealDate"),
             pl.col("AllPagesText")
             .str.extract(r"Disposition Date Of Appeal: (\d\d?/\d\d?/\d\d\d\d)")
             .str.replace_all(r"[\n\s:\-]", "")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("DispositionDateOfAppeal"),
             pl.col("AllPagesText")
             .str.extract(r"Disposition Type Of Appeal: [^A-Za-z]+")
             .str.replace_all(r"[\n\s:\-]", "")
             .str.strip()
             .alias("DispositionTypeOfAppeal"),
             pl.col("AllPagesText")
@@ -1933,95 +1966,113 @@
             pl.col("AllPagesText")
             .str.extract(r"Updated By: (\w{3})")
             .str.strip()
             .alias("AdminUpdatedBy"),
             pl.col("AllPagesText")
             .str.extract(r"Transfer to Admin Doc Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("TransferToAdminDocDate"),
             pl.col("AllPagesText")
             .str.extract(r"Transfer Desc: ([A-Z\s]{0,15} \d\d?/\d\d?/\d\d\d\d)")
             .str.replace_all(r"(Transfer Desc:)", "")
             .str.strip()
             .alias("TransferDesc"),
             pl.col("AllPagesText")
             .str.extract(r"Date Trial Began but No Verdict \(TBNV1\): ([^\n]+)")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("TBNV1"),
             pl.col("AllPagesText")
             .str.extract(r"Date Trial Began but No Verdict \(TBNV2\): ([^\n]+)")
             .str.replace(r"Financial", "")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("TBNV2"),
             pl.col("AllPagesText")
-            .str.extract(r"TurnOver Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"TurnOver Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
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
-            .str.extract(r"Due Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Due Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("DueDate"),
             pl.col("AllPagesText")
-            .str.extract(r"Last Paid Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Last Paid Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("LastPaidDate"),
-            pl.col("AllPagesText").str.extract(r"Payor\: ([A-Z0-9]{4})").alias("Payor"),
+            pl.col("AllPagesText").str.extract(r"Payor\: ([A-Z0-9]{4})").cast(pl.Categorical).alias("Payor"),
             pl.col("AllPagesText")
             .str.extract(r"Enforcement Status\: ([A-Z\:,\s]+)")
             .str.replace_all(r"\s+", " ")
             .str.replace(r" F$", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("EnforcementStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Frequency\: ([W|M])")
             .str.replace(r"Cost Paid By\:", "")
             .str.strip()
             .alias("Frequency"),
             pl.col("AllPagesText")
             .str.extract(r"Placement Status\: (.+)")
             .str.strip()
             .alias("PlacementStatus"),
             pl.col("AllPagesText")
             .str.extract(r"PreTrial\: (YES|NO)")
+            .cast(pl.Categorical)
             .alias("PreTrial"),
             pl.col("AllPagesText")
             .str.extract(r"PreTrail Date\: (.+)PreTrial")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("PreTrialDate"),
             pl.col("AllPagesText")
             .str.extract(r"PreTrial Terms\: (YES|NO)")
+            .cast(pl.Categorical)
             .alias("PreTrialTerms"),
             pl.col("AllPagesText")
-            .str.extract(r"Pre Terms Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Pre Terms Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("PreTermsDate"),
             pl.col("AllPagesText")
             .str.extract(r"Delinquent\: (YES|NO)")
+            .cast(pl.Categorical)
             .alias("Delinquent"),
             pl.col("AllPagesText")
-            .str.extract(r"Delinquent Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Delinquent Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("DelinquentDate"),
             pl.col("AllPagesText")
             .str.extract(r"DA Mailer\: (YES|NO)")
+            .cast(pl.Categorical)
             .alias("DAMailer"),
             pl.col("AllPagesText")
-            .str.extract(r"DA Mailer Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"DA Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("DAMailerDate"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Mailer\: (YES|NO)")
+            .cast(pl.Categorical)
             .alias("WarrantMailer"),
             pl.col("AllPagesText")
-            .str.extract(r"Warrant Mailer Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Warrant Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("WarrantMailerDate"),
             pl.col("AllPagesText")
-            .str.extract(r"Last Update\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Last Update\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("EnforcementLastUpdate"),
             pl.col("AllPagesText")
             .str.extract(r"Updated By\: ([A-Z]{3})")
             .alias("EnforcementUpdatedBy"),
         ]
     )
     cases = cases.with_columns(
@@ -2205,14 +2256,15 @@
         ]
     )
     fh = fh.explode("FinancialHistory")
     fh = fh.with_columns(
         [
             pl.col("FinancialHistory")
             .str.extract(r"(\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("TransactionDate"),
             pl.col("FinancialHistory")
             .str.extract(r"(RECEIPT|CREDIT)")
             .alias("Description"),
             pl.col("FinancialHistory")
             .str.extract(r"(\$\d+\.\d\d)")
             .str.replace(r"\$", "")
@@ -2457,15 +2509,20 @@
             )
             .str.strip()
             .str.replace(r",$", "")
             .str.replace(r"\s+", " ")
             .alias("ChargesSummary")
         ]
     )
-
+    charges = charges.with_columns([
+        pl.col("CourtActionDate").str.to_date('%m/%d/%Y', strict=False),
+        pl.col("Category").cast(pl.Categorical),
+        pl.col("TypeDescription").cast(pl.Categorical),
+        pl.col("CourtAction").cast(pl.Categorical)
+        ])
     charges = charges.select(
         "Name",
         "CaseNumber",
         "Num",
         "Code",
         "Cite",
         "Description",
@@ -2793,14 +2850,15 @@
             pl.col("CaseNumber"),
             pl.col("Sentence")
             .str.extract(r"Sentence\s(\d)\s")
             .cast(pl.Int64, strict=False)
             .alias("Number"),
             pl.col("Sentence")
             .str.extract(r"Last Update\:\s(\d\d?/\d\d?/\d\d\d\d)\sUpdated By\: [A-Z]{3}")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("LastUpdate"),
             pl.col("Sentence")
             .str.extract(r"Last Update\:\s\d\d?/\d\d?/\d\d\d\d\sUpdated By\: ([A-Z]{3})")
             .alias("UpdatedBy"),
             pl.col("Sentence")
             .str.extract(r"Probation Revoke\:(.+?) (Sentence|License)")
             .str.replace(r'Sentence.*','')
@@ -2814,37 +2872,43 @@
             .str.extract(r"Days\.\s*(\d+ Years, \d+ Months, \d+ Days\.)\s+")
             .alias("JailCreditPeriod"), 
             pl.col("Sentence")
             .str.extract(r"Probation Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
             .alias("ProbationPeriod"),
             pl.col("Sentence")
             .str.extract(r"Sentence Provisions\: ([YN])")
+            .cast(pl.Categorical)
             .alias("Provisions"),
             pl.col("Sentence")
             .str.extract(r"Requrements Completed\: (YES|NO)")
+            .cast(pl.Categorical)
             .alias("RequirementsCompleted"),
             pl.col("Sentence")
             .str.extract(r"Sentence Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("SentenceDate"),
             pl.col("Sentence")
             .str.extract(r"Sentence Start Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("StartDate"),
             pl.col("Sentence")
             .str.extract(r"Sentence End Date\: .{0,40}? (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("EndDate"),
             pl.col("Sentence")
             .str.extract(r"Jail Fee\:(.+?)Costs")
             .str.replace(r"[A-Z]-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("JailFee"),
             pl.col("Sentence")
             .str.extract(r"Costs\: (.+?)Fine\:")
             .str.replace(r'Fine.+','')
             .str.strip()
+            .cast(pl.Categorical)
             .alias("Costs"),
             # pl.col("Sentence")
             # .str.extract(r"Fine\:(.+?)Crime Victims") 
             # .str.strip()
             # .alias("Fine"),
             # pl.col("Sentence")
             # .str.extract(r"Crime Victims Fee\:(.+?)Monetary")
@@ -2876,14 +2940,15 @@
             # .str.replace(r'Prelim Hearing.+','')
             # .str.strip()
             # .alias("DrugDocketFees"),
             pl.col("Sentence")
             .str.extract(r"Prelim Hearing\:(.+?)Amt Over Minimum CVF")
             .str.replace(r'Amt.+','') 
             .str.strip()
+            .cast(pl.Categorical)
             .alias("PrelimHearing"),
             pl.col("Sentence")
             .str.extract(r"Amt Over Minimum CVF\: (.+?) WC Fee DA")
             .str.replace_all(r"[A-Z\s]|\-|\$", "")
             .cast(pl.Float64, strict=False)
             .alias("AmtOverMinimumCVF"),
             # pl.col("Sentence")
@@ -2893,38 +2958,42 @@
             # pl.col("Sentence")
             # .str.extract(r"Removal Bill\: (.+?)Crime History Fee")
             # .str.strip()
             # .alias("RemovalBill"),
             pl.col("Sentence")
             .str.extract(r"Crime History Fee\: (.+?) SX10") 
             .str.strip()
+            .cast(pl.Categorical)
             .alias("CrimeHistoryFee"),
             pl.col("Sentence")
             .str.extract(r"SX10\: (.+?)License Suspension Fee")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("SX10"),
             pl.col("Sentence")
             .str.extract(r"License Suspension Fee\: (.+?) WC Fee 85%")
             .str.replace_all(r"[A-Z\s]+", "")
             .cast(pl.Float64, strict=False)
             .alias("LicenseSuspensionFee"),
             pl.col("Sentence")
             .str.extract(r"WC Fee 85%\: (.+?) Demand Reduction Hearing\:") 
             .str.replace(r'Demand Reduction Hearing.+','')
             .str.strip()
+            .cast(pl.Categorical)
             .alias("WCFee85"),
             pl.col("Sentence")
             .str.extract(r"Demand Reduction Hearing\: (.+?)Drug User Fee") 
             .str.replace_all(r"[A-Z]\-|\s|\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("DemandReductionHearing"),
             pl.col("Sentence")
             .str.extract(r"Drug User Fee\: (.+?) Subpoena")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("DrugUserFee"),
             pl.col("Sentence")
             .str.extract(r"Subpoena\: (.+?) Attorney Fees")
             .str.replace_all(r"[X\-\s\$]", "")
             .cast(pl.Float64, strict=False)
             .alias("Subpoena"),
             # pl.col("Sentence")
@@ -2951,20 +3020,22 @@
                 r"Suspended Confinement Period (\d+ Years, \d+ Months, \d+ Days\.)"
             )
             .alias("SuspendedConfinementPeriod"),
             pl.col("Sentence")
             .str.extract(r"Boot Camp\: (.+?) (Penitentiary|Life Without Parole)")
             .str.replace(r'Penitentiary.+','')
             .str.strip()
+            .cast(pl.Categorical)
             .alias("BootCamp"),
             pl.col("Sentence")
             .str.extract(r"Life Without Parole\: (.+?) (Restitution|Death\:)", group_index=1) 
             .str.replace(r'Death.+','')
             .str.replace(r'Restitution.+','')
             .str.strip()
+            .cast(pl.Categorical)
             .alias("LifeWithoutParole"),
             # pl.col("Sentence")
             # .str.extract(r"Split\: (.+?) (Concurrent|Confinement)", group_index=1) 
             # .str.strip()
             # .alias("Split"),
             # pl.col("Sentence")
             # .str.extract(r"Concurrent Sentence\:\s+([A-Z]?)\s")
@@ -2973,58 +3044,65 @@
             # pl.col("Sentence")
             # .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s") 
             # .str.strip()
             # .alias("ConsecutiveSentence"),
             pl.col("Sentence")
             .str.extract(r"Electronic Monitoring\: (.+?) Reverse Split")
             .str.replace_all(r"[-0\s]", "")
+            .cast(pl.Categorical)
             .alias("ElectronicMonitoring"),
             pl.col("Sentence")
             .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)") 
             .str.replace_all(r"Death\: Life\:", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("ReverseSplit"),
             # pl.col("Sentence")
             # .str.extract(r"Coterminous Sentence\:\s+([A-Z]?)\s")
             # .alias("CoterminousSentence"),
             # pl.col("Sentence").str.extract(r"Death\:\s+(X?)").alias("Death"),
             pl.col("Sentence").str.extract(r"Life\:\s+(X?)").alias("Life"),
             pl.col("Sentence")
             .str.extract(r"Chain Gang\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
             .alias("ChainGang"),
-            pl.col("Sentence").str.extract(r"Jail\:\s+([0-9]|X?)").alias("Jail"),
+            pl.col("Sentence").str.extract(r"Jail\:\s+([0-9]|X?)").cast(pl.Categorical).alias("Jail"),
             # pl.col("Sentence")
             # .str.extract(r"Community Service Hrs\:\s+([0-9]|X?)") 
             # .alias("CommunityServiceHrs"),
             pl.col("Sentence")
             .str.extract(r"Jail Diversion\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
             .alias("JailDiversion"),
             # pl.col("Sentence")
             # .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s") 
             # .alias("Alcoholics Anonymous"),
             # pl.col("Sentence")
             # .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s") 
             # .alias("BadCheckSchool"),
             pl.col("Sentence")
             .str.extract(r"Informal Probation\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
             .alias("InformalProbation"),
             pl.col("Sentence")
             .str.extract(r"Court Referral Program\:\s+([0-9]|X?)\s") 
+            .cast(pl.Categorical)
             .alias("CourtReferralProgram"),
             # pl.col("Sentence")
             # .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s") 
             # .alias("CommunityService"),
             # pl.col("Sentence")
             # .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s") 
             # .alias("AlternativeSentencing"),
             # pl.col("Sentence")
             # .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s") 
             # .alias("PreTrialDiversion"),
             pl.col("Sentence")
             .str.extract(r"Dui School\:\s+([0-9A-Z]?)\s")
+            .cast(pl.Categorical)
             .alias("DUISchool"),
             # pl.col("Sentence")
             # .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s") 
             # .alias("DefensiveDrivingSchool"),
             # pl.col("Sentence")
             # .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)") 
             # .alias("DocCommunityCorrections"),
@@ -3035,38 +3113,43 @@
             # .str.extract(r"Mental Health\:\s+([0-9]|X?)")
             # .alias("MentalHealth"),
             # pl.col("Sentence")
             # .str.extract(r"Anger Management Program\:\s+([0-9]|X?)") 
             # .alias("AngerManagementProgram"),
             pl.col("Sentence")
             .str.extract(r"Drug Court\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
             .alias("DrugCourt"),
             pl.col("Sentence")
             .str.extract(r"Doc Drug Program\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
             .alias("DocDrugProgram"),
             # pl.col("Sentence")
             # .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project") 
             # .str.strip()
             # .alias("DrugMeasureUnit"),
             pl.col("Sentence")
             .str.extract(r"Drug Near Project\: (.+?)Drugs Near School")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("DrugNearProject"),
             pl.col("Sentence")
             .str.extract(r"Drugs Near School\: (.+?)Habitual Offender") 
             .str.replace(r'Habitual Offender\:','')
             .str.replace(r'Sex Offender Community Notification\:','')
             .str.replace(r'Drug Volume\:','')
             .str.replace(r'Drug\:','')
             .str.replace(r'Drug Code\:\s?\d*','')
             .str.strip()
+            .cast(pl.Categorical)
             .alias("DrugsNearSchool"),
             pl.col("Sentence")
             .str.extract(r"Habitual Offender\: (.+?)Sex Offender")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("HabitualOffender"),
             # pl.col("Sentence")
             # .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume") 
             # .str.replace_all(r"[X\s0-9]", "")
             # .str.replace(r'\.','')
             # .alias("SexOffenderCommunityNotification"),
             pl.col("Sentence")
@@ -3080,14 +3163,15 @@
             .alias("DrugCode"),
             pl.col("Sentence")
             .str.extract(r"Habitual Offender Number\: (.+?)Victim")
             .str.strip()
             .alias("HabitualOffenderNumber"),
             pl.col("Sentence")
             .str.extract(r"Victim DOB\:\s+(\d?\d?/?\d?\d?/?\d?\d?\d?\d?)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("VictimDOB"),
         ]
     )
     sent = sent.fill_null("")
     return sent
```

### Comparing `alacorder-80.2.4/src/alacorder/alac.py` & `alacorder-80.2.5/src/alacorder/alac.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.2.4"
+version = "80.2.5"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -641,15 +641,15 @@
     support_singletable = (
         True
         if outputext in (".xls", ".xlsx", "none", ".json", ".parquet", ".csv")
         else False
     )
     support_archive = (
         True
-        if outputext in (".xls", ".xlsx", ".csv", ".parquet", ".zip", ".json", "none")
+        if outputext in (".xls", ".xlsx", ".csv", ".parquet", ".json", "none")
         else False
     )
     if force not in (  # raise file extension not supported
         ".xls",
         ".xlsx",
         ".csv",
         ".parquet",
@@ -1620,14 +1620,15 @@
             .str.replace(r"\:", "")
             .str.strip()
             .alias("Alias"),
             pl.col("AllPagesText")
             .str.extract(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", group_index=1)
             .str.replace(r"[^\d/]", "")  # _all
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("DOB"),
             pl.concat_str(
                 [
                     pl.col("AllPagesText").str.extract(
                         r"(County: )(\d{2})", group_index=2
                     ),
                     pl.lit("-"),
@@ -1636,16 +1637,16 @@
             ).alias("CaseNumber"),
             pl.col("AllPagesText")
             .str.extract(r"(Phone: )(.+)", group_index=2)
             .str.replace_all(r"[^0-9]", "")
             .str.slice(0, 10)
             .str.replace(r"(.{3}0000000)", "")  # _all
             .alias("RE_Phone"),
-            pl.col("AllPagesText").str.extract(r"(B|W|H|A)/(?:F|M)").alias("Race"),
-            pl.col("AllPagesText").str.extract(r"(?:B|W|H|A)/(F|M)").alias("Sex"),
+            pl.col("AllPagesText").str.extract(r"(B|W|H|A)/(?:F|M)").cast(pl.Categorical).alias("Race"),
+            pl.col("AllPagesText").str.extract(r"(?:B|W|H|A)/(F|M)").cast(pl.Categorical).alias("Sex"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Address 1:)(.+)(?:Phone)*?", group_index=1)
             .str.replace(r"(Phone.+)", "")
             .str.strip()
             .alias("Address1"),
             pl.col("AllPagesText")
             .str.extract(r"(?:Address 2:)(.+)")
@@ -1659,14 +1660,15 @@
             pl.col("AllPagesText")
             .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=1)
             .str.strip()
             .alias("City"),
             pl.col("AllPagesText")
             .str.extract(r"(?:City: )(.*)(?:State: )(.*)", group_index=2)
             .str.strip()
+            .cast(pl.Categorical)
             .alias("State"),
             pl.col("AllPagesText")
             .str.extract(r"(Total:.+\$[^\n]*)")
             .str.replace_all(r"[^0-9|\.|\s|\$]", "")
             .str.extract_all(r"\s\$\d+\.\d{2}")
             .alias("TOTALS"),
             pl.col("AllPagesText")
@@ -1678,62 +1680,72 @@
             .alias("D999RAW"),
             pl.col("AllPagesText")
             .str.extract_all(r"(\w{2}\d{12})")
             .arr.join("/")
             .alias("RelatedCases"),
             pl.col("AllPagesText")
             .str.extract(r"Filing Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("FilingDate"),
             pl.col("AllPagesText")
             .str.extract(r"Case Initiation Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("CaseInitiationDate"),
             pl.col("AllPagesText")
             .str.extract(r"Arrest Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("ArrestDate"),
             pl.col("AllPagesText")
             .str.extract(r"Offense Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("OffenseDate"),
             pl.col("AllPagesText")
             .str.extract(r"Indictment Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("IndictmentDate"),
             pl.col("AllPagesText")
             .str.extract(r"Youthful Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("YouthfulDate"),
             pl.col("AllPagesText")
             .str.extract(r"AL Institutional Service Num: ([^\na-z])")
             .str.strip()
             .alias("ALInstitutionalServiceNum"),
             pl.col("AllPagesText")
             .str.extract(r"Alacourt\.com (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("Retrieved"),
             pl.col("AllPagesText")
             .str.extract(
                 r"Court Action: (BOUND|GUILTY PLEA|WAIVED TO GJ|DISMISSED|TIME LAPSED|NOL PROSS|CONVICTED|INDICTED|DISMISSED|FORFEITURE|TRANSFER|REMANDED|WAIVED|ACQUITTED|WITHDRAWN|PETITION|PRETRIAL|COND\. FORF\.)"
             )
             .alias("CourtAction"),
             pl.col("AllPagesText")
             .str.extract(r"Court Action Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("CourtActionDate"),
             pl.col("AllPagesText")
             .str.extract(r"Charge: ([A-Z\.0-9\-\s]+)")
             .str.rstrip("C")
             .str.strip()
             .alias("Description"),
             pl.col("AllPagesText")
             .str.extract(r"Jury Demand: ([A-Z]+)")
+            .cast(pl.Categorical)
             .alias("JuryDemand"),
             pl.col("AllPagesText").str.extract(
                 r"Inpatient Treatment Ordered: ([YES|NO]?)"
             )
-            # .str.strip()
+            .cast(pl.Categorical)
             .alias("InpatientTreatmentOrdered"),
             pl.col("AllPagesText")
             .str.extract(r"Trial Type: ([A-Z]+)")
             .str.replace(r"[S|N]$", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("TrialType"),
             pl.col("AllPagesText")
             .str.extract(r"Case Number: (\d\d-\w+) County:")
             .str.strip()
             .alias("County"),
             pl.col("AllPagesText")
             .str.extract(r"Judge: ([A-Z\-\.\s]+)")
@@ -1745,24 +1757,26 @@
             .alias("PROBATIONOFFICENUMBERRAW"),
             pl.col("AllPagesText")
             .str.extract(r"Defendant Status: ([A-Z\s]+)")
             .str.rstrip("J")
             .str.replace(r"\n", " ")
             .str.replace(r"\s+", " ")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("DefendantStatus"),
             pl.col("AllPagesText")
             .str.extract(r"([^0-9]+) Arresting Agency Type:")
             .str.replace(r"^\-.+", "")
             .str.replace(r"County\:", "")
             .str.replace(r"Defendant Status\:", "")
             .str.replace(r"Judge\:", "")
             .str.replace(r"Trial Type\:", "")
             .str.replace(r"Probation Office \#\:", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("ArrestingAgencyType"),
             pl.col("AllPagesText")
             .str.extract(r"Arresting Officer: ([A-Z\s]+)")
             .str.replace(r"[\s\n]+[A-Z0-9]$", "")
             .str.strip()
             .alias("ArrestingOfficer"),
             pl.col("AllPagesText")
@@ -1776,17 +1790,19 @@
             .str.strip()
             .cast(pl.Int64, strict=False)
             .alias("PreviousDUIConvictions"),
             pl.col("AllPagesText")
             .str.extract(r"Case Initiation Type: ([A-Z\s]+)")
             .str.rstrip("J")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("CaseInitiationType"),
             pl.col("AllPagesText")
             .str.extract(r"Domestic Violence: ([YES|NO])")
+            .cast(pl.Categorical)
             .alias("DomesticViolence"),
             pl.col("AllPagesText")
             .str.extract(r"Agency ORI: ([A-Z\s]+)")
             .str.rstrip("C")
             .str.replace(r"\n", "")
             .str.replace(r"\s+", " ")
             .str.strip()
@@ -1813,115 +1829,132 @@
             pl.col("AllPagesText")
             .str.extract(r"Eyes/Hair: (\w{3})/(\w{3})", group_index=2)
             .alias("Hair"),
             pl.col("AllPagesText")
             .str.extract(r"Country: (\w*+)")
             .str.replace(r"(Enforcement|Party)", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("Country"),
             pl.col("AllPagesText")
             .str.extract(r"(\d\d?/\d\d?/\d\d\d\d) Warrant Issuance Date:")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("WarrantIssuanceDate"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Action Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("WarrantActionDate"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Issuance Status: (\w+)")
             .str.replace(r"Description", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("WarrantIssuanceStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Action Status: (\w+)")
             .str.replace(r"Description", "")
             .str.strip()
             .alias("WarrantActionStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Location Status: (\w+)")
             .str.replace(r"Description", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("WarrantLocationStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Number Of Warrants: (\d{3}\s\d{3})")
             .str.strip()
             .alias("NumberOfWarrants"),
             pl.col("AllPagesText")
             .str.extract(r"Bond Type: (\w+)")  # +
             .str.replace(r"Bond", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("BondType"),
             pl.col("AllPagesText")
             .str.extract(r"Bond Type Desc: ([A-Z\s]+)")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("BondTypeDesc"),
             pl.col("AllPagesText")
             .str.extract(r"([\d\.]+) Bond Amount:")
             .cast(pl.Float64, strict=False)
             .alias("BondAmt"),
             pl.col("AllPagesText")
             .str.extract(r"Bond Company: ([A-Z0-9]+)")
             .str.rstrip("S")
             .alias("BondCompany"),
             pl.col("AllPagesText").str.extract(r"Surety Code: ([A-Z0-9]{4})")
             .alias("SuretyCode"),
             pl.col("AllPagesText").str.extract(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("BondReleaseDate"),
             pl.col("AllPagesText").str.extract(
                 r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)"
             )
+            .str.to_date('%m/%d/%Y', strict=False)
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
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("AppealDate"),
             pl.col("AllPagesText")
             .str.extract(r"([A-Z\-\s]+) Appeal Case Number")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("AppealCourt"),
             pl.col("AllPagesText")
             .str.extract(r"Orgin Of Appeal: ([A-Z\-\s]+)")
             .str.rstrip("L")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("OriginOfAppeal"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal To Desc: ([A-Z\-\s]+)")
             .str.replace(r"[\s\n]+[A-Z0-9]$", "")
             .str.rstrip("O")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("AppealToDesc"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal Status: ([A-Z\-\s]+)")
             .str.rstrip("A")
             .str.replace_all(r'\n','')
             .str.strip()
+            .cast(pl.Categorical)
             .alias("AppealStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Appeal To: (\w*) Appeal")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("AppealTo"),
             pl.col("AllPagesText")
             .str.extract(r"LowerCourt Appeal Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.replace_all(r"[\n\s:\-]", "")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("LowerCourtAppealDate"),
             pl.col("AllPagesText")
             .str.extract(r"Disposition Date Of Appeal: (\d\d?/\d\d?/\d\d\d\d)")
             .str.replace_all(r"[\n\s:\-]", "")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("DispositionDateOfAppeal"),
             pl.col("AllPagesText")
             .str.extract(r"Disposition Type Of Appeal: [^A-Za-z]+")
             .str.replace_all(r"[\n\s:\-]", "")
             .str.strip()
             .alias("DispositionTypeOfAppeal"),
             pl.col("AllPagesText")
@@ -1933,95 +1966,113 @@
             pl.col("AllPagesText")
             .str.extract(r"Updated By: (\w{3})")
             .str.strip()
             .alias("AdminUpdatedBy"),
             pl.col("AllPagesText")
             .str.extract(r"Transfer to Admin Doc Date: (\d\d?/\d\d?/\d\d\d\d)")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("TransferToAdminDocDate"),
             pl.col("AllPagesText")
             .str.extract(r"Transfer Desc: ([A-Z\s]{0,15} \d\d?/\d\d?/\d\d\d\d)")
             .str.replace_all(r"(Transfer Desc:)", "")
             .str.strip()
             .alias("TransferDesc"),
             pl.col("AllPagesText")
             .str.extract(r"Date Trial Began but No Verdict \(TBNV1\): ([^\n]+)")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("TBNV1"),
             pl.col("AllPagesText")
             .str.extract(r"Date Trial Began but No Verdict \(TBNV2\): ([^\n]+)")
             .str.replace(r"Financial", "")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("TBNV2"),
             pl.col("AllPagesText")
-            .str.extract(r"TurnOver Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"TurnOver Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
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
-            .str.extract(r"Due Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Due Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("DueDate"),
             pl.col("AllPagesText")
-            .str.extract(r"Last Paid Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Last Paid Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("LastPaidDate"),
-            pl.col("AllPagesText").str.extract(r"Payor\: ([A-Z0-9]{4})").alias("Payor"),
+            pl.col("AllPagesText").str.extract(r"Payor\: ([A-Z0-9]{4})").cast(pl.Categorical).alias("Payor"),
             pl.col("AllPagesText")
             .str.extract(r"Enforcement Status\: ([A-Z\:,\s]+)")
             .str.replace_all(r"\s+", " ")
             .str.replace(r" F$", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("EnforcementStatus"),
             pl.col("AllPagesText")
             .str.extract(r"Frequency\: ([W|M])")
             .str.replace(r"Cost Paid By\:", "")
             .str.strip()
             .alias("Frequency"),
             pl.col("AllPagesText")
             .str.extract(r"Placement Status\: (.+)")
             .str.strip()
             .alias("PlacementStatus"),
             pl.col("AllPagesText")
             .str.extract(r"PreTrial\: (YES|NO)")
+            .cast(pl.Categorical)
             .alias("PreTrial"),
             pl.col("AllPagesText")
             .str.extract(r"PreTrail Date\: (.+)PreTrial")
             .str.strip()
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("PreTrialDate"),
             pl.col("AllPagesText")
             .str.extract(r"PreTrial Terms\: (YES|NO)")
+            .cast(pl.Categorical)
             .alias("PreTrialTerms"),
             pl.col("AllPagesText")
-            .str.extract(r"Pre Terms Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Pre Terms Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("PreTermsDate"),
             pl.col("AllPagesText")
             .str.extract(r"Delinquent\: (YES|NO)")
+            .cast(pl.Categorical)
             .alias("Delinquent"),
             pl.col("AllPagesText")
-            .str.extract(r"Delinquent Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Delinquent Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("DelinquentDate"),
             pl.col("AllPagesText")
             .str.extract(r"DA Mailer\: (YES|NO)")
+            .cast(pl.Categorical)
             .alias("DAMailer"),
             pl.col("AllPagesText")
-            .str.extract(r"DA Mailer Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"DA Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("DAMailerDate"),
             pl.col("AllPagesText")
             .str.extract(r"Warrant Mailer\: (YES|NO)")
+            .cast(pl.Categorical)
             .alias("WarrantMailer"),
             pl.col("AllPagesText")
-            .str.extract(r"Warrant Mailer Date\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Warrant Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("WarrantMailerDate"),
             pl.col("AllPagesText")
-            .str.extract(r"Last Update\: (\d\d/\d\d/\d\d\d\d)")
+            .str.extract(r"Last Update\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("EnforcementLastUpdate"),
             pl.col("AllPagesText")
             .str.extract(r"Updated By\: ([A-Z]{3})")
             .alias("EnforcementUpdatedBy"),
         ]
     )
     cases = cases.with_columns(
@@ -2205,14 +2256,15 @@
         ]
     )
     fh = fh.explode("FinancialHistory")
     fh = fh.with_columns(
         [
             pl.col("FinancialHistory")
             .str.extract(r"(\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("TransactionDate"),
             pl.col("FinancialHistory")
             .str.extract(r"(RECEIPT|CREDIT)")
             .alias("Description"),
             pl.col("FinancialHistory")
             .str.extract(r"(\$\d+\.\d\d)")
             .str.replace(r"\$", "")
@@ -2457,15 +2509,20 @@
             )
             .str.strip()
             .str.replace(r",$", "")
             .str.replace(r"\s+", " ")
             .alias("ChargesSummary")
         ]
     )
-
+    charges = charges.with_columns([
+        pl.col("CourtActionDate").str.to_date('%m/%d/%Y', strict=False),
+        pl.col("Category").cast(pl.Categorical),
+        pl.col("TypeDescription").cast(pl.Categorical),
+        pl.col("CourtAction").cast(pl.Categorical)
+        ])
     charges = charges.select(
         "Name",
         "CaseNumber",
         "Num",
         "Code",
         "Cite",
         "Description",
@@ -2793,14 +2850,15 @@
             pl.col("CaseNumber"),
             pl.col("Sentence")
             .str.extract(r"Sentence\s(\d)\s")
             .cast(pl.Int64, strict=False)
             .alias("Number"),
             pl.col("Sentence")
             .str.extract(r"Last Update\:\s(\d\d?/\d\d?/\d\d\d\d)\sUpdated By\: [A-Z]{3}")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("LastUpdate"),
             pl.col("Sentence")
             .str.extract(r"Last Update\:\s\d\d?/\d\d?/\d\d\d\d\sUpdated By\: ([A-Z]{3})")
             .alias("UpdatedBy"),
             pl.col("Sentence")
             .str.extract(r"Probation Revoke\:(.+?) (Sentence|License)")
             .str.replace(r'Sentence.*','')
@@ -2814,37 +2872,43 @@
             .str.extract(r"Days\.\s*(\d+ Years, \d+ Months, \d+ Days\.)\s+")
             .alias("JailCreditPeriod"), 
             pl.col("Sentence")
             .str.extract(r"Probation Period\: (\d+ Years, \d+ Months, \d+ Days\.)")
             .alias("ProbationPeriod"),
             pl.col("Sentence")
             .str.extract(r"Sentence Provisions\: ([YN])")
+            .cast(pl.Categorical)
             .alias("Provisions"),
             pl.col("Sentence")
             .str.extract(r"Requrements Completed\: (YES|NO)")
+            .cast(pl.Categorical)
             .alias("RequirementsCompleted"),
             pl.col("Sentence")
             .str.extract(r"Sentence Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("SentenceDate"),
             pl.col("Sentence")
             .str.extract(r"Sentence Start Date\: (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("StartDate"),
             pl.col("Sentence")
             .str.extract(r"Sentence End Date\: .{0,40}? (\d\d?/\d\d?/\d\d\d\d)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("EndDate"),
             pl.col("Sentence")
             .str.extract(r"Jail Fee\:(.+?)Costs")
             .str.replace(r"[A-Z]-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("JailFee"),
             pl.col("Sentence")
             .str.extract(r"Costs\: (.+?)Fine\:")
             .str.replace(r'Fine.+','')
             .str.strip()
+            .cast(pl.Categorical)
             .alias("Costs"),
             # pl.col("Sentence")
             # .str.extract(r"Fine\:(.+?)Crime Victims") 
             # .str.strip()
             # .alias("Fine"),
             # pl.col("Sentence")
             # .str.extract(r"Crime Victims Fee\:(.+?)Monetary")
@@ -2876,14 +2940,15 @@
             # .str.replace(r'Prelim Hearing.+','')
             # .str.strip()
             # .alias("DrugDocketFees"),
             pl.col("Sentence")
             .str.extract(r"Prelim Hearing\:(.+?)Amt Over Minimum CVF")
             .str.replace(r'Amt.+','') 
             .str.strip()
+            .cast(pl.Categorical)
             .alias("PrelimHearing"),
             pl.col("Sentence")
             .str.extract(r"Amt Over Minimum CVF\: (.+?) WC Fee DA")
             .str.replace_all(r"[A-Z\s]|\-|\$", "")
             .cast(pl.Float64, strict=False)
             .alias("AmtOverMinimumCVF"),
             # pl.col("Sentence")
@@ -2893,38 +2958,42 @@
             # pl.col("Sentence")
             # .str.extract(r"Removal Bill\: (.+?)Crime History Fee")
             # .str.strip()
             # .alias("RemovalBill"),
             pl.col("Sentence")
             .str.extract(r"Crime History Fee\: (.+?) SX10") 
             .str.strip()
+            .cast(pl.Categorical)
             .alias("CrimeHistoryFee"),
             pl.col("Sentence")
             .str.extract(r"SX10\: (.+?)License Suspension Fee")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("SX10"),
             pl.col("Sentence")
             .str.extract(r"License Suspension Fee\: (.+?) WC Fee 85%")
             .str.replace_all(r"[A-Z\s]+", "")
             .cast(pl.Float64, strict=False)
             .alias("LicenseSuspensionFee"),
             pl.col("Sentence")
             .str.extract(r"WC Fee 85%\: (.+?) Demand Reduction Hearing\:") 
             .str.replace(r'Demand Reduction Hearing.+','')
             .str.strip()
+            .cast(pl.Categorical)
             .alias("WCFee85"),
             pl.col("Sentence")
             .str.extract(r"Demand Reduction Hearing\: (.+?)Drug User Fee") 
             .str.replace_all(r"[A-Z]\-|\s|\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("DemandReductionHearing"),
             pl.col("Sentence")
             .str.extract(r"Drug User Fee\: (.+?) Subpoena")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("DrugUserFee"),
             pl.col("Sentence")
             .str.extract(r"Subpoena\: (.+?) Attorney Fees")
             .str.replace_all(r"[X\-\s\$]", "")
             .cast(pl.Float64, strict=False)
             .alias("Subpoena"),
             # pl.col("Sentence")
@@ -2951,20 +3020,22 @@
                 r"Suspended Confinement Period (\d+ Years, \d+ Months, \d+ Days\.)"
             )
             .alias("SuspendedConfinementPeriod"),
             pl.col("Sentence")
             .str.extract(r"Boot Camp\: (.+?) (Penitentiary|Life Without Parole)")
             .str.replace(r'Penitentiary.+','')
             .str.strip()
+            .cast(pl.Categorical)
             .alias("BootCamp"),
             pl.col("Sentence")
             .str.extract(r"Life Without Parole\: (.+?) (Restitution|Death\:)", group_index=1) 
             .str.replace(r'Death.+','')
             .str.replace(r'Restitution.+','')
             .str.strip()
+            .cast(pl.Categorical)
             .alias("LifeWithoutParole"),
             # pl.col("Sentence")
             # .str.extract(r"Split\: (.+?) (Concurrent|Confinement)", group_index=1) 
             # .str.strip()
             # .alias("Split"),
             # pl.col("Sentence")
             # .str.extract(r"Concurrent Sentence\:\s+([A-Z]?)\s")
@@ -2973,58 +3044,65 @@
             # pl.col("Sentence")
             # .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s") 
             # .str.strip()
             # .alias("ConsecutiveSentence"),
             pl.col("Sentence")
             .str.extract(r"Electronic Monitoring\: (.+?) Reverse Split")
             .str.replace_all(r"[-0\s]", "")
+            .cast(pl.Categorical)
             .alias("ElectronicMonitoring"),
             pl.col("Sentence")
             .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)") 
             .str.replace_all(r"Death\: Life\:", "")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("ReverseSplit"),
             # pl.col("Sentence")
             # .str.extract(r"Coterminous Sentence\:\s+([A-Z]?)\s")
             # .alias("CoterminousSentence"),
             # pl.col("Sentence").str.extract(r"Death\:\s+(X?)").alias("Death"),
             pl.col("Sentence").str.extract(r"Life\:\s+(X?)").alias("Life"),
             pl.col("Sentence")
             .str.extract(r"Chain Gang\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
             .alias("ChainGang"),
-            pl.col("Sentence").str.extract(r"Jail\:\s+([0-9]|X?)").alias("Jail"),
+            pl.col("Sentence").str.extract(r"Jail\:\s+([0-9]|X?)").cast(pl.Categorical).alias("Jail"),
             # pl.col("Sentence")
             # .str.extract(r"Community Service Hrs\:\s+([0-9]|X?)") 
             # .alias("CommunityServiceHrs"),
             pl.col("Sentence")
             .str.extract(r"Jail Diversion\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
             .alias("JailDiversion"),
             # pl.col("Sentence")
             # .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s") 
             # .alias("Alcoholics Anonymous"),
             # pl.col("Sentence")
             # .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s") 
             # .alias("BadCheckSchool"),
             pl.col("Sentence")
             .str.extract(r"Informal Probation\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
             .alias("InformalProbation"),
             pl.col("Sentence")
             .str.extract(r"Court Referral Program\:\s+([0-9]|X?)\s") 
+            .cast(pl.Categorical)
             .alias("CourtReferralProgram"),
             # pl.col("Sentence")
             # .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s") 
             # .alias("CommunityService"),
             # pl.col("Sentence")
             # .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s") 
             # .alias("AlternativeSentencing"),
             # pl.col("Sentence")
             # .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s") 
             # .alias("PreTrialDiversion"),
             pl.col("Sentence")
             .str.extract(r"Dui School\:\s+([0-9A-Z]?)\s")
+            .cast(pl.Categorical)
             .alias("DUISchool"),
             # pl.col("Sentence")
             # .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s") 
             # .alias("DefensiveDrivingSchool"),
             # pl.col("Sentence")
             # .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)") 
             # .alias("DocCommunityCorrections"),
@@ -3035,38 +3113,43 @@
             # .str.extract(r"Mental Health\:\s+([0-9]|X?)")
             # .alias("MentalHealth"),
             # pl.col("Sentence")
             # .str.extract(r"Anger Management Program\:\s+([0-9]|X?)") 
             # .alias("AngerManagementProgram"),
             pl.col("Sentence")
             .str.extract(r"Drug Court\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
             .alias("DrugCourt"),
             pl.col("Sentence")
             .str.extract(r"Doc Drug Program\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
             .alias("DocDrugProgram"),
             # pl.col("Sentence")
             # .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project") 
             # .str.strip()
             # .alias("DrugMeasureUnit"),
             pl.col("Sentence")
             .str.extract(r"Drug Near Project\: (.+?)Drugs Near School")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("DrugNearProject"),
             pl.col("Sentence")
             .str.extract(r"Drugs Near School\: (.+?)Habitual Offender") 
             .str.replace(r'Habitual Offender\:','')
             .str.replace(r'Sex Offender Community Notification\:','')
             .str.replace(r'Drug Volume\:','')
             .str.replace(r'Drug\:','')
             .str.replace(r'Drug Code\:\s?\d*','')
             .str.strip()
+            .cast(pl.Categorical)
             .alias("DrugsNearSchool"),
             pl.col("Sentence")
             .str.extract(r"Habitual Offender\: (.+?)Sex Offender")
             .str.strip()
+            .cast(pl.Categorical)
             .alias("HabitualOffender"),
             # pl.col("Sentence")
             # .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume") 
             # .str.replace_all(r"[X\s0-9]", "")
             # .str.replace(r'\.','')
             # .alias("SexOffenderCommunityNotification"),
             pl.col("Sentence")
@@ -3080,14 +3163,15 @@
             .alias("DrugCode"),
             pl.col("Sentence")
             .str.extract(r"Habitual Offender Number\: (.+?)Victim")
             .str.strip()
             .alias("HabitualOffenderNumber"),
             pl.col("Sentence")
             .str.extract(r"Victim DOB\:\s+(\d?\d?/?\d?\d?/?\d?\d?\d?\d?)")
+            .str.to_date('%m/%d/%Y', strict=False)
             .alias("VictimDOB"),
         ]
     )
     sent = sent.fill_null("")
     return sent
```

### Comparing `alacorder-80.2.4/PKG-INFO` & `alacorder-80.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.2.4
+Version: 80.2.5
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

