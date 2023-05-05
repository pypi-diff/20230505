# Comparing `tmp/scikit-fibers-0.9.2.tar.gz` & `tmp/scikit-fibers-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-fibers-0.9.2.tar", last modified: Fri Mar  3 00:16:35 2023, max compression
+gzip compressed data, was "scikit-fibers-0.9.3.tar", last modified: Thu May  4 17:18:24 2023, max compression
```

## Comparing `scikit-fibers-0.9.2.tar` & `scikit-fibers-0.9.3.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 harshbandhey   (507) staff       (20)        0 2023-03-03 00:16:35.565502 scikit-fibers-0.9.2/
--rw-r--r--   0 harshbandhey   (507) staff       (20)     1072 2023-03-02 22:03:35.000000 scikit-fibers-0.9.2/LICENSE
--rw-r--r--   0 harshbandhey   (507) staff       (20)     3783 2023-03-03 00:16:35.565585 scikit-fibers-0.9.2/PKG-INFO
--rw-r--r--   0 harshbandhey   (507) staff       (20)     3312 2023-03-02 23:13:54.000000 scikit-fibers-0.9.2/README.md
--rw-r--r--   0 harshbandhey   (507) staff       (20)      655 2023-03-03 00:16:35.565981 scikit-fibers-0.9.2/setup.cfg
--rw-r--r--   0 harshbandhey   (507) staff       (20)      889 2023-03-03 00:16:08.000000 scikit-fibers-0.9.2/setup.py
-drwxr-xr-x   0 harshbandhey   (507) staff       (20)        0 2023-03-03 00:16:35.561272 scikit-fibers-0.9.2/src/
-drwxr-xr-x   0 harshbandhey   (507) staff       (20)        0 2023-03-03 00:16:35.563441 scikit-fibers-0.9.2/src/scikit_fibers.egg-info/
--rw-r--r--   0 harshbandhey   (507) staff       (20)     3783 2023-03-03 00:16:35.000000 scikit-fibers-0.9.2/src/scikit_fibers.egg-info/PKG-INFO
--rw-r--r--   0 harshbandhey   (507) staff       (20)      377 2023-03-03 00:16:35.000000 scikit-fibers-0.9.2/src/scikit_fibers.egg-info/SOURCES.txt
--rw-r--r--   0 harshbandhey   (507) staff       (20)        1 2023-03-03 00:16:35.000000 scikit-fibers-0.9.2/src/scikit_fibers.egg-info/dependency_links.txt
--rw-r--r--   0 harshbandhey   (507) staff       (20)       56 2023-03-03 00:16:35.000000 scikit-fibers-0.9.2/src/scikit_fibers.egg-info/requires.txt
--rw-r--r--   0 harshbandhey   (507) staff       (20)        9 2023-03-03 00:16:35.000000 scikit-fibers-0.9.2/src/scikit_fibers.egg-info/top_level.txt
-drwxr-xr-x   0 harshbandhey   (507) staff       (20)        0 2023-03-03 00:16:35.564211 scikit-fibers-0.9.2/src/skfibers/
--rw-r--r--   0 harshbandhey   (507) staff       (20)      181 2023-03-03 00:16:08.000000 scikit-fibers-0.9.2/src/skfibers/__init__.py
--rw-r--r--   0 harshbandhey   (507) staff       (20)    12882 2023-03-02 23:24:15.000000 scikit-fibers-0.9.2/src/skfibers/fibers.py
--rw-r--r--   0 harshbandhey   (507) staff       (20)    40431 2023-03-02 20:07:39.000000 scikit-fibers-0.9.2/src/skfibers/methods.py
-drwxr-xr-x   0 harshbandhey   (507) staff       (20)        0 2023-03-03 00:16:35.565118 scikit-fibers-0.9.2/tests/
--rw-rw-r--   0 harshbandhey   (507) staff       (20)     6165 2023-03-02 20:43:00.000000 scikit-fibers-0.9.2/tests/test_common_separation.py
--rw-rw-r--   0 harshbandhey   (507) staff       (20)    17182 2023-03-02 20:43:56.000000 scikit-fibers-0.9.2/tests/test_crossover_mutation.py
+drwxr-xr-x   0 harshbandhey   (507) staff       (20)        0 2023-05-04 17:18:24.365486 scikit-fibers-0.9.3/
+-rw-r--r--   0 harshbandhey   (507) staff       (20)     1072 2023-03-02 22:03:35.000000 scikit-fibers-0.9.3/LICENSE
+-rw-r--r--   0 harshbandhey   (507) staff       (20)     3866 2023-05-04 17:18:24.365589 scikit-fibers-0.9.3/PKG-INFO
+-rw-r--r--   0 harshbandhey   (507) staff       (20)     3395 2023-04-19 19:17:36.000000 scikit-fibers-0.9.3/README.md
+-rw-r--r--   0 harshbandhey   (507) staff       (20)      683 2023-05-04 17:18:24.366002 scikit-fibers-0.9.3/setup.cfg
+-rw-r--r--   0 harshbandhey   (507) staff       (20)      948 2023-04-19 19:16:15.000000 scikit-fibers-0.9.3/setup.py
+drwxr-xr-x   0 harshbandhey   (507) staff       (20)        0 2023-05-04 17:18:24.357236 scikit-fibers-0.9.3/src/
+drwxr-xr-x   0 harshbandhey   (507) staff       (20)        0 2023-05-04 17:18:24.360492 scikit-fibers-0.9.3/src/scikit_fibers.egg-info/
+-rw-r--r--   0 harshbandhey   (507) staff       (20)     3866 2023-05-04 17:18:24.000000 scikit-fibers-0.9.3/src/scikit_fibers.egg-info/PKG-INFO
+-rw-r--r--   0 harshbandhey   (507) staff       (20)      585 2023-05-04 17:18:24.000000 scikit-fibers-0.9.3/src/scikit_fibers.egg-info/SOURCES.txt
+-rw-r--r--   0 harshbandhey   (507) staff       (20)        1 2023-05-04 17:18:24.000000 scikit-fibers-0.9.3/src/scikit_fibers.egg-info/dependency_links.txt
+-rw-r--r--   0 harshbandhey   (507) staff       (20)       76 2023-05-04 17:18:24.000000 scikit-fibers-0.9.3/src/scikit_fibers.egg-info/requires.txt
+-rw-r--r--   0 harshbandhey   (507) staff       (20)        9 2023-05-04 17:18:24.000000 scikit-fibers-0.9.3/src/scikit_fibers.egg-info/top_level.txt
+drwxr-xr-x   0 harshbandhey   (507) staff       (20)        0 2023-05-04 17:18:24.361334 scikit-fibers-0.9.3/src/skfibers/
+-rw-r--r--   0 harshbandhey   (507) staff       (20)      209 2023-04-12 21:20:00.000000 scikit-fibers-0.9.3/src/skfibers/__init__.py
+drwxr-xr-x   0 harshbandhey   (507) staff       (20)        0 2023-05-04 17:18:24.363190 scikit-fibers-0.9.3/src/skfibers/experiments/
+-rw-r--r--   0 harshbandhey   (507) staff       (20)      135 2023-04-17 21:30:41.000000 scikit-fibers-0.9.3/src/skfibers/experiments/__init__.py
+-rw-r--r--   0 harshbandhey   (507) staff       (20)     6794 2023-05-03 23:03:48.000000 scikit-fibers-0.9.3/src/skfibers/experiments/datagen.py
+-rw-r--r--   0 harshbandhey   (507) staff       (20)        7 2023-04-17 21:10:46.000000 scikit-fibers-0.9.3/src/skfibers/experiments/test_experiments.py
+-rw-r--r--   0 harshbandhey   (507) staff       (20)    19754 2023-05-04 10:30:35.000000 scikit-fibers-0.9.3/src/skfibers/fibers.py
+drwxr-xr-x   0 harshbandhey   (507) staff       (20)        0 2023-05-04 17:18:24.363702 scikit-fibers-0.9.3/src/skfibers/methods/
+-rw-r--r--   0 harshbandhey   (507) staff       (20)        0 2023-04-12 21:20:00.000000 scikit-fibers-0.9.3/src/skfibers/methods/__init__.py
+-rw-rw-r--   0 harshbandhey   (507) staff       (20)    52223 2023-05-04 07:34:39.000000 scikit-fibers-0.9.3/src/skfibers/methods/algorithms.py
+drwxr-xr-x   0 harshbandhey   (507) staff       (20)        0 2023-05-04 17:18:24.365191 scikit-fibers-0.9.3/src/skfibers/tests/
+-rw-r--r--   0 harshbandhey   (507) staff       (20)        0 2023-04-12 21:20:00.000000 scikit-fibers-0.9.3/src/skfibers/tests/__init__.py
+-rw-r--r--   0 harshbandhey   (507) staff       (20)    13941 2023-05-04 17:15:32.000000 scikit-fibers-0.9.3/src/skfibers/tests/test_experiments.py
+-rw-r--r--   0 harshbandhey   (507) staff       (20)     7985 2023-04-17 21:12:52.000000 scikit-fibers-0.9.3/src/skfibers/tests/test_skfibers_stub.py
```

### Comparing `scikit-fibers-0.9.2/LICENSE` & `scikit-fibers-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-fibers-0.9.2/PKG-INFO` & `scikit-fibers-0.9.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-fibers
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Scikit Learn compatible implementation of FIBERS Algorithm
 Home-page: https://github.com/UrbsLab/scikit-FIBERS
 Author: Harsh Bandhey
 Author-email: harsh.bandhey@cshs.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,12 +43,13 @@
 8) set_number_of_bins: the population size of candidate bins
 9) min_features_per_group: the minimum number of features in a bin
 10) max_number_of_groups_with_feature: the maximum number of bins containing a feature
 11) informative_cutoff: the minimum proportion allowed for a risk group, all bins that result in a smaller risk group representing a proportion below this cutoff will automatically be assigned a fitness score of 0 (e.g., 0.2 means that both the low risk group and high risk group must represent over 20% of the total population)
 12) crossover_probability: the probability of each feature in an offspring bin to crossover to the paired offspring bin (recommendation: 0.5 to 0.8)
 13) mutation_probability: the probability of each feature in a bin to be deleted (a proportionate probability is automatically applied on each feature outside the bin to be added (recommendation: 0.05 to 0.5 depending on situation and number of iterations run)
 14) elitism_parameter: the proportion of elite bins in the current generation to be preserved for the next evolutionary cycle (recommendation: 0.2 to 0.8 depending on conservativeness of approach and number of iterations run)
