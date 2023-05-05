# Comparing `tmp/pizurscan-0.1.5.tar.gz` & `tmp/pizurscan-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizurscan-0.1.5.tar", last modified: Tue May  2 17:34:04 2023, max compression
+gzip compressed data, was "pizurscan-0.1.6.tar", last modified: Fri May  5 08:06:54 2023, max compression
```

## Comparing `pizurscan-0.1.5.tar` & `pizurscan-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:34:04.993137 pizurscan-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-02 17:34:04.993137 pizurscan-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-02 17:33:50.000000 pizurscan-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:34:04.989137 pizurscan-0.1.5/pizurscan/
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-02 17:33:50.000000 pizurscan-0.1.5/pizurscan/InputProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-05-02 17:33:50.000000 pizurscan-0.1.5/pizurscan/InputValidator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-02 17:33:50.000000 pizurscan-0.1.5/pizurscan/OutputProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-02 17:33:50.000000 pizurscan-0.1.5/pizurscan/PI_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-02 17:33:50.000000 pizurscan-0.1.5/pizurscan/Scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 17:33:50.000000 pizurscan-0.1.5/pizurscan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:34:04.993137 pizurscan-0.1.5/pizurscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-02 17:34:04.000000 pizurscan-0.1.5/pizurscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-02 17:34:04.000000 pizurscan-0.1.5/pizurscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:34:04.000000 pizurscan-0.1.5/pizurscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-02 17:34:04.000000 pizurscan-0.1.5/pizurscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 17:34:04.000000 pizurscan-0.1.5/pizurscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 17:34:04.993137 pizurscan-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-02 17:33:50.000000 pizurscan-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:34:04.993137 pizurscan-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    23204 2023-05-02 17:33:50.000000 pizurscan-0.1.5/tests/testclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:06:54.553270 pizurscan-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-05 08:06:54.553270 pizurscan-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-05 08:06:46.000000 pizurscan-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:06:54.549270 pizurscan-0.1.6/pizurscan/
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-05 08:06:46.000000 pizurscan-0.1.6/pizurscan/InputProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-05-05 08:06:46.000000 pizurscan-0.1.6/pizurscan/InputValidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-05 08:06:46.000000 pizurscan-0.1.6/pizurscan/OutputProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-05 08:06:46.000000 pizurscan-0.1.6/pizurscan/PI_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-05 08:06:46.000000 pizurscan-0.1.6/pizurscan/Scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:06:46.000000 pizurscan-0.1.6/pizurscan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:06:54.549270 pizurscan-0.1.6/pizurscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-05 08:06:54.000000 pizurscan-0.1.6/pizurscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-05 08:06:54.000000 pizurscan-0.1.6/pizurscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:06:54.000000 pizurscan-0.1.6/pizurscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 08:06:54.000000 pizurscan-0.1.6/pizurscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 08:06:54.000000 pizurscan-0.1.6/pizurscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:06:54.553270 pizurscan-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-05 08:06:46.000000 pizurscan-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:06:54.553270 pizurscan-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25984 2023-05-05 08:06:46.000000 pizurscan-0.1.6/tests/testclasses.py
```

### Comparing `pizurscan-0.1.5/pizurscan/InputProcessor.py` & `pizurscan-0.1.6/pizurscan/InputProcessor.py`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.5/pizurscan/InputValidator.py` & `pizurscan-0.1.6/pizurscan/InputValidator.py`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.5/pizurscan/OutputProcessor.py` & `pizurscan-0.1.6/pizurscan/OutputProcessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         """
         Save the cleaned 1D data to a file named "cleaned_1D_data.txt".
 
         Args:
         - targets (ndarray): a NumPy array containing the target positions
         - avg_data (ndarray): a NumPy array containing the averaged data
         """
-        out_name = "cleaned_1D_data.txt"
+        out_name = "output/cleaned_1D_data.txt"
         out_file = np.column_stack((targets,avg_data))
         np.savetxt(out_name, out_file, fmt = "%10.6f", delimiter = ",")
 
     def save_processed_data(self):
         """
         Process the 1D data, averaging it if necessary (discrete scan), and save it to a file named "cleaned_1D_data.txt".
         """
```

### Comparing `pizurscan-0.1.5/pizurscan/PI_commands.py` & `pizurscan-0.1.6/pizurscan/PI_commands.py`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.5/pizurscan/Scanner.py` & `pizurscan-0.1.6/pizurscan/Scanner.py`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.5/setup.py` & `pizurscan-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="pizurscan",
-    version="0.1.5",
+    version="0.1.6",
     description="Library to interface PI controllers and Zurich lock-in",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pizur-scanner.readthedocs.io/",
     author="Giacomo Rizzi",
     author_email="rizzigiacomo@pm.me",
     license="MIT",
