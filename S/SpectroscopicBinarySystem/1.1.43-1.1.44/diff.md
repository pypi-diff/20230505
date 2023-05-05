# Comparing `tmp/SpectroscopicBinarySystem-1.1.43.tar.gz` & `tmp/SpectroscopicBinarySystem-1.1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.1.43.tar", last modified: Wed May  3 12:42:38 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.1.44.tar", last modified: Fri May  5 09:13:18 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.1.43.tar` & `SpectroscopicBinarySystem-1.1.44.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 12:42:38.660517 SpectroscopicBinarySystem-1.1.43/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.1.43/LICENSE
--rw-rw-rw-   0        0        0     4732 2023-05-03 12:42:38.660517 SpectroscopicBinarySystem-1.1.43/PKG-INFO
--rw-rw-rw-   0        0        0     4340 2023-05-03 12:42:11.000000 SpectroscopicBinarySystem-1.1.43/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 12:42:38.658010 SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     4732 2023-05-03 12:42:38.000000 SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-05-03 12:42:38.000000 SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 12:42:38.000000 SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-05-03 12:42:38.000000 SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-05-03 12:42:38.000000 SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.1.43/pyproject.toml
--rw-rw-rw-   0        0        0      725 2023-05-03 12:42:38.664540 SpectroscopicBinarySystem-1.1.43/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 12:42:38.660517 SpectroscopicBinarySystem-1.1.43/spectroscopicbinarysystem/
--rw-rw-rw-   0        0        0    30330 2023-05-03 12:40:47.000000 SpectroscopicBinarySystem-1.1.43/spectroscopicbinarysystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:13:18.307776 SpectroscopicBinarySystem-1.1.44/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.1.44/LICENSE
+-rw-rw-rw-   0        0        0     4732 2023-05-05 09:13:18.308875 SpectroscopicBinarySystem-1.1.44/PKG-INFO
+-rw-rw-rw-   0        0        0     4340 2023-05-05 09:13:15.000000 SpectroscopicBinarySystem-1.1.44/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 09:13:18.305408 SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     4732 2023-05-05 09:13:18.000000 SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-05-05 09:13:18.000000 SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 09:13:18.000000 SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-05-05 09:13:18.000000 SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-05-05 09:13:18.000000 SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.1.44/pyproject.toml
+-rw-rw-rw-   0        0        0      725 2023-05-05 09:13:18.310326 SpectroscopicBinarySystem-1.1.44/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 09:13:18.306414 SpectroscopicBinarySystem-1.1.44/spectroscopicbinarysystem/
+-rw-rw-rw-   0        0        0    30236 2023-05-05 09:09:16.000000 SpectroscopicBinarySystem-1.1.44/spectroscopicbinarysystem/__init__.py
```

### Comparing `SpectroscopicBinarySystem-1.1.43/LICENSE` & `SpectroscopicBinarySystem-1.1.44/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.1.43/PKG-INFO` & `SpectroscopicBinarySystem-1.1.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.1.43
+Version: 1.1.44
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.43)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.44)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
```

### Comparing `SpectroscopicBinarySystem-1.1.43/README.md` & `SpectroscopicBinarySystem-1.1.44/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.43)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.44)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
```

### Comparing `SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/PKG-INFO` & `SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.1.43
+Version: 1.1.44
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Spectroscopic Binary System
 
