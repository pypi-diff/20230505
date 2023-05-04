# Comparing `tmp/voxelmap-4.2.0.tar.gz` & `tmp/voxelmap-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxelmap-4.2.0.tar", max compression
+gzip compressed data, was "voxelmap-4.3.0.tar", max compression
```

## Comparing `voxelmap-4.2.0.tar` & `voxelmap-4.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-4.2.0/LICENSE
--rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-4.2.0/README.md
--rw-r--r--   0        0        0      590 2023-05-01 23:49:48.096334 voxelmap-4.2.0/pyproject.toml
--rw-r--r--   0        0        0       87 2023-05-01 21:53:23.971994 voxelmap-4.2.0/voxelmap/__init__.py
--rw-r--r--   0        0        0    18090 2023-05-01 23:31:17.709032 voxelmap-4.2.0/voxelmap/annex.py
--rw-r--r--   0        0        0     3469 2023-05-01 22:00:09.289822 voxelmap-4.2.0/voxelmap/legacy.py
--rwxr-xr-x   0        0        0    29202 2023-05-01 23:31:20.000989 voxelmap-4.2.0/voxelmap/main.py
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 voxelmap-4.2.0/setup.py
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 voxelmap-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-4.3.0/LICENSE
+-rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-4.3.0/README.md
+-rw-r--r--   0        0        0      693 2023-05-04 17:31:28.671767 voxelmap-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-05-01 21:53:23.971994 voxelmap-4.3.0/voxelmap/__init__.py
+-rw-r--r--   0        0        0    18090 2023-05-01 23:31:17.709032 voxelmap-4.3.0/voxelmap/annex.py
+-rw-r--r--   0        0        0     3469 2023-05-01 22:00:09.289822 voxelmap-4.3.0/voxelmap/legacy.py
+-rwxr-xr-x   0        0        0    29600 2023-05-04 20:29:07.581316 voxelmap-4.3.0/voxelmap/main.py
+-rw-r--r--   0        0        0     2885 1970-01-01 00:00:00.000000 voxelmap-4.3.0/setup.py
+-rw-r--r--   0        0        0     3009 1970-01-01 00:00:00.000000 voxelmap-4.3.0/PKG-INFO
```

### Comparing `voxelmap-4.2.0/LICENSE` & `voxelmap-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voxelmap-4.2.0/README.md` & `voxelmap-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `voxelmap-4.2.0/pyproject.toml` & `voxelmap-4.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voxelmap"
-version = "4.2.0"
+version = "4.3.0"
 description = "A Python library for making voxel and 3D models from NumPy arrays."
 authors = ["andrewrgarcia <garcia.gtr@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
@@ -15,11 +15,16 @@
 scipy = "^1.10.0"
 scikit-image = "^0.19.3"
 pyvista = "^0.38.2"
 colorcet = "^3.0.1"
 pytest = "^7.3.1"
 sphinx = "^6.1.3"
 sphinx-rtd-theme = "^1.2.0"
+transformers = "^4.28.1"
+torch = "^2.0.0"
+open3d = "^0.17.0"
+scikit-learn = "^1.2.2"
+addict = "^2.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `voxelmap-4.2.0/voxelmap/annex.py` & `voxelmap-4.3.0/voxelmap/annex.py`

 * *Files identical despite different names*

### Comparing `voxelmap-4.2.0/voxelmap/legacy.py` & `voxelmap-4.3.0/voxelmap/legacy.py`

 * *Files identical despite different names*

### Comparing `voxelmap-4.2.0/voxelmap/main.py` & `voxelmap-4.3.0/voxelmap/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
 
         voxels = Model(self.array).build()
 
         ax.voxels(voxels, facecolors=voxcolors, edgecolors=edgecolors)
         set_axes_equal(ax)
         plt.show()
 
