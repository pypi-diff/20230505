# Comparing `tmp/delia-1.0.8.tar.gz` & `tmp/delia-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delia-1.0.8.tar", last modified: Thu Jan 12 16:28:01 2023, max compression
+gzip compressed data, was "delia-1.0.9.tar", last modified: Thu Jan 12 16:33:00 2023, max compression
```

## Comparing `delia-1.0.8.tar` & `delia-1.0.9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.224672 delia-1.0.8/
--rw-rw-rw-   0        0        0    11549 2023-01-12 16:21:25.000000 delia-1.0.8/LICENSE
--rw-rw-rw-   0        0        0    14520 2023-01-12 16:28:01.224672 delia-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    13888 2023-01-12 16:21:25.000000 delia-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.161622 delia-1.0.8/delia/
--rw-rw-rw-   0        0        0      678 2023-01-12 16:27:02.000000 delia-1.0.8/delia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.161622 delia-1.0.8/delia/databases/
--rw-rw-rw-   0        0        0       49 2023-01-12 16:21:25.000000 delia-1.0.8/delia/databases/__init__.py
--rw-rw-rw-   0        0        0    13207 2023-01-12 16:21:25.000000 delia-1.0.8/delia/databases/patients_database.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.161622 delia-1.0.8/delia/extractors/
--rw-rw-rw-   0        0        0      144 2023-01-12 16:21:25.000000 delia-1.0.8/delia/extractors/__init__.py
--rw-rw-rw-   0        0        0    14741 2023-01-12 16:21:25.000000 delia-1.0.8/delia/extractors/patients_data_extractor.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.161622 delia-1.0.8/delia/radiomics/
--rw-rw-rw-   0        0        0      115 2023-01-12 16:21:25.000000 delia-1.0.8/delia/radiomics/__init__.py
--rw-rw-rw-   0        0        0    11712 2023-01-12 16:21:25.000000 delia-1.0.8/delia/radiomics/radiomics_dataset.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.161622 delia-1.0.8/delia/readers/
--rw-rw-rw-   0        0        0       65 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.177248 delia-1.0.8/delia/readers/image/
--rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/image/__init__.py
--rw-rw-rw-   0        0        0    10842 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/image/dicom_reader.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.177248 delia-1.0.8/delia/readers/patient_data/
--rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/patient_data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.177248 delia-1.0.8/delia/readers/patient_data/factories/
--rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/patient_data/factories/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/patient_data/factories/base_patient_data_factory.py
--rw-rw-rw-   0        0        0     7615 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/patient_data/factories/patient_data_factories.py
--rw-rw-rw-   0        0        0     3783 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/patient_data/patient_data_query_context.py
--rw-rw-rw-   0        0        0      963 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/patient_data/patient_data_query_strategy.py
--rw-rw-rw-   0        0        0    10082 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/patient_data/patient_data_reader.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.193012 delia-1.0.8/delia/readers/segmentation/
--rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/segmentation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.193012 delia-1.0.8/delia/readers/segmentation/factories/
--rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/segmentation/factories/__init__.py
--rw-rw-rw-   0        0        0     2042 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/segmentation/factories/base_segmentation_factory.py
--rw-rw-rw-   0        0        0     6278 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/segmentation/factories/dicom_segmentation_factories.py
--rw-rw-rw-   0        0        0     1260 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/segmentation/factories/segment.py
--rw-rw-rw-   0        0        0     2830 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/segmentation/factories/segmentation.py
--rw-rw-rw-   0        0        0     4848 2023-01-12 16:26:28.000000 delia-1.0.8/delia/readers/segmentation/segmentation_context.py
--rw-rw-rw-   0        0        0     2801 2023-01-12 16:26:28.000000 delia-1.0.8/delia/readers/segmentation/segmentation_reader.py
--rw-rw-rw-   0        0        0     2217 2023-01-12 16:21:25.000000 delia-1.0.8/delia/readers/segmentation/segmentation_strategy.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.201015 delia-1.0.8/delia/transforms/
--rw-rw-rw-   0        0        0      496 2023-01-12 16:21:25.000000 delia-1.0.8/delia/transforms/__init__.py
--rw-rw-rw-   0        0        0    11984 2023-01-12 16:21:25.000000 delia-1.0.8/delia/transforms/applications.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.201015 delia-1.0.8/delia/transforms/array_space/
--rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.8/delia/transforms/array_space/__init__.py
--rw-rw-rw-   0        0        0     3078 2023-01-12 16:21:25.000000 delia-1.0.8/delia/transforms/array_space/matching_crop_foreground.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.201015 delia-1.0.8/delia/transforms/data/
--rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.8/delia/transforms/data/__init__.py
--rw-rw-rw-   0        0        0     4471 2023-01-12 16:21:25.000000 delia-1.0.8/delia/transforms/data/copy_segmentations.py
--rw-rw-rw-   0        0        0     1882 2023-01-12 16:21:25.000000 delia-1.0.8/delia/transforms/data/transform.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.209044 delia-1.0.8/delia/transforms/physical_space/
--rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.8/delia/transforms/physical_space/__init__.py
--rw-rw-rw-   0        0        0     9656 2023-01-12 16:21:25.000000 delia-1.0.8/delia/transforms/physical_space/pet_to_suv.py
--rw-rw-rw-   0        0        0     3470 2023-01-12 16:21:25.000000 delia-1.0.8/delia/transforms/physical_space/resample.py
--rw-rw-rw-   0        0        0     3086 2023-01-12 16:21:25.000000 delia-1.0.8/delia/transforms/physical_space/transform.py
--rw-rw-rw-   0        0        0     2326 2023-01-12 16:21:25.000000 delia-1.0.8/delia/transforms/tools.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.209044 delia-1.0.8/delia/utils/
--rw-rw-rw-   0        0        0       42 2023-01-12 16:21:25.000000 delia-1.0.8/delia/utils/__init__.py
--rw-rw-rw-   0        0        0     4101 2023-01-12 16:26:28.000000 delia-1.0.8/delia/utils/data_model.py
--rw-rw-rw-   0        0        0     1329 2023-01-12 16:21:25.000000 delia-1.0.8/delia/utils/tools.py
--rw-rw-rw-   0        0        0     2131 2023-01-12 16:21:25.000000 delia-1.0.8/delia/utils/transforms_history.py
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.161622 delia-1.0.8/delia.egg-info/
--rw-rw-rw-   0        0        0    14520 2023-01-12 16:28:01.000000 delia-1.0.8/delia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2041 2023-01-12 16:28:01.000000 delia-1.0.8/delia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-12 16:28:01.000000 delia-1.0.8/delia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-01-12 16:28:01.000000 delia-1.0.8/delia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-01-12 16:28:01.000000 delia-1.0.8/delia.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-12 16:28:01.224672 delia-1.0.8/examples/
--rw-rw-rw-   0        0        0       38 2023-01-12 16:21:25.000000 delia-1.0.8/examples/__init__.py
--rw-rw-rw-   0        0        0      712 2023-01-12 16:21:25.000000 delia-1.0.8/examples/env_examples.py
--rw-rw-rw-   0        0        0     3097 2023-01-12 16:21:25.000000 delia-1.0.8/examples/ex01.py
--rw-rw-rw-   0        0        0     3106 2023-01-12 16:21:25.000000 delia-1.0.8/examples/ex02.py
--rw-rw-rw-   0        0        0     2750 2023-01-12 16:21:25.000000 delia-1.0.8/examples/ex03.py
--rw-rw-rw-   0        0        0     5641 2023-01-12 16:21:25.000000 delia-1.0.8/examples/ex04.py
--rw-rw-rw-   0        0        0       42 2023-01-12 16:28:01.224672 delia-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1041 2023-01-12 16:27:02.000000 delia-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.272609 delia-1.0.9/
+-rw-rw-rw-   0        0        0    11549 2023-01-12 16:21:25.000000 delia-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0    14520 2023-01-12 16:33:00.272609 delia-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    13888 2023-01-12 16:21:25.000000 delia-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.217234 delia-1.0.9/delia/
+-rw-rw-rw-   0        0        0      678 2023-01-12 16:32:22.000000 delia-1.0.9/delia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.222235 delia-1.0.9/delia/databases/
+-rw-rw-rw-   0        0        0       49 2023-01-12 16:21:25.000000 delia-1.0.9/delia/databases/__init__.py
+-rw-rw-rw-   0        0        0    13207 2023-01-12 16:21:25.000000 delia-1.0.9/delia/databases/patients_database.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.223235 delia-1.0.9/delia/extractors/
+-rw-rw-rw-   0        0        0      144 2023-01-12 16:21:25.000000 delia-1.0.9/delia/extractors/__init__.py
+-rw-rw-rw-   0        0        0    14741 2023-01-12 16:21:25.000000 delia-1.0.9/delia/extractors/patients_data_extractor.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.225236 delia-1.0.9/delia/radiomics/
+-rw-rw-rw-   0        0        0      115 2023-01-12 16:21:25.000000 delia-1.0.9/delia/radiomics/__init__.py
+-rw-rw-rw-   0        0        0    11712 2023-01-12 16:21:25.000000 delia-1.0.9/delia/radiomics/radiomics_dataset.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.225236 delia-1.0.9/delia/readers/
+-rw-rw-rw-   0        0        0       65 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.236238 delia-1.0.9/delia/readers/image/
+-rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/image/__init__.py
+-rw-rw-rw-   0        0        0    10842 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/image/dicom_reader.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.236238 delia-1.0.9/delia/readers/patient_data/
+-rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/patient_data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.236238 delia-1.0.9/delia/readers/patient_data/factories/
+-rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/patient_data/factories/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/patient_data/factories/base_patient_data_factory.py
+-rw-rw-rw-   0        0        0     7615 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/patient_data/factories/patient_data_factories.py
+-rw-rw-rw-   0        0        0     3783 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/patient_data/patient_data_query_context.py
+-rw-rw-rw-   0        0        0      963 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/patient_data/patient_data_query_strategy.py
+-rw-rw-rw-   0        0        0    10082 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/patient_data/patient_data_reader.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.236238 delia-1.0.9/delia/readers/segmentation/
+-rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/segmentation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.251889 delia-1.0.9/delia/readers/segmentation/factories/
+-rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/segmentation/factories/__init__.py
+-rw-rw-rw-   0        0        0     2042 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/segmentation/factories/base_segmentation_factory.py
+-rw-rw-rw-   0        0        0     6278 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/segmentation/factories/dicom_segmentation_factories.py
+-rw-rw-rw-   0        0        0     1260 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/segmentation/factories/segment.py
+-rw-rw-rw-   0        0        0     2830 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/segmentation/factories/segmentation.py
+-rw-rw-rw-   0        0        0     4841 2023-01-12 16:31:41.000000 delia-1.0.9/delia/readers/segmentation/segmentation_context.py
+-rw-rw-rw-   0        0        0     2801 2023-01-12 16:26:28.000000 delia-1.0.9/delia/readers/segmentation/segmentation_reader.py
+-rw-rw-rw-   0        0        0     2217 2023-01-12 16:21:25.000000 delia-1.0.9/delia/readers/segmentation/segmentation_strategy.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.251889 delia-1.0.9/delia/transforms/
+-rw-rw-rw-   0        0        0      496 2023-01-12 16:21:25.000000 delia-1.0.9/delia/transforms/__init__.py
+-rw-rw-rw-   0        0        0    11984 2023-01-12 16:21:25.000000 delia-1.0.9/delia/transforms/applications.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.251889 delia-1.0.9/delia/transforms/array_space/
+-rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.9/delia/transforms/array_space/__init__.py
+-rw-rw-rw-   0        0        0     3078 2023-01-12 16:21:25.000000 delia-1.0.9/delia/transforms/array_space/matching_crop_foreground.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.251889 delia-1.0.9/delia/transforms/data/
+-rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.9/delia/transforms/data/__init__.py
+-rw-rw-rw-   0        0        0     4471 2023-01-12 16:21:25.000000 delia-1.0.9/delia/transforms/data/copy_segmentations.py
+-rw-rw-rw-   0        0        0     1882 2023-01-12 16:21:25.000000 delia-1.0.9/delia/transforms/data/transform.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.251889 delia-1.0.9/delia/transforms/physical_space/
+-rw-rw-rw-   0        0        0        0 2023-01-12 16:21:25.000000 delia-1.0.9/delia/transforms/physical_space/__init__.py
+-rw-rw-rw-   0        0        0     9656 2023-01-12 16:21:25.000000 delia-1.0.9/delia/transforms/physical_space/pet_to_suv.py
+-rw-rw-rw-   0        0        0     3470 2023-01-12 16:21:25.000000 delia-1.0.9/delia/transforms/physical_space/resample.py
+-rw-rw-rw-   0        0        0     3086 2023-01-12 16:21:25.000000 delia-1.0.9/delia/transforms/physical_space/transform.py
+-rw-rw-rw-   0        0        0     2326 2023-01-12 16:21:25.000000 delia-1.0.9/delia/transforms/tools.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.251889 delia-1.0.9/delia/utils/
+-rw-rw-rw-   0        0        0       42 2023-01-12 16:21:25.000000 delia-1.0.9/delia/utils/__init__.py
+-rw-rw-rw-   0        0        0     4101 2023-01-12 16:26:28.000000 delia-1.0.9/delia/utils/data_model.py
+-rw-rw-rw-   0        0        0     1329 2023-01-12 16:21:25.000000 delia-1.0.9/delia/utils/tools.py
+-rw-rw-rw-   0        0        0     2131 2023-01-12 16:21:25.000000 delia-1.0.9/delia/utils/transforms_history.py
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.220234 delia-1.0.9/delia.egg-info/
+-rw-rw-rw-   0        0        0    14520 2023-01-12 16:33:00.000000 delia-1.0.9/delia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2041 2023-01-12 16:33:00.000000 delia-1.0.9/delia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-12 16:33:00.000000 delia-1.0.9/delia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-01-12 16:33:00.000000 delia-1.0.9/delia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-01-12 16:33:00.000000 delia-1.0.9/delia.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-01-12 16:33:00.271608 delia-1.0.9/examples/
+-rw-rw-rw-   0        0        0       38 2023-01-12 16:21:25.000000 delia-1.0.9/examples/__init__.py
+-rw-rw-rw-   0        0        0      712 2023-01-12 16:21:25.000000 delia-1.0.9/examples/env_examples.py
+-rw-rw-rw-   0        0        0     3097 2023-01-12 16:21:25.000000 delia-1.0.9/examples/ex01.py
+-rw-rw-rw-   0        0        0     3106 2023-01-12 16:21:25.000000 delia-1.0.9/examples/ex02.py
+-rw-rw-rw-   0        0        0     2750 2023-01-12 16:21:25.000000 delia-1.0.9/examples/ex03.py
+-rw-rw-rw-   0        0        0     5641 2023-01-12 16:21:25.000000 delia-1.0.9/examples/ex04.py
+-rw-rw-rw-   0        0        0       42 2023-01-12 16:33:00.273609 delia-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2023-01-12 16:32:36.000000 delia-1.0.9/setup.py
```

### Comparing `delia-1.0.8/LICENSE` & `delia-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/PKG-INFO` & `delia-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delia
-Version: 1.0.8
+Version: 1.0.9
 Summary: DICOM Extraction for Large-scale Image Analysis (DELIA).
 Home-page: https://github.com/MaxenceLarose/delia
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: dicom hdf5 medical image segmentation pre-processing python3 radiomics deep-learning dicom-seg rt-struct
 Classifier: Programming Language :: Python :: 3
