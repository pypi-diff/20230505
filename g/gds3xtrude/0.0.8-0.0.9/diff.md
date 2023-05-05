# Comparing `tmp/gds3xtrude-0.0.8.tar.gz` & `tmp/gds3xtrude-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gds3xtrude-0.0.8.tar", last modified: Thu Mar 28 15:25:54 2019, max compression
+gzip compressed data, was "dist/gds3xtrude-0.0.9.tar", last modified: Sun Apr 19 15:51:51 2020, max compression
```

## Comparing `gds3xtrude-0.0.8.tar` & `gds3xtrude-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2019-03-28 15:25:54.000000 gds3xtrude-0.0.8/
--rw-r--r--   0 user      (1000) user      (1000)    34523 2019-01-03 13:00:22.000000 gds3xtrude-0.0.8/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)       64 2019-03-22 14:14:28.000000 gds3xtrude-0.0.8/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     7201 2019-03-28 15:25:54.000000 gds3xtrude-0.0.8/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     5367 2019-03-28 15:24:16.000000 gds3xtrude-0.0.8/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2019-03-28 15:25:54.000000 gds3xtrude-0.0.8/bin/
--rw-r--r--   0 user      (1000) user      (1000)     6213 2019-03-28 15:24:16.000000 gds3xtrude-0.0.8/bin/gds3xtrude
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2019-03-28 15:25:54.000000 gds3xtrude-0.0.8/examples/
--rw-r--r--   0 user      (1000) user      (1000)     2115 2019-03-28 15:24:16.000000 gds3xtrude-0.0.8/examples/freepdk45.layerstack
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2019-03-28 15:25:54.000000 gds3xtrude-0.0.8/gds3xtrude/
--rw-r--r--   0 user      (1000) user      (1000)      806 2019-03-28 15:24:16.000000 gds3xtrude-0.0.8/gds3xtrude/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     5104 2019-03-28 15:24:16.000000 gds3xtrude-0.0.8/gds3xtrude/blender.py
--rw-r--r--   0 user      (1000) user      (1000)     2285 2019-03-28 15:24:16.000000 gds3xtrude-0.0.8/gds3xtrude/blender_extrusion_example.py
--rw-r--r--   0 user      (1000) user      (1000)     9392 2019-03-28 15:24:16.000000 gds3xtrude-0.0.8/gds3xtrude/blender_test.py
--rw-r--r--   0 user      (1000) user      (1000)     3822 2019-03-28 15:24:16.000000 gds3xtrude-0.0.8/gds3xtrude/builder.py
--rw-r--r--   0 user      (1000) user      (1000)     9302 2019-03-28 15:24:16.000000 gds3xtrude-0.0.8/gds3xtrude/gds3xtrude.py
--rw-r--r--   0 user      (1000) user      (1000)     1563 2019-03-28 15:24:16.000000 gds3xtrude-0.0.8/gds3xtrude/include.py
--rw-r--r--   0 user      (1000) user      (1000)     1796 2019-03-28 15:24:16.000000 gds3xtrude-0.0.8/gds3xtrude/layer_operations.py
--rw-r--r--   0 user      (1000) user      (1000)     5036 2019-03-28 15:24:16.000000 gds3xtrude-0.0.8/gds3xtrude/openscad.py
--rw-r--r--   0 user      (1000) user      (1000)     4486 2019-03-28 15:24:16.000000 gds3xtrude-0.0.8/gds3xtrude/polygon_approx.py
--rw-r--r--   0 user      (1000) user      (1000)     1260 2019-03-28 15:24:16.000000 gds3xtrude-0.0.8/gds3xtrude/types.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2019-03-28 15:25:54.000000 gds3xtrude-0.0.8/gds3xtrude.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     7201 2019-03-28 15:25:54.000000 gds3xtrude-0.0.8/gds3xtrude.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      569 2019-03-28 15:25:54.000000 gds3xtrude-0.0.8/gds3xtrude.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2019-03-28 15:25:54.000000 gds3xtrude-0.0.8/gds3xtrude.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2019-01-08 13:13:33.000000 gds3xtrude-0.0.8/gds3xtrude.egg-info/not-zip-safe
--rw-r--r--   0 user      (1000) user      (1000)       34 2019-03-28 15:25:54.000000 gds3xtrude-0.0.8/gds3xtrude.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       11 2019-03-28 15:25:54.000000 gds3xtrude-0.0.8/gds3xtrude.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2019-03-28 15:25:54.000000 gds3xtrude-0.0.8/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1122 2019-03-28 15:24:16.000000 gds3xtrude-0.0.8/setup.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-04-19 15:51:51.000000 gds3xtrude-0.0.9/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    34523 2020-04-19 15:42:48.000000 gds3xtrude-0.0.9/LICENSE
+-rw-r--r--   0 kramert   (1000) kramert   (1000)       64 2020-04-19 15:42:48.000000 gds3xtrude-0.0.9/MANIFEST.in
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     7255 2020-04-19 15:51:51.000000 gds3xtrude-0.0.9/PKG-INFO
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     5413 2020-04-19 15:48:59.000000 gds3xtrude-0.0.9/README.md
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-04-19 15:51:51.000000 gds3xtrude-0.0.9/bin/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     6213 2020-04-19 15:42:48.000000 gds3xtrude-0.0.9/bin/gds3xtrude
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-04-19 15:51:51.000000 gds3xtrude-0.0.9/examples/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     2115 2020-04-19 15:42:48.000000 gds3xtrude-0.0.9/examples/freepdk45.layerstack
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-04-19 15:51:51.000000 gds3xtrude-0.0.9/gds3xtrude/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      806 2020-04-19 15:42:48.000000 gds3xtrude-0.0.9/gds3xtrude/__init__.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     5372 2020-04-19 15:45:50.000000 gds3xtrude-0.0.9/gds3xtrude/blender.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     2285 2020-04-19 15:42:48.000000 gds3xtrude-0.0.9/gds3xtrude/blender_extrusion_example.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     9392 2020-04-19 15:42:48.000000 gds3xtrude-0.0.9/gds3xtrude/blender_test.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     3960 2020-04-19 15:42:48.000000 gds3xtrude-0.0.9/gds3xtrude/builder.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     9302 2020-04-19 15:42:48.000000 gds3xtrude-0.0.9/gds3xtrude/gds3xtrude.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1563 2020-04-19 15:42:48.000000 gds3xtrude-0.0.9/gds3xtrude/include.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1796 2020-04-19 15:42:48.000000 gds3xtrude-0.0.9/gds3xtrude/layer_operations.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     5030 2020-04-19 15:42:48.000000 gds3xtrude-0.0.9/gds3xtrude/openscad.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     4486 2020-04-19 15:42:48.000000 gds3xtrude-0.0.9/gds3xtrude/polygon_approx.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1260 2020-04-19 15:42:48.000000 gds3xtrude-0.0.9/gds3xtrude/types.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-04-19 15:51:51.000000 gds3xtrude-0.0.9/gds3xtrude.egg-info/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     7255 2020-04-19 15:51:51.000000 gds3xtrude-0.0.9/gds3xtrude.egg-info/PKG-INFO
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      569 2020-04-19 15:51:51.000000 gds3xtrude-0.0.9/gds3xtrude.egg-info/SOURCES.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2020-04-19 15:51:51.000000 gds3xtrude-0.0.9/gds3xtrude.egg-info/dependency_links.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2020-04-19 15:51:51.000000 gds3xtrude-0.0.9/gds3xtrude.egg-info/not-zip-safe
+-rw-r--r--   0 kramert   (1000) kramert   (1000)       34 2020-04-19 15:51:51.000000 gds3xtrude-0.0.9/gds3xtrude.egg-info/requires.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)       11 2020-04-19 15:51:51.000000 gds3xtrude-0.0.9/gds3xtrude.egg-info/top_level.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)       38 2020-04-19 15:51:51.000000 gds3xtrude-0.0.9/setup.cfg
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1122 2020-04-19 15:50:12.000000 gds3xtrude-0.0.9/setup.py
```

### Comparing `gds3xtrude-0.0.8/LICENSE` & `gds3xtrude-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gds3xtrude-0.0.8/PKG-INFO` & `gds3xtrude-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gds3xtrude
-Version: 0.0.8
+Version: 0.0.9
 Summary: 3D GDS viewer based on OpenSCAD
 Home-page: https://codeberg.org/tok/gds3xtrude
 Author: T. Kramer
 Author-email: code@tkramer.ch
 License: AGPL
 Description: # gds3xtrude
         A simple layout to 3D converter.
