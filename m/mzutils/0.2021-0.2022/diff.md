# Comparing `tmp/mzutils-0.2021-py3-none-any.whl.zip` & `tmp/mzutils-0.2022-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 33237 bytes, number of entries: 25
--rw-r--r--  2.0 unx      453 b- defN 23-Feb-28 22:59 mzutils/__init__.py
+Zip file size: 33912 bytes, number of entries: 26
+-rw-r--r--  2.0 unx      478 b- defN 23-May-04 22:05 mzutils/__init__.py
+-rw-r--r--  2.0 unx     1604 b- defN 23-May-04 22:09 mzutils/aws_funcs.py
 -rw-r--r--  2.0 unx     4001 b- defN 23-Jan-25 15:39 mzutils/computing_funcs.py
 -rw-r--r--  2.0 unx     2668 b- defN 23-Jan-25 15:39 mzutils/control_models.py
 -rw-r--r--  2.0 unx     6258 b- defN 23-Jan-25 15:39 mzutils/ctsv_funcs.py
 -rw-r--r--  2.0 unx     4471 b- defN 23-Jan-25 15:39 mzutils/data_structures.py
 -rw-r--r--  2.0 unx     1220 b- defN 23-Feb-28 22:57 mzutils/dataframe_funcs.py
 -rw-r--r--  2.0 unx     3534 b- defN 23-Jan-25 15:39 mzutils/gym_space_management.py
 -rw-r--r--  2.0 unx      419 b- defN 23-Jan-25 15:39 mzutils/json_funcs.py
@@ -14,14 +15,14 @@
 -rw-r--r--  2.0 unx      792 b- defN 23-Jan-25 15:39 mzutils/serialize_funcs.py
 -rw-r--r--  2.0 unx    10986 b- defN 23-Jan-25 15:39 mzutils/string_funcs.py
 -rw-r--r--  2.0 unx     4320 b- defN 23-Jan-25 15:39 mzutils/tf_funcs.py
 -rw-r--r--  2.0 unx    13467 b- defN 23-Jan-25 15:39 mzutils/torch_funcs.py
 -rw-r--r--  2.0 unx       86 b- defN 23-Jan-25 15:39 mzutils/nlp_tasks/__init__.py
 -rw-r--r--  2.0 unx     7505 b- defN 23-Jan-25 15:39 mzutils/nlp_tasks/data_preprocessing.py
 -rw-r--r--  2.0 unx     3761 b- defN 23-Jan-25 15:39 mzutils/nlp_tasks/ner_funcs.py
--rw-r--r--  2.0 unx    27566 b- defN 23-Mar-20 20:24 mzutils/nlp_tasks/nlp_metrics.py
--rw-r--r--  2.0 unx     1073 b- defN 23-Mar-20 20:24 mzutils-0.2021.dist-info/LICENSE
--rw-r--r--  2.0 unx     2562 b- defN 23-Mar-20 20:24 mzutils-0.2021.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-20 20:24 mzutils-0.2021.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Mar-20 20:24 mzutils-0.2021.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2030 b- defN 23-Mar-20 20:24 mzutils-0.2021.dist-info/RECORD
-25 files, 114682 bytes uncompressed, 29983 bytes compressed:  73.9%
+-rw-r--r--  2.0 unx    27566 b- defN 23-Mar-20 20:35 mzutils/nlp_tasks/nlp_metrics.py
+-rw-r--r--  2.0 unx     1073 b- defN 23-May-04 22:09 mzutils-0.2022.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2720 b- defN 23-May-04 22:09 mzutils-0.2022.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 22:09 mzutils-0.2022.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-04 22:09 mzutils-0.2022.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2107 b- defN 23-May-04 22:09 mzutils-0.2022.dist-info/RECORD
+26 files, 116546 bytes uncompressed, 30542 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: mzutils/__init__.py
 Comment: 
 
+Filename: mzutils/aws_funcs.py
+Comment: 
+
 Filename: mzutils/computing_funcs.py
 Comment: 
 
 Filename: mzutils/control_models.py
 Comment: 
 
 Filename: mzutils/ctsv_funcs.py
@@ -54,23 +57,23 @@
 
 Filename: mzutils/nlp_tasks/ner_funcs.py
 Comment: 
 
 Filename: mzutils/nlp_tasks/nlp_metrics.py
 Comment: 
 
-Filename: mzutils-0.2021.dist-info/LICENSE
+Filename: mzutils-0.2022.dist-info/LICENSE
 Comment: 
 
-Filename: mzutils-0.2021.dist-info/METADATA
+Filename: mzutils-0.2022.dist-info/METADATA
 Comment: 
 
-Filename: mzutils-0.2021.dist-info/WHEEL
+Filename: mzutils-0.2022.dist-info/WHEEL
 Comment: 
 
-Filename: mzutils-0.2021.dist-info/top_level.txt
+Filename: mzutils-0.2022.dist-info/top_level.txt
 Comment: 
 
-Filename: mzutils-0.2021.dist-info/RECORD
+Filename: mzutils-0.2022.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mzutils/__init__.py

```diff
@@ -10,7 +10,8 @@
 from .parser import *
 from .probabilities_funcs import *
 from .serialize_funcs import *
 from .string_funcs import *
 from .tf_funcs import *
 from .torch_funcs import *
 from .dataframe_funcs import *
+from .aws_funcs import *
```