```

### Comparing `delia-1.0.8/README.md` & `delia-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/__init__.py` & `delia-1.0.9/delia/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 from .utils import PatientDataModel
 
 stream_handler = logging.StreamHandler()
 stream_handler.setLevel(logging.WARNING)
 logging.getLogger(__name__).addHandler(stream_handler)
 
 __author__ = "Maxence Larose"
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 __copyright__ = "Copyright 2022, Maxence Larose"
 __credits__ = ["Maxence Larose"]
 __license__ = "Apache License 2.0"
 __maintainer__ = "Maxence Larose"
 __email__ = "maxence.larose.1@ulaval.ca"
 __status__ = "Production"
```

### Comparing `delia-1.0.8/delia/databases/patients_database.py` & `delia-1.0.9/delia/databases/patients_database.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/extractors/patients_data_extractor.py` & `delia-1.0.9/delia/extractors/patients_data_extractor.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/radiomics/radiomics_dataset.py` & `delia-1.0.9/delia/radiomics/radiomics_dataset.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/readers/image/dicom_reader.py` & `delia-1.0.9/delia/readers/image/dicom_reader.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/readers/patient_data/factories/base_patient_data_factory.py` & `delia-1.0.9/delia/readers/patient_data/factories/base_patient_data_factory.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/readers/patient_data/factories/patient_data_factories.py` & `delia-1.0.9/delia/readers/patient_data/factories/patient_data_factories.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/readers/patient_data/patient_data_query_context.py` & `delia-1.0.9/delia/readers/patient_data/patient_data_query_context.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/readers/patient_data/patient_data_query_strategy.py` & `delia-1.0.9/delia/readers/patient_data/patient_data_query_strategy.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/readers/patient_data/patient_data_reader.py` & `delia-1.0.9/delia/readers/patient_data/patient_data_reader.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/readers/segmentation/factories/base_segmentation_factory.py` & `delia-1.0.9/delia/readers/segmentation/factories/base_segmentation_factory.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/readers/segmentation/factories/dicom_segmentation_factories.py` & `delia-1.0.9/delia/readers/segmentation/factories/dicom_segmentation_factories.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/readers/segmentation/factories/segment.py` & `delia-1.0.9/delia/readers/segmentation/factories/segment.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/readers/segmentation/factories/segmentation.py` & `delia-1.0.9/delia/readers/segmentation/factories/segmentation.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/readers/segmentation/segmentation_context.py` & `delia-1.0.9/delia/readers/segmentation/segmentation_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,17 +92,17 @@
         Segmentation dicom header.
 
         Returns
         -------
         segmentation_dicom_header : pydicom.dataset.FileDataset
             Segmentation dicom header.
         """
-        dicom = pydicom.dcmread(self.path_to_segmentation, stop_before_pixels=True)
+        header = pydicom.dcmread(self.path_to_segmentation, stop_before_pixels=True)
 
-        return dicom.Modality
+        return header
 
     @property
     def segmentation_strategy(self) -> SegmentationStrategy:
         """
         Segmentation strategy corresponding to the given segmentation modality.
 
         Returns
