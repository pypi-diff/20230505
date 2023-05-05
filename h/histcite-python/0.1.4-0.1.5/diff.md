# Comparing `tmp/histcite-python-0.1.4.tar.gz` & `tmp/histcite-python-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histcite-python-0.1.4.tar", last modified: Wed May  3 12:18:45 2023, max compression
+gzip compressed data, was "histcite-python-0.1.5.tar", last modified: Fri May  5 05:51:03 2023, max compression
```

## Comparing `histcite-python-0.1.4.tar` & `histcite-python-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:18:45.771508 histcite-python-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 12:18:32.000000 histcite-python-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-03 12:18:45.771508 histcite-python-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-03 12:18:32.000000 histcite-python-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:18:45.771508 histcite-python-0.1.4/histcite/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 12:18:32.000000 histcite-python-0.1.4/histcite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-03 12:18:32.000000 histcite-python-0.1.4/histcite/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-03 12:18:32.000000 histcite-python-0.1.4/histcite/compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-03 12:18:32.000000 histcite-python-0.1.4/histcite/network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-03 12:18:32.000000 histcite-python-0.1.4/histcite/parse_citation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-03 12:18:32.000000 histcite-python-0.1.4/histcite/process_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:18:45.771508 histcite-python-0.1.4/histcite_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-03 12:18:45.000000 histcite-python-0.1.4/histcite_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-03 12:18:45.000000 histcite-python-0.1.4/histcite_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:18:45.000000 histcite-python-0.1.4/histcite_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 12:18:45.000000 histcite-python-0.1.4/histcite_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 12:18:45.000000 histcite-python-0.1.4/histcite_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 12:18:45.000000 histcite-python-0.1.4/histcite_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:18:45.771508 histcite-python-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-03 12:18:32.000000 histcite-python-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:18:45.771508 histcite-python-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-03 12:18:32.000000 histcite-python-0.1.4/tests/test_compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-03 12:18:32.000000 histcite-python-0.1.4/tests/test_network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-03 12:18:32.000000 histcite-python-0.1.4/tests/test_parse_citation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:51:03.588145 histcite-python-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-05 05:50:52.000000 histcite-python-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-05 05:51:03.588145 histcite-python-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-05 05:50:52.000000 histcite-python-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:51:03.584145 histcite-python-0.1.5/histcite/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 05:50:52.000000 histcite-python-0.1.5/histcite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-05 05:50:52.000000 histcite-python-0.1.5/histcite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-05 05:50:52.000000 histcite-python-0.1.5/histcite/compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-05 05:50:52.000000 histcite-python-0.1.5/histcite/network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-05 05:50:52.000000 histcite-python-0.1.5/histcite/parse_citation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-05-05 05:50:52.000000 histcite-python-0.1.5/histcite/process_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:51:03.588145 histcite-python-0.1.5/histcite_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-05 05:51:03.000000 histcite-python-0.1.5/histcite_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-05 05:51:03.000000 histcite-python-0.1.5/histcite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:51:03.000000 histcite-python-0.1.5/histcite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 05:51:03.000000 histcite-python-0.1.5/histcite_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 05:51:03.000000 histcite-python-0.1.5/histcite_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 05:51:03.000000 histcite-python-0.1.5/histcite_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:51:03.588145 histcite-python-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-05 05:50:52.000000 histcite-python-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:51:03.588145 histcite-python-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-05 05:50:52.000000 histcite-python-0.1.5/tests/test_compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-05 05:50:52.000000 histcite-python-0.1.5/tests/test_network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-05 05:50:52.000000 histcite-python-0.1.5/tests/test_parse_citation.py
```

### Comparing `histcite-python-0.1.4/LICENSE` & `histcite-python-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.4/PKG-INFO` & `histcite-python-0.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: histcite-python
-Version: 0.1.4
-Summary: A Python interface to histcite.
-Home-page: https://github.com/doublessay/histcite-python
-Author: WangK2
-Author-email: kw221225@gmail.com
-License: MIT
-Keywords: histcite,web of science,citation network
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # HistCite工具的Python实现
 
 由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，并且可以跨平台使用。
 
 核心功能：
 - 生成引文网络图；
 - 生成包含文献、作者、机构、期刊、关键词等分析单元的引文统计数据；  
@@ -105,21 +82,25 @@
 with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
     f.write(dot_text)
 
 # 保存引文网络图节点文件
 graph_node_file = graph.generate_graph_node_file()
 graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