-    def draw(self, coloring='none', geometry = 'voxels', scalars='', background_color='#cccccc', wireframe=False, wireframe_color='k', window_size=[1024, 768],voxel_spacing=(1,1,1),show=True):
+    def draw(self, coloring='none', geometry = 'voxels', scalars='', background_color='#cccccc', wireframe=False, wireframe_color='k', window_size=[1024, 768],len_voxel=1,show=True):
         '''Draws voxel model after building it with the provided `array` with PyVista library 
 
         Parameters
         ----------
         coloring: string  
             voxel coloring scheme
                 * 'custom'                      --> colors voxel model based on the provided keys to its array integers, defined in the `hashblocks` variable from the `Model` class
@@ -341,16 +341,16 @@
             background color of pyvista plot
         wireframe: bool
             Represent mesh as wireframe instead of solid polyhedron if True (default: False). 
         wireframe_color: string / hex 
             edges or wireframe colors
         window_size : (float,float)
             defines plot window dimensions. Defaults to [1024, 768], unless set differently in the relevant theme’s window_size property [pyvista.Plotter]
-        voxel_spacing : (float,float,float)
-            changes voxel spacing by defining length scales of x y and z directions (default:(1,1,1)).
+        len_voxel : float [for geometry='voxels' or 'particles'] / (float,float,float) [for geometry='voxels']
+            The characteristic side length (or lengths) of the voxel. For 'voxels' geometry, the x,y,z side lengths may be set by defining them in a tuple i.e. len_voxel=(x_len,y_len,z_len); if the len_voxel is set to a singular value, it assumes all box side lengths are the same. For 'particles' geometry, len_voxel=radius (default=1) 
         show : bool
             Display Pyvista 3-D render of drawn 3-D model if True (default: True)
         '''
 
         xx, yy, zz, voxid = matrix_toXY(self.array, 1).T
 
         centers = np.vstack((xx.ravel(), yy.ravel(), zz.ravel())).T
@@ -416,25 +416,25 @@
                     if memory_blocks:
                         #add custom hashblocks from memory here
                         for j in memory_blocks.keys():
                             self.hashblocks[j] = memory_blocks[j]                            
                     
                     print('Voxelmap draw. Using custom colormap: ',colormap)
 
-                except: 
+                except Exception as e: 
                     print('ERROR: colormap {} does not exist / is not available ',colormap)
-
+                    print(e)
 
         for i in range(len(centers)):
 
-            x_len,y_len,z_len = voxel_spacing
+            x_len,y_len,z_len = tuple(3*[len_voxel]) if type(len_voxel) == int or float else len_voxel
 
             # Voxel Geometry
             if geometry == 'particles':
-                voxel = pyvista.Sphere(center=centers[i],radius=0.5)
+                voxel = pyvista.Sphere(center=centers[i],radius=len_voxel)
                 smooth = True
             else:
                 voxel = pyvista.Cube(center=centers[i],x_length=x_len, y_length=y_len, z_length=z_len)
                 smooth= None
 
             # Mesh creation and coloring
             if coloring[:6] == 'custom' or coloring[:4] == 'cmap' :