+15) random_seed: random seed parameter to introduce reproducibility of experiments
 
 ## Contact
 
 Please email sdasariraju23@lawrenceville.org and Ryan.Urbanowicz@cshs.org for any 
 inquiries related to FIBERS.
```

### Comparing `scikit-fibers-0.9.2/README.md` & `scikit-fibers-0.9.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,12 +29,13 @@
 8) set_number_of_bins: the population size of candidate bins
 9) min_features_per_group: the minimum number of features in a bin
 10) max_number_of_groups_with_feature: the maximum number of bins containing a feature
 11) informative_cutoff: the minimum proportion allowed for a risk group, all bins that result in a smaller risk group representing a proportion below this cutoff will automatically be assigned a fitness score of 0 (e.g., 0.2 means that both the low risk group and high risk group must represent over 20% of the total population)
 12) crossover_probability: the probability of each feature in an offspring bin to crossover to the paired offspring bin (recommendation: 0.5 to 0.8)
 13) mutation_probability: the probability of each feature in a bin to be deleted (a proportionate probability is automatically applied on each feature outside the bin to be added (recommendation: 0.05 to 0.5 depending on situation and number of iterations run)
 14) elitism_parameter: the proportion of elite bins in the current generation to be preserved for the next evolutionary cycle (recommendation: 0.2 to 0.8 depending on conservativeness of approach and number of iterations run)
