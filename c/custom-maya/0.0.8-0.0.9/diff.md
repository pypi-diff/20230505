# Comparing `tmp/custom_maya-0.0.8.tar.gz` & `tmp/custom_maya-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_maya-0.0.8.tar", max compression
+gzip compressed data, was "custom_maya-0.0.9.tar", max compression
```

## Comparing `custom_maya-0.0.8.tar` & `custom_maya-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      107 2023-02-02 14:21:58.479991 custom_maya-0.0.8/custom_maya/__init__.py
--rw-r--r--   0        0        0      843 2023-02-03 01:52:36.614006 custom_maya-0.0.8/custom_maya/async_functions.py
--rw-r--r--   0        0        0      723 2023-02-02 14:12:12.352027 custom_maya-0.0.8/custom_maya/base_function.py
--rw-r--r--   0        0        0       25 2023-01-24 13:41:50.464689 custom_maya-0.0.8/custom_maya/customclass/__init__.py
--rw-r--r--   0        0        0      175 2023-01-27 13:24:51.656169 custom_maya-0.0.8/custom_maya/customclass/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5081 2023-02-04 13:03:31.514132 custom_maya-0.0.8/custom_maya/customclass/__pycache__/base_class.cpython-39.pyc
--rw-r--r--   0        0        0     3960 2023-02-04 07:49:29.341140 custom_maya-0.0.8/custom_maya/customclass/base_class.py
--rw-r--r--   0        0        0        0 2023-01-24 12:50:11.626618 custom_maya-0.0.8/custom_maya/functions.py
--rw-r--r--   0        0        0     1679 2023-01-27 04:20:58.986367 custom_maya-0.0.8/custom_maya/test_open_scene.py
--rw-r--r--   0        0        0        0 2023-01-24 12:49:46.715105 custom_maya-0.0.8/custom_maya/tools/__init__.py
--rw-r--r--   0        0        0     3841 2023-02-04 13:45:36.236188 custom_maya-0.0.8/custom_maya/tools/get_scene_evaluate.py
--rw-r--r--   0        0        0     1091 2023-01-25 12:34:04.811797 custom_maya-0.0.8/LICENSE
--rw-r--r--   0        0        0      492 2023-02-04 13:51:03.086588 custom_maya-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1529 2023-02-04 13:46:31.373757 custom_maya-0.0.8/README.md
--rw-r--r--   0        0        0     2212 1970-01-01 00:00:00.000000 custom_maya-0.0.8/setup.py
--rw-r--r--   0        0        0     1974 1970-01-01 00:00:00.000000 custom_maya-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      107 2023-02-04 13:49:52.177168 custom_maya-0.0.9/custom_maya/__init__.py
+-rw-r--r--   0        0        0      843 2023-02-04 13:49:52.177168 custom_maya-0.0.9/custom_maya/async_functions.py
+-rw-r--r--   0        0        0      723 2023-02-04 13:49:52.178166 custom_maya-0.0.9/custom_maya/base_function.py
+-rw-r--r--   0        0        0       25 2023-01-28 13:10:28.506458 custom_maya-0.0.9/custom_maya/customclass/__init__.py
+-rw-r--r--   0        0        0      193 2023-02-05 11:59:36.462334 custom_maya-0.0.9/custom_maya/customclass/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5904 2023-02-05 11:59:36.466308 custom_maya-0.0.9/custom_maya/customclass/__pycache__/base_class.cpython-39.pyc
+-rw-r--r--   0        0        0     4892 2023-02-05 11:58:26.330703 custom_maya-0.0.9/custom_maya/customclass/base_class.py
+-rw-r--r--   0        0        0        0 2023-01-28 13:10:28.507455 custom_maya-0.0.9/custom_maya/functions.py
+-rw-r--r--   0        0        0     1679 2023-01-28 13:25:51.052235 custom_maya-0.0.9/custom_maya/test_open_scene.py
+-rw-r--r--   0        0        0        0 2023-01-28 13:10:28.508930 custom_maya-0.0.9/custom_maya/tools/__init__.py
+-rw-r--r--   0        0        0     3886 2023-02-05 12:06:40.145808 custom_maya-0.0.9/custom_maya/tools/get_scene_evaluate.py
+-rw-r--r--   0        0        0     1091 2023-01-28 13:10:28.503689 custom_maya-0.0.9/LICENSE
+-rw-r--r--   0        0        0      506 2023-02-05 12:07:59.271599 custom_maya-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1529 2023-02-04 13:52:29.775599 custom_maya-0.0.9/README.md
+-rw-r--r--   0        0        0     2224 1970-01-01 00:00:00.000000 custom_maya-0.0.9/setup.py
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 custom_maya-0.0.9/PKG-INFO
```

### Comparing `custom_maya-0.0.8/custom_maya/async_functions.py` & `custom_maya-0.0.9/custom_maya/async_functions.py`

 * *Files identical despite different names*

### Comparing `custom_maya-0.0.8/custom_maya/base_function.py` & `custom_maya-0.0.9/custom_maya/base_function.py`

 * *Files identical despite different names*

### Comparing `custom_maya-0.0.8/custom_maya/customclass/base_class.py` & `custom_maya-0.0.9/custom_maya/customclass/base_class.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 
+import maya.OpenMaya as om
 import maya.cmds as cmds
 
 
 class CustomObjectBase(object):
     def __init__(self):
         # 储存所有属性的字典
         self.__custom_properties = {}
