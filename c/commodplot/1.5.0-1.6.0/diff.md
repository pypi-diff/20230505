# Comparing `tmp/commodplot-1.5.0.tar.gz` & `tmp/commodplot-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commodplot-1.5.0.tar", last modified: Tue Mar  7 12:54:45 2023, max compression
+gzip compressed data, was "commodplot-1.6.0.tar", last modified: Fri May  5 14:19:28 2023, max compression
```

## Comparing `commodplot-1.5.0.tar` & `commodplot-1.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:54:45.192865 commodplot-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-07 12:54:45.192865 commodplot-1.5.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:54:45.188865 commodplot-1.5.0/commodplot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 12:54:33.000000 commodplot-1.5.0/commodplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-03-07 12:54:33.000000 commodplot-1.5.0/commodplot/commodplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-03-07 12:54:33.000000 commodplot-1.5.0/commodplot/commodplottable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-03-07 12:54:33.000000 commodplot-1.5.0/commodplot/commodplottrace.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-07 12:54:33.000000 commodplot-1.5.0/commodplot/commodplottransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-03-07 12:54:33.000000 commodplot-1.5.0/commodplot/commodplotutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-03-07 12:54:33.000000 commodplot-1.5.0/commodplot/jinjautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-03-07 12:54:33.000000 commodplot-1.5.0/commodplot/messaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:54:45.188865 commodplot-1.5.0/commodplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-07 12:54:45.000000 commodplot-1.5.0/commodplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-07 12:54:45.000000 commodplot-1.5.0/commodplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 12:54:45.000000 commodplot-1.5.0/commodplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-07 12:54:45.000000 commodplot-1.5.0/commodplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-07 12:54:45.000000 commodplot-1.5.0/commodplot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-07 12:54:45.192865 commodplot-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-07 12:54:33.000000 commodplot-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 12:54:45.188865 commodplot-1.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 12:54:33.000000 commodplot-1.5.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-03-07 12:54:33.000000 commodplot-1.5.0/test/test_commodplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-07 12:54:33.000000 commodplot-1.5.0/test/test_commodplottable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-03-07 12:54:33.000000 commodplot-1.5.0/test/test_commodplottrace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-07 12:54:33.000000 commodplot-1.5.0/test/test_commodplotutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-07 12:54:33.000000 commodplot-1.5.0/test/test_jinjautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-07 12:54:33.000000 commodplot-1.5.0/test/test_messaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:19:28.377368 commodplot-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-05 14:19:28.377368 commodplot-1.6.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:19:28.373368 commodplot-1.6.0/commodplot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:19:17.000000 commodplot-1.6.0/commodplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16416 2023-05-05 14:19:17.000000 commodplot-1.6.0/commodplot/commodplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-05 14:19:17.000000 commodplot-1.6.0/commodplot/commodplottable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-05-05 14:19:17.000000 commodplot-1.6.0/commodplot/commodplottrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-05 14:19:17.000000 commodplot-1.6.0/commodplot/commodplottransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-05 14:19:17.000000 commodplot-1.6.0/commodplot/commodplotutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-05 14:19:17.000000 commodplot-1.6.0/commodplot/jinjautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-05-05 14:19:17.000000 commodplot-1.6.0/commodplot/messaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:19:28.377368 commodplot-1.6.0/commodplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-05 14:19:28.000000 commodplot-1.6.0/commodplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-05 14:19:28.000000 commodplot-1.6.0/commodplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:19:28.000000 commodplot-1.6.0/commodplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 14:19:28.000000 commodplot-1.6.0/commodplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 14:19:28.000000 commodplot-1.6.0/commodplot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-05 14:19:28.377368 commodplot-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-05 14:19:17.000000 commodplot-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:19:28.377368 commodplot-1.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:19:17.000000 commodplot-1.6.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-05-05 14:19:17.000000 commodplot-1.6.0/test/test_commodplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-05 14:19:17.000000 commodplot-1.6.0/test/test_commodplottable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-05 14:19:17.000000 commodplot-1.6.0/test/test_commodplottrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-05 14:19:17.000000 commodplot-1.6.0/test/test_commodplotutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-05 14:19:17.000000 commodplot-1.6.0/test/test_jinjautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-05 14:19:17.000000 commodplot-1.6.0/test/test_messaging.py
```

### Comparing `commodplot-1.5.0/commodplot/commodplot.py` & `commodplot-1.6.0/commodplot/commodplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import itertools
 
