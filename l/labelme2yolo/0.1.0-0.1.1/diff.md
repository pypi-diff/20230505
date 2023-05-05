# Comparing `tmp/labelme2yolo-0.1.0.tar.gz` & `tmp/labelme2yolo-0.1.1.tar.gz`

## Comparing `labelme2yolo-0.1.0.tar` & `labelme2yolo-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 labelme2yolo-0.1.0/requirements.txt
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 labelme2yolo-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 labelme2yolo-0.1.0/src/labelme2yolo/__about__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 labelme2yolo-0.1.0/src/labelme2yolo/__init__.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 labelme2yolo-0.1.0/src/labelme2yolo/__main__.py
--rw-r--r--   0        0        0    11887 2020-02-02 00:00:00.000000 labelme2yolo-0.1.0/src/labelme2yolo/l2y.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 labelme2yolo-0.1.0/src/labelme2yolo/cli/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 labelme2yolo-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 labelme2yolo-0.1.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 labelme2yolo-0.1.0/LICENSE
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 labelme2yolo-0.1.0/README.md
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 labelme2yolo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4858 2020-02-02 00:00:00.000000 labelme2yolo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/src/labelme2yolo/__about__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/src/labelme2yolo/__init__.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/src/labelme2yolo/__main__.py
+-rw-r--r--   0        0        0    12806 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/src/labelme2yolo/l2y.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/src/labelme2yolo/cli/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3840 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/README.md
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 labelme2yolo-0.1.1/PKG-INFO
```

### Comparing `labelme2yolo-0.1.0/src/labelme2yolo/l2y.py` & `labelme2yolo-0.1.1/src/labelme2yolo/l2y.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
         with io.BytesIO() as f_in:
             img.save(f_in, "PNG")
             f_in.seek(0)
             return f_in.read()
 
 
-def get_label_id_map(json_dir):
+def get_label_id_map(json_dir: str):
     label_set = set()
 
     for file_name in os.listdir(json_dir):
         if file_name.endswith("json"):
             json_path = os.path.join(json_dir, file_name)
             data = json.load(open(json_path))
             for shape in data["shapes"]:
@@ -114,32 +114,47 @@
         for yolo_obj in yolo_obj_list:
             label, points = yolo_obj
             points = [str(item) for item in points]
             yolo_obj_line = f"{label} {' '.join(points)}\n"
             f.write(yolo_obj_line)
 
 
-def save_yolo_image(json_data, json_name, image_dir_path, target_dir):
+def save_yolo_image(json_data, json_path, image_dir_path, target_dir):
+    json_name = os.path.basename(json_path)
     img_name = json_name.replace(".json", ".png")
+
+    # make image_path and save image
     img_path = os.path.join(image_dir_path, target_dir, img_name)
 
-    if not os.path.exists(img_path):
+    if json_data["imageData"] is None:
+        dirname = os.path.dirname(json_path)
+        image_name = json_data["imagePath"]
+        src_image_name = os.path.join(dirname, image_name)
+        src_image = cv2.imread(src_image_name)
+        cv2.imwrite(img_path, src_image)
+    else:
         img = img_b64_to_arr(json_data["imageData"])
         PIL.Image.fromarray(img).save(img_path)
 
     return img_path
 
 
 class Labelme2YOLO(object):
 
-    def __init__(self, json_dir, output_format):
+    def __init__(self, json_dir, output_format, label_list):
         self._json_dir = json_dir
         self._output_format = output_format
+        self._label_list = label_list
 
-        self._label_id_map = get_label_id_map(self._json_dir)
+        if label_list:
+            self._label_id_map = {label: label_id
+                                  for label_id, label in enumerate(label_list)}
+        else:
+            self._label_id_map = get_label_id_map(self._json_dir)
+            self._label_list = [label for label in self._label_id_map.keys()]
 
     def _make_train_val_dir(self):
         self._label_dir_path = os.path.join(self._json_dir,
                                             'YOLODataset/labels/')
         self._image_dir_path = os.path.join(self._json_dir,
                                             'YOLODataset/images/')
 
@@ -218,15 +233,15 @@
         json_path = os.path.join(self._json_dir, json_name)
         json_data = json.load(open(json_path))
 
         print('Converting %s for %s ...' %
               (json_name, target_dir.replace('/', '')))
 
         img_path = save_yolo_image(json_data,
-                                   json_name,
+                                   json_path,
                                    self._image_dir_path,
                                    target_dir)
         yolo_obj_list = self._get_yolo_object_list(json_data, img_path)
         save_yolo_label(json_name,
                         self._label_dir_path,
                         target_dir,
                         yolo_obj_list)
@@ -271,30 +286,37 @@
         obj_h = 2 * radius
 
         yolo_center_x = round(float(obj_center_x / img_w), 6)
         yolo_center_y = round(float(obj_center_y / img_h), 6)
         yolo_w = round(float(obj_w / img_w), 6)
         yolo_h = round(float(obj_h / img_h), 6)
 
