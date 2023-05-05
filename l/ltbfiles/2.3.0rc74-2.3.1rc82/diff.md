# Comparing `tmp/ltbfiles-2.3.0rc74.tar.gz` & `tmp/ltbfiles-2.3.1rc82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltbfiles-2.3.0rc74.tar", last modified: Mon Mar 20 14:16:41 2023, max compression
+gzip compressed data, was "ltbfiles-2.3.1rc82.tar", last modified: Fri May  5 13:30:05 2023, max compression
```

## Comparing `ltbfiles-2.3.0rc74.tar` & `ltbfiles-2.3.1rc82.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 14:16:41.068852 ltbfiles-2.3.0rc74/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2023-03-20 14:16:27.000000 ltbfiles-2.3.0rc74/LICENSE_GPL_v3.txt
--rw-r--r--   0 root         (0) root         (0)     1119 2023-03-20 14:16:41.068852 ltbfiles-2.3.0rc74/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      548 2023-03-20 14:16:27.000000 ltbfiles-2.3.0rc74/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 14:16:41.067019 ltbfiles-2.3.0rc74/ltbfiles/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-03-20 14:16:27.000000 ltbfiles-2.3.0rc74/ltbfiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15713 2023-03-20 14:16:27.000000 ltbfiles-2.3.0rc74/ltbfiles/ltbfiles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 14:16:41.067935 ltbfiles-2.3.0rc74/ltbfiles.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1119 2023-03-20 14:16:41.000000 ltbfiles-2.3.0rc74/ltbfiles.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      269 2023-03-20 14:16:41.000000 ltbfiles-2.3.0rc74/ltbfiles.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 14:16:41.000000 ltbfiles-2.3.0rc74/ltbfiles.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-03-20 14:16:41.000000 ltbfiles-2.3.0rc74/ltbfiles.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-20 14:16:41.000000 ltbfiles-2.3.0rc74/ltbfiles.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-03-20 14:16:27.000000 ltbfiles-2.3.0rc74/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       43 2023-03-20 14:16:41.068852 ltbfiles-2.3.0rc74/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 14:16:41.068852 ltbfiles-2.3.0rc74/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4465 2023-03-20 14:16:27.000000 ltbfiles-2.3.0rc74/tests/test_load_files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:30:05.861968 ltbfiles-2.3.1rc82/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/LICENSE_GPL_v3.txt
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-05-05 13:30:05.861968 ltbfiles-2.3.1rc82/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      548 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:30:05.858968 ltbfiles-2.3.1rc82/ltbfiles/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/ltbfiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15777 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/ltbfiles/ltbfiles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:30:05.860968 ltbfiles-2.3.1rc82/ltbfiles.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-05-05 13:30:05.000000 ltbfiles-2.3.1rc82/ltbfiles.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-05 13:30:05.000000 ltbfiles-2.3.1rc82/ltbfiles.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 13:30:05.000000 ltbfiles-2.3.1rc82/ltbfiles.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-05 13:30:05.000000 ltbfiles-2.3.1rc82/ltbfiles.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-05 13:30:05.000000 ltbfiles-2.3.1rc82/ltbfiles.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-05 13:30:05.861968 ltbfiles-2.3.1rc82/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:30:05.860968 ltbfiles-2.3.1rc82/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4776 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/tests/test_load_files.py
```

### Comparing `ltbfiles-2.3.0rc74/LICENSE_GPL_v3.txt` & `ltbfiles-2.3.1rc82/LICENSE_GPL_v3.txt`

 * *Files identical despite different names*

### Comparing `ltbfiles-2.3.0rc74/PKG-INFO` & `ltbfiles-2.3.1rc82/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltbfiles
-Version: 2.3.0rc74
+Version: 2.3.1rc82
 Summary: Module for loading of files created with spectrometers from LTB
 Author: Sven Merk
 Project-URL: Homepage, https://gitlab.com/ltb_berlin/ltb_files
 Project-URL: Bug Tracker, https://gitlab.com/ltb_berlin/ltb_files/-/issues
 Project-URL: Wiki, https://gitlab.com/ltb_berlin/ltb_files/-/wikis/home
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `ltbfiles-2.3.0rc74/README.md` & `ltbfiles-2.3.1rc82/README.md`

 * *Files identical despite different names*