-import cufflinks as cf
 import pandas as pd
 import plotly as py
 import plotly.express as px
 import plotly.graph_objects as go
 from commodutil import dates
 from commodutil import transforms
 from plotly.subplots import make_subplots
@@ -267,32 +266,51 @@
 def bar_line_plot(df, linecol="Total", **kwargs):
     """
     Give a dataframe, make a stacked bar chart along with overlaying line chart.
     """
     if linecol not in df:
         df[linecol] = df.sum(1, skipna=False)
 
-    barcols = [x for x in df.columns if linecol not in x]
-    barspecs = {"kind": "bar", "barmode": "relative", "title": "d", "columns": barcols}
-    linespecs = {"kind": "scatter", "columns": linecol, "color": "black"}
+    fig = go.Figure()
+    # create the bar trace
+    for col in df.columns:
+        if col != linecol:
+            bar_trace = go.Bar(
+                x=df.index,
+                y=df[col],
+                name=col,
+            )
+            fig.add_trace(bar_trace)
 
-    fig = cf.tools.figures(df, [barspecs, linespecs])  # returns dict
-    fig = go.Figure(fig)
+    # create the line trace
+    line_trace = go.Scatter(
+        x=df.index,
+        y=df[linecol],
+        name=linecol,
+        mode="lines",
+        line=dict(color="black"),
+    )
+
+    fig.add_trace(line_trace)
+
+    # update the figure layout if needed
     yaxis_title = kwargs.get("yaxis_title", None)
     yaxis_range = kwargs.get("yaxis_range", None)
     title = kwargs.get("title", None)
     fig.update_layout(
         title=title,
         title_x=0.01,
         xaxis_title="Date",
         yaxis_title=yaxis_title,
-        margin=preset_margins,
+        barmode="relative",
+        margin=dict(l=40, r=20, t=40, b=20),
     )
     if yaxis_range is not None:
         fig.update_layout(yaxis=dict(range=yaxis_range))
+
     return fig
 
 
 def diff_plot(df, **kwargs):
     """
     Given a dataframe, plot each column as line plot with a subplot below
     showing differences between each column.
@@ -314,24 +332,20 @@
         fig.add_trace(go.Scatter(x=df.index, y=df[col], name=col))
 
     for col in barcols:
         fig.add_trace(go.Bar(x=df.index, y=df[col], name=col), row=2, col=1)
 
     today = pd.Timestamp.today()
     vline = go.layout.Shape(
-        type='line',
+        type="line",
         x0=today,
         x1=today,
         y0=df.min().min(),  # Set y0 to the minimum value of y_data
         y1=df.max().max(),  # Set y1 to the maximum value of y_data
-        line=dict(
-            color='grey',
-            width=1,
-            dash='dash'
-        )
+        line=dict(color="grey", width=1, dash="dash"),
     )
     fig.update_layout(shapes=[vline])
 
     title = kwargs.get("title", "")
     fig.update_layout(title_text=title, title_x=0.01, margin=preset_margins)
     return fig
```

### Comparing `commodplot-1.5.0/commodplot/commodplottable.py` & `commodplot-1.6.0/commodplot/commodplottable.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 
 
 def generate_table(
     df: pd.DataFrame,
     precision: t.Tuple[int, dict] = None,
     accounting_col_columns: list = None,
 ):
-
     if precision:
         if isinstance(precision, int):
             format_var = "{:.%sf}" % precision
             df = df.applymap(lambda x: format_var.format(x))
         elif isinstance(precision, dict):
             for col, col_precision in precision.items():
                 format_var = "{:,.%sf}" % col_precision
```

### Comparing `commodplot-1.5.0/commodplot/commodplottrace.py` & `commodplot-1.6.0/commodplot/commodplottrace.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,15 +216,20 @@
         )
         traces.append(trace)
 
     return traces
 
 
 def timeseries_to_reindex_year_trace(
-    dft, text, dash=None, current_select_year=None, showlegend=True, visible_line_years=None
+    dft,
+    text,
+    dash=None,
+    current_select_year=None,
+    showlegend=True,
+    visible_line_years=None,
 ):
     traces = []
     colyearmap = cpu.dates.find_year(dft)
 
     for col in dft.columns:
         colyear = colyearmap[col]
         width = 1.2
@@ -325,15 +330,19 @@
     if shaded_range is not None:
         res["shaded_range"] = shaded_range_traces(
             df, shaded_range, showlegend=showlegend
         )
 
     # historical / solid lines
     res["hist"] = timeseries_to_reindex_year_trace(
-        df, text, current_select_year=current_select_year, showlegend=showlegend, visible_line_years=visible_line_years
+        df,
+        text,
+        current_select_year=current_select_year,
+        showlegend=showlegend,
+        visible_line_years=visible_line_years,
     )
 
     return res
 
 
 def timeseries_trace(series: pd.Series, **kwargs) -> go.Scatter:
     """