-        label_id = self._label_id_map[shape['label']]
+        if shape['label'] in self._label_id_map:
+            label_id = self._label_id_map[shape['label']]
+        else:
+            print('label %s not in %s' % shape['label'], self._label_list)
 
         return label_id, yolo_center_x, yolo_center_y, yolo_w, yolo_h
 
     def _get_other_shape_yolo_object(self, shape, img_h, img_w):
 
         point_list = shape['points']
         points = np.zeros(2 * len(point_list))
         points[::2] = [float(point[0]) / img_w for point in point_list]
         points[1::2] = [float(point[1]) / img_h for point in point_list]
         if len(points) == 4:
             if self._output_format == "polygon":
                 points = extend_point_list(points)
             if self._output_format == "bbox":
                 points = extend_point_list(points, "bbox")
-        label_id = self._label_id_map[shape['label']]
+
+        if shape['label'] in self._label_id_map:
+            label_id = self._label_id_map[shape['label']]
+        else:
+            print('label %s not in %s' % shape['label'], self._label_list)
 
         return label_id, points.tolist()
 
     def _save_dataset_yaml(self):
         yaml_path = os.path.join(
             self._json_dir, 'YOLODataset/', 'dataset.yaml')
```

### Comparing `labelme2yolo-0.1.0/src/labelme2yolo/cli/__init__.py` & `labelme2yolo-0.1.1/src/labelme2yolo/cli/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,22 +35,31 @@
     parser.add_argument(
         "--output_format",
         type=str,
         default="polygon",
         help='The default output format for labelme2yolo is "polygon".'
         ' However, you can choose to output in bbox format by specifying the "bbox" option.',
     )
+    parser.add_argument(
+        "--label_list",
+        type=str,
+        nargs="+",
+        default=None,
+        help="The ordered label list, for example --label_list cat dog",
+        required=False,
+    )
 
     args = parser.parse_args()
 
     if not args.json_dir:
         parser.print_help()
         return 0
 
-    convertor = Labelme2YOLO(args.json_dir, args.output_format)
+    convertor = Labelme2YOLO(
+        args.json_dir, args.output_format, args.label_list)
 
     if args.json_name is None:
         convertor.convert(val_size=args.val_size, test_size=args.test_size)
     else:
         convertor.convert_one(args.json_name)
 
     return 0
```

### Comparing `labelme2yolo-0.1.0/.gitignore` & `labelme2yolo-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `labelme2yolo-0.1.0/LICENSE` & `labelme2yolo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `labelme2yolo-0.1.0/README.md` & `labelme2yolo-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 **--test\_size (Optional)** Test dataset size, for example 0.2 means 20% for Test.
 
 **--json\_name (Optional)** Convert single LabelMe JSON file.
 
 **--output\_format (Optional)** The output format of label.
 
+**--label\_list (Optional)** The pre-assigned category labels.
+
 ## How to Use
 
 ### 1. Convert JSON files, split training, validation and test dataset by --val\_size and --test\_size
 
 Put all LabelMe JSON files under **labelme\_json\_dir**, and run this python command.
 
 ```bash
```

### Comparing `labelme2yolo-0.1.0/pyproject.toml` & `labelme2yolo-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "opencv-python>=4.1.2",
-  "Pillow>=9.2,<9.5",
+  "Pillow>=9.2,<9.6",
   "scikit-learn>=1.1.1,<1.3.0",
   "numpy>=1.23.1,<1.25.0"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/greatv/labelme2yolo#readme"
```

### Comparing `labelme2yolo-0.1.0/PKG-INFO` & `labelme2yolo-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labelme2yolo
-Version: 0.1.0
+Version: 0.1.1
 Summary: This script converts the JSON format output by LabelMe to the text format required by YOLO serirs.
 Project-URL: Documentation, https://github.com/greatv/labelme2yolo#readme
 Project-URL: Issues, https://github.com/greatv/labelme2yolo/issues
 Project-URL: Source, https://github.com/greatv/labelme2yolo
 Author-email: "GreatV(Wang Xin)" <xinwang614@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: numpy<1.25.0,>=1.23.1
 Requires-Dist: opencv-python>=4.1.2
-Requires-Dist: pillow<9.5,>=9.2
+Requires-Dist: pillow<9.6,>=9.2
 Requires-Dist: scikit-learn<1.3.0,>=1.1.1
 Description-Content-Type: text/markdown
 
 # Labelme2YOLO
 
 **Forked from [rooneysh/Labelme2YOLO](https://github.com/rooneysh/Labelme2YOLO)**
 
@@ -53,14 +53,16 @@
 
 **--test\_size (Optional)** Test dataset size, for example 0.2 means 20% for Test.
 
 **--json\_name (Optional)** Convert single LabelMe JSON file.
 
 **--output\_format (Optional)** The output format of label.
 
+**--label\_list (Optional)** The pre-assigned category labels.
+
 ## How to Use
 
 ### 1. Convert JSON files, split training, validation and test dataset by --val\_size and --test\_size
 
 Put all LabelMe JSON files under **labelme\_json\_dir**, and run this python command.
 
 ```bash
```

