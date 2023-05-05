# Comparing `tmp/cicc_excel-0.0.1.tar.gz` & `tmp/cicc_excel-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cicc_excel-0.0.1.tar", last modified: Tue May  2 04:49:22 2023, max compression
+gzip compressed data, was "dist/cicc_excel-0.0.2.tar", last modified: Fri May  5 13:14:24 2023, max compression
```

## Comparing `cicc_excel-0.0.1.tar` & `cicc_excel-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 js         (501) staff       (20)        0 2023-05-02 04:49:22.000000 cicc_excel-0.0.1/
--rw-r--r--   0 js         (501) staff       (20)      655 2023-05-02 04:49:22.000000 cicc_excel-0.0.1/PKG-INFO
--rwxr-xr-x   0 js         (501) staff       (20)       51 2023-05-02 04:19:48.000000 cicc_excel-0.0.1/README.md
-drwxr-xr-x   0 js         (501) staff       (20)        0 2023-05-02 04:49:22.000000 cicc_excel-0.0.1/cicc_excel/
--rwxr-xr-x   0 js         (501) staff       (20)        0 2020-07-20 03:22:51.000000 cicc_excel-0.0.1/cicc_excel/__init__.py
--rwxr-xr-x   0 js         (501) staff       (20)    11577 2023-05-02 04:28:07.000000 cicc_excel-0.0.1/cicc_excel/excelwriter.py
-drwxr-xr-x   0 js         (501) staff       (20)        0 2023-05-02 04:49:22.000000 cicc_excel-0.0.1/cicc_excel.egg-info/
--rwxr-xr-x   0 js         (501) staff       (20)      655 2023-05-02 04:49:22.000000 cicc_excel-0.0.1/cicc_excel.egg-info/PKG-INFO
--rwxr-xr-x   0 js         (501) staff       (20)      203 2023-05-02 04:49:22.000000 cicc_excel-0.0.1/cicc_excel.egg-info/SOURCES.txt
--rwxr-xr-x   0 js         (501) staff       (20)        1 2023-05-02 04:49:22.000000 cicc_excel-0.0.1/cicc_excel.egg-info/dependency_links.txt
--rwxr-xr-x   0 js         (501) staff       (20)       11 2023-05-02 04:49:22.000000 cicc_excel-0.0.1/cicc_excel.egg-info/top_level.txt
--rw-r--r--   0 js         (501) staff       (20)       38 2023-05-02 04:49:22.000000 cicc_excel-0.0.1/setup.cfg
--rwxr-xr-x   0 js         (501) staff       (20)      771 2023-05-02 04:49:07.000000 cicc_excel-0.0.1/setup.py
+drwxr-xr-x   0 js         (501) staff       (20)        0 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/
+-rw-r--r--   0 js         (501) staff       (20)     1651 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/PKG-INFO
+-rwxr-xr-x   0 js         (501) staff       (20)      783 2023-05-05 13:09:46.000000 cicc_excel-0.0.2/README.md
+drwxr-xr-x   0 js         (501) staff       (20)        0 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/cicc_excel/
+-rwxr-xr-x   0 js         (501) staff       (20)        0 2020-07-20 03:22:51.000000 cicc_excel-0.0.2/cicc_excel/__init__.py
+-rwxr-xr-x   0 js         (501) staff       (20)    12078 2023-05-05 12:54:10.000000 cicc_excel-0.0.2/cicc_excel/excelwriter.py
+drwxr-xr-x   0 js         (501) staff       (20)        0 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/cicc_excel.egg-info/
+-rwxr-xr-x   0 js         (501) staff       (20)     1651 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/cicc_excel.egg-info/PKG-INFO
+-rwxr-xr-x   0 js         (501) staff       (20)      203 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/cicc_excel.egg-info/SOURCES.txt
+-rwxr-xr-x   0 js         (501) staff       (20)        1 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/cicc_excel.egg-info/dependency_links.txt
+-rwxr-xr-x   0 js         (501) staff       (20)       11 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/cicc_excel.egg-info/top_level.txt
+-rw-r--r--   0 js         (501) staff       (20)       38 2023-05-05 13:14:24.000000 cicc_excel-0.0.2/setup.cfg
+-rwxr-xr-x   0 js         (501) staff       (20)      771 2023-05-05 13:01:10.000000 cicc_excel-0.0.2/setup.py
```

### Comparing `cicc_excel-0.0.1/cicc_excel/excelwriter.py` & `cicc_excel-0.0.2/cicc_excel/excelwriter.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,137 +9,145 @@
 import re
 import xlsxwriter
 
 class ExcelWriter(object):
     """
     Class for writing data to an xlsx file.
     """
-    def __init__(self, filename, sheet_name='Sheet1'):
+    def __init__(self, filename, en_font='Arial', ch_font='宋体', num_font='Arial'):
         """
         Initialize an open workbook and add a worksheets.
         """
         self.filename = filename
         self.workbook = xlsxwriter.Workbook(filename, {'nan_inf_to_errors':True})
         self.styles = {
             'normal':{},
             'hl':{}
         }