-> 注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低LCS的文献节点，默认为 `False`。
+> 注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
 
 ## 工具对比：
 | 对比项 | [histcite-python](https://github.com/doublessay/histcite-python) | [histcite pro](https://zhuanlan.zhihu.com/p/20902898) |
 | :-: | :-: | :-: |
 | 是否跨平台 | 是 | 否，仅限 `Windows` |
 | 是否开源 | 是 | 否 |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
 | 性能 | ... | |
 
+## Q&A
+1、如何识别引文关系？  
+每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` 信息，则判断 `第一作者`、`发表年份`、`期刊名称`、`期号` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用关系。  
+
 ## TODO
 - [ ] 支持 `scopus` 题录数据
-- [ ] 构建GUI页面
+- [ ] 构建 `GUI` 页面
```

### Comparing `histcite-python-0.1.4/histcite/cli.py` & `histcite-python-0.1.5/histcite/cli.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.4/histcite/compute_metrics.py` & `histcite-python-0.1.5/histcite/compute_metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,29 @@
 class ComputeMetrics:
     """生成统计结果"""
 
     def __init__(self,docs_table,reference_table):
         self.docs_table = docs_table
         self.reference_table = reference_table
 
-    def __generate_table(self,use_cols:list,col:str,split_char=None)->pd.DataFrame:
+    def __generate_table(self,use_cols:list,col:str,split_char=None,str_lower=False)->pd.DataFrame:
         
         df = self.docs_table[use_cols]
         # 如果字段包含多个值，则进行拆分
         if split_char:
             
             df = df.dropna(subset=[col])
             df = df.astype({col:'str'})
-            df[col] = df[col].str.split(split_char)
+            
+            if str_lower:
+                col_str_lower = df[col].str.lower()
+                df[col] = col_str_lower.str.split(split_char)
+            else:
+                df[col] = df[col].str.split(split_char)
+                
             df = df.explode(col)
             df = df.reset_index(drop=True)
         
         if 'LCS' in use_cols:
             grouped_df = df.groupby(col).agg({col: 'count', 'LCS': 'sum', 'TC': 'sum'})
             grouped_df = grouped_df.rename(columns={col: 'Recs', 'LCS': 'TLCS', 'TC': 'TGCS'})
         else:
@@ -29,15 +35,15 @@
     
     def _generate_author_table(self):
         use_cols = ['AU','LCS','TC']
         return self.__generate_table(use_cols,'AU','; ')
     
     def _generate_keywords_table(self):
         use_cols = ['DE','LCS','TC']
-        return self.__generate_table(use_cols,'DE','; ')
+        return self.__generate_table(use_cols,'DE','; ',True)
     
     def _generate_institution_table(self):
         use_cols = ['C3','LCS','TC']
         return self.__generate_table(use_cols,'C3','; ')
     
     def _generate_records_table(self):
         """生成文献简表"""
```

### Comparing `histcite-python-0.1.4/histcite/network_graph.py` & `histcite-python-0.1.5/histcite/network_graph.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.4/histcite/parse_citation.py` & `histcite-python-0.1.5/histcite/parse_citation.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.4/histcite/process_table.py` & `histcite-python-0.1.5/histcite/process_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def concat_table(self):
         """合并多个dataframe"""
         if len(self.file_name_list)>1:
             docs_table = pd.concat([self._read_table(file_name) for file_name in self.file_name_list],ignore_index=True,copy=False)
         elif len(self.file_name_list)==1:
             docs_table = self._read_table(self.file_name_list[0])
         else:
-            raise ValueError('No valid file in the folder')
+            raise FileNotFoundError('No valid file in the folder')
         
         # 根据入藏号删除重复数据，一般不会有重复数据
         docs_table.drop_duplicates(subset='UT',ignore_index=True,inplace=True)
 
         # 转换数据类型
         docs_table['BP'] = docs_table['BP'].apply(pd.to_numeric,errors='coerce')
         docs_table['VL'] = docs_table['VL'].apply(pd.to_numeric,errors='coerce')
```

### Comparing `histcite-python-0.1.4/histcite_python.egg-info/PKG-INFO` & `histcite-python-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
 Classifier: Intended Audience :: Developers
@@ -105,21 +105,25 @@
 with open(os.path.join(folder_path,'result','graph.dot'), 'w') as f:
     f.write(dot_text)
 
 # 保存引文网络图节点文件
 graph_node_file = graph.generate_graph_node_file()
 graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
-> 注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低LCS的文献节点，默认为 `False`。
+> 注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`, 图文件中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
 
 ## 工具对比：
 | 对比项 | [histcite-python](https://github.com/doublessay/histcite-python) | [histcite pro](https://zhuanlan.zhihu.com/p/20902898) |
 | :-: | :-: | :-: |
 | 是否跨平台 | 是 | 否，仅限 `Windows` |
 | 是否开源 | 是 | 否 |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较细腻 | 位图，比较粗糙 |
 | 性能 | ... | |
 
+## Q&A
+1、如何识别引文关系？  
+每条文献元数据都包含 `CR` 字段，表示该文献的参考文献集合。发表时间等于或早于当前文献的其他文献为候选文献，如果这些候选文献存在 `DOI` 信息，则判断 `DOI` 是否在参考文献集合的 `DOI` 列表中；如果不存在 `DOI` 信息，则判断 `第一作者`、`发表年份`、`期刊名称`、`期号` 四个字段信息是否与参考文献集合的某条记录一致，一致则判断为引用关系。  
+
 ## TODO
 - [ ] 支持 `scopus` 题录数据
-- [ ] 构建GUI页面
+- [ ] 构建 `GUI` 页面
```

### Comparing `histcite-python-0.1.4/setup.py` & `histcite-python-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name="histcite-python",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.1.4",
+    version="0.1.5",
     description="A Python interface to histcite.",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["histcite","web of science","citation network"],
     license="MIT",
     url="https://github.com/doublessay/histcite-python",
     packages=["histcite"],
```

### Comparing `histcite-python-0.1.4/tests/test_parse_citation.py` & `histcite-python-0.1.5/tests/test_parse_citation.py`

 * *Files identical despite different names*

