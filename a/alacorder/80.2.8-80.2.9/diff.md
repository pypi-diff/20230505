# Comparing `tmp/alacorder-80.2.8.tar.gz` & `tmp/alacorder-80.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.2.8.tar", max compression
+gzip compressed data, was "alacorder-80.2.9.tar", max compression
```

## Comparing `alacorder-80.2.8.tar` & `alacorder-80.2.9.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.2.8/LICENSE
--rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.2.8/README.md
--rw-r--r--   0        0        0      697 2023-05-05 19:56:30.927112 alacorder-80.2.8/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-05 19:36:29.887923 alacorder-80.2.8/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.2.8/src/alacorder/__init__.py
--rw-r--r--   0        0        0   219919 2023-05-05 19:55:49.707172 alacorder-80.2.8/src/alacorder/__main__.py
--rw-r--r--   0        0        0   219919 2023-05-05 19:55:34.492224 alacorder-80.2.8/src/alacorder/alac.py
--rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.2.9/LICENSE
+-rw-r--r--   0        0        0     6889 2023-04-30 22:20:34.472204 alacorder-80.2.9/README.md
+-rw-r--r--   0        0        0      697 2023-05-05 21:04:13.328849 alacorder-80.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.2.9/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   220075 2023-05-05 21:03:50.354455 alacorder-80.2.9/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   220075 2023-05-05 21:03:45.400426 alacorder-80.2.9/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 alacorder-80.2.9/PKG-INFO
```

### Comparing `alacorder-80.2.8/LICENSE` & `alacorder-80.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.2.8/README.md` & `alacorder-80.2.9/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.2.8/pyproject.toml` & `alacorder-80.2.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.2.8"
+version = "80.2.9"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.2.8/src/alacorder/__main__.py` & `alacorder-80.2.9/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.2.8"
+version = "80.2.9"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2939,67 +2939,68 @@
             .alias("JailFee"),
             pl.col("Sentence")
             .str.extract(r"Costs\: (.+?)Fine\:")
             .str.replace(r"Fine.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("Costs"),
-            # pl.col("Sentence")
-            # .str.extract(r"Fine\:(.+?)Crime Victims")
-            # .str.strip()
-            # .alias("Fine"),
-            # pl.col("Sentence")
-            # .str.extract(r"Crime Victims Fee\:(.+?)Monetary")
-            # .str.strip()
-            # .alias("CrimeVictimsFee"),
+            pl.col("Sentence")
+            .str.extract(r"Fine\:(.+?)Crime Victims")
+            .str.strip()
+            .cast(pl.Categorical)
+            .alias("Fine"),
+            pl.col("Sentence")
+            .str.extract(r"Crime Victims Fee\:(.+?)Monetary")
+            .str.strip()
+            .alias("CrimeVictimsFee"),
             pl.col("Sentence")
             .str.extract(r"Municipal Court\:(.+?)Fine Suspended")  ## NONE
             .str.replace(r"X-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("MunicipalCourt"),
-            # pl.col("Sentence")
-            # .str.extract(r"Fine Suspended\: (.+?)Immigration Fine")
-            # .str.strip()
-            # .alias("FineSuspended"),
+            pl.col("Sentence")
+            .str.extract(r"Fine Suspended\: (.+?)Immigration Fine")
+            .str.strip()
+            .alias("FineSuspended"),
             pl.col("Sentence")
             .str.extract(r"Immigration Fine\: (.+?)Fine")
             .str.replace(r"X\-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("ImmigrationFine"),
             pl.col("Sentence")
             .str.extract(r"Fine Imposed\: (.+?) Alias Warrant")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("FineImposed"),
-            # pl.col("Sentence")
-            # .str.extract(r"Drug Docket Fees\: (.+?)Prelim Hearing")
-            # .str.replace(r'Prelim Hearing.+','')
-            # .str.strip()
-            # .alias("DrugDocketFees"),
+            pl.col("Sentence")
+            .str.extract(r"Drug Docket Fees\: (.+?)Prelim Hearing")
+            .str.replace(r'Prelim Hearing.+','')
+            .str.strip()
+            .alias("DrugDocketFees"),
             pl.col("Sentence")
             .str.extract(r"Prelim Hearing\:(.+?)Amt Over Minimum CVF")
             .str.replace(r"Amt.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("PrelimHearing"),
             pl.col("Sentence")
             .str.extract(r"Amt Over Minimum CVF\: (.+?) WC Fee DA")
             .str.replace_all(r"[A-Z\s]|\-|\$", "")
             .cast(pl.Float64, strict=False)
             .alias("AmtOverMinimumCVF"),
-            # pl.col("Sentence")
-            # .str.extract(r"WC Fee DA\: (.+?)Removal Bill")
-            # .str.strip()
-            # .alias("WCFeeDA"),
-            # pl.col("Sentence")
-            # .str.extract(r"Removal Bill\: (.+?)Crime History Fee")
-            # .str.strip()
-            # .alias("RemovalBill"),
+            pl.col("Sentence")
+            .str.extract(r"WC Fee DA\: (.+?)Removal Bill")
+            .str.strip()
+            .alias("WCFeeDA"),
+            pl.col("Sentence")
+            .str.extract(r"Removal Bill\: (.+?)Crime History Fee")
+            .str.strip()
+            .alias("RemovalBill"),
             pl.col("Sentence")
             .str.extract(r"Crime History Fee\: (.+?) SX10")
             .str.strip()
             .cast(pl.Categorical)
             .alias("CrimeHistoryFee"),
             pl.col("Sentence")
             .str.extract(r"SX10\: (.+?)License Suspension Fee")
@@ -3029,23 +3030,23 @@
             .cast(pl.Categorical)
             .alias("DrugUserFee"),
             pl.col("Sentence")
             .str.extract(r"Subpoena\: (.+?) Attorney Fees")
             .str.replace_all(r"[X\-\s\$]", "")
             .cast(pl.Float64, strict=False)
             .alias("Subpoena"),
-            # pl.col("Sentence")
-            # .str.extract(r"Attorney Fees\: (.+?) (Confinement|Split|Restitution)")
-            # .str.replace("© Alacourt.com", "", literal=True)
-            # .str.replace(r'Split.+','')
-            # .str.replace(r'Confinement.+','')
-            # .str.replace(r"\d?\d/\d?\d/\d\d\d\d \d", "")
-            # .str.replace(r"\$|Recipient", "")
-            # .str.replace_all(r"\s+", "")
-            # .alias("AttorneyFees"),
+            pl.col("Sentence")
+            .str.extract(r"Attorney Fees\: (.+?) (Confinement|Split|Restitution)")
+            .str.replace("© Alacourt.com", "", literal=True)
+            .str.replace(r'Split.+','')
+            .str.replace(r'Confinement.+','')
+            .str.replace(r"\d?\d/\d?\d/\d\d\d\d \d", "")
+            .str.replace(r"\$|Recipient", "")
+            .str.replace_all(r"\s+", "")
+            .alias("AttorneyFees"),
             pl.col("Sentence")
             .str.extract(
                 r"Imposed Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
             )
             .alias("ImposedConfinementPeriod"),
             pl.col("Sentence")
             .str.extract(
@@ -3068,111 +3069,119 @@
                 r"Life Without Parole\: (.+?) (Restitution|Death\:)", group_index=1
             )
             .str.replace(r"Death.+", "")
             .str.replace(r"Restitution.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("LifeWithoutParole"),
-            # pl.col("Sentence")
-            # .str.extract(r"Split\: (.+?) (Concurrent|Confinement)", group_index=1)
-            # .str.strip()
-            # .alias("Split"),
-            # pl.col("Sentence")
-            # .str.extract(r"Concurrent Sentence\:\s+([A-Z]?)\s")
-            # .str.strip()
-            # .alias("ConcurrentSentence"),
-            # pl.col("Sentence")
-            # .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s")
-            # .str.strip()
-            # .alias("ConsecutiveSentence"),
+            pl.col("Sentence")
+            .str.extract(r"Split\: (.+?) (Concurrent|Confinement)", group_index=1)
+            .str.strip()
+            .alias("Split"),
+            pl.col("Sentence")
+            .str.extract(r"Concurrent Sentence\:\s+([A-Z]?)\s")
+            .str.strip()
+            .alias("ConcurrentSentence"),
+            pl.col("Sentence")
+            .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s")
+            .str.strip()
+            .alias("ConsecutiveSentence"),
             pl.col("Sentence")
             .str.extract(r"Electronic Monitoring\: (.+?) Reverse Split")
             .str.replace_all(r"[-0\s]", "")
             .cast(pl.Categorical)
             .alias("ElectronicMonitoring"),
             pl.col("Sentence")
             .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)")
             .str.replace_all(r"Death\: Life\:", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("ReverseSplit"),
-            # pl.col("Sentence")
-            # .str.extract(r"Coterminous Sentence\:\s+([A-Z]?)\s")
-            # .alias("CoterminousSentence"),
-            # pl.col("Sentence").str.extract(r"Death\:\s+(X?)").alias("Death"),
+            pl.col("Sentence")
+            .str.extract(r"Coterminous Sentence\:\s+([A-Z]?)\s")
+            .alias("CoterminousSentence"),
+            pl.col("Sentence").str.extract(r"Death\:\s+(X?)").alias("Death"),
             pl.col("Sentence").str.extract(r"Life\:\s+(X?)").alias("Life"),
             pl.col("Sentence")
             .str.extract(r"Chain Gang\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("ChainGang"),
             pl.col("Sentence")
             .str.extract(r"Jail\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("Jail"),
-            # pl.col("Sentence")
-            # .str.extract(r"Community Service Hrs\:\s+([0-9]|X?)")
-            # .alias("CommunityServiceHrs"),
+            pl.col("Sentence")
+            .str.extract(r"Community Service Hrs\:\s+([0-9]|X?)")
+            .alias("CommunityServiceHrs"),
             pl.col("Sentence")
             .str.extract(r"Jail Diversion\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("JailDiversion"),
-            # pl.col("Sentence")
-            # .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s")
-            # .alias("Alcoholics Anonymous"),
-            # pl.col("Sentence")
-            # .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s")
-            # .alias("BadCheckSchool"),
+            pl.col("Sentence")
+            .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s")
+            .cast(pl.Categorical)
+            .alias("Alcoholics Anonymous"),
+            pl.col("Sentence")
+            .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s")
+            .cast(pl.Categorical)
+            .alias("BadCheckSchool"),
             pl.col("Sentence")
             .str.extract(r"Informal Probation\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("InformalProbation"),
             pl.col("Sentence")
             .str.extract(r"Court Referral Program\:\s+([0-9]|X?)\s")
             .cast(pl.Categorical)
             .alias("CourtReferralProgram"),
-            # pl.col("Sentence")
-            # .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s")
-            # .alias("CommunityService"),
-            # pl.col("Sentence")
-            # .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s")
-            # .alias("AlternativeSentencing"),
-            # pl.col("Sentence")
-            # .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s")
-            # .alias("PreTrialDiversion"),
+            pl.col("Sentence")
+            .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s")
+            .alias("CommunityService"),
+            pl.col("Sentence")
+            .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s")
+            .alias("AlternativeSentencing"),
+            pl.col("Sentence")
+            .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s")
+            .alias("PreTrialDiversion"),
             pl.col("Sentence")
             .str.extract(r"Dui School\:\s+([0-9A-Z]?)\s")
             .cast(pl.Categorical)
             .alias("DUISchool"),
-            # pl.col("Sentence")
-            # .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s")
-            # .alias("DefensiveDrivingSchool"),
-            # pl.col("Sentence")
-            # .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)")
-            # .alias("DocCommunityCorrections"),
-            # pl.col("Sentence")
-            # .str.extract(r"Jail Community Corrections\:\s+([0-9]|X?)")
-            # .alias("JailCommunityCorrections"),
-            # pl.col("Sentence")
-            # .str.extract(r"Mental Health\:\s+([0-9]|X?)")
-            # .alias("MentalHealth"),
-            # pl.col("Sentence")
-            # .str.extract(r"Anger Management Program\:\s+([0-9]|X?)")
-            # .alias("AngerManagementProgram"),
+            pl.col("Sentence")
+            .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s")
+            .cast(pl.Categorical)
+            .alias("DefensiveDrivingSchool"),
+            pl.col("Sentence")
+            .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
+            .alias("DocCommunityCorrections"),
+            pl.col("Sentence")
+            .str.extract(r"Jail Community Corrections\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
+            .alias("JailCommunityCorrections"),
+            pl.col("Sentence")
+            .str.extract(r"Mental Health\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
+            .alias("MentalHealth"),
+            pl.col("Sentence")
+            .str.extract(r"Anger Management Program\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
+            .alias("AngerManagementProgram"),
             pl.col("Sentence")
             .str.extract(r"Drug Court\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("DrugCourt"),
             pl.col("Sentence")
             .str.extract(r"Doc Drug Program\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("DocDrugProgram"),
-            # pl.col("Sentence")
-            # .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project")
-            # .str.strip()
-            # .alias("DrugMeasureUnit"),
+            pl.col("Sentence")
+            .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project")
+            .str.strip()
+            .cast(pl.Categorical)
+            .alias("DrugMeasureUnit"),
             pl.col("Sentence")
             .str.extract(r"Drug Near Project\: (.+?)Drugs Near School")
             .str.strip()
             .cast(pl.Categorical)
             .alias("DrugNearProject"),
             pl.col("Sentence")
             .str.extract(r"Drugs Near School\: (.+?)Habitual Offender")
@@ -3185,19 +3194,20 @@
             .cast(pl.Categorical)
             .alias("DrugsNearSchool"),
             pl.col("Sentence")
             .str.extract(r"Habitual Offender\: (.+?)Sex Offender")
             .str.strip()
             .cast(pl.Categorical)
             .alias("HabitualOffender"),
-            # pl.col("Sentence")
-            # .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume")
-            # .str.replace_all(r"[X\s0-9]", "")
-            # .str.replace(r'\.','')
-            # .alias("SexOffenderCommunityNotification"),
+            pl.col("Sentence")
+            .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume")
+            .str.replace_all(r"[X\s0-9]", "")
+            .str.replace(r'\.','')
+            .cast(pl.Categorical)
+            .alias("SexOffenderCommunityNotification"),
             pl.col("Sentence")
             .str.extract(r"(\d+\.\d\d)\sDrug Volume\:")
             .cast(pl.Float64, strict=False)
             .alias("DrugVolume"),
             pl.col("Sentence")
             .str.extract(r"Drug Code\: (.+?)Habitual Offender Number")
             .str.strip()
```

### Comparing `alacorder-80.2.8/src/alacorder/alac.py` & `alacorder-80.2.9/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.2.8"
+version = "80.2.9"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2939,67 +2939,68 @@
             .alias("JailFee"),
             pl.col("Sentence")
             .str.extract(r"Costs\: (.+?)Fine\:")
             .str.replace(r"Fine.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("Costs"),
-            # pl.col("Sentence")
-            # .str.extract(r"Fine\:(.+?)Crime Victims")
-            # .str.strip()
-            # .alias("Fine"),
-            # pl.col("Sentence")
-            # .str.extract(r"Crime Victims Fee\:(.+?)Monetary")
-            # .str.strip()
-            # .alias("CrimeVictimsFee"),
+            pl.col("Sentence")
+            .str.extract(r"Fine\:(.+?)Crime Victims")
+            .str.strip()
+            .cast(pl.Categorical)
+            .alias("Fine"),
+            pl.col("Sentence")
+            .str.extract(r"Crime Victims Fee\:(.+?)Monetary")
+            .str.strip()
+            .alias("CrimeVictimsFee"),
             pl.col("Sentence")
             .str.extract(r"Municipal Court\:(.+?)Fine Suspended")  ## NONE
             .str.replace(r"X-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("MunicipalCourt"),
-            # pl.col("Sentence")
-            # .str.extract(r"Fine Suspended\: (.+?)Immigration Fine")
-            # .str.strip()
-            # .alias("FineSuspended"),
+            pl.col("Sentence")
+            .str.extract(r"Fine Suspended\: (.+?)Immigration Fine")
+            .str.strip()
+            .alias("FineSuspended"),
             pl.col("Sentence")
             .str.extract(r"Immigration Fine\: (.+?)Fine")
             .str.replace(r"X\-\$", "")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("ImmigrationFine"),
             pl.col("Sentence")
             .str.extract(r"Fine Imposed\: (.+?) Alias Warrant")
             .str.strip()
             .cast(pl.Float64, strict=False)
             .alias("FineImposed"),
-            # pl.col("Sentence")
-            # .str.extract(r"Drug Docket Fees\: (.+?)Prelim Hearing")
-            # .str.replace(r'Prelim Hearing.+','')
-            # .str.strip()
-            # .alias("DrugDocketFees"),
+            pl.col("Sentence")
+            .str.extract(r"Drug Docket Fees\: (.+?)Prelim Hearing")
+            .str.replace(r'Prelim Hearing.+','')
+            .str.strip()
+            .alias("DrugDocketFees"),
             pl.col("Sentence")
             .str.extract(r"Prelim Hearing\:(.+?)Amt Over Minimum CVF")
             .str.replace(r"Amt.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("PrelimHearing"),
             pl.col("Sentence")
             .str.extract(r"Amt Over Minimum CVF\: (.+?) WC Fee DA")
             .str.replace_all(r"[A-Z\s]|\-|\$", "")
             .cast(pl.Float64, strict=False)
             .alias("AmtOverMinimumCVF"),
-            # pl.col("Sentence")
-            # .str.extract(r"WC Fee DA\: (.+?)Removal Bill")
-            # .str.strip()
-            # .alias("WCFeeDA"),
-            # pl.col("Sentence")
-            # .str.extract(r"Removal Bill\: (.+?)Crime History Fee")
-            # .str.strip()
-            # .alias("RemovalBill"),
+            pl.col("Sentence")
+            .str.extract(r"WC Fee DA\: (.+?)Removal Bill")
+            .str.strip()
+            .alias("WCFeeDA"),
+            pl.col("Sentence")
+            .str.extract(r"Removal Bill\: (.+?)Crime History Fee")
+            .str.strip()
+            .alias("RemovalBill"),
             pl.col("Sentence")
             .str.extract(r"Crime History Fee\: (.+?) SX10")
             .str.strip()
             .cast(pl.Categorical)
             .alias("CrimeHistoryFee"),
             pl.col("Sentence")
             .str.extract(r"SX10\: (.+?)License Suspension Fee")
@@ -3029,23 +3030,23 @@
             .cast(pl.Categorical)
             .alias("DrugUserFee"),
             pl.col("Sentence")
             .str.extract(r"Subpoena\: (.+?) Attorney Fees")
             .str.replace_all(r"[X\-\s\$]", "")
             .cast(pl.Float64, strict=False)
             .alias("Subpoena"),
-            # pl.col("Sentence")
-            # .str.extract(r"Attorney Fees\: (.+?) (Confinement|Split|Restitution)")
-            # .str.replace("© Alacourt.com", "", literal=True)
-            # .str.replace(r'Split.+','')
-            # .str.replace(r'Confinement.+','')
-            # .str.replace(r"\d?\d/\d?\d/\d\d\d\d \d", "")
-            # .str.replace(r"\$|Recipient", "")
-            # .str.replace_all(r"\s+", "")
-            # .alias("AttorneyFees"),
+            pl.col("Sentence")
+            .str.extract(r"Attorney Fees\: (.+?) (Confinement|Split|Restitution)")
+            .str.replace("© Alacourt.com", "", literal=True)
+            .str.replace(r'Split.+','')
+            .str.replace(r'Confinement.+','')
+            .str.replace(r"\d?\d/\d?\d/\d\d\d\d \d", "")
+            .str.replace(r"\$|Recipient", "")
+            .str.replace_all(r"\s+", "")
+            .alias("AttorneyFees"),
             pl.col("Sentence")
             .str.extract(
                 r"Imposed Confinement Period\: (\d+ Years, \d+ Months, \d+ Days\.)"
             )
             .alias("ImposedConfinementPeriod"),
             pl.col("Sentence")
             .str.extract(
@@ -3068,111 +3069,119 @@
                 r"Life Without Parole\: (.+?) (Restitution|Death\:)", group_index=1
             )
             .str.replace(r"Death.+", "")
             .str.replace(r"Restitution.+", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("LifeWithoutParole"),
-            # pl.col("Sentence")
-            # .str.extract(r"Split\: (.+?) (Concurrent|Confinement)", group_index=1)
-            # .str.strip()
-            # .alias("Split"),
-            # pl.col("Sentence")
-            # .str.extract(r"Concurrent Sentence\:\s+([A-Z]?)\s")
-            # .str.strip()
-            # .alias("ConcurrentSentence"),
-            # pl.col("Sentence")
-            # .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s")
-            # .str.strip()
-            # .alias("ConsecutiveSentence"),
+            pl.col("Sentence")
+            .str.extract(r"Split\: (.+?) (Concurrent|Confinement)", group_index=1)
+            .str.strip()
+            .alias("Split"),
+            pl.col("Sentence")
+            .str.extract(r"Concurrent Sentence\:\s+([A-Z]?)\s")
+            .str.strip()
+            .alias("ConcurrentSentence"),
+            pl.col("Sentence")
+            .str.extract(r"Consecutive Sentence\:\s+([A-Z]?)\s")
+            .str.strip()
+            .alias("ConsecutiveSentence"),
             pl.col("Sentence")
             .str.extract(r"Electronic Monitoring\: (.+?) Reverse Split")
             .str.replace_all(r"[-0\s]", "")
             .cast(pl.Categorical)
             .alias("ElectronicMonitoring"),
             pl.col("Sentence")
             .str.extract(r"Reverse Split\: (.+?) (Boot Camp|Coterminous)")
             .str.replace_all(r"Death\: Life\:", "")
             .str.strip()
             .cast(pl.Categorical)
             .alias("ReverseSplit"),
-            # pl.col("Sentence")
-            # .str.extract(r"Coterminous Sentence\:\s+([A-Z]?)\s")
-            # .alias("CoterminousSentence"),
-            # pl.col("Sentence").str.extract(r"Death\:\s+(X?)").alias("Death"),
+            pl.col("Sentence")
+            .str.extract(r"Coterminous Sentence\:\s+([A-Z]?)\s")
+            .alias("CoterminousSentence"),
+            pl.col("Sentence").str.extract(r"Death\:\s+(X?)").alias("Death"),
             pl.col("Sentence").str.extract(r"Life\:\s+(X?)").alias("Life"),
             pl.col("Sentence")
             .str.extract(r"Chain Gang\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("ChainGang"),
             pl.col("Sentence")
             .str.extract(r"Jail\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("Jail"),
-            # pl.col("Sentence")
-            # .str.extract(r"Community Service Hrs\:\s+([0-9]|X?)")
-            # .alias("CommunityServiceHrs"),
+            pl.col("Sentence")
+            .str.extract(r"Community Service Hrs\:\s+([0-9]|X?)")
+            .alias("CommunityServiceHrs"),
             pl.col("Sentence")
             .str.extract(r"Jail Diversion\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("JailDiversion"),
-            # pl.col("Sentence")
-            # .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s")
-            # .alias("Alcoholics Anonymous"),
-            # pl.col("Sentence")
-            # .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s")
-            # .alias("BadCheckSchool"),
+            pl.col("Sentence")
+            .str.extract(r"Alcoholics Anonymous\:\s+([0-9]|[A-Z]?)\s")
+            .cast(pl.Categorical)
+            .alias("Alcoholics Anonymous"),
+            pl.col("Sentence")
+            .str.extract(r"Bad Check School\:\s+([0-9]|[A-Z]?)\s")
+            .cast(pl.Categorical)
+            .alias("BadCheckSchool"),
             pl.col("Sentence")
             .str.extract(r"Informal Probation\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("InformalProbation"),
             pl.col("Sentence")
             .str.extract(r"Court Referral Program\:\s+([0-9]|X?)\s")
             .cast(pl.Categorical)
             .alias("CourtReferralProgram"),
-            # pl.col("Sentence")
-            # .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s")
-            # .alias("CommunityService"),
-            # pl.col("Sentence")
-            # .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s")
-            # .alias("AlternativeSentencing"),
-            # pl.col("Sentence")
-            # .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s")
-            # .alias("PreTrialDiversion"),
+            pl.col("Sentence")
+            .str.extract(r"Community Service\:\s+([0-9A-Z]?)\s")
+            .alias("CommunityService"),
+            pl.col("Sentence")
+            .str.extract(r"Alternative Sentencing\:\s+([0-9A-Z]?)\s")
+            .alias("AlternativeSentencing"),
+            pl.col("Sentence")
+            .str.extract(r"PreTrail Diversion\:\s+([0-9A-Z]?)\s")
+            .alias("PreTrialDiversion"),
             pl.col("Sentence")
             .str.extract(r"Dui School\:\s+([0-9A-Z]?)\s")
             .cast(pl.Categorical)
             .alias("DUISchool"),
-            # pl.col("Sentence")
-            # .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s")
-            # .alias("DefensiveDrivingSchool"),
-            # pl.col("Sentence")
-            # .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)")
-            # .alias("DocCommunityCorrections"),
-            # pl.col("Sentence")
-            # .str.extract(r"Jail Community Corrections\:\s+([0-9]|X?)")
-            # .alias("JailCommunityCorrections"),
-            # pl.col("Sentence")
-            # .str.extract(r"Mental Health\:\s+([0-9]|X?)")
-            # .alias("MentalHealth"),
-            # pl.col("Sentence")
-            # .str.extract(r"Anger Management Program\:\s+([0-9]|X?)")
-            # .alias("AngerManagementProgram"),
+            pl.col("Sentence")
+            .str.extract(r"Defensive Driving School\:\s+([0-9A-Z]?)\s")
+            .cast(pl.Categorical)
+            .alias("DefensiveDrivingSchool"),
+            pl.col("Sentence")
+            .str.extract(r"Doc Community Corrections\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
+            .alias("DocCommunityCorrections"),
+            pl.col("Sentence")
+            .str.extract(r"Jail Community Corrections\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
+            .alias("JailCommunityCorrections"),
+            pl.col("Sentence")
+            .str.extract(r"Mental Health\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
+            .alias("MentalHealth"),
+            pl.col("Sentence")
+            .str.extract(r"Anger Management Program\:\s+([0-9]|X?)")
+            .cast(pl.Categorical)
+            .alias("AngerManagementProgram"),
             pl.col("Sentence")
             .str.extract(r"Drug Court\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("DrugCourt"),
             pl.col("Sentence")
             .str.extract(r"Doc Drug Program\:\s+([0-9]|X?)")
             .cast(pl.Categorical)
             .alias("DocDrugProgram"),
-            # pl.col("Sentence")
-            # .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project")
-            # .str.strip()
-            # .alias("DrugMeasureUnit"),
+            pl.col("Sentence")
+            .str.extract(r"Drug Measure Unit\: (.+?)Drug Near Project")
+            .str.strip()
+            .cast(pl.Categorical)
+            .alias("DrugMeasureUnit"),
             pl.col("Sentence")
             .str.extract(r"Drug Near Project\: (.+?)Drugs Near School")
             .str.strip()
             .cast(pl.Categorical)
             .alias("DrugNearProject"),
             pl.col("Sentence")
             .str.extract(r"Drugs Near School\: (.+?)Habitual Offender")
@@ -3185,19 +3194,20 @@
             .cast(pl.Categorical)
             .alias("DrugsNearSchool"),
             pl.col("Sentence")
             .str.extract(r"Habitual Offender\: (.+?)Sex Offender")
             .str.strip()
             .cast(pl.Categorical)
             .alias("HabitualOffender"),
-            # pl.col("Sentence")
-            # .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume")
-            # .str.replace_all(r"[X\s0-9]", "")
-            # .str.replace(r'\.','')
-            # .alias("SexOffenderCommunityNotification"),
+            pl.col("Sentence")
+            .str.extract(r"Sex Offender Community Notification\: (.+?)Drug Volume")
+            .str.replace_all(r"[X\s0-9]", "")
+            .str.replace(r'\.','')
+            .cast(pl.Categorical)
+            .alias("SexOffenderCommunityNotification"),
             pl.col("Sentence")
             .str.extract(r"(\d+\.\d\d)\sDrug Volume\:")
             .cast(pl.Float64, strict=False)
             .alias("DrugVolume"),
             pl.col("Sentence")
             .str.extract(r"Drug Code\: (.+?)Habitual Offender Number")
             .str.strip()
```

### Comparing `alacorder-80.2.8/PKG-INFO` & `alacorder-80.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.2.8
+Version: 80.2.9
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