+15) random_seed: random seed parameter to introduce reproducibility of experiments
 
 ## Contact
 
 Please email sdasariraju23@lawrenceville.org and Ryan.Urbanowicz@cshs.org for any 
 inquiries related to FIBERS.
```

### Comparing `scikit-fibers-0.9.2/setup.cfg` & `scikit-fibers-0.9.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scikit-fibers
-version = 0.9.2
+version = 0.9.3
 author = Harsh Bandhey
 author_email = harsh.bandhey@cshs.org
 description = A Scikit Learn compatible implementation of FIBERS Algorithm
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/UrbsLab/scikit-FIBERS
 classifiers = 
@@ -15,18 +15,21 @@
 [options]
 package_dir = 
 	= src
 python_requires = >=3.6
 install_requires = 
 	numpy
 	pandas
-	sklearn
+	scikit-learn
 	lifelines
 	skrebate==0.7
 	matplotlib
+	seaborn
+	pytest
+	tqdm
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `scikit-fibers-0.9.2/setup.py` & `scikit-fibers-0.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scikit-fibers",
-    version="0.9.2",
+    version="0.9.3",
     author="Harsh Bandhey",
     author_email="harsh.bandhey@cshs.org",
     description="A Scikit Learn compatible implementation of FIBERS Algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/UrbsLab/scikit-FIBERS",
     classifiers=[
@@ -19,12 +19,16 @@
     ],
     install_requires=[
         "numpy",
         "pandas",
         "sklearn",
         "lifelines",
         "skrebate==0.7",
-        "matplotlib"],
+        "matplotlib",
+        "seaborn",
+        "pytest",
+        "tqdm",
+    ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6"
 )
```