+        self.hl_cols = {}
         #Setting Styles
+        self.header_format = self.workbook.add_format({'border':None,
+                                    'bold': True,
+                                    'font_size': 10,
+                                    'font_name': ch_font,
+                                    'bg_color': '#EEECE1',
+                                    'align': 'center',
+                                    'valign': 'vcenter'})
         self.styles['normal']['number_format'] = self.workbook.add_format({
             'font_size': 10,
             'align': 'right',
             'valign': 'vcenter',
-            'font_name': 'Times New Roman',
+            'font_name': num_font,
             'num_format': '#,##0'
         })
         self.styles['normal']['worktime_format'] = self.workbook.add_format({
             'font_size': 10,
             'align': 'right',
             'valign': 'vcenter',
-            'font_name': 'Times New Roman',
+            'font_name': num_font,
             'num_format': '#,##0.00'
         })
         self.styles['normal']['percent_format'] = self.workbook.add_format({
             'font_size': 10,
             'align': 'right',
             'valign': 'vcenter',
-            'font_name': 'Times New Roman',
+            'font_name': num_font,
             'num_format': '0.00%'
         })
         self.styles['normal']['chinese_format'] = self.workbook.add_format({
-            'font_name': '宋体',
+            'font_name': ch_font,
             'font_size': 10,
             'align': 'left',
             'valign': 'vcenter'
         })
         self.styles['normal']['english_format'] = self.workbook.add_format({
-            'font_name': 'Times New Roman',
+            'font_name': en_font,
             'font_size': 10,
             'align': 'left',
             'valign': 'vcenter'
         })
         self.styles['normal']['sn_format'] = self.workbook.add_format({
-            'font_name': 'Times New Roman',
+            'font_name': en_font,
             'font_size': 10,
             'align': 'left',
             'valign': 'vcenter',
             'bold': True
         })
         self.styles['normal']['date_format'] = self.workbook.add_format({
             'font_size': 10,
             'align': 'right',
             'valign': 'vcenter',
-            'font_name': 'Times New Roman',
+            'font_name': en_font,
             'num_format':'yyyy/mm/dd'
         })
         self.styles['normal']['default_format'] = self.workbook.add_format({
             'font_size':10,
             'align': 'left',
             'valign': 'vcenter'
         })
         # Set Highlight Styles
         self.styles['hl']['number_format'] = self.workbook.add_format({
             'font_size': 10,
             'bg_color': '#EEECE1',
             'font_color': '#9B3519',
             'align': 'right',
             'valign': 'vcenter',
-            'font_name': 'Times New Roman',
+            'font_name': num_font,
             'num_format': '#,##0'
         })
         self.styles['hl']['worktime_format'] = self.workbook.add_format({
             'font_size': 10,
             'bg_color': '#EEECE1',
             'font_color': '#9B3519',
             'align': 'right',
             'valign': 'vcenter',
-            'font_name': 'Times New Roman',
+            'font_name': num_font,
             'num_format': '#,##0.00'
         })
         self.styles['hl']['percent_format'] = self.workbook.add_format({
             'font_size': 10,
             'bg_color': '#EEECE1',
             'font_color': '#9B3519',
             'align': 'right',
             'valign': 'vcenter',
-            'font_name': 'Times New Roman',
+            'font_name': num_font,
             'num_format': '0.00%'
         })
         self.styles['hl']['chinese_format'] = self.workbook.add_format({
-            'font_name': '宋体',
+            'font_name': ch_font,
             'bg_color': '#EEECE1',
             'font_color': '#9B3519',
             'font_size': 10,
             'align': 'left',
             'valign': 'vcenter'
         })
         self.styles['hl']['english_format'] = self.workbook.add_format({
-            'font_name': 'Times New Roman',
+            'font_name': en_font,
             'bg_color': '#EEECE1',
             'font_color': '#9B3519',
             'font_size': 10,
             'valign': 'vcenter',
             'align': 'left'
         })
         self.styles['hl']['sn_format'] = self.workbook.add_format({
-            'font_name': 'Times New Roman',
+            'font_name': en_font,
             'bg_color': '#EEECE1',
             'font_color': '#9B3519',
             'font_size': 10,
             'align': 'left',
             'valign': 'vcenter',
             'bold': True
         })
         self.styles['hl']['date_format'] = self.workbook.add_format({
             'font_size': 10,
             'bg_color': '#EEECE1',
             'font_color': '#9B3519',
             'align': 'right',
             'valign': 'vcenter',
-            'font_name': 'Times New Roman',
+            'font_name': en_font,
             'num_format':'yyyy/mm/dd'
         })
         self.styles['hl']['default_format'] = self.workbook.add_format({
             'font_size':10,
             'bg_color': '#EEECE1',
             'font_color': '#9B3519',
             'align': 'left',
@@ -168,40 +176,40 @@
         write data into workbook
         """
         ws = self.workbook.add_worksheet(sheet_name)
         headers = list(self.data.columns)
         # add header
         for col_num, header_title in enumerate(headers):
             ws.write(0, col_num, header_title)
-        self.set_first_row_format()
+        self.set_first_row_format(sheet_name)
         date_columns = []
         num_columns = []
         text_columns = []
         percent_columns = []
         worktime_columns = []
         sn_columns = []
         for col_name in self.data.columns:
             if pd.api.types.is_datetime64_dtype(self.data[col_name]):
                 date_columns.append(col_name)
             elif '%' in col_name:
                 percent_columns.append(col_name)
-            elif '工号' in col_name or '编号' in col_name or '编码' in col_name or '姓名' in col_name:
+            elif '工号' in col_name or '编号' in col_name or '编码' in col_name:
                 sn_columns.append(col_name)
             elif 'yr' in col_name or '工时' in col_name:
                 worktime_columns.append(col_name)
             elif pd.api.types.is_numeric_dtype(self.data[col_name]):
                 num_columns.append(col_name)
             else:
                 text_columns.append(col_name)
 
         # add data
         for col_num, column_name in enumerate(self.data.columns):
             #set high light column
             style = self.styles['normal']
-            if column_name in self.hl_cols:
+            if sheet_name in self.hl_cols and column_name in self.hl_cols[sheet_name]:
                 style = self.styles['hl']
             #set width
             if column_name in date_columns:
                 ws.set_column(col_num, col_num, self.column_width['date'], None)
             elif column_name in sn_columns:
                 ws.set_column(col_num, col_num, self.column_width['sn'], None)
             elif column_name in num_columns:
@@ -260,61 +268,69 @@
         """
         return self.workbook.add_format(format)
     
     def set_first_row_format(self, sheet_name='Sheet1'):
         """
         Add a format to the first row.
         """
-        self.header_format = self.workbook.add_format({'border':None,
-                                           'bold': True,
-                                           'font_size': 10,
-                                           'font_name': '宋体',
-                                           'bg_color': '#EEECE1',
-                                           'align': 'center',
-                                           'valign': 'vcenter'})
         ws = self.workbook.get_worksheet_by_name(sheet_name)
-        ws.set_row(0, 20, self.header_format)
-        ws.autofilter(0, 0, ws.dim_rowmax,ws.dim_colmax)
+        if ws is not None:
+            ws.set_row(0, 20, self.header_format)
+            ws.autofilter(0, 0, ws.dim_rowmax,ws.dim_colmax)
+        else:
+            print("Error: worksheets", sheet_name, "not found")
 
     def set_global_format(self):
         """
         Set the global format for all worksheets.
         """
         df_format = self.workbook.formats[0]
         df_format.set_font_size(10)
     
     def freeze(self, row=1, col=1, sheet_name='Sheet1'):
         """
         Freeze the first row and first column.
         """
         ws = self.workbook.get_worksheet_by_name(sheet_name)
-        ws.freeze_panes(row, col)
+        if ws is not None:
+            ws.freeze_panes(row, col)
+        else:
+            print("Error: worksheets", sheet_name, "not found")
     
     def autofit(self, sheet_name='Sheet1'):
         """
         Fit the width of all columns.
         """
         ws = self.workbook.get_worksheet_by_name(sheet_name)
-        ws.autofit()
+        if ws is not None:
+            ws.autofit()
+        else:
+            print("Error: worksheets", sheet_name, "not found")
 
     def hide_col(self, s_col=0, end_col=0, sheet_name='Sheet1'):
         """
         Hide acolumns.
         """
         ws = self.workbook.get_worksheet_by_name(sheet_name)
-        ws.set_column(s_col, end_col, None, None, {'hidden': True})
+        if ws is not None:
+            ws.set_column(s_col, end_col, None, None, {'hidden': True})
+        else:
+            print("Error: worksheets", sheet_name, "not found")
 
     def collapse_col(self, s_col=0, end_col=0, sheet_name='Sheet1'):
         """
         Hide acolumns.
         """
         ws = self.workbook.get_worksheet_by_name(sheet_name)
-        ws.set_column(s_col, end_col, None, None, {'collapsed': True})
+        if ws is not None:
+            ws.set_column(s_col, end_col, None, None, {'collapsed': True})
+        else:
+            print("Error: worksheets", sheet_name, "not found")
     
-    def set_hl_col_by_names(self, col_names):
+    def set_hl_col_by_names(self, col_names, sheet_name):
         """
         Set col by col name
         """
-        self.hl_cols = col_names
+        self.hl_cols[sheet_name] = col_names
```

### Comparing `cicc_excel-0.0.1/setup.py` & `cicc_excel-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cicc_excel",
-    version="0.0.1",
+    version="0.0.2",
     author="Pengcheng Song",
     author_email="smth_spc@hotmail.com",
     description="Library of export pandas into excel for CICCers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nyuspc/cicc_excel",
     packages=setuptools.find_packages(),
```