## Comparing `mzutils-0.2021.dist-info/LICENSE` & `mzutils-0.2022.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mzutils-0.2021.dist-info/METADATA` & `mzutils-0.2022.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mzutils
-Version: 0.2021
+Version: 0.2022
 Summary: Mohan Zhang's toolkit
 Home-page: https://github.com/Mohan-Zhang-u/mzutils
 Author: Mohan Zhang
 Author-email: mohan.zhang.mz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,21 +21,25 @@
 Requires-Dist: nltk
 Requires-Dist: pandas
 Provides-Extra: all
 Requires-Dist: PyYAML ; extra == 'all'
 Requires-Dist: tensorflow ; extra == 'all'
 Requires-Dist: hanlp ; extra == 'all'
 Requires-Dist: pyarrow ; extra == 'all'
+Requires-Dist: s3fs ; extra == 'all'
+Requires-Dist: hashfile ; extra == 'all'
 Provides-Extra: nlp
 Requires-Dist: hanlp ; extra == 'nlp'
 Requires-Dist: pyarrow ; extra == 'nlp'
 Provides-Extra: tf
 Requires-Dist: tensorflow ; extra == 'tf'
 Provides-Extra: yaml
 Requires-Dist: PyYAML ; extra == 'yaml'
+Requires-Dist: s3fs ; extra == 'yaml'
+Requires-Dist: hashfile ; extra == 'yaml'
 
 .. _mzutils: https://pypi.org/project/mzutils/
 
 `mzutils`_ is a personal toolkit that contains various methods to do miscellaneous jobs related to data cleaning, preprocessing, visualizing, evaluating and modeling in various fields of machine learning, especially NLP and RL. It supports Datasets like SQuAD, GLUE, Deepmind CNN/DailyMail in NLP and d4rl in offlineRL, as well as their conversions to JSON, CSV, numpy arrays and tensors.
 
 The purpose of this toolkit is to reuse the code and make Mohan Zhang's life easier.
```

## Comparing `mzutils-0.2021.dist-info/RECORD` & `mzutils-0.2022.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-mzutils/__init__.py,sha256=RAqTWdmjiukRD0FaOwh20dB5rXks8z-Ct4dSOFIP_3A,453
+mzutils/__init__.py,sha256=Kn2AvqyvK_OCwgMU-1rAFEcBFhCLZ-XYbnWbikO5FXs,478
+mzutils/aws_funcs.py,sha256=N1VbGkJVG20CE9JzJgtpLNtsvuHxUqAc4elh4zwM2VM,1604
 mzutils/computing_funcs.py,sha256=1m-NkMd03G8o4wZPFpz7dqvi4QEZ5PjHFGpXsgPpukc,4001
 mzutils/control_models.py,sha256=88RwNkl0BkUTJ2_zgh_6XJL-jHxq2a2aI1LNYN-NRZI,2668
 mzutils/ctsv_funcs.py,sha256=4tbUyR8oxxNOHswryb3boheQnbjqCc515HE4DHU9QQY,6258
 mzutils/data_structures.py,sha256=0iGzryZTiuKAWWNZKApwMbhCBJqdhP-dY4pjk7Wnv9U,4471
 mzutils/dataframe_funcs.py,sha256=P8q2DsIM92IVHNNeDEQs9Gu_Ev23wybMSMZANFaAvBY,1220
 mzutils/gym_space_management.py,sha256=BJnuvv_f9WAVjMKyMqNx9LRT64x9YYtOvY_tuMqnE8k,3534
 mzutils/json_funcs.py,sha256=y7s264Jt8Jcb4udOpPSAtNwuQ7XJvXWoRNwbJ83J_P0,419
@@ -14,12 +15,12 @@
 mzutils/string_funcs.py,sha256=NS3iDGam6RIAV3Y3X75DLR6RWxrV6O1RZ7khKLe14U8,10986
 mzutils/tf_funcs.py,sha256=DFlvznPzrAz0LKH1bwKw8qeZ0u6SX7hZz_jTWI0TihQ,4320
 mzutils/torch_funcs.py,sha256=vDhd9sOFIie1f4t2OKvPFtmq5e27a4s3ZtP1AK9dZgY,13467
 mzutils/nlp_tasks/__init__.py,sha256=DJ8pBQWIibqFW9lT6S3l5cdc8fGbz7Dw_bCEs41pKr8,86
 mzutils/nlp_tasks/data_preprocessing.py,sha256=dN_SGYj2Y0pv1rb4FHsgS2x7iDyebomcTQVN1uWuwec,7505
 mzutils/nlp_tasks/ner_funcs.py,sha256=yyPtg3a-udmgzWA7NsHHiR0RTLs7zoKFj_7nGT9BZaE,3761
 mzutils/nlp_tasks/nlp_metrics.py,sha256=25gTnpPg2nGGdWbwVsXhVbCEuDQtDH6G94RdmgkIfCQ,27566
-mzutils-0.2021.dist-info/LICENSE,sha256=2bm9uFabQZ3Ykb_SaSU_uUbAj2-htc6WJQmS_65qD00,1073
-mzutils-0.2021.dist-info/METADATA,sha256=bMhe6frtBxUh3wihR_AMnSAN9DSmF0JB2YOqJcC6od0,2562
-mzutils-0.2021.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mzutils-0.2021.dist-info/top_level.txt,sha256=23PQspP6KkBGEjUUYCDsSInomyiX4IiwEV1Yt0wJ-RA,8
-mzutils-0.2021.dist-info/RECORD,,
+mzutils-0.2022.dist-info/LICENSE,sha256=2bm9uFabQZ3Ykb_SaSU_uUbAj2-htc6WJQmS_65qD00,1073
+mzutils-0.2022.dist-info/METADATA,sha256=vwdF7dcZUTvrTG5Xr7H7oOClqz6VeDUBSR7vWDMA9ms,2720
+mzutils-0.2022.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mzutils-0.2022.dist-info/top_level.txt,sha256=23PQspP6KkBGEjUUYCDsSInomyiX4IiwEV1Yt0wJ-RA,8
+mzutils-0.2022.dist-info/RECORD,,
```