### Comparing `scikit-fibers-0.9.2/src/scikit_fibers.egg-info/PKG-INFO` & `scikit-fibers-0.9.3/src/scikit_fibers.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-fibers
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Scikit Learn compatible implementation of FIBERS Algorithm
 Home-page: https://github.com/UrbsLab/scikit-FIBERS
 Author: Harsh Bandhey
 Author-email: harsh.bandhey@cshs.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -43,12 +43,13 @@
 8) set_number_of_bins: the population size of candidate bins
 9) min_features_per_group: the minimum number of features in a bin
 10) max_number_of_groups_with_feature: the maximum number of bins containing a feature
 11) informative_cutoff: the minimum proportion allowed for a risk group, all bins that result in a smaller risk group representing a proportion below this cutoff will automatically be assigned a fitness score of 0 (e.g., 0.2 means that both the low risk group and high risk group must represent over 20% of the total population)
 12) crossover_probability: the probability of each feature in an offspring bin to crossover to the paired offspring bin (recommendation: 0.5 to 0.8)
 13) mutation_probability: the probability of each feature in a bin to be deleted (a proportionate probability is automatically applied on each feature outside the bin to be added (recommendation: 0.05 to 0.5 depending on situation and number of iterations run)
 14) elitism_parameter: the proportion of elite bins in the current generation to be preserved for the next evolutionary cycle (recommendation: 0.2 to 0.8 depending on conservativeness of approach and number of iterations run)
+15) random_seed: random seed parameter to introduce reproducibility of experiments
 
 ## Contact
 
 Please email sdasariraju23@lawrenceville.org and Ryan.Urbanowicz@cshs.org for any 
 inquiries related to FIBERS.
```

