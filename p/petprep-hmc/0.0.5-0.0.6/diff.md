# Comparing `tmp/petprep_hmc-0.0.5.tar.gz` & `tmp/petprep_hmc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petprep_hmc-0.0.5.tar", last modified: Thu May  4 08:25:16 2023, max compression
+gzip compressed data, was "petprep_hmc-0.0.6.tar", last modified: Fri May  5 11:57:48 2023, max compression
```

## Comparing `petprep_hmc-0.0.5.tar` & `petprep_hmc-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-04 08:25:16.776436 petprep_hmc-0.0.5/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)    11357 2023-04-18 08:13:25.000000 petprep_hmc-0.0.5/LICENSE
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-05-04 08:25:16.776273 petprep_hmc-0.0.5/PKG-INFO
--rw-r--r--   0 martinnorgaard   (501) staff       (20)     4576 2023-05-03 20:44:42.000000 petprep_hmc-0.0.5/README.md
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-04 08:25:16.774854 petprep_hmc-0.0.5/petprep_hmc/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)        0 2023-04-18 08:17:50.000000 petprep_hmc-0.0.5/petprep_hmc/__init__.py
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-04 08:25:16.775598 petprep_hmc-0.0.5/petprep_hmc.egg-info/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-05-04 08:25:16.000000 petprep_hmc-0.0.5/petprep_hmc.egg-info/PKG-INFO
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      242 2023-05-04 08:25:16.000000 petprep_hmc-0.0.5/petprep_hmc.egg-info/SOURCES.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)        1 2023-05-04 08:25:16.000000 petprep_hmc-0.0.5/petprep_hmc.egg-info/dependency_links.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      422 2023-05-04 08:25:16.000000 petprep_hmc-0.0.5/petprep_hmc.egg-info/requires.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)       12 2023-05-04 08:25:16.000000 petprep_hmc-0.0.5/petprep_hmc.egg-info/top_level.txt
--rw-r--r--   0 martinnorgaard   (501) staff       (20)       38 2023-05-04 08:25:16.776514 petprep_hmc-0.0.5/setup.cfg
--rw-r--r--   0 martinnorgaard   (501) staff       (20)     1584 2023-05-04 08:23:15.000000 petprep_hmc-0.0.5/setup.py
-drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-04 08:25:16.775876 petprep_hmc-0.0.5/tests/
--rw-r--r--   0 martinnorgaard   (501) staff       (20)      510 2023-05-03 19:40:26.000000 petprep_hmc-0.0.5/tests/test_cli.py
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-05 11:57:48.554680 petprep_hmc-0.0.6/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)    11357 2023-04-18 08:13:25.000000 petprep_hmc-0.0.6/LICENSE
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-05-05 11:57:48.554431 petprep_hmc-0.0.6/PKG-INFO
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)     4578 2023-05-05 11:54:59.000000 petprep_hmc-0.0.6/README.md
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-05 11:57:48.553225 petprep_hmc-0.0.6/petprep_hmc/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)        0 2023-04-18 08:17:50.000000 petprep_hmc-0.0.6/petprep_hmc/__init__.py
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-05 11:57:48.553923 petprep_hmc-0.0.6/petprep_hmc.egg-info/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      650 2023-05-05 11:57:48.000000 petprep_hmc-0.0.6/petprep_hmc.egg-info/PKG-INFO
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      242 2023-05-05 11:57:48.000000 petprep_hmc-0.0.6/petprep_hmc.egg-info/SOURCES.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)        1 2023-05-05 11:57:48.000000 petprep_hmc-0.0.6/petprep_hmc.egg-info/dependency_links.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      422 2023-05-05 11:57:48.000000 petprep_hmc-0.0.6/petprep_hmc.egg-info/requires.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)       12 2023-05-05 11:57:48.000000 petprep_hmc-0.0.6/petprep_hmc.egg-info/top_level.txt
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)       38 2023-05-05 11:57:48.554837 petprep_hmc-0.0.6/setup.cfg
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)     1584 2023-05-05 11:56:26.000000 petprep_hmc-0.0.6/setup.py
+drwxr-xr-x   0 martinnorgaard   (501) staff       (20)        0 2023-05-05 11:57:48.554072 petprep_hmc-0.0.6/tests/
+-rw-r--r--   0 martinnorgaard   (501) staff       (20)      510 2023-05-03 19:40:26.000000 petprep_hmc-0.0.6/tests/test_cli.py
```

### Comparing `petprep_hmc-0.0.5/LICENSE` & `petprep_hmc-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `petprep_hmc-0.0.5/PKG-INFO` & `petprep_hmc-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petprep_hmc
-Version: 0.0.5
+Version: 0.0.6
 Summary: PETPrep Head Motion Correction Workflow
 Home-page: https://github.com/mnoergaard/petprep_hmc
 Author: Martin Norgaard
 Author-email: martin.noergaard@di.ku.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petprep_hmc-0.0.5/README.md` & `petprep_hmc-0.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 cd petprep_hmc
 pip install -e .
 </pre>
 
 The package is also pip installable and can be installed using the following command
 
 <pre>
-pip install petprep-hmc==0.0.4
+pip install petprep-hmc
 </pre>
 
 ## Usage
 
 To run the PETPrep Head Motion Correction BIDS App, use the following command:
 
 `python3 run.py --bids_dir /path/to/bids_input --output_dir /path/to/bids_output --analysis_level participant [--participant_label PARTICIPANT_LABEL]`
@@ -53,17 +53,17 @@
 - `--no_resample`: (Optional) Whether or not to resample the motion corrected PET data to lowest x/y/z dim in original data (default = False). 
 - `--skip_bids_validator`: (Optional) Whether or not to perform BIDS dataset validation.
 
 For example, to process participant `sub-01`, use the following command:
 
 `python3 run.py --bids_dir /data/bids_input --output_dir /data/bids_output --participant_label 01`
 
-## Output
+## Outputs
 
-The output will be saved in the specified `--output_dir` following the BIDS Derivatives standard. Preprocessed PET data will be stored in the `petprep_hmc` directory in the derivatives directory, along with the estimated motion parameters (confounds) and motion plots.
+Preprocessed PET data along with the estimated motion parameters (confounds) and motion plots will be stored in the directory specified by `--output_dir` or, if no output directory is specified, in `<bids_dir>/derivatives/petprep_hmc` following the BIDS Derivatives standard. 
 
 ## Installation and Running the Code using Docker
 
 ### Prerequisites
 To run petprep_hmc workflow using Docker, you must first have Docker installed on your system. You can download and install Docker from https://www.docker.com/.
 
 ### Pulling the Docker Image
```

### Comparing `petprep_hmc-0.0.5/petprep_hmc.egg-info/PKG-INFO` & `petprep_hmc-0.0.6/petprep_hmc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petprep-hmc
-Version: 0.0.5
+Version: 0.0.6
 Summary: PETPrep Head Motion Correction Workflow
 Home-page: https://github.com/mnoergaard/petprep_hmc
 Author: Martin Norgaard
 Author-email: martin.noergaard@di.ku.dk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `petprep_hmc-0.0.5/setup.py` & `petprep_hmc-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="petprep_hmc",
-    version="0.0.5",
+    version="0.0.6",
     description='PETPrep Head Motion Correction Workflow',
     author='Martin Norgaard',
     author_email='martin.noergaard@di.ku.dk',
     url='https://github.com/mnoergaard/petprep_hmc',
     packages=find_packages(),
     install_requires=[
         "click==8.1.3",
```