-[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.43)](https://badge.fury.io/py/spectroscopicbinarysystem)
+[![PyPI version](https://badge.fury.io/py/spectroscopicbinarysystem.svg?1.1.44)](https://badge.fury.io/py/spectroscopicbinarysystem)
 
 **Spectroscopic Binary System** is a package intended to contain functionality and some common tools needed for performing astrophysics on spectroscopic binary stars with Python. It allows, among other things, to automatically measure the radial velocity of SB1 type systems and to find their orbital solution with **BinaryStarSolver** (https://github.com/NickMilsonPhysics/BinaryStarSolver)
 
 
 ## Installation
 
 To install **spectroscopicbinarysystem** with pip, run:
```

### Comparing `SpectroscopicBinarySystem-1.1.43/SpectroscopicBinarySystem.egg-info/SOURCES.txt` & `SpectroscopicBinarySystem-1.1.44/SpectroscopicBinarySystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.1.43/setup.cfg` & `SpectroscopicBinarySystem-1.1.44/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 312e 3433 0d0a  rsion = 1.1.43..
+00000030: 7273 696f 6e20 3d20 312e 312e 3434 0d0a  rsion = 1.1.44..
 00000040: 6175 7468 6f72 203d 2047 7569 6c6c 6175  author = Guillau
 00000050: 6d65 2042 6572 7472 616e 640d 0a61 7574  me Bertrand..aut
 00000060: 686f 725f 656d 6169 6c20 3d20 6762 652e  hor_email = gbe.
 00000070: 696f 4070 6d2e 6d65 0d0a 6465 7363 7269  io@pm.me..descri
 00000080: 7074 696f 6e20 3d20 5079 7468 6f6e 2061  ption = Python a
 00000090: 7374 726f 6e6f 6d79 2074 6f6f 6c73 2066  stronomy tools f
 000000a0: 6f72 2073 7065 6374 726f 7363 6f70 6963  or spectroscopic
```

### Comparing `SpectroscopicBinarySystem-1.1.43/spectroscopicbinarysystem/__init__.py` & `SpectroscopicBinarySystem-1.1.44/spectroscopicbinarysystem/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,47 +182,44 @@
         # > Hack to replace zero values of the spectra.
         # Sometimes first value for the intensity is equal to 0.00 and prevents finding the true minima.
         # Ex : sample/alphadra/_alphadra_20230406_856.fits
         self.flux[self.flux == 0] = 1 * u.Jy
         ipeak = self.flux.argmin()
         xpeak = self.spectral_axis[ipeak].to(u.AA)
 
-        invert_s = extract_region(Spectrum1D(flux=self.flux * -1, wcs=self.wcs),
-                                  SpectralRegion(xpeak - (w1 * u.AA), xpeak + (w1 * u.AA)))
+        spec1d_line = extract_region(Spectrum1D(flux=self.flux, wcs=self.wcs),
+                                     SpectralRegion(xpeak - (w1 * u.AA), xpeak + (w1 * u.AA)))
 
-        s_fit = fit_generic_continuum(invert_s,
-                                      exclude_regions=[SpectralRegion(xpeak - (w2 * u.AA), xpeak + (w2 * u.AA))])
-        invert_s = invert_s / s_fit(invert_s.spectral_axis)
-        invert_s = invert_s - 1
+        s_fit = fit_generic_continuum(spec1d_line, exclude_regions=[
+                                      SpectralRegion(xpeak - (w2 * u.AA), xpeak + (w2 * u.AA))])
+        spec1d_line = spec1d_line / s_fit(spec1d_line.spectral_axis)
+        spec1d_line = spec1d_line - 1
 
         match self._conf['LINE_FIT_MODEL']:
             case 'gaussian':
                 g_init = models.Gaussian1D(
-                    mean=xpeak, amplitude=invert_s.flux.argmax())
+                    mean=xpeak, amplitude=spec1d_line.flux.argmin())
             case 'voigt':
                 g_init = models.Voigt1D(
-                    x_0=xpeak, amplitude_L=2 / (np.pi * fwhm))
+                    x_0=xpeak, amplitude_L=spec1d_line.flux.argmin())
             case 'lorentz':
                 g_init = models.Lorentz1D(x_0=xpeak, fwhm=fwhm)
-            case _:
-                g_init = models.Gaussian1D(
-                    mean=xpeak, amplitude=invert_s.flux.argmax())
         #
 
-        g_fit = fit_lines(invert_s, g_init, window=SpectralRegion(
+        g_fit = fit_lines(spec1d_line, g_init, window=SpectralRegion(
             xpeak - (w2 * u.AA), xpeak + (w2 * u.AA)))
-        y_fit = g_fit(invert_s.spectral_axis)
+        y_fit = g_fit(spec1d_line.spectral_axis)
 
         match self._conf['LINE_FIT_MODEL']:
             case 'gaussian':
                 center = g_fit.mean
             case _:
                 center = g_fit.x_0
 
-        self._debug_line_fitting = (invert_s, y_fit)
+        self._debug_line_fitting = (spec1d_line, y_fit)
         self._center_of_line = center.value
 
     def __str__(self):
         return f"Spectrum : {self._basename}\n- obs: {self._observer}\n- jd: {self._jd}\n- center: {self._center_of_line} A\n- {self._conf['RV_CORR_TYPE']}: {self._rv_corr}\n- rv: {self._rv}\n "
 
 #
```