```

### Comparing `voxelmap-4.2.0/setup.py` & `voxelmap-4.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,29 +4,34 @@
 packages = \
 ['voxelmap']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['colorcet>=3.0.1,<4.0.0',
+['addict>=2.4.0,<3.0.0',
+ 'colorcet>=3.0.1,<4.0.0',
  'matplotlib>=3.6.2,<4.0.0',
  'numpy>=1.24.1,<2.0.0',
+ 'open3d>=0.17.0,<0.18.0',
  'opencv-python>=4.7.0.68,<5.0.0.0',
  'pandas>=1.5.2,<2.0.0',
  'pytest>=7.3.1,<8.0.0',
  'pyvista>=0.38.2,<0.39.0',
  'scikit-image>=0.19.3,<0.20.0',
+ 'scikit-learn>=1.2.2,<2.0.0',
  'scipy>=1.10.0,<2.0.0',
  'sphinx-rtd-theme>=1.2.0,<2.0.0',
- 'sphinx>=6.1.3,<7.0.0']
+ 'sphinx>=6.1.3,<7.0.0',
+ 'torch>=2.0.0,<3.0.0',
+ 'transformers>=4.28.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'voxelmap',
-    'version': '4.2.0',
+    'version': '4.3.0',
     'description': 'A Python library for making voxel and 3D models from NumPy arrays.',
     'long_description': '# voxelmap\n\n[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/voxelmap/badge/?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)\n\nA Python library for making voxel and three-dimensional models from NumPy arrays. \n\n<a href="https://voxelmap.readthedocs.io/en/latest/">\n<img src="https://github.com/andrewrgarcia/voxelmap/blob/main/voxelmap.svg?raw=true" width="250"></a>\n\n## Installation and Local Usage \n\n```ruby\npip install voxelmap\n```\n\nIt is recommended you run voxelmap using a `virtualenv` virtual environment. To do so, follow the below simple protocol to create the virtual environment, run it, and install the package there:\n\n```ruby \nvirtualenv venv\nsource venv/bin/activate\npip install voxelmap\npython [your-voxelmap-script.py]\n```\nTo exit the virtual environment, simply type `deactivate`. To access it at any other time again, enter with the above `source venv...` command. \n\n## Just starting? Remote Usage with a Colab notebook (click below)\n\n<a href="https://colab.research.google.com/drive/1RMEMgZHlk_tKAzfS4QfXLJV9joDgdh8N?usp=sharing">\n<img src="https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/docs/img/colaboratory.png" width="500" ></a>\n\n\n## Disclaimer: Use At Your Own Risk\n\nThis program is free software. It comes without any warranty, to the extent permitted by applicable law. You can redistribute it and/or modify it under the terms of the MIT LICENSE, as published by Andrew Garcia. See LICENSE below for more details.\n\n**[MIT license](./LICENSE)** Copyright 2022 © <a href="https://github.com/andrewrgarcia" target="_blank">Andrew Garcia</a>.\n',
     'author': 'andrewrgarcia',
     'author_email': 'garcia.gtr@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['voxelmap']
-package_data = \ {'': ['*']} install_requires = \ ['colorcet>=3.0.1,<4.0.0',
-'matplotlib>=3.6.2,<4.0.0', 'numpy>=1.24.1,<2.0.0', 'opencv-
-python>=4.7.0.68,<5.0.0.0', 'pandas>=1.5.2,<2.0.0', 'pytest>=7.3.1,<8.0.0',
-'pyvista>=0.38.2,<0.39.0', 'scikit-image>=0.19.3,<0.20.0',
+package_data = \ {'': ['*']} install_requires = \ ['addict>=2.4.0,<3.0.0',
+'colorcet>=3.0.1,<4.0.0', 'matplotlib>=3.6.2,<4.0.0', 'numpy>=1.24.1,<2.0.0',
+'open3d>=0.17.0,<0.18.0', 'opencv-python>=4.7.0.68,<5.0.0.0',
+'pandas>=1.5.2,<2.0.0', 'pytest>=7.3.1,<8.0.0', 'pyvista>=0.38.2,<0.39.0',
+'scikit-image>=0.19.3,<0.20.0', 'scikit-learn>=1.2.2,<2.0.0',
 'scipy>=1.10.0,<2.0.0', 'sphinx-rtd-theme>=1.2.0,<2.0.0',
-'sphinx>=6.1.3,<7.0.0'] setup_kwargs = { 'name': 'voxelmap', 'version':
-'4.2.0', 'description': 'A Python library for making voxel and 3D models from
-NumPy arrays.', 'long_description': '# voxelmap\n\n[![License](http://
-img.shields.io/:license-mit-blue.svg?style=flat-square)](https://
-raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)\n[!
-[Documentation Status](https://readthedocs.org/projects/voxelmap/badge/
-?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)\n\nA
-Python library for making voxel and three-dimensional models from NumPy arrays.
-\n\n\n[https://github.com/andrewrgarcia/voxelmap/blob/main/
-voxelmap.svg?raw=true]\n\n## Installation and Local Usage \n\n```ruby\npip
-install voxelmap\n```\n\nIt is recommended you run voxelmap using a
-`virtualenv` virtual environment. To do so, follow the below simple protocol to
-create the virtual environment, run it, and install the package there:
-\n\n```ruby \nvirtualenv venv\nsource venv/bin/activate\npip install
-voxelmap\npython [your-voxelmap-script.py]\n```\nTo exit the virtual
-environment, simply type `deactivate`. To access it at any other time again,
-enter with the above `source venv...` command. \n\n## Just starting? Remote
-Usage with a Colab notebook (click below)\n\n\n[https://
+'sphinx>=6.1.3,<7.0.0', 'torch>=2.0.0,<3.0.0', 'transformers>=4.28.1,<5.0.0']
+setup_kwargs = { 'name': 'voxelmap', 'version': '4.3.0', 'description': 'A
+Python library for making voxel and 3D models from NumPy arrays.',
+'long_description': '# voxelmap\n\n[![License](http://img.shields.io/:license-
+mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/
+andrewrgarcia/voxelmap/main/LICENSE)\n[![Documentation Status](https://
+readthedocs.org/projects/voxelmap/badge/?version=latest)](https://
+voxelmap.readthedocs.io/en/latest/?badge=latest)\n\nA Python library for making
+voxel and three-dimensional models from NumPy arrays. \n\n\n[https://
+github.com/andrewrgarcia/voxelmap/blob/main/voxelmap.svg?raw=true]\n\n##
+Installation and Local Usage \n\n```ruby\npip install voxelmap\n```\n\nIt is
+recommended you run voxelmap using a `virtualenv` virtual environment. To do
+so, follow the below simple protocol to create the virtual environment, run it,
+and install the package there:\n\n```ruby \nvirtualenv venv\nsource venv/bin/
+activate\npip install voxelmap\npython [your-voxelmap-script.py]\n```\nTo exit
+the virtual environment, simply type `deactivate`. To access it at any other
+time again, enter with the above `source venv...` command. \n\n## Just
+starting? Remote Usage with a Colab notebook (click below)\n\n\n[https://
 raw.githubusercontent.com/andrewrgarcia/voxelmap/main/docs/img/
 colaboratory.png]\n\n\n## Disclaimer: Use At Your Own Risk\n\nThis program is
 free software. It comes without any warranty, to the extent permitted by
 applicable law. You can redistribute it and/or modify it under the terms of the
 MIT LICENSE, as published by Andrew Garcia. See LICENSE below for more
 details.\n\n**[MIT license](./LICENSE)** Copyright 2022 Â© Andrew_Garcia.\n',
 'author': 'andrewrgarcia', 'author_email': 'garcia.gtr@gmail.com',
```

### Comparing `voxelmap-4.2.0/PKG-INFO` & `voxelmap-4.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: voxelmap
-Version: 4.2.0
+Version: 4.3.0
 Summary: A Python library for making voxel and 3D models from NumPy arrays.
 License: MIT
 Author: andrewrgarcia
 Author-email: garcia.gtr@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: addict (>=2.4.0,<3.0.0)
 Requires-Dist: colorcet (>=3.0.1,<4.0.0)
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
+Requires-Dist: open3d (>=0.17.0,<0.18.0)
 Requires-Dist: opencv-python (>=4.7.0.68,<5.0.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: pyvista (>=0.38.2,<0.39.0)
 Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
 Requires-Dist: sphinx (>=6.1.3,<7.0.0)
 Requires-Dist: sphinx-rtd-theme (>=1.2.0,<2.0.0)
+Requires-Dist: torch (>=2.0.0,<3.0.0)
+Requires-Dist: transformers (>=4.28.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # voxelmap
 
 [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)
 [![Documentation Status](https://readthedocs.org/projects/voxelmap/badge/?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)
```

#### html2text {}

```diff
@@ -1,24 +1,27 @@
-Metadata-Version: 2.1 Name: voxelmap Version: 4.2.0 Summary: A Python library
+Metadata-Version: 2.1 Name: voxelmap Version: 4.3.0 Summary: A Python library
 for making voxel and 3D models from NumPy arrays. License: MIT Author:
 andrewrgarcia Author-email: garcia.gtr@gmail.com Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: colorcet (>=3.0.1,<4.0.0) Requires-Dist: matplotlib
-(>=3.6.2,<4.0.0) Requires-Dist: numpy (>=1.24.1,<2.0.0) Requires-Dist: opencv-
-python (>=4.7.0.68,<5.0.0.0) Requires-Dist: pandas (>=1.5.2,<2.0.0) Requires-
-Dist: pytest (>=7.3.1,<8.0.0) Requires-Dist: pyvista (>=0.38.2,<0.39.0)
-Requires-Dist: scikit-image (>=0.19.3,<0.20.0) Requires-Dist: scipy
-(>=1.10.0,<2.0.0) Requires-Dist: sphinx (>=6.1.3,<7.0.0) Requires-Dist: sphinx-
-rtd-theme (>=1.2.0,<2.0.0) Description-Content-Type: text/markdown # voxelmap
-[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)]
-(https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE) [!
-[Documentation Status](https://readthedocs.org/projects/voxelmap/badge/
+Requires-Dist: addict (>=2.4.0,<3.0.0) Requires-Dist: colorcet (>=3.0.1,<4.0.0)
+Requires-Dist: matplotlib (>=3.6.2,<4.0.0) Requires-Dist: numpy
+(>=1.24.1,<2.0.0) Requires-Dist: open3d (>=0.17.0,<0.18.0) Requires-Dist:
+opencv-python (>=4.7.0.68,<5.0.0.0) Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pytest (>=7.3.1,<8.0.0) Requires-Dist: pyvista
+(>=0.38.2,<0.39.0) Requires-Dist: scikit-image (>=0.19.3,<0.20.0) Requires-
+Dist: scikit-learn (>=1.2.2,<2.0.0) Requires-Dist: scipy (>=1.10.0,<2.0.0)
+Requires-Dist: sphinx (>=6.1.3,<7.0.0) Requires-Dist: sphinx-rtd-theme
+(>=1.2.0,<2.0.0) Requires-Dist: torch (>=2.0.0,<3.0.0) Requires-Dist:
+transformers (>=4.28.1,<5.0.0) Description-Content-Type: text/markdown #
+voxelmap [![License](http://img.shields.io/:license-mit-blue.svg?style=flat-
+square)](https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)
+[![Documentation Status](https://readthedocs.org/projects/voxelmap/badge/
 ?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest) A
 Python library for making voxel and three-dimensional models from NumPy arrays.
 [https://github.com/andrewrgarcia/voxelmap/blob/main/voxelmap.svg?raw=true] ##
 Installation and Local Usage ```ruby pip install voxelmap ``` It is recommended
 you run voxelmap using a `virtualenv` virtual environment. To do so, follow the
 below simple protocol to create the virtual environment, run it, and install
 the package there: ```ruby virtualenv venv source venv/bin/activate pip install
```