```

### Comparing `commodplot-1.5.0/commodplot/commodplottransform.py` & `commodplot-1.6.0/commodplot/commodplottransform.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.5.0/commodplot/commodplotutil.py` & `commodplot-1.6.0/commodplot/commodplotutil.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.5.0/commodplot/jinjautils.py` & `commodplot-1.6.0/commodplot/jinjautils.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.5.0/commodplot/messaging.py` & `commodplot-1.6.0/commodplot/messaging.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.5.0/commodplot.egg-info/SOURCES.txt` & `commodplot-1.6.0/commodplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commodplot-1.5.0/setup.py` & `commodplot-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="commodplot",
-    version="1.5.0",
+    version="1.6.0",
     author="aeorxc",
     author_email="author@example.com",
     description="common commodity plotting including seasonal charts using plotly",
     url="https://github.com/aeorxc/commodplot",
     project_urls={
         "Source": "https://github.com/aeorxc/commodplot",
     },
@@ -16,15 +16,14 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "pandas",
         "plotly",
         "commodutil",
-        "cufflinks",
         "kaleido",
         "jinja2",
     ],
     python_requires=">=3.6",
     setup_requires=["pytest-runner"],
     tests_require=["pytest"],
 )
```

### Comparing `commodplot-1.5.0/test/test_commodplot.py` & `commodplot-1.6.0/test/test_commodplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,17 @@
                 x: pd.to_datetime(forwards.convert_contract_to_date(x))
                 for x in cl.columns
             }
         )
 
         sp = forwards.time_spreads(cl, 12, 12)
 
-        res = commodplot.reindex_year_line_plot(sp, max_results=360, visible_line_years=7)
+        res = commodplot.reindex_year_line_plot(
+            sp, max_results=360, visible_line_years=7
+        )
         self.assertTrue(isinstance(res, go.Figure))
 
     def test_fwd_hist_plot(self):
         dirname, filename = os.path.split(os.path.abspath(__file__))
         cl = pd.read_csv(
             os.path.join(dirname, "test_cl_fwd.csv"),
             index_col=0,
@@ -254,10 +256,23 @@
         df = pd.DataFrame(
             data={"col1": [1, 2, 3, 4], "col2": [5, 6, 7, 8]}, index=multi_index
         ).T
 
         res = commodplot.stacked_grouped_bar_chart(df)
         self.assertTrue(isinstance(res, go.Figure))
 
+    def test_bar_line_plot(self):
+        dirname, filename = os.path.split(os.path.abspath(__file__))
+        cl = pd.read_csv(
+            os.path.join(dirname, "test_cl.csv"),
+            index_col=0,
+            parse_dates=True,
+            dayfirst=True,
+        )
+        cl = cl.dropna(how="all", axis=1)[["CL_2020F", "CL_2020G"]]
+        cl = cl.rename(columns={"CL_2020F": "A", "CL_2020G": "B"})
+        res = commodplot.bar_line_plot(cl, title="Test")
+        self.assertTrue(isinstance(res, go.Figure))
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `commodplot-1.5.0/test/test_commodplottable.py` & `commodplot-1.6.0/test/test_commodplottable.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.5.0/test/test_commodplottrace.py` & `commodplot-1.6.0/test/test_commodplottrace.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.5.0/test/test_commodplotutil.py` & `commodplot-1.6.0/test/test_commodplotutil.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.5.0/test/test_jinjautils.py` & `commodplot-1.6.0/test/test_jinjautils.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.5.0/test/test_messaging.py` & `commodplot-1.6.0/test/test_messaging.py`

 * *Files identical despite different names*