```

### Comparing `delia-1.0.8/delia/readers/segmentation/segmentation_reader.py` & `delia-1.0.9/delia/readers/segmentation/segmentation_reader.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/readers/segmentation/segmentation_strategy.py` & `delia-1.0.9/delia/readers/segmentation/segmentation_strategy.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/transforms/applications.py` & `delia-1.0.9/delia/transforms/applications.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/transforms/array_space/matching_crop_foreground.py` & `delia-1.0.9/delia/transforms/array_space/matching_crop_foreground.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/transforms/data/copy_segmentations.py` & `delia-1.0.9/delia/transforms/data/copy_segmentations.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/transforms/data/transform.py` & `delia-1.0.9/delia/transforms/data/transform.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/transforms/physical_space/pet_to_suv.py` & `delia-1.0.9/delia/transforms/physical_space/pet_to_suv.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/transforms/physical_space/resample.py` & `delia-1.0.9/delia/transforms/physical_space/resample.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/transforms/physical_space/transform.py` & `delia-1.0.9/delia/transforms/physical_space/transform.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/transforms/tools.py` & `delia-1.0.9/delia/transforms/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/utils/data_model.py` & `delia-1.0.9/delia/utils/data_model.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/utils/tools.py` & `delia-1.0.9/delia/utils/tools.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia/utils/transforms_history.py` & `delia-1.0.9/delia/utils/transforms_history.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/delia.egg-info/PKG-INFO` & `delia-1.0.9/delia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delia
-Version: 1.0.8
+Version: 1.0.9
 Summary: DICOM Extraction for Large-scale Image Analysis (DELIA).
 Home-page: https://github.com/MaxenceLarose/delia
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: dicom hdf5 medical image segmentation pre-processing python3 radiomics deep-learning dicom-seg rt-struct
 Classifier: Programming Language :: Python :: 3
```

### Comparing `delia-1.0.8/delia.egg-info/SOURCES.txt` & `delia-1.0.9/delia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/examples/env_examples.py` & `delia-1.0.9/examples/env_examples.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/examples/ex01.py` & `delia-1.0.9/examples/ex01.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/examples/ex02.py` & `delia-1.0.9/examples/ex02.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/examples/ex03.py` & `delia-1.0.9/examples/ex03.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/examples/ex04.py` & `delia-1.0.9/examples/ex04.py`

 * *Files identical despite different names*

### Comparing `delia-1.0.8/setup.py` & `delia-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="delia",
-    version="1.0.8",
+    version="1.0.9",
     author="Maxence Larose",
     author_email="maxence.larose.1@ulaval.ca",
     description="DICOM Extraction for Large-scale Image Analysis (DELIA).",
     long_description=open('README.md', "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/MaxenceLarose/delia",
     license="Apache License 2.0",
```