@@ -79,33 +80,56 @@
             **{
                 'HasSameTransform': self.has_same_name_transform(),
                 'HasSameJoint': self.has_same_name_joint(),
             },
             **self.get_blendshape_evaluate(),
         }
 
-    @staticmethod
-    def get_poly_evaluate():
+    def get_poly_evaluate(self):
         __meshes = cmds.ls(type='mesh')
         return {
             'Verts': cmds.polyEvaluate(__meshes, vertex=True) if len(__meshes) > 0 else 0,
             'Edges': cmds.polyEvaluate(__meshes, edge=True) if len(__meshes) > 0 else 0,
             'Faces': cmds.polyEvaluate(__meshes, face=True) if len(__meshes) > 0 else 0,
             'Tris': cmds.polyEvaluate(__meshes, triangle=True) if len(__meshes) > 0 else 0,
             'UVs': cmds.polyEvaluate(__meshes, uv=True) if len(__meshes) > 0 else 0,
+            'Ngons': len(self.get_objects_with_more_than_4_sides_long_list())
         }
 
-    @staticmethod
-    def get_joint_evaluate():
+    def get_objects_with_more_than_4_sides_long_list(self):
+        cmds.select(cmds.ls(type='mesh'))
+        sel = om.MSelectionList()
+        om.MGlobal.getActiveSelectionList(sel)
+        poly_objects = []
+
+        for i in range(sel.length()):
+            m_obj = om.MObject()
+            sel.getDependNode(i, m_obj)
+
+            if m_obj.hasFn(om.MFn.kMesh):
+                dag_path = om.MDagPath()
+                sel.getDagPath(i, dag_path)
+                poly = om.MFnMesh(dag_path)
+
+                for j in range(poly.numPolygons()):
+                    vertices = om.MIntArray()
+                    poly.getPolygonVertices(j, vertices)
+
+                    if len(vertices) > 4:
+                        poly_objects.append(dag_path.fullPathName())
+                        break
+        cmds.select(cl=True)
+        return poly_objects
+
+    def get_joint_evaluate(self):
         return {
             'Joints': len(cmds.ls(type='joint'))
         }
 