@@ -129,14 +129,15 @@
         
         ## Blender
         3D models can also be generated in blender. Use the command line tool for this:
         ```sh
         gds3xtrude --tech freepdk45.layerstack --input NAND2X1.gds --cad blender
         ```
         Note that the current implementation over the Blender scripting API is very slow and therefore only small things such as standard cells can be visualized.
+        Also make sure to use Blender 2.82 or higher.
         
         ## FreeCAD
         The generated OpenSCAD models (.scad) can be imported into FreeCAD.
         
         ### Color Issue
         When applying a boolean union FreeCAD strips away colors. Therefore an exported .obj model will by totally gray. There is a workaround:
         * Open the OpenSCAD model in FreeCAD
```

### Comparing `gds3xtrude-0.0.8/README.md` & `gds3xtrude-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 
 ## Blender
 3D models can also be generated in blender. Use the command line tool for this:
 ```sh
 gds3xtrude --tech freepdk45.layerstack --input NAND2X1.gds --cad blender
 ```
 Note that the current implementation over the Blender scripting API is very slow and therefore only small things such as standard cells can be visualized.
+Also make sure to use Blender 2.82 or higher.
 
 ## FreeCAD
 The generated OpenSCAD models (.scad) can be imported into FreeCAD.
 
 ### Color Issue
 When applying a boolean union FreeCAD strips away colors. Therefore an exported .obj model will by totally gray. There is a workaround:
 * Open the OpenSCAD model in FreeCAD
