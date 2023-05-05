# Comparing `tmp/transtab-0.0.4.tar.gz` & `tmp/transtab-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transtab-0.0.4.tar", last modified: Tue Apr 25 15:32:20 2023, max compression
+gzip compressed data, was "transtab-0.0.5.tar", last modified: Fri May  5 02:50:40 2023, max compression
```

## Comparing `transtab-0.0.4.tar` & `transtab-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 15:32:20.000000 transtab-0.0.4/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1316 2022-08-23 14:54:33.000000 transtab-0.0.4/LICENSE
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5145 2023-04-25 15:32:20.000000 transtab-0.0.4/PKG-INFO
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4475 2023-02-03 17:30:10.000000 transtab-0.0.4/README.md
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       38 2023-04-25 15:32:20.000000 transtab-0.0.4/setup.cfg
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1202 2023-04-25 15:31:30.000000 transtab-0.0.4/setup.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 15:32:20.000000 transtab-0.0.4/transtab/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       61 2023-04-25 15:30:33.000000 transtab-0.0.4/transtab/__init__.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      368 2022-08-31 18:57:31.000000 transtab-0.0.4/transtab/constants.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    10943 2022-08-31 18:28:18.000000 transtab-0.0.4/transtab/dataset.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5835 2023-02-03 17:30:10.000000 transtab-0.0.4/transtab/evaluator.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    50323 2023-02-03 17:47:03.000000 transtab-0.0.4/transtab/modeling_transtab.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13825 2023-02-03 17:54:22.000000 transtab-0.0.4/transtab/trainer.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7764 2022-08-26 01:52:18.000000 transtab-0.0.4/transtab/trainer_utils.py
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15248 2022-09-05 21:13:13.000000 transtab-0.0.4/transtab/transtab.py
-drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-04-25 15:32:20.000000 transtab-0.0.4/transtab.egg-info/
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5145 2023-04-25 15:32:20.000000 transtab-0.0.4/transtab.egg-info/PKG-INFO
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      367 2023-04-25 15:32:20.000000 transtab-0.0.4/transtab.egg-info/SOURCES.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        1 2023-04-25 15:32:20.000000 transtab-0.0.4/transtab.egg-info/dependency_links.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       84 2023-04-25 15:32:20.000000 transtab-0.0.4/transtab.egg-info/requires.txt
--rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        9 2023-04-25 15:32:20.000000 transtab-0.0.4/transtab.egg-info/top_level.txt
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-05-05 02:50:40.466778 transtab-0.0.5/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1316 2023-05-04 23:36:05.000000 transtab-0.0.5/LICENSE
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5200 2023-05-05 02:50:40.466778 transtab-0.0.5/PKG-INFO
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     4530 2023-05-05 02:45:26.000000 transtab-0.0.5/README.md
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       38 2023-05-05 02:50:40.466778 transtab-0.0.5/setup.cfg
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     1202 2023-05-05 02:44:55.000000 transtab-0.0.5/setup.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-05-05 02:50:40.465778 transtab-0.0.5/transtab/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       61 2023-05-05 02:50:18.000000 transtab-0.0.5/transtab/__init__.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      368 2023-05-04 23:36:05.000000 transtab-0.0.5/transtab/constants.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    12408 2023-05-05 02:49:22.000000 transtab-0.0.5/transtab/dataset.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5891 2023-05-05 00:08:24.000000 transtab-0.0.5/transtab/evaluator.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    50349 2023-05-04 23:41:11.000000 transtab-0.0.5/transtab/modeling_transtab.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    13825 2023-05-04 23:38:57.000000 transtab-0.0.5/transtab/trainer.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     7764 2023-05-04 23:36:05.000000 transtab-0.0.5/transtab/trainer_utils.py
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)    15248 2023-05-04 23:36:05.000000 transtab-0.0.5/transtab/transtab.py
+drwxrwxr-x   0 zifengw2 (1163739) zifengw2 (1163739)        0 2023-05-05 02:50:40.466778 transtab-0.0.5/transtab.egg-info/
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)     5200 2023-05-05 02:50:40.000000 transtab-0.0.5/transtab.egg-info/PKG-INFO
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)      367 2023-05-05 02:50:40.000000 transtab-0.0.5/transtab.egg-info/SOURCES.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        1 2023-05-05 02:50:40.000000 transtab-0.0.5/transtab.egg-info/dependency_links.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)       84 2023-05-05 02:50:40.000000 transtab-0.0.5/transtab.egg-info/requires.txt
+-rw-rw-r--   0 zifengw2 (1163739) zifengw2 (1163739)        9 2023-05-05 02:50:40.000000 transtab-0.0.5/transtab.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `transtab-0.0.4/LICENSE` & `transtab-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `transtab-0.0.4/PKG-INFO` & `transtab-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transtab
-Version: 0.0.4
+Version: 0.0.5
 Summary: A flexible tabular prediction model that handles variable-column input tables.
 Home-page: https://github.com/RyanWangZf/transtab
 Author: Zifeng Wang
 Author-email: zifengw2@illinois.edu
 Keywords: tabular data,machine learning,data mining,data science
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -30,14 +30,16 @@
 Document is available at https://transtab.readthedocs.io/en/latest/index.html.
 
 Paper is available at https://arxiv.org/pdf/2205.09328.pdf.
 
 5 min blog to understand TransTab at [realsunlab.medium.com](https://realsunlab.medium.com/transtab-learning-transferable-tabular-transformers-across-tables-1e34eec161b8)!
 
 ### News!
+- [05/04/23] Check the version `0.0.5` of `TransTab`!
+
 - [01/04/23] Check the version `0.0.3` of `TransTab`!
 
 - [12/03/22] Check out our [[blog]](https://realsunlab.medium.com/transtab-learning-transferable-tabular-transformers-across-tables-1e34eec161b8) for a quick understanding of TransTab!
 
 - [08/31/22] `0.0.2` Support encode tabular inputs into embeddings directly. An example is provided [here](examples/table_embedding.ipynb). Several bugs are fixed.
 
 ## TODO
```

### Comparing `transtab-0.0.4/README.md` & `transtab-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 Document is available at https://transtab.readthedocs.io/en/latest/index.html.
 
 Paper is available at https://arxiv.org/pdf/2205.09328.pdf.
 
 5 min blog to understand TransTab at [realsunlab.medium.com](https://realsunlab.medium.com/transtab-learning-transferable-tabular-transformers-across-tables-1e34eec161b8)!
 
 ### News!
+- [05/04/23] Check the version `0.0.5` of `TransTab`!
+
 - [01/04/23] Check the version `0.0.3` of `TransTab`!
 
 - [12/03/22] Check out our [[blog]](https://realsunlab.medium.com/transtab-learning-transferable-tabular-transformers-across-tables-1e34eec161b8) for a quick understanding of TransTab!
 
 - [08/31/22] `0.0.2` Support encode tabular inputs into embeddings directly. An example is provided [here](examples/table_embedding.ipynb). Several bugs are fixed.
 
 ## TODO
```

### Comparing `transtab-0.0.4/setup.py` & `transtab-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # read the contents of requirements.txt
 with open(os.path.join(this_directory, 'requirements.txt'),
           encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name = 'transtab',
-    version = '0.0.4',
+    version = '0.0.5',
     author = 'Zifeng Wang',
     author_email = 'zifengw2@illinois.edu',
     description = 'A flexible tabular prediction model that handles variable-column input tables.',
     url = 'https://github.com/RyanWangZf/transtab',
     keywords=['tabular data', 'machine learning', 'data mining', 'data science'],
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `transtab-0.0.4/transtab/dataset.py` & `transtab-0.0.5/transtab/dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,29 @@
 # }
 
 
 OPENML_DATACONFIG = {
     'credit-g': {'bin': ['own_telephone', 'foreign_worker']},
 }
 
+EXAMPLE_DATACONFIG = {
+    "example": {
+        "bin": ["bin1", "bin2"],
+        "cat": ["cat1", "cat2"],
+        "num": ["num1", "num2"],
+        "cols": ["bin1", "bin2", "cat1", "cat2", "num1", "num2"],
+        "binary_indicator": ["1", "yes", "true", "positive", "t", "y"],
+        "data_split_idx": {
+            "train":[0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
+            "val":[10, 11, 12, 13, 14, 15, 16, 17, 18, 19],
+            "test":[20, 21, 22, 23, 24, 25, 26, 27, 28, 29],
+        }
+    }
+}
+
 def load_data(dataname, dataset_config=None, encode_cat=False, data_cut=None, seed=123):
     '''Load datasets from the local device or from openml.datasets.
 
     Parameters
     ----------
     dataname: str or int
         the dataset name/index intended to be loaded from openml. or the directory to the local dataset.
@@ -72,16 +87,17 @@
     
     if isinstance(dataname, list):
         # load a list of datasets, combine together and outputs
         num_col_list, cat_col_list, bin_col_list = [], [], []
         all_list = []
         train_list, val_list, test_list = [], [], []
         for dataname_ in dataname:
+            data_config = dataset_config.get(dataname_, None)
             allset, trainset, valset, testset, cat_cols, num_cols, bin_cols = \
-                load_single_data(dataname_, dataset_config=dataset_config, encode_cat=encode_cat, data_cut=data_cut, seed=seed)
+                load_single_data(dataname_, dataset_config=data_config, encode_cat=encode_cat, data_cut=data_cut, seed=seed)
             num_col_list.extend(num_cols)
             cat_col_list.extend(cat_cols)
             bin_col_list.extend(bin_cols)
             all_list.append(allset)
             train_list.append(trainset)
             val_list.append(valset)
             test_list.append(testset)
@@ -97,15 +113,14 @@
         encode_cat:  Set `False` if we are using transtab, otherwise we set it True to encode categorical values into indexes.
         data_cut: The number of cuts of the training set. Cut is performed on both rows and columns.
     outputs:
         allset: (X,y) that contains all samples of this dataset
         trainset, valset, testset: the train/val/test split
         num_cols, cat_cols, bin_cols: the list of numerical/categorical/binary column names
     '''
-    if dataset_config is None: dataset_config = OPENML_DATACONFIG
     print('####'*10)
     if os.path.exists(dataname):
         print(f'load from local data dir {dataname}')
         filename = os.path.join(dataname, 'data_processed.csv')
         df = pd.read_csv(filename, index_col=0)
         y = df['target_label']
         X = df.drop(['target_label'],axis=1)
@@ -122,28 +137,27 @@
         if os.path.exists(bnfile):
             with open(bnfile,'r') as f: bin_cols = [x.strip().lower() for x in f.readlines()]
         else:
             bin_cols = []
         cat_cols = [col for col in all_cols if col not in num_cols and col not in bin_cols]
 
         # update cols by loading dataset_config
-        if dataname in dataset_config:
-            data_config = dataset_config[dataname]
-            if 'columns' in data_config:
-                new_cols = dataset_config[dataname]['columns']
+        if dataset_config is not None:
+            if 'columns' in dataset_config:
+                new_cols = dataset_config['columns']
                 X.columns = new_cols
 
-            if 'bin' in data_config:
-                bin_cols = data_config['bin']
+            if 'bin' in dataset_config:
+                bin_cols = dataset_config['bin']
             
-            if 'cat' in data_config:
-                cat_cols = data_config['cat']
+            if 'cat' in dataset_config:
+                cat_cols = dataset_config['cat']
 
-            if 'num' in data_config:
-                num_cols = data_config['num']
+            if 'num' in dataset_config:
+                num_cols = dataset_config['num']
         
     else:
         dataset = openml.datasets.get_dataset(dataname)
         X,y,categorical_indicator, attribute_names = dataset.get_data(dataset_format='dataframe', target=dataset.default_target_attribute)
         
         if isinstance(dataname, int):
             openml_list = openml.datasets.list_datasets(output_format="dataframe")  # returns a dict
@@ -159,16 +173,16 @@
 
         all_cols = np.array(attribute_names)
         categorical_indicator = np.array(categorical_indicator)
         cat_cols = [col for col in all_cols[categorical_indicator] if col not in drop_cols]
         num_cols = [col for col in all_cols[~categorical_indicator] if col not in drop_cols]
         all_cols = [col for col in all_cols if col not in drop_cols]
         
-        if dataname in dataset_config:
-            if 'bin' in dataset_config[dataname]: bin_cols = [c for c in cat_cols if c in dataset_config[dataname]['bin']]
+        if dataset_config is not None:
+            if 'bin' in dataset_config: bin_cols = [c for c in cat_cols if c in dataset_config['bin']]
         else: bin_cols = []
         cat_cols = [c for c in cat_cols if c not in bin_cols]
 
         # encode target label
         y = LabelEncoder().fit_transform(y.values)
         y = pd.Series(y,index=X.index)
 
@@ -184,47 +198,77 @@
         if encode_cat:
             X[cat_cols] = OrdinalEncoder().fit_transform(X[cat_cols])
         else:
             X[cat_cols] = X[cat_cols].astype(str)
 
     if len(bin_cols) > 0:
         for col in bin_cols: X[col].fillna(X[col].mode()[0], inplace=True)
-        if dataname in dataset_config:
-            if 'binary_indicator' in dataset_config[dataname]:
-                X[bin_cols] = X[bin_cols].astype(str).applymap(lambda x: 1 if x.lower() in dataset_config[dataname]['binary_indicator'] else 0).values
-            else:
-                X[bin_cols] = X[bin_cols].astype(str).applymap(lambda x: 1 if x.lower() in ['yes','true','1','t'] else 0).values        
+        if 'binary_indicator' in dataset_config:
+            X[bin_cols] = X[bin_cols].astype(str).applymap(lambda x: 1 if x.lower() in dataset_config['binary_indicator'] else 0).values
+        else:
+            X[bin_cols] = X[bin_cols].astype(str).applymap(lambda x: 1 if x.lower() in ['yes','true','1','t'] else 0).values        
+        
         # if no dataset_config given, keep its original format
+        # raise warning if there is not only 0/1 in the binary columns
+        if (~X[bin_cols].isin([0,1])).any().any():
+            raise ValueError(f'binary columns {bin_cols} contains values other than 0/1.')
+
     
     X = X[bin_cols + num_cols + cat_cols]
 
     # rename column names if is given
-    if dataname in dataset_config:
-        data_config = dataset_config[dataname]
+    if dataset_config is not None:
+        data_config = dataset_config
         if 'columns' in data_config:
             new_cols = data_config['columns']
             X.columns = new_cols
             attribute_names = new_cols
 
         if 'bin' in data_config:
             bin_cols = data_config['bin']
         
         if 'cat' in data_config:
             cat_cols = data_config['cat']
 
         if 'num' in data_config:
             num_cols = data_config['num']
 
+
     # split train/val/test
-    train_dataset, test_dataset, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=seed, stratify=y, shuffle=True)
-    val_size = int(len(y)*0.1)
-    val_dataset = train_dataset.iloc[-val_size:]
-    y_val = y_train[-val_size:]
-    train_dataset = train_dataset.iloc[:-val_size]
-    y_train = y_train[:-val_size]
+    data_split_idx = None
+    if dataset_config is not None:
+        data_split_idx = dataset_config.get('data_split_idx', None)
+
+    if data_split_idx is not None:
+        train_idx = data_split_idx.get('train', None)
+        val_idx = data_split_idx.get('val', None)
+        test_idx = data_split_idx.get('test', None)
+
+        if train_idx is None or test_idx is None:
+            raise ValueError('train/test split indices must be provided together')
+    
+        else:
+            train_dataset = X.iloc[train_idx]
+            y_train = y[train_idx]
+            test_dataset = X.iloc[test_idx]
+            y_test = y[test_idx]
+            if val_idx is not None:
+                val_dataset = X.iloc[val_idx]
+                y_val = y[val_idx]
+            else:
+                val_dataset = None
+                y_val = None
+    else:
+        # split train/val/test
+        train_dataset, test_dataset, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=seed, stratify=y, shuffle=True)
+        val_size = int(len(y)*0.1)
+        val_dataset = train_dataset.iloc[-val_size:]
+        y_val = y_train[-val_size:]
+        train_dataset = train_dataset.iloc[:-val_size]
+        y_train = y_train[:-val_size]
 
     if data_cut is not None:
         np.random.shuffle(all_cols)
         sp_size=int(len(all_cols)/data_cut)
         col_splits = np.split(all_cols, range(0,len(all_cols),sp_size))[1:]
         new_col_splits = []
         for split in col_splits:
```

### Comparing `transtab-0.0.4/transtab/evaluator.py` & `transtab-0.0.5/transtab/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,17 @@
         if ``return_loss=True``, return the mean loss of the predictions made by TransTabClassifier.
 
     '''
     clf.eval()
     pred_list, loss_list = [], []
     for i in range(0, len(x_test), eval_batch_size):
         bs_x_test = x_test.iloc[i:i+eval_batch_size]
+        bs_y_test = y_test.iloc[i:i+eval_batch_size]
         with torch.no_grad():
-            logits, loss = clf(bs_x_test, y_test)
+            logits, loss = clf(bs_x_test, bs_y_test)
         
         if loss is not None:
             loss_list.append(loss.item())
         if logits.shape[-1] == 1: # binary classification
             pred_list.append(logits.sigmoid().detach().cpu().numpy())
         else: # multi-class classification
             pred_list.append(torch.softmax(logits,-1).detach().cpu().numpy())
```

### Comparing `transtab-0.0.4/transtab/modeling_transtab.py` & `transtab-0.0.5/transtab/modeling_transtab.py`

 * *Files 0% similar despite different names*

```diff
@@ -423,15 +423,15 @@
         return self.dropout2(h)
 
     def __setstate__(self, state):
         if 'activation' not in state:
             state['activation'] = F.relu
         super().__setstate__(state)
 
-    def forward(self, src, src_mask= None, src_key_padding_mask= None) -> Tensor:
+    def forward(self, src, src_mask= None, src_key_padding_mask= None, is_causal=None, **kwargs) -> Tensor:
         r"""Pass the input through the encoder layer.
 
         Args:
             src: the sequence to the encoder layer (required).
             src_mask: the mask for the src sequence (optional).
             src_key_padding_mask: the mask for the src keys per batch (optional).
```

### Comparing `transtab-0.0.4/transtab/trainer.py` & `transtab-0.0.5/transtab/trainer.py`

 * *Files identical despite different names*

### Comparing `transtab-0.0.4/transtab/trainer_utils.py` & `transtab-0.0.5/transtab/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `transtab-0.0.4/transtab/transtab.py` & `transtab-0.0.5/transtab/transtab.py`

 * *Files identical despite different names*

### Comparing `transtab-0.0.4/transtab.egg-info/PKG-INFO` & `transtab-0.0.5/transtab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transtab
-Version: 0.0.4
+Version: 0.0.5
 Summary: A flexible tabular prediction model that handles variable-column input tables.
 Home-page: https://github.com/RyanWangZf/transtab
 Author: Zifeng Wang
 Author-email: zifengw2@illinois.edu
 Keywords: tabular data,machine learning,data mining,data science
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -30,14 +30,16 @@
 Document is available at https://transtab.readthedocs.io/en/latest/index.html.
 
 Paper is available at https://arxiv.org/pdf/2205.09328.pdf.
 
 5 min blog to understand TransTab at [realsunlab.medium.com](https://realsunlab.medium.com/transtab-learning-transferable-tabular-transformers-across-tables-1e34eec161b8)!
 
 ### News!
+- [05/04/23] Check the version `0.0.5` of `TransTab`!
+
 - [01/04/23] Check the version `0.0.3` of `TransTab`!
 
 - [12/03/22] Check out our [[blog]](https://realsunlab.medium.com/transtab-learning-transferable-tabular-transformers-across-tables-1e34eec161b8) for a quick understanding of TransTab!
 
 - [08/31/22] `0.0.2` Support encode tabular inputs into embeddings directly. An example is provided [here](examples/table_embedding.ipynb). Several bugs are fixed.
 
 ## TODO
```