### Comparing `ltbfiles-2.3.0rc74/ltbfiles/ltbfiles.py` & `ltbfiles-2.3.1rc82/ltbfiles/ltbfiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,23 +342,23 @@
             o = np.ones(x.size)
 
     head['filename'] = filename
     return Spectra(y, x, o, head)
 
 
 def _make_header_from_array(data):
-    head = {'ChipWidth': data[0],
-            'ChipHeight': data[1],
-            'PixelSize': data[2],
-            'HorBinning': data[3],
-            'VerBinning': data[4],
-            'BottomOffset': data[5],
-            'LeftOffset': data[6],
-            'ImgHeight': data[7],
-            'ImgWidth': data[8]
+    head = {'ChipWidth': int(data[0]),
+            'ChipHeight': int(data[1]),
+            'PixelSize': float(data[2]),
+            'HorBinning': int(data[3]),
+            'VerBinning': int(data[4]),
+            'BottomOffset': int(data[5]),
+            'LeftOffset': int(data[6]),
+            'ImgHeight': int(data[7]),
+            'ImgWidth': int(data[8])
             }
     return head
 
 
 def read_ltb_raw(filename: Union[Path,str]) -> Tuple[np.ndarray, dict]:
     """
     This function reads *.raw image files created with LTB spectrometers.
@@ -369,15 +369,15 @@
     Outputs
     -------
     image : np.array of image shape
     head : dict containing image properties
     """
     data = np.loadtxt(filename)
     head = _make_header_from_array(data[0:9])
-    image = np.reshape(data[9:], (head['ImgHeight'], head['ImgWidth']))
+    image = np.reshape(data[9:].astype(np.int32), (head['ImgHeight'], head['ImgWidth']))
     return image, head
 
 
 def read_ltb_rawb(filename: Union[Path,str]) -> Tuple[np.ndarray, dict]:
     """
     This function reads *.rawb image files created with LTB spectrometers.
     Input
@@ -433,10 +433,10 @@
                 sophi_file_full = os.path.join(extract_folder, i_file)
                 sophi_head.read(sophi_file_full)
         width = int(aryelle_head['CCD']['width']) // int(sophi_head['Echelle 1']['vertical binning'])
         height = int(aryelle_head['CCD']['height']) // int(sophi_head['Echelle 1']['horizontal binning'])
         head = {'sophi_ini': sophi_head,
                 'aryelle_ini': aryelle_head}
         assert image is not None
-        image = image.reshape((width, height))
+        image = image.reshape((height, width))
 
     return image, head
```

### Comparing `ltbfiles-2.3.0rc74/ltbfiles.egg-info/PKG-INFO` & `ltbfiles-2.3.1rc82/ltbfiles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltbfiles
-Version: 2.3.0rc74
+Version: 2.3.1rc82
 Summary: Module for loading of files created with spectrometers from LTB
 Author: Sven Merk
 Project-URL: Homepage, https://gitlab.com/ltb_berlin/ltb_files
 Project-URL: Bug Tracker, https://gitlab.com/ltb_berlin/ltb_files/-/issues
 Project-URL: Wiki, https://gitlab.com/ltb_berlin/ltb_files/-/wikis/home
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `ltbfiles-2.3.0rc74/pyproject.toml` & `ltbfiles-2.3.1rc82/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ltbfiles-2.3.0rc74/tests/test_load_files.py` & `ltbfiles-2.3.1rc82/tests/test_load_files.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,13 +127,26 @@
 
 def test_load_non_matching_folder(files_dir):
     with pytest.raises(Exception) as excinfo:
         ltbfiles.load_folder(files_dir)
     assert str(files_dir) in excinfo.value.args[0]
 
 
-def test_load_rawx(files_dir):
-    filename = files_dir / 'deuterium.rawx'
-    img, head = ltbfiles.read_ltb_rawx(filename)
-    assert (2048, 512) == img.shape
+def test_load_raw(raw_file):
+    img, head = ltbfiles.read_ltb_raw(raw_file)
+    assert (512, 2048) == img.shape
+    assert isinstance(head, dict)
+    assert 9 == len(head)
+
+
+def test_load_rawb(rawb_file):
+    img, head = ltbfiles.read_ltb_rawb(rawb_file)
+    assert (512, 2048) == img.shape
+    assert isinstance(head, dict)
+    assert 9 == len(head)
+
+
+def test_load_rawx(rawx_file):
+    img, head = ltbfiles.read_ltb_rawx(rawx_file)
+    assert (512, 2048) == img.shape
     assert isinstance(head, dict)
     assert 2 == len(head)
```