```

### Comparing `pizurscan-0.1.5/tests/testclasses.py` & `pizurscan-0.1.6/tests/testclasses.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from pizurscan.PI_commands import Stepper
-from pizurscan.Scanners import Scan1D
+from pizurscan.Scanner import Scanner
 from pizurscan.InputProcessor import InputProcessor
 from pipython import pitools,GCS2Commands,GCSDevice
 from pizurscan.OutputProcessor import OutputProcessor
+from pizurscan.InputValidator import InputValidator
+import pytest as pytest
 from math import isclose
 import numpy as np 
 
 class TestStepper:
     stepper = Stepper('C-663', 'L-406.40SD00')
     
     def test_initialization_pidevice(self):
@@ -266,15 +268,15 @@
             "ID":"C-663",
             "stage_ID": "L-406.40SD00",
             "refmode": "FNL",
             "trig_type":6
 		    }
             }
     
-    scanner = Scan1D(inPars)
+    scanner = Scanner(inPars)
     
     def test_initialization_pars(self):
         """Tests that when an instance of Scan1D is created, the inizialitation of the 
         object's attributes through __init__ method is correct."""
         assert self.scanner.PI["ID"] == "C-663"
         assert self.scanner.PI["stage_ID"] == "L-406.40SD00"
         assert self.scanner.PI["refmode"] == "FNL"
@@ -459,8 +461,67 @@
         # expected output
         expected_output = ''
         for i in range(len(targets)):
             expected_output += '\b'+str(targets[i])+', '+'{:.6f}'.format(avg_val[i])+'\n'
 
         # Read the file contents and compare with expected output
         with open("cleaned_1D_data.txt", "rb") as f:
-            assert f.read(),expected_output
+            assert f.read(),expected_output
+            
+        
+class TestInputValidator:
+    """ A class to test that when invalid input scan parameters are inserted, an exeption is raised and the code stops the execution. 
+     Although a lower-level control is already present in the internal PI subroutines, it takes time to be activated. 
+     Therefore, this additional entrance control find out invalid inputs without the need of connecting to the PI instrument. 
+    """
+
+    scanPars = {		
+        "type": "discrete",
+        "scan_edges": [0,1],
+        "stepsize" : 0.1,
+        "velocity" : 1,
+        "acceleration" : 1,
+        "sampling_freq" : 100
+        }
+    
+    
+    inputval = InputValidator(scan_pars=scanPars)
+      
+    def test_valid_input(self):
+        """Tests that when an InputValidator class is instantiated and corrected values of scan parameters
+        are provided, the validate method does not raise any error and return True."""
+        assert self.inputval.validate() == True
+
+    def test_invalid_type(self):
+        """Tests that when an InputValidator class is instantiated and an invalid value of 'type' is passed 
+        to the validate_type function, an exception is raised."""
+        self.inputval.type = "invalid"
+        with pytest.raises(ValueError):
+            self.inputval.validate_type()
+
+    def test_invalid_scan_edges(self):
+        """ Tests that when an InputValidator class is instantiated an invalid value of 'scan_edges' is passed 
+        to the validate_scan_edges function, an exception is raised """
+        self.inputval.scan_edges = [-10, 110]
+        with pytest.raises(ValueError):
+            self.inputval.validate_scan_edges()
+    
+    def test_invalid_stepsize(self):
+        """ Tests that when an InputValidator class is instantiated an invalid value of 'stepsize' is passed 
+        to the validate_stepsize function, an exception is raised """
+        self.inputval.stepsize = 200
+        with pytest.raises(ValueError):
+            self.inputval.validate_stepsize()
+
+    def test_invalid_velocity(self):
+        """ Tests that when an InputValidator class is instantiated an invalid value of 'velocity' is passed 
+        to the validate_velocity function, an exception is raised """
+        self.inputval.velocity = -5
+        with pytest.raises(ValueError):
+            self.inputval.validate_velocity()
+
+    def test_invalid_acceleration(self):
+        """ Tests that when an InputValidator class is instantiated an invalid value of 'acceleration' is passed 
+        to the validate_velocity function, an exception is raised """
+        self.inputval.acceleration = 30
+        with pytest.raises(ValueError):
+            self.inputval.validate_acceleration()
```