```

### Comparing `gds3xtrude-0.0.8/bin/gds3xtrude` & `gds3xtrude-0.0.9/bin/gds3xtrude`

 * *Files identical despite different names*

### Comparing `gds3xtrude-0.0.8/examples/freepdk45.layerstack` & `gds3xtrude-0.0.9/examples/freepdk45.layerstack`

 * *Files identical despite different names*

### Comparing `gds3xtrude-0.0.8/gds3xtrude/__init__.py` & `gds3xtrude-0.0.9/gds3xtrude/__init__.py`

 * *Files identical despite different names*

### Comparing `gds3xtrude-0.0.8/gds3xtrude/blender.py` & `gds3xtrude-0.0.9/gds3xtrude/blender.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,16 +48,22 @@
         """
         Get or create blender material.
         :param m:
         :return: Blender material.
         """
         if m not in self.materials:
             mat = bpy.data.materials.new(m.name)
-            mat.diffuse_color = m.getattr('color', DEFAULT_COLOR)
+            col = tuple(m.getattr('color', DEFAULT_COLOR))
+            
+            if len(col) == 3:
+                col = col + (1,)
+
+            mat.diffuse_color = col
             self.materials[m] = mat
+
         return self.materials[m]
 
     def add_polygon(self,
                     hull: Iterable[Tuple[int, int]],
                     holes: Iterable[Iterable[Tuple[int, int]]],
                     z_offset: float,
                     thickness: float,
@@ -73,50 +79,59 @@
         #  Create edge list for hull and create object
         edges = [[i, i + 1] for i in range(len(hull) - 1)]
         edges.append([len(hull) - 1, 0])
 
         index = next(self.counter)
 
         object_name_hull = "hull_{}".format(index)
+        bpy.ops.object.select_all(action="DESELECT")
+
 
         mesh = bpy.data.meshes.new(object_name_hull)
         mesh.from_pydata(hull, edges, faces=[])
+
         obj = bpy.data.objects.new(object_name_hull, mesh)
         scene = bpy.context.scene
-        scene.objects.link(obj)
+        scene.collection.objects.link(obj)
+        obj.select_set(True)
+
+        # Set material
+        obj.active_material = self.get_blender_material(material)
+       
 
         #  Create edge list for holes and create object
         for i, hole in enumerate(holes):
             object_name_hole = "hole.{}.{}".format(index, i)
             edges = [[i, i + 1] for i in range(len(hole) - 1)]
             edges.append([len(hole) - 1, 0])
             mesh = bpy.data.meshes.new(object_name_hole)
             mesh.from_pydata(hole, edges, faces=[])
             obj = bpy.data.objects.new(object_name_hole, mesh)
-            scene.objects.link(obj)
+            scene.collection.objects.link(obj)
+            obj.select_set(True)
+        
+        bpy.context.view_layer.objects.active = bpy.data.objects[object_name_hull]
+
+        # Join all objects (if needed)
+        if len(holes) > 0:
+            bpy.ops.object.join()
 
-        # Join all objects
-        # bpy.ops.object.select_all(action='TOGGLE')
-        bpy.context.scene.objects.active = bpy.data.objects[object_name_hull]
-        bpy.ops.object.join()
         #  Create faces using fill command
         bpy.ops.object.editmode_toggle()
         bpy.ops.mesh.fill()
         bpy.ops.mesh.select_mode(type='FACE')
         bpy.ops.mesh.select_all(action='SELECT')
 
         #  Extrude faces
         bpy.ops.mesh.extrude_region_move(
             TRANSFORM_OT_translate={"value": (0, 0, thickness)}
         )
 
         bpy.ops.object.editmode_toggle()
-
-        # Set material
-        obj.active_material = self.get_blender_material(material)
+        
 
         return obj
 
     def scale(self, f: float):
         self.scale_factor = f
 
     def translate(self, t: Tuple[float, float, float]):
```

### Comparing `gds3xtrude-0.0.8/gds3xtrude/blender_extrusion_example.py` & `gds3xtrude-0.0.9/gds3xtrude/blender_extrusion_example.py`

 * *Files identical despite different names*

### Comparing `gds3xtrude-0.0.8/gds3xtrude/blender_test.py` & `gds3xtrude-0.0.9/gds3xtrude/blender_test.py`

 * *Files identical despite different names*

### Comparing `gds3xtrude-0.0.8/gds3xtrude/builder.py` & `gds3xtrude-0.0.9/gds3xtrude/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,17 @@
         :param f:
         :return:
         """
         pass
 
 
 class ApproximateLayerStackBuilder(LayerStackBuilder):
+    """
+    Wraps any `LayerStackBuilder` by approximating and simplifying all polygons first before passing them to the builder.
+    """
 
     def __init__(self, layer_stack_builder: LayerStackBuilder, approx_error: float
                  ):
         self.builder = layer_stack_builder
         self.approx_error = approx_error
 
     def add_region(self, region: pya.Region,
```

### Comparing `gds3xtrude-0.0.8/gds3xtrude/gds3xtrude.py` & `gds3xtrude-0.0.9/gds3xtrude/gds3xtrude.py`

 * *Files identical despite different names*

### Comparing `gds3xtrude-0.0.8/gds3xtrude/include.py` & `gds3xtrude-0.0.9/gds3xtrude/include.py`

 * *Files identical despite different names*

### Comparing `gds3xtrude-0.0.8/gds3xtrude/layer_operations.py` & `gds3xtrude-0.0.9/gds3xtrude/layer_operations.py`

 * *Files identical despite different names*

### Comparing `gds3xtrude-0.0.8/gds3xtrude/openscad.py` & `gds3xtrude-0.0.9/gds3xtrude/openscad.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         if len(holes) > 0:
             solid_poly = difference()(solid_hull, *solid_holes)
         else:
             solid_poly = solid_hull
 
         volume = linear_extrude(thickness)(solid_poly)
         volume = utils.up(z_offset)(volume)
-        volume = utils.color(material.getattr('color', DEFAULT_COLOR))(volume)
+        volume = color(material.getattr('color', DEFAULT_COLOR))(volume)
 
         self.volumes.append(volume)
 
     def scale(self, f: float):
         self.scale_factor = f
 
     def translate(self, t: Tuple[float, float, float]):
```

### Comparing `gds3xtrude-0.0.8/gds3xtrude/polygon_approx.py` & `gds3xtrude-0.0.9/gds3xtrude/polygon_approx.py`

 * *Files identical despite different names*

### Comparing `gds3xtrude-0.0.8/gds3xtrude/types.py` & `gds3xtrude-0.0.9/gds3xtrude/types.py`

 * *Files identical despite different names*

### Comparing `gds3xtrude-0.0.8/gds3xtrude.egg-info/PKG-INFO` & `gds3xtrude-0.0.9/gds3xtrude.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gds3xtrude
-Version: 0.0.8
+Version: 0.0.9
 Summary: 3D GDS viewer based on OpenSCAD
 Home-page: https://codeberg.org/tok/gds3xtrude
 Author: T. Kramer
 Author-email: code@tkramer.ch
 License: AGPL
 Description: # gds3xtrude
         A simple layout to 3D converter.
@@ -129,14 +129,15 @@
         
         ## Blender
         3D models can also be generated in blender. Use the command line tool for this:
         ```sh
         gds3xtrude --tech freepdk45.layerstack --input NAND2X1.gds --cad blender
         ```
         Note that the current implementation over the Blender scripting API is very slow and therefore only small things such as standard cells can be visualized.
+        Also make sure to use Blender 2.82 or higher.
         
         ## FreeCAD
         The generated OpenSCAD models (.scad) can be imported into FreeCAD.
         
         ### Color Issue
         When applying a boolean union FreeCAD strips away colors. Therefore an exported .obj model will by totally gray. There is a workaround:
         * Open the OpenSCAD model in FreeCAD
```

### Comparing `gds3xtrude-0.0.8/gds3xtrude.egg-info/SOURCES.txt` & `gds3xtrude-0.0.9/gds3xtrude.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gds3xtrude-0.0.8/setup.py` & `gds3xtrude-0.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
 
 setup(name='gds3xtrude',
-      version='0.0.8',
+      version='0.0.9',
       description='3D GDS viewer based on OpenSCAD',
       long_description=readme(),
       long_description_content_type="text/markdown",
       keywords='gds openscad 3d viewer layout klayout',
       classifiers=[
           'License :: OSI Approved :: GNU Affero General Public License v3',
           'Development Status :: 3 - Alpha',
```