-    @staticmethod
-    def get_blendshape_evaluate():
+    def get_blendshape_evaluate(self):
         blend_shapes = cmds.ls(type='blendShape')
         morph_target_counter = 0
         for bs in blend_shapes:
             morph_target_counter += cmds.blendShape(bs, query=True, weightCount=True)
         return {
             'BlendShapes': len(blend_shapes),
             'MorphTargets': morph_target_counter
@@ -123,9 +147,7 @@
         for i in cmds.ls(type='transform'):
             if '|' in i:
                 return True
         return False
 
     def func(self):
         pass
-
-
```

### Comparing `custom_maya-0.0.8/custom_maya/test_open_scene.py` & `custom_maya-0.0.9/custom_maya/test_open_scene.py`

 * *Files identical despite different names*

### Comparing `custom_maya-0.0.8/custom_maya/tools/get_scene_evaluate.py` & `custom_maya-0.0.9/custom_maya/tools/get_scene_evaluate.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,26 +19,26 @@
     @classmethod
     def check_maya_path(cls, paths):
         res = []
         for i in paths:
             if not os.path.exists(i):
                 res.append(i)
 
-
     @classmethod
     def check_excel_path(cls, path):
         try:
             pd.DataFrame([{}]).to_excel(path, index=False)
         except PermissionError:
             raise PermissionError('请关闭所要保存的Excel文件')
             return
         except FileNotFoundError:
             raise FileNotFoundError('你输入的保存Excel文件的路径时错误的')
             return
         except Exception as e:
+            print(e)
             raise Exception('你输入的保存Excel文件的路径时错误的，请重新输入正确的文件名')
 
     @classmethod
     def export_data(cls, excel_path):
         df = pd.DataFrame(cls.all_data)
         temp_path = os.path.join(os.path.expanduser('~'), 'custom_maya_get_scene_evaluate_temp.xlsx')
         try:
@@ -92,21 +92,20 @@
 
 
 def get_scene_evaluate(file_paths=[], export_to_excel_path=None):
     # start_time = time.time()
     mf = MyFuncClass()
     MyFuncClass.check_excel_path(export_to_excel_path)
 
-
     # root_dir:你的Maya场景所在的根目录地址,并获取此目录下的所有Maya文件地址。
     # file_paths = get_file_path_list(root_dir=r'D:\test_scenes')
 
     # 执行程序
     asyncio.run(async_scene(file_paths, mf))
     if export_to_excel_path:
         MyFuncClass.export_data(export_to_excel_path)
     # print(f'程序运行了{time.time() - start_time}')
 
 
-# if __name__ == '__main__':
-#     get_scene_evaluate(export_to_excel_path=r'd:\test\scene_file.xlsx',
-#                        file_paths=get_file_path_list(r'd:/test_scenes'))
+if __name__ == '__main__':
+    get_scene_evaluate(export_to_excel_path=os.path.join(os.path.expanduser("~"), 'test.xlsx'),
+                       file_paths=get_file_path_list(r'C:\temp\maya_test_files'))
```

### Comparing `custom_maya-0.0.8/LICENSE` & `custom_maya-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_maya-0.0.8/README.md` & `custom_maya-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `custom_maya-0.0.8/setup.py` & `custom_maya-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['custom_maya', 'custom_maya.customclass', 'custom_maya.tools']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['custom_maya', 'pandas']
+['custom_maya', 'openpyxl', 'pandas']
 
 setup_kwargs = {
     'name': 'custom-maya',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Maya的便利工具',
     'long_description': '# 项目说明\n\n此工具内含各种实用工具。**仅为测试用！！！**\n\n仅支持Maya2023及以上版本。\n\n\n参照\n* [如何使用mayapy运行venv](https://knowledge.autodesk.com/zh-hans/support/maya/learn-explore/caas/CloudHelp/cloudhelp/2023/CHS/Maya-Scripting/files/GUID-6AF99E9C-1473-481E-A144-357577A53717-htm.html)\n* [Maya Python 解释器 mayapy](https://knowledge.autodesk.com/zh-hans/support/maya/learn-explore/caas/CloudHelp/cloudhelp/2023/CHS/Maya-Scripting/files/GUID-D64ACA64-2566-42B3-BE0F-BCE843A1702F-htm.html)\n\n\n## 安装并获取更新\n\n使用 pip 安装\n```shell\npip install custom-maya\n```\n\n需要使用 mayapy 环境安装。\n\n测试用\n```shell\nXcopy custom_maya "C:\\Program Files\\Autodesk\\Maya2023\\Python\\Lib\\site-packages\\custom_maya" /E/H/C/I\n```\n\n\n## 如何设置IDE\n\n\n### 制作从名为 python 的命令创建指向 mayapy 的软链接\n\n```shell\ncd "C:\\Program Files\\Autodesk\\Maya2023\\bin"\nmklink python.exe mayapy.exe\n```\n\n### 将IDE的解释器设置为\n```\n"C:\\Program Files\\Autodesk\\Maya2023\\bin\\python.exe"\n```\n\n\n\n\n## 例子\n\n### 获取某根目录下所有Maya文件的信息\n\n```python\n\n```\n\n\n\n\n\n## 打包上传到pipy\n\n升级\n```shell\npython.exe -m pip install --upgrade build\npython.exe -m pip install --upgrade pip\n```\n\n```shell\npython -m build\n```\n\n上传测试包\n```shell\npython -m twine upload --repository testpypi dist/*\n```\n\n\n上传正式版本包\n```shell\npython -m twine upload dist/*\n```\n\n',
     'author': 'Yuanzhen Qiao',
     'author_email': 'narutozbjp@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `custom_maya-0.0.8/PKG-INFO` & `custom_maya-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: custom-maya
-Version: 0.0.8
+Version: 0.0.9
 Summary: Maya的便利工具
 Author: Yuanzhen Qiao
 Author-email: narutozbjp@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: custom_maya
+Requires-Dist: openpyxl
 Requires-Dist: pandas
 Project-URL: Homepage, https://github.com/narutozb/custom_maya
 Description-Content-Type: text/markdown
 
 # 项目说明
 
 此工具内含各种实用工具。**仅为测试用！！！**
```

