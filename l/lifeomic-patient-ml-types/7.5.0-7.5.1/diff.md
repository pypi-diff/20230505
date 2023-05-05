# Comparing `tmp/lifeomic_patient_ml_types-7.5.0.tar.gz` & `tmp/lifeomic_patient_ml_types-7.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeomic_patient_ml_types-7.5.0.tar", max compression
+gzip compressed data, was "lifeomic_patient_ml_types-7.5.1.tar", max compression
```

## Comparing `lifeomic_patient_ml_types-7.5.0.tar` & `lifeomic_patient_ml_types-7.5.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    14143 2023-04-24 14:01:40.035117 lifeomic_patient_ml_types-7.5.0/lifeomic_patient_ml_types/schemas.py
--rw-r--r--   0        0        0      664 2023-04-24 14:02:54.210471 lifeomic_patient_ml_types-7.5.0/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.5.0/setup.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.5.0/PKG-INFO
+-rw-r--r--   0        0        0    13974 2023-05-05 09:39:38.254231 lifeomic_patient_ml_types-7.5.1/lifeomic_patient_ml_types/schemas.py
+-rw-r--r--   0        0        0      664 2023-05-05 09:40:54.262696 lifeomic_patient_ml_types-7.5.1/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.5.1/setup.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.5.1/PKG-INFO
```

### Comparing `lifeomic_patient_ml_types-7.5.0/lifeomic_patient_ml_types/schemas.py` & `lifeomic_patient_ml_types-7.5.1/lifeomic_patient_ml_types/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,26 +225,14 @@
     class Config:
         extra = Extra.forbid
 
     filterType: Literal["FhirCodesFilter"]
     codes: List[str] = Field(..., max_items=10, min_items=1)
 
 
-class TrainingApproachBase(BaseModel):
-    class Config:
-        extra = Extra.allow
-
-    id: str
-    """
-    UUID uniquely identifying this training approach.
-    """
-    name: str
-    description: str
-
-
 class CategoricalParameterSpace(BaseModel):
     class Config:
         extra = Extra.forbid
 
     type: Literal["categorical"]
     name: str
     values: List[str]
@@ -297,15 +285,18 @@
     class Config:
         extra = Extra.forbid
 
     name: str
     regex: str
 
 
-class TuningJobTrainingApproach(TrainingApproachBase):
+class TuningJobTrainingApproach(BaseModel):
+    class Config:
+        extra = Extra.allow
+
     type: Literal["tuningJob"]
     trainingImage: str = Field(
         ...,
         regex="^[0-9]+\\.dkr.ecr.[-a-z0-9]+\\.amazonaws\\.com\\/[-_a-zA-Z0-9]+:[-_a-zA-Z0-9]+$",
     )
     """
     An aws ecr image uri of the form <account-id>.dkr.ecr.<region>.amazonaws.com/<repo-name>:<tag>
```

### Comparing `lifeomic_patient_ml_types-7.5.0/pyproject.toml` & `lifeomic_patient_ml_types-7.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lifeomic-patient-ml-types"
-version = "7.5.0"
+version = "7.5.1"
 description = "Shared types for the patient-ml-service repos."
 authors = ["LifeOmic <development@lifeomic.com>"]
 license = "UNLICENSED"
 
 [tool.poe.tasks]
 format = "black lifeomic_patient_ml_types"
 lint = "pyright lifeomic_patient_ml_types"
```

### Comparing `lifeomic_patient_ml_types-7.5.0/setup.py` & `lifeomic_patient_ml_types-7.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['lifeomic_patient_ml_types']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'lifeomic-patient-ml-types',
-    'version': '7.5.0',
+    'version': '7.5.1',
     'description': 'Shared types for the patient-ml-service repos.',
     'long_description': 'None',
     'author': 'LifeOmic',
     'author_email': 'development@lifeomic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

