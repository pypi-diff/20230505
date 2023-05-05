# Comparing `tmp/ifd_python-7.6.8.tar.gz` & `tmp/ifd_python-7.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifd_python-7.6.8.tar", max compression
+gzip compressed data, was "ifd_python-7.6.9.tar", max compression
```

## Comparing `ifd_python-7.6.8.tar` & `ifd_python-7.6.9.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.6.8/LICENSE
--rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.6.8/README.md
--rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/__init__.py
--rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/entities/Abstract/ADetection.py
--rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/entities/Abstract/__init__.py
--rw-r--r--   0        0        0      734 2023-04-19 13:21:34.036921 ifd_python-7.6.8/ifd/entities/Classification.py
--rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/entities/Couleur.py
--rw-r--r--   0        0        0      707 2023-04-13 09:26:25.358120 ifd_python-7.6.8/ifd/entities/Detection.py
--rw-r--r--   0        0        0     2303 2023-04-19 08:19:41.294208 ifd_python-7.6.8/ifd/entities/Image.py
--rw-r--r--   0        0        0     1377 2023-04-19 11:57:33.930576 ifd_python-7.6.8/ifd/entities/LogResult.py
--rw-r--r--   0        0        0      477 2023-04-13 09:26:25.358120 ifd_python-7.6.8/ifd/entities/Modele.py
--rw-r--r--   0        0        0      777 2023-04-21 09:53:14.432345 ifd_python-7.6.8/ifd/entities/OCR.py
--rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/entities/RabbitMqMessage.py
--rw-r--r--   0        0        0      709 2023-04-19 08:27:21.531854 ifd_python-7.6.8/ifd/entities/Tag.py
--rw-r--r--   0        0        0      262 2023-04-19 09:19:06.169869 ifd_python-7.6.8/ifd/entities/__init__.py
--rw-r--r--   0        0        0      717 2023-04-13 09:26:25.358120 ifd_python-7.6.8/ifd/entities/bbox.py
--rw-r--r--   0        0        0     2219 2023-04-14 12:09:37.448293 ifd_python-7.6.8/ifd/repository/AmqpImageRepository.py
--rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/repository/Interfaces/IImageRepository.py
--rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/repository/Interfaces/__init__.py
--rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/repository/MemoryImageRepository.py
--rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/repository/__init__.py
--rw-r--r--   0        0        0      644 2023-04-17 07:37:46.512419 ifd_python-7.6.8/ifd/spec.py
--rw-r--r--   0        0        0      526 2023-04-19 08:19:41.298208 ifd_python-7.6.8/ifd/tools.py
--rw-r--r--   0        0        0      131 2023-04-14 12:36:19.030168 ifd_python-7.6.8/ifd/usecase/Interfaces/IFonction.py
--rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.6.8/ifd/usecase/Interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 09:53:31.196553 ifd_python-7.6.8/ifd/usecase/__init__.py
--rw-r--r--   0        0        0      329 2023-04-21 09:53:40.652670 ifd_python-7.6.8/pyproject.toml
--rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 ifd_python-7.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-12 12:43:31.521191 ifd_python-7.6.9/LICENSE
+-rw-r--r--   0        0        0      551 2023-04-12 12:43:31.521191 ifd_python-7.6.9/README.md
+-rw-r--r--   0        0        0      283 2023-04-12 12:43:31.521191 ifd_python-7.6.9/ifd/__init__.py
+-rw-r--r--   0        0        0      971 2023-04-12 12:43:31.521191 ifd_python-7.6.9/ifd/entities/Abstract/ADetection.py
+-rw-r--r--   0        0        0       34 2023-04-12 12:43:31.521191 ifd_python-7.6.9/ifd/entities/Abstract/__init__.py
+-rw-r--r--   0        0        0      734 2023-04-19 13:21:34.036921 ifd_python-7.6.9/ifd/entities/Classification.py
+-rw-r--r--   0        0        0      228 2023-04-12 12:43:31.521191 ifd_python-7.6.9/ifd/entities/Couleur.py
+-rw-r--r--   0        0        0      707 2023-04-13 09:26:25.358120 ifd_python-7.6.9/ifd/entities/Detection.py
+-rw-r--r--   0        0        0     2303 2023-04-19 08:19:41.294208 ifd_python-7.6.9/ifd/entities/Image.py
+-rw-r--r--   0        0        0     1377 2023-04-19 11:57:33.930576 ifd_python-7.6.9/ifd/entities/LogResult.py
+-rw-r--r--   0        0        0      477 2023-04-13 09:26:25.358120 ifd_python-7.6.9/ifd/entities/Modele.py
+-rw-r--r--   0        0        0      777 2023-04-21 09:53:14.432345 ifd_python-7.6.9/ifd/entities/OCR.py
+-rw-r--r--   0        0        0      517 2023-04-12 12:43:31.521191 ifd_python-7.6.9/ifd/entities/RabbitMqMessage.py
+-rw-r--r--   0        0        0      709 2023-04-19 08:27:21.531854 ifd_python-7.6.9/ifd/entities/Tag.py
+-rw-r--r--   0        0        0      296 2023-05-04 07:08:06.242828 ifd_python-7.6.9/ifd/entities/Ticket.py
+-rw-r--r--   0        0        0      290 2023-05-03 16:41:43.255646 ifd_python-7.6.9/ifd/entities/__init__.py
+-rw-r--r--   0        0        0      717 2023-04-13 09:26:25.358120 ifd_python-7.6.9/ifd/entities/bbox.py
+-rw-r--r--   0        0        0     2219 2023-04-14 12:09:37.448293 ifd_python-7.6.9/ifd/repository/AmqpImageRepository.py
+-rw-r--r--   0        0        0       88 2023-04-12 12:43:31.521191 ifd_python-7.6.9/ifd/repository/Interfaces/IImageRepository.py
+-rw-r--r--   0        0        0       46 2023-04-12 12:43:31.521191 ifd_python-7.6.9/ifd/repository/Interfaces/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-12 12:43:31.521191 ifd_python-7.6.9/ifd/repository/MemoryImageRepository.py
+-rw-r--r--   0        0        0      110 2023-04-12 12:43:31.521191 ifd_python-7.6.9/ifd/repository/__init__.py
+-rw-r--r--   0        0        0      644 2023-04-17 07:37:46.512419 ifd_python-7.6.9/ifd/spec.py
+-rw-r--r--   0        0        0      526 2023-04-19 08:19:41.298208 ifd_python-7.6.9/ifd/tools.py
+-rw-r--r--   0        0        0      131 2023-04-14 12:36:19.030168 ifd_python-7.6.9/ifd/usecase/Interfaces/IFonction.py
+-rw-r--r--   0        0        0       32 2023-04-12 12:43:31.521191 ifd_python-7.6.9/ifd/usecase/Interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 07:08:19.402987 ifd_python-7.6.9/ifd/usecase/__init__.py
+-rw-r--r--   0        0        0      329 2023-05-04 07:08:28.627099 ifd_python-7.6.9/pyproject.toml
+-rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 ifd_python-7.6.9/PKG-INFO
```

### Comparing `ifd_python-7.6.8/LICENSE` & `ifd_python-7.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.8/README.md` & `ifd_python-7.6.9/README.md`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.8/ifd/entities/Abstract/ADetection.py` & `ifd_python-7.6.9/ifd/entities/Abstract/ADetection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.8/ifd/entities/Classification.py` & `ifd_python-7.6.9/ifd/entities/Classification.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.8/ifd/entities/Detection.py` & `ifd_python-7.6.9/ifd/entities/Detection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.8/ifd/entities/Image.py` & `ifd_python-7.6.9/ifd/entities/Image.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.8/ifd/entities/LogResult.py` & `ifd_python-7.6.9/ifd/entities/LogResult.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.8/ifd/entities/OCR.py` & `ifd_python-7.6.9/ifd/entities/OCR.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.8/ifd/entities/RabbitMqMessage.py` & `ifd_python-7.6.9/ifd/entities/RabbitMqMessage.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.8/ifd/entities/Tag.py` & `ifd_python-7.6.9/ifd/entities/Tag.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.8/ifd/entities/bbox.py` & `ifd_python-7.6.9/ifd/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.8/ifd/repository/AmqpImageRepository.py` & `ifd_python-7.6.9/ifd/repository/AmqpImageRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.8/ifd/spec.py` & `ifd_python-7.6.9/ifd/spec.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.8/ifd/tools.py` & `ifd_python-7.6.9/ifd/tools.py`

 * *Files identical despite different names*

### Comparing `ifd_python-7.6.8/PKG-INFO` & `ifd_python-7.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifd-python
-Version: 7.6.8
+Version: 7.6.9
 Summary: 
 Author: Antonin Lemoine
 Author-email: antonin.lemoine@altitudeinfra.fr
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

