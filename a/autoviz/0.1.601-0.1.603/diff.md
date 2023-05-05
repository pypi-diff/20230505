# Comparing `tmp/autoviz-0.1.601.tar.gz` & `tmp/autoviz-0.1.603.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoviz-0.1.601.tar", last modified: Tue Apr 18 13:24:18 2023, max compression
+gzip compressed data, was "autoviz-0.1.603.tar", last modified: Fri May  5 14:02:25 2023, max compression
```

## Comparing `autoviz-0.1.601.tar` & `autoviz-0.1.603.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-18 13:24:18.485915 autoviz-0.1.601/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    14161 2023-04-18 13:24:18.470300 autoviz-0.1.601/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)    12342 2023-04-18 13:22:22.000000 autoviz-0.1.601/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-18 13:24:18.338756 autoviz-0.1.601/autoviz/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    30554 2023-04-18 12:33:51.000000 autoviz-0.1.601/autoviz/AutoViz_Class.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    61007 2022-10-02 14:52:48.000000 autoviz-0.1.601/autoviz/AutoViz_Holo.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2022-10-02 14:52:48.000000 autoviz-0.1.601/autoviz/AutoViz_NLP.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)   117576 2023-04-18 13:15:24.000000 autoviz-0.1.601/autoviz/AutoViz_Utils.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1323 2022-10-02 14:52:48.000000 autoviz-0.1.601/autoviz/__init__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)      404 2023-04-18 11:01:32.000000 autoviz-0.1.601/autoviz/__version__.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)    24678 2023-04-18 12:53:31.000000 autoviz-0.1.601/autoviz/classify_method.py
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-18 13:24:18.454671 autoviz-0.1.601/autoviz.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    14161 2023-04-18 13:24:17.000000 autoviz-0.1.601/autoviz.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2023-04-18 13:24:17.000000 autoviz-0.1.601/autoviz.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-04-18 13:24:17.000000 autoviz-0.1.601/autoviz.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)      241 2023-04-18 13:24:17.000000 autoviz-0.1.601/autoviz.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2023-04-18 13:24:17.000000 autoviz-0.1.601/autoviz.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-04-18 13:24:18.485915 autoviz-0.1.601/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)     1205 2023-04-18 13:18:30.000000 autoviz-0.1.601/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-05 14:02:25.967815 autoviz-0.1.603/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    15853 2023-05-05 14:02:25.963811 autoviz-0.1.603/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    13747 2023-05-05 13:59:34.000000 autoviz-0.1.603/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-05 14:02:25.823558 autoviz-0.1.603/autoviz/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    30554 2023-04-18 12:33:51.000000 autoviz-0.1.603/autoviz/AutoViz_Class.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    61007 2022-10-02 14:52:48.000000 autoviz-0.1.603/autoviz/AutoViz_Holo.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    24022 2022-10-02 14:52:48.000000 autoviz-0.1.603/autoviz/AutoViz_NLP.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)   118079 2023-05-05 13:05:30.000000 autoviz-0.1.603/autoviz/AutoViz_Utils.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1323 2022-10-02 14:52:48.000000 autoviz-0.1.603/autoviz/__init__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      404 2023-05-05 12:31:56.000000 autoviz-0.1.603/autoviz/__version__.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    24678 2023-04-18 12:53:31.000000 autoviz-0.1.603/autoviz/classify_method.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-05-05 14:02:25.941772 autoviz-0.1.603/autoviz.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    15853 2023-05-05 14:02:25.000000 autoviz-0.1.603/autoviz.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      339 2023-05-05 14:02:25.000000 autoviz-0.1.603/autoviz.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-05-05 14:02:25.000000 autoviz-0.1.603/autoviz.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      241 2023-05-05 14:02:25.000000 autoviz-0.1.603/autoviz.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        8 2023-05-05 14:02:25.000000 autoviz-0.1.603/autoviz.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-05-05 14:02:25.971820 autoviz-0.1.603/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     1205 2023-05-05 13:06:48.000000 autoviz-0.1.603/setup.py
```

### Comparing `autoviz-0.1.601/PKG-INFO` & `autoviz-0.1.603/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,214 +1,255 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.601
+Version: 0.1.603
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz
 Author: Ram Seshadri
 License: Apache License 2.0
-Description: # AutoViz
+Description: # AutoViz: The One-Line Automatic Data Visualization Library
         
-        Automatically Visualize any dataset, any size with a single line of code. Now you can save these interactive charts as HTML files automatically with the `"html"` setting.
+        ![logo](logo.png)
+        
+        Unlock the power of **AutoViz** to visualize any dataset, any size, with just a single line of code! Plus, now you can save these interactive charts as HTML files automatically with the `html` setting.
         
         [![Pepy Downloads](https://pepy.tech/badge/autoviz)](https://pepy.tech/project/autoviz)
         [![Pepy Downloads per week](https://pepy.tech/badge/autoviz/week)](https://pepy.tech/project/autoviz)
         [![Pepy Downloads per month](https://pepy.tech/badge/autoviz/month)](https://pepy.tech/project/autoviz)
         [![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg)](https://github.com/RichardLitt/standard-readme)
         [![Python Versions](https://img.shields.io/pypi/pyversions/autoviz.svg)](https://pypi.org/project/autoviz)
         [![PyPI Version](https://img.shields.io/pypi/v/autoviz.svg)](https://pypi.org/project/autoviz)
         [![PyPI License](https://img.shields.io/pypi/l/autoviz.svg)](https://github.com/AutoViML/AutoViz/blob/master/LICENSE)
         
-        AutoViz performs automatic visualization of any dataset with one line of code.
-        Give it any input file (CSV, txt or json format) of any size and AutoViz will visualize it, provided you set the `max_rows_analyzed` and `max_cols_analyzed` setting within the bounds of your machine's memory limit.
-        
-        AutoViz can now create charts in multiple  formats using the `chart_format` setting:
-        - If `chart_format ='png'` or `'svg'` or `'jpg'`: Matplotlib charts are plotted inline.
-            * Can be saved locally (using `verbose=2` setting) or displayed (`verbose=1`) in Jupyter Notebooks.
-            * This is the default behavior for AutoViz.
-        - If `chart_format='bokeh'`: Interactive Bokeh charts are plotted in Jupyter Notebooks.
-        - If `chart_format='server'`, dashboards will pop up for each kind of chart on your browser.
-        - If `chart_format='html'`, interactive Bokeh charts will be created and silently saved as HTML files under the `AutoViz_Plots` directory (under working folder) or any other directory that you specify using the `save_plot_dir` setting (during input).
+        With AutoViz, you can easily and quickly generate insightful visualizations for your data. Whether you're a beginner or an expert in data analysis, AutoViz can help you explore your data and uncover valuable insights. Try it out and see the power of automated visualization for yourself!
         
         ## Table of Contents
         
-        - [Install](#install)
-        - [Usage](#usage)
-        - [API](#api)
+        - [The purpose and motivation for AutoViz](#motivation)
+        - [How to install and setup AutoViz in your environment](#installation)
+        - [How to use AutoViz with various options and settings](#usage)
+        - [The API and available options](#api)
+        - [Examples to get you started](#examples)
         - [Maintainers](#maintainers)
-        - [Contributing](#contributing)
+        - [Contributing to the project](#contributing)
         - [License](#license)
+        - [Additional Tips before you start](#tips)
+        - [Disclaimer](#disclaimer)
         
-        ## Install
+        # Motivation
+        <p>The motivation to create AutoViz stems from the need for a more efficient, user-friendly, and automated approach to data visualization. Visualizing data is a crucial step in the data analysis process, as it helps users understand patterns, trends, and relationships in the data. However, creating insightful visualizations can be time-consuming and require specialized knowledge of various plotting libraries and techniques.</p>
         
-        **Prerequsites**
+        <p>AutoViz addresses these challenges by providing an easy-to-use, automated solution for generating meaningful visualizations with minimal effort. Its key motivation is to:</p>
         
-        - [Anaconda](https://docs.anaconda.com/anaconda/install/)
+        <ol>
+          <li><strong>Save time and effort</strong>: AutoViz simplifies the visualization process by requiring just a single line of code to generate multiple insightful plots, eliminating the need to write multiple lines of code for each chart.</li>
+          <li><strong>Handle large datasets</strong>: AutoViz is designed to work with datasets of any size, intelligently sampling the data when necessary to ensure that the visualizations are generated quickly and efficiently, without compromising on the insights.</li>
+          <li><strong>Accessibility</strong>: AutoViz makes data visualization accessible to a broader audience, including non-experts and beginners in data analysis, by abstracting away the complexities of various plotting libraries.</li>
+          <li><strong>Automate the visualization process</strong>: AutoViz intelligently selects the appropriate visualizations for the given data, taking into account the data types and relationships among variables, which helps users quickly gain insights without having to manually decide which plots to create.</li>
+          <li><strong>Customization and interactivity</strong>: AutoViz offers various options for customization, enabling users to tailor the generated visualizations to their specific needs and preferences. Moreover, with interactive chart formats like Bokeh, users can explore the data more dynamically.</li>
+        </ol>
         
-        To clone AutoViz, it's better to create a new environment, and install the required dependencies:
+        <p>In summary, the motivation behind AutoViz is to make data visualization more efficient, accessible, and automated, enabling users to quickly gain valuable insights from their data and focus on making data-driven decisions.</p>
         
-        To install from PyPi:
+        ## Installation
         
-        ```sh
-        conda create -n <your_env_name> python=3.7 anaconda
-        conda activate <your_env_name> # ON WINDOWS: `source activate <your_env_name>`
-        pip install autoviz
-        ```
+        **Prerequisites**
+        - [Anaconda](https://docs.anaconda.com/anaconda/install/)
         
-        To install from source:
+        Create a new environment and install the required dependencies to clone AutoViz:
         
+        **From PyPi:**
         ```sh
         cd <AutoViz_Destination>
         git clone git@github.com:AutoViML/AutoViz.git
         # or download and unzip https://github.com/AutoViML/AutoViz/archive/master.zip
         conda create -n <your_env_name> python=3.7 anaconda
         conda activate <your_env_name> # ON WINDOWS: `source activate <your_env_name>`
         cd AutoViz
         pip install -r requirements.txt
         ```
+        # Usage
+        Discover how to use AutoViz in this <a href="https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad?gi=822a01be6cd0">Medium article</a>.
         
-        ## Usage
-        
-        Read this Medium article to know how to use [AutoViz](https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad).
-        
-        In the AutoViz directory, open a Jupyter Notebook and use this line to instantiate the AutoViz_Class.<br>
-        <b>Alert!</b>: You no longer have to do: `from autoviz.AutoViz_Class import AutoViz_Class`. <br>
-        Instead, you can simply do<br>
+        In the AutoViz directory, open a Jupyter Notebook or on the command terminal and use this line to instantiate the AutoViz_Class. <b>Note: You no longer need to use from autoviz.AutoViz_Class import AutoViz_Class</b>. Instead, simply run:
         
-        ```py
+        ```
         from autoviz import AutoViz_Class
         AV = AutoViz_Class()
+        dft = AV.AutoViz(filename)
         ```
         
-        Load a dataset (any CSV or text file) into a Pandas dataframe or give the name of the path and filename you want to visualize.
-        If you don't have a filename, you can simply assign the filename argument `""` (empty string).
+        Feed AutoViz any input filename (in CSV, txt, or JSON format), and set `max_rows_analyzed` and `max_cols_analyzed` based on memory limitations in your environment, and watch the magic happen!
+        <p>AutoViz generates charts in multiple formats using the `chart_format` setting which can one of the following:
+        - `'png'`, `'svg'`, or `'jpg'`: Inline Matplotlib charts
+            * Save locally (`verbose=2`) or display in Jupyter Notebooks (`verbose=1`)
+            * Default AutoViz behavior
+        - `'bokeh'`: Interactive Bokeh charts in Jupyter Notebooks
+        - `'server'`: Browser-based dashboards with individual chart types
+        - `'html'`: Interactive Bokeh charts saved as HTML files under the `AutoViz_Plots` directory (working folder) or specified directory using the `save_plot_dir` setting
         
-        Call AutoViz method using the filename (or dataframe) along with the separator and the name of the target variable in the input.
-        
-        ```py
-        filename = ""
-        sep = ","
-        dft = AV.AutoViz(
-            filename,
-            sep=",",
-            depVar="",
-            dfte=None,
-            header=0,
-            verbose=0,
-            lowess=False,
-            chart_format="svg",
-            max_rows_analyzed=150000,
-            max_cols_analyzed=30,
-            save_plot_dir=None
-        )
-        ```
-        AutoViz will do the rest. You will see charts and plots on your screen.
+        AutoViz takes care of the rest. You'll see charts and plots on your screen.
         
         ![var_charts](var_charts.JPG)
         
-        `AV.AutoViz` is the main plotting function in AV. Depending on what `chart_format` you choose, AutoViz will automatically call either the `AutoViz_Main` function or `AutoViz_Holo` function.
+        AV.AutoViz is the main plotting function in AutoViz_Class (AV). Depending on the chart_format you choose, AutoViz will automatically call either the AutoViz_Main function or AutoViz_Holo function.
         
-        **Notes:**
+        # API
+        Arguments for AV.AutoViz() method:
         
-        * AutoViz will visualize any sized file using a statistically valid sample.
-        * `COMMA` is assumed as default separator in file. But you can change it.
-        * Assumes first row as header in file but you can change it.
-        - `verbose` option
-          - if 0, display minimal information but displays charts on your notebook
-          - if 1, print extra information on the notebook and also display charts
-          - if 2, will not display any charts, it will simply save them in your local machine under `AutoViz_Plots` directory under your current working folder.
-        
-        - `chart_format` option
-          - if `'svg','jpg' or 'png'`, displays all charts or saves them depending on verbose option.
-          - if `'bokeh'`, plots interactive charts using Bokeh on your Jupyter Notebook
-          - if `'server'`, will display charts on your browser with one chart type in each tab
-          - if `'html'`, will create bokeh interactive charts and silently save them under `AutoViz_Plots` directory or any directory you specify in the `save_plot_dir` setting.
+        - `filename`: Use an empty string ("") if there's no associated filename and you want to use a dataframe; set dfte as the dataframe name. Provide a filename and leave dfte empty to load the dataset.
+        - `sep`: File separator (comma, semi-colon, tab, or any column-separating value).
+        - `depVar`: Target variable in your dataset; leave empty if not applicable.
+        - `dfte`: Input dataframe for plotting charts; leave empty if providing a filename.
+        - `header`: Row number of the header row in your file (0 for the first row).
+        - `verbose`: 0 for minimal info and charts, 1 for more info and charts, or 2 for saving charts locally without display.
+        - `lowess`: Use regression lines for each pair of continuous variables against the target variable in small datasets; avoid using for large datasets (>100,000 rows).
+        - `chart_format`: `'svg', 'png', 'jpg', 'bokeh', 'server', or 'html'` for displaying or saving charts in various formats, depending on the `verbose` option.
+        - `max_rows_analyzed`: Limit the max number of rows for chart display, particularly useful for very large datasets (millions of rows) to reduce chart generation time. A statistically valid sample will be used.
+        - `max_cols_analyzed`: Limit the number of continuous variables to be analyzed.
+        - `save_plot_dir`: Directory for saving plots. Default is None, which saves plots under the current directory in a subfolder named AutoViz_Plots. If the save_plot_dir doesn't exist, it will be created.
         
         ![bokeh_charts](bokeh_charts.JPG)
         
-        ## API
-        
-        **Arguments**
-        
-        - `filename` - Make sure that you give filename as empty string ("") if there is no filename associated with this data and you want to use a dataframe, then use dfte to give the name of the dataframe. Otherwise, fill in the file name and leave dfte as empty string. Only one of these two is needed to load the data set.
-        - `sep` - this is the separator in the file. It can be comma, semi-colon or tab or any value that you see in your file that separates each column.
-        - `depVar` - target variable in your dataset. You can leave it as empty string if you don't have a target variable in your data.
-        - `dfte` - this is the input dataframe in case you want to load a pandas dataframe to plot charts. In that case, leave filename as an empty string.
-        - `header` - the row number of the header row in your file. If it is the first row, then this must be zero.
-        - `verbose` - it has 3 acceptable values: 0, 1 or 2. With zero, you get all charts but limited info. With 1 you get all charts and more info. With 2, you will not see any charts but they will be quietly generated and save in your local current directory under the AutoViz_Plots directory which will be created. Make sure you delete this folder periodically, otherwise, you will have lots of charts saved here if you used verbose=2 option a lot.
-        - `lowess` - this option is very nice for small datasets where you can see regression lines for each pair of continuous variable against the target variable. Don't use this for large data sets (that is over 100,000 rows)
-        - `chart_format` - this can be `'svg', 'png', 'jpg'` or `'bokeh'` or `'server'` or `'html'`. You will get charts generated (inline with `verbose=0` or `1` option). Instead you can silently save them in multiple formats if you used `verbose=2` option. The latter options are useful for interactive charts.
-        - `max_rows_analyzed` - limits the max number of rows that is used to display charts. If you have a very large data set with millions of rows, then use this option to limit the amount of time it takes to generate charts. We will take a statistically valid sample.
-        - `max_cols_analyzed` - limits the number of continuous vars that can be analyzed
-        - `save_plot_dir` - directory you want the plots to be saved. Default is None which means it is saved under the current directory under a sub-folder named `AutoViz_Plots`. If the `save_plot_dir` does not exist, it creates it.
+        ## Additional Notes
+        <ul>
+          <li>AutoViz will visualize any sized file using a statistically valid sample.</li>
+          <li>COMMA is the default separator in the file, but you can change it.</li>
+          <li>Assumes the first row as the header in the file, but this can be changed.</li>
+        </ul>
+        
+        <h3>Verbose Option</h3>
+        <ol>
+          <li>Display minimal information but show charts in your notebook</li>
+          <li>Print extra information on the notebook and display charts</li>
+          <li>Do not display charts; save them locally under the AutoViz_Plots directory in your current working folder.</li>
+        </ol>
+        
+        <h3>Chart Format Option</h3>
+        <ul>
+          <li><code>'svg', 'jpg' or 'png'</code>: Display or save all charts, depending on the verbose option</li>
+          <li><code>'bokeh'</code>: Plot interactive charts using Bokeh in your Jupyter Notebook</li>
+          <li><code>'server'</code>: Display charts in your browser, with one chart type per tab</li>
+          <li><code>'html'</code>: Create interactive Bokeh charts and save them under the AutoViz_Plots directory or the directory specified in the save_plot_dir setting.</li>
+        </ul>
         
         ![server_charts](server_charts.JPG)
         
-        ### Apr-2023 Update: AutoViz now creates scatter plots for categorical variables when data contains only cat variables
-        From version 0.1.600 onwards, AutoViz now automatically draws `catscatter` plots for pairs of categorical variables in a data frame. A `catscatter` plot is a type of scatter plot that shows the frequency of each combination of categories in two variables. It can be useful for exploring the relationship between categorical variables and identifying patterns or outliers. It creates these plots only if the data contains no numeric variables. Otherwise, it doesn't create them since it would be unncessary.
+        # Examples
+        Here are some examples to help you get started with AutoViz:
+        
+        ## Example 1: Visualize a CSV file with a target variable
         
         ```
-        AutoViz is grateful to the cascatter implementation of Myr Barnés, 2020.
-        You can see the original here: https://github.com/myrthings/catscatter/blob/master/catscatter.py
-        # More info about this function here:
-        # - https://towardsdatascience.com/visualize-categorical-relationships-with-catscatter-e60cdb164395
-        # - https://github.com/myrthings/catscatter/blob/master/README.md
-        ```
+        from autoviz import AutoViz_Class
+        AV = AutoViz_Class()
         
-        ### Sep-2022 Update: AutoViz now provides data cleansing suggestions! #autoviz #datacleaning
-        From version 0.1.50 onwards, AutoViz now automatically analyzes your dataset and provides suggestions for how to clean your  data set. It detects missing values, identifies rare categories, finds infinite values, detects mixed data types, and so much more. This will help you tremendously speed up your data cleaning activities. If you have suggestions to add more data cleaning steps please file an `Issue` in our GitHub and we will gladly consider it. Here is an example of how data cleaning suggestions look:<br>
-        <img align="center" src="https://i.ibb.co/NKf1gdg/autoviz-data-cleaning.png">
+        filename = "your_file.csv"
+        target_variable = "your_target_variable"
         
-        In order to get this latest function, you must upgrade autoviz to the latest version by:
-        ```
-        pip install autoviz --upgrade
+        dft = AV.AutoViz(
+            filename,
+            sep=",",
+            depVar=target_variable,
+            dfte=None,
+            header=0,
+            verbose=1,
+            lowess=False,
+            chart_format="svg",
+            max_rows_analyzed=150000,
+            max_cols_analyzed=30,
+            save_plot_dir=None
+        )
         ```
         
-        In the same version, you can also get data suggestions by using `AV.AutoViz(......, verbose=1)` or by simply importing it:<br>
+        ## Example 2: Visualize a Pandas DataFrame without a target variable:
         
         ```
-        from autoviz import data_cleaning_suggestions
-        data_cleaning_suggestions(df)
-        ```
+        import pandas as pd
+        from autoviz import AutoViz_Class
         
-        ### Dec-23-2021 Update: AutoViz now does Wordclouds! #autoviz #wordcloud
-        AutoViz can now create Wordclouds automatically for your NLP variables in data. It detects NLP variables automatically and creates wordclouds for them. See Colab notebook for example: [AutoViz Demo with HTML setting](https://colab.research.google.com/drive/1r5QqESRZDY98FFfDOgVtMAVA_oaGtqqx?usp=sharing)
+        AV = AutoViz_Class()
         
-        <img align="center" src="https://i.postimg.cc/DyT466xP/wordclouds.png">
+        data = {'col1': [1, 2, 3, 4, 5], 'col2': [5, 4, 3, 2, 1]}
+        df = pd.DataFrame(data)
         
-        ### Dec 21, 2021: AutoViz now runs on Docker containers as part of MLOps pipelines. Check out Orchest.io
-        We are excited to announce that AutoViz and Deep_AutoViML are now available as containerized applications on Docker. This means that you can build data pipelines using a fantastic tool like [orchest.io](orchest.io) to build MLOps pipelines visually. Here are two sample pipelines we have created:
+        dft = AV.AutoViz(
+            "",
+            sep=",",
+            depVar="",
+            dfte=df,
+            header=0,
+            verbose=1,
+            lowess=False,
+            chart_format="svg",
+            max_rows_analyzed=150000,
+            max_cols_analyzed=30,
+            save_plot_dir=None
+        )
+        ```
+        
+        ## Example 3: Generate interactive Bokeh charts and save them as HTML files in a custom directory
         
-        <b>AutoViz pipeline</b>: https://lnkd.in/g5uC-z66
-        <b>Deep_AutoViML pipeline</b>: https://lnkd.in/gdnWTqCG
+        ```
+        from autoviz import AutoViz_Class
+        AV = AutoViz_Class()
         
-        You can find more examples and a wonderful video on [orchest's web site](https://github.com/orchest/orchest-examples)
-        ![banner](https://github.com/rsesha/autoviz_pipeline/blob/main/autoviz_orchest.png)
+        filename = "your_file.csv"
+        target_variable = "your_target_variable"
+        custom_plot_dir = "your_custom_plot_directory"
         
-        ### Dec-17-2021 AutoViz now uses HoloViews to display dashboards with Bokeh and save them as Dynamic HTML for web serving #HTML #Bokeh #Holoviews
-        Now you can use AutoViz to create Interactive Bokeh charts and dashboards (see below) either in Jupyter Notebooks or in the browser. Use chart_format as follows:
-        - `chart_format='bokeh'`: interactive Bokeh dashboards are plotted in Jupyter Notebooks.
-        - `chart_format='server'`, dashboards will pop up for each kind of chart on your web browser.
-        - `chart_format='html'`, interactive Bokeh charts will be silently saved as Dynamic HTML files under `AutoViz_Plots` directory
-        <img align="center" src="https://i.postimg.cc/MTCZ6GzQ/Auto-Viz-HTML-dashboards.png" />
+        dft = AV.AutoViz(
+            filename,
+            sep=",",
+            depVar=target_variable,
+            dfte=None,
+            header=0,
+            verbose=2,
+            lowess=False,
+            chart_format="html",
+            max_rows_analyzed=150000,
+            max_cols_analyzed=30,
+            save_plot_dir=custom_plot_dir
+        )
+        ```
         
-        ## Maintainers
+        These examples should give you an idea of how to use AutoViz with different scenarios and settings. By tailoring the options and settings, you can generate visualizations that best suit your needs, whether you're working with large datasets, interactive charts, or simply exploring the relationships between variables.
         
+        # Maintainers
+        AutoViz is actively maintained and improved by a team of dedicated developers. If you have any questions, suggestions or issues, feel free to reach out to the maintainers.
         * [@AutoViML](https://github.com/AutoViML)
         * [@morenoh149](https://github.com/morenoh149)
         * [@hironroy](https://github.com/hironroy)
         
-        ## Contributing
         
-        See [the contributing file](contributing.md)!
+        # Contributing
+        We welcome contributions from the community! If you're interested in contributing to AutoViz, please follow these steps:
         
-        PRs accepted.
+        <h2>Fork the repository on GitHub</h2>
+        <ol>
+          <li>Clone your fork and create a new branch for your feature or bugfix.</li>
+          <li>Commit your changes to the new branch, ensuring that you follow coding standards and write appropriate tests.</li>
+          <li>Push your changes to your fork on GitHub.</li>
+          <li>Submit a pull request to the main repository, detailing your changes and referencing any related issues.</li>
+        </ol>
+        
+        See [the contributing file](contributing.md)!
         
-        ## License
+        # License
+        AutoViz is released under the Apache License, Version 2.0. By using AutoViz, you agree to the terms and conditions specified in the license.
         
-        Apache License, Version 2.0
+        # Tips
+        <p>That covers the main aspects of AutoViz, but here are some additional tips and reminders to help you make the most of the library:</p>
+        <ul>
+          <li>Make sure to regularly upgrade AutoViz to benefit from the <a href="https://github.com/AutoViML/AutoViz/blob/main/updates.md">latest features, bug fixes, and improvements</a>. You can update it using <code>pip install --upgrade autoviz</code>.</li>
+          <li>AutoViz is highly customizable, so don't hesitate to explore and experiment with various settings, such as <code>chart_format</code>, <code>verbose</code>, and <code>max_rows_analyzed</code>. This will allow you to create visualizations that better suit your specific needs and preferences.</li>
+          <li>Remember to delete the <code>AutoViz_Plots</code> directory (or any custom directory you specified) periodically if you used the <code>verbose=2</code> option, as it can accumulate a large number of saved charts over time.</li>
+          <li>For further guidance or inspiration, check out the <a href="https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad">Medium article on AutoViz</a>, as well as other online resources and tutorials.</li>
+          <li>If you encounter any issues, have questions, or want to suggest improvements, don't hesitate to engage with the AutoViz community through the <a href="https://github.com/AutoViML/AutoViz">GitHub repository</a> or other online platforms.</li>
+        </ul>
+        <p>By leveraging AutoViz's powerful and flexible features, you can streamline your data visualization process and gain valuable insights more efficiently. Happy visualizing!</p>
         
         ## DISCLAIMER
         This project is not an official Google project. It is not supported by Google and Google specifically disclaims all warranties as to its quality, merchantability, or fitness for a particular purpose.
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `autoviz-0.1.601/README.md` & `autoviz-0.1.603/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,203 +1,244 @@
-# AutoViz
+# AutoViz: The One-Line Automatic Data Visualization Library
 
-Automatically Visualize any dataset, any size with a single line of code. Now you can save these interactive charts as HTML files automatically with the `"html"` setting.
+![logo](logo.png)
+
+Unlock the power of **AutoViz** to visualize any dataset, any size, with just a single line of code! Plus, now you can save these interactive charts as HTML files automatically with the `html` setting.
 
 [![Pepy Downloads](https://pepy.tech/badge/autoviz)](https://pepy.tech/project/autoviz)
 [![Pepy Downloads per week](https://pepy.tech/badge/autoviz/week)](https://pepy.tech/project/autoviz)
 [![Pepy Downloads per month](https://pepy.tech/badge/autoviz/month)](https://pepy.tech/project/autoviz)
 [![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg)](https://github.com/RichardLitt/standard-readme)
 [![Python Versions](https://img.shields.io/pypi/pyversions/autoviz.svg)](https://pypi.org/project/autoviz)
 [![PyPI Version](https://img.shields.io/pypi/v/autoviz.svg)](https://pypi.org/project/autoviz)
 [![PyPI License](https://img.shields.io/pypi/l/autoviz.svg)](https://github.com/AutoViML/AutoViz/blob/master/LICENSE)
 
-AutoViz performs automatic visualization of any dataset with one line of code.
-Give it any input file (CSV, txt or json format) of any size and AutoViz will visualize it, provided you set the `max_rows_analyzed` and `max_cols_analyzed` setting within the bounds of your machine's memory limit.
-
-AutoViz can now create charts in multiple  formats using the `chart_format` setting:
-- If `chart_format ='png'` or `'svg'` or `'jpg'`: Matplotlib charts are plotted inline.
-    * Can be saved locally (using `verbose=2` setting) or displayed (`verbose=1`) in Jupyter Notebooks.
-    * This is the default behavior for AutoViz.
-- If `chart_format='bokeh'`: Interactive Bokeh charts are plotted in Jupyter Notebooks.
-- If `chart_format='server'`, dashboards will pop up for each kind of chart on your browser.
-- If `chart_format='html'`, interactive Bokeh charts will be created and silently saved as HTML files under the `AutoViz_Plots` directory (under working folder) or any other directory that you specify using the `save_plot_dir` setting (during input).
+With AutoViz, you can easily and quickly generate insightful visualizations for your data. Whether you're a beginner or an expert in data analysis, AutoViz can help you explore your data and uncover valuable insights. Try it out and see the power of automated visualization for yourself!
 
 ## Table of Contents
 
-- [Install](#install)
-- [Usage](#usage)
-- [API](#api)
+- [The purpose and motivation for AutoViz](#motivation)
+- [How to install and setup AutoViz in your environment](#installation)
+- [How to use AutoViz with various options and settings](#usage)
+- [The API and available options](#api)
+- [Examples to get you started](#examples)
 - [Maintainers](#maintainers)
-- [Contributing](#contributing)
+- [Contributing to the project](#contributing)
 - [License](#license)
+- [Additional Tips before you start](#tips)
+- [Disclaimer](#disclaimer)
 
-## Install
+# Motivation
+<p>The motivation to create AutoViz stems from the need for a more efficient, user-friendly, and automated approach to data visualization. Visualizing data is a crucial step in the data analysis process, as it helps users understand patterns, trends, and relationships in the data. However, creating insightful visualizations can be time-consuming and require specialized knowledge of various plotting libraries and techniques.</p>
 
-**Prerequsites**
+<p>AutoViz addresses these challenges by providing an easy-to-use, automated solution for generating meaningful visualizations with minimal effort. Its key motivation is to:</p>
 
-- [Anaconda](https://docs.anaconda.com/anaconda/install/)
+<ol>
+  <li><strong>Save time and effort</strong>: AutoViz simplifies the visualization process by requiring just a single line of code to generate multiple insightful plots, eliminating the need to write multiple lines of code for each chart.</li>
+  <li><strong>Handle large datasets</strong>: AutoViz is designed to work with datasets of any size, intelligently sampling the data when necessary to ensure that the visualizations are generated quickly and efficiently, without compromising on the insights.</li>
+  <li><strong>Accessibility</strong>: AutoViz makes data visualization accessible to a broader audience, including non-experts and beginners in data analysis, by abstracting away the complexities of various plotting libraries.</li>
+  <li><strong>Automate the visualization process</strong>: AutoViz intelligently selects the appropriate visualizations for the given data, taking into account the data types and relationships among variables, which helps users quickly gain insights without having to manually decide which plots to create.</li>
+  <li><strong>Customization and interactivity</strong>: AutoViz offers various options for customization, enabling users to tailor the generated visualizations to their specific needs and preferences. Moreover, with interactive chart formats like Bokeh, users can explore the data more dynamically.</li>
+</ol>
 
-To clone AutoViz, it's better to create a new environment, and install the required dependencies:
+<p>In summary, the motivation behind AutoViz is to make data visualization more efficient, accessible, and automated, enabling users to quickly gain valuable insights from their data and focus on making data-driven decisions.</p>
 
-To install from PyPi:
+## Installation
 
-```sh
-conda create -n <your_env_name> python=3.7 anaconda
-conda activate <your_env_name> # ON WINDOWS: `source activate <your_env_name>`
-pip install autoviz
-```
+**Prerequisites**
+- [Anaconda](https://docs.anaconda.com/anaconda/install/)
 
-To install from source:
+Create a new environment and install the required dependencies to clone AutoViz:
 
+**From PyPi:**
 ```sh
 cd <AutoViz_Destination>
 git clone git@github.com:AutoViML/AutoViz.git
 # or download and unzip https://github.com/AutoViML/AutoViz/archive/master.zip
 conda create -n <your_env_name> python=3.7 anaconda
 conda activate <your_env_name> # ON WINDOWS: `source activate <your_env_name>`
 cd AutoViz
 pip install -r requirements.txt
 ```
+# Usage
+Discover how to use AutoViz in this <a href="https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad?gi=822a01be6cd0">Medium article</a>.
 
-## Usage
-
-Read this Medium article to know how to use [AutoViz](https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad).
-
-In the AutoViz directory, open a Jupyter Notebook and use this line to instantiate the AutoViz_Class.<br>
-<b>Alert!</b>: You no longer have to do: `from autoviz.AutoViz_Class import AutoViz_Class`. <br>
-Instead, you can simply do<br>
+In the AutoViz directory, open a Jupyter Notebook or on the command terminal and use this line to instantiate the AutoViz_Class. <b>Note: You no longer need to use from autoviz.AutoViz_Class import AutoViz_Class</b>. Instead, simply run:
 
-```py
+```
 from autoviz import AutoViz_Class
 AV = AutoViz_Class()
+dft = AV.AutoViz(filename)
 ```
 
-Load a dataset (any CSV or text file) into a Pandas dataframe or give the name of the path and filename you want to visualize.
-If you don't have a filename, you can simply assign the filename argument `""` (empty string).
+Feed AutoViz any input filename (in CSV, txt, or JSON format), and set `max_rows_analyzed` and `max_cols_analyzed` based on memory limitations in your environment, and watch the magic happen!
+<p>AutoViz generates charts in multiple formats using the `chart_format` setting which can one of the following:
+- `'png'`, `'svg'`, or `'jpg'`: Inline Matplotlib charts
+    * Save locally (`verbose=2`) or display in Jupyter Notebooks (`verbose=1`)
+    * Default AutoViz behavior
+- `'bokeh'`: Interactive Bokeh charts in Jupyter Notebooks
+- `'server'`: Browser-based dashboards with individual chart types
+- `'html'`: Interactive Bokeh charts saved as HTML files under the `AutoViz_Plots` directory (working folder) or specified directory using the `save_plot_dir` setting
 
-Call AutoViz method using the filename (or dataframe) along with the separator and the name of the target variable in the input.
-
-```py
-filename = ""
-sep = ","
-dft = AV.AutoViz(
-    filename,
-    sep=",",
-    depVar="",
-    dfte=None,
-    header=0,
-    verbose=0,
-    lowess=False,
-    chart_format="svg",
-    max_rows_analyzed=150000,
-    max_cols_analyzed=30,
-    save_plot_dir=None
-)
-```
-AutoViz will do the rest. You will see charts and plots on your screen.
+AutoViz takes care of the rest. You'll see charts and plots on your screen.
 
 ![var_charts](var_charts.JPG)
 
-`AV.AutoViz` is the main plotting function in AV. Depending on what `chart_format` you choose, AutoViz will automatically call either the `AutoViz_Main` function or `AutoViz_Holo` function.
+AV.AutoViz is the main plotting function in AutoViz_Class (AV). Depending on the chart_format you choose, AutoViz will automatically call either the AutoViz_Main function or AutoViz_Holo function.
 
-**Notes:**
+# API
+Arguments for AV.AutoViz() method:
 
-* AutoViz will visualize any sized file using a statistically valid sample.
-* `COMMA` is assumed as default separator in file. But you can change it.
-* Assumes first row as header in file but you can change it.
-- `verbose` option
-  - if 0, display minimal information but displays charts on your notebook
-  - if 1, print extra information on the notebook and also display charts
-  - if 2, will not display any charts, it will simply save them in your local machine under `AutoViz_Plots` directory under your current working folder.
-
-- `chart_format` option
-  - if `'svg','jpg' or 'png'`, displays all charts or saves them depending on verbose option.
-  - if `'bokeh'`, plots interactive charts using Bokeh on your Jupyter Notebook
-  - if `'server'`, will display charts on your browser with one chart type in each tab
-  - if `'html'`, will create bokeh interactive charts and silently save them under `AutoViz_Plots` directory or any directory you specify in the `save_plot_dir` setting.
+- `filename`: Use an empty string ("") if there's no associated filename and you want to use a dataframe; set dfte as the dataframe name. Provide a filename and leave dfte empty to load the dataset.
+- `sep`: File separator (comma, semi-colon, tab, or any column-separating value).
+- `depVar`: Target variable in your dataset; leave empty if not applicable.
+- `dfte`: Input dataframe for plotting charts; leave empty if providing a filename.
+- `header`: Row number of the header row in your file (0 for the first row).
+- `verbose`: 0 for minimal info and charts, 1 for more info and charts, or 2 for saving charts locally without display.
+- `lowess`: Use regression lines for each pair of continuous variables against the target variable in small datasets; avoid using for large datasets (>100,000 rows).
+- `chart_format`: `'svg', 'png', 'jpg', 'bokeh', 'server', or 'html'` for displaying or saving charts in various formats, depending on the `verbose` option.
+- `max_rows_analyzed`: Limit the max number of rows for chart display, particularly useful for very large datasets (millions of rows) to reduce chart generation time. A statistically valid sample will be used.
+- `max_cols_analyzed`: Limit the number of continuous variables to be analyzed.
+- `save_plot_dir`: Directory for saving plots. Default is None, which saves plots under the current directory in a subfolder named AutoViz_Plots. If the save_plot_dir doesn't exist, it will be created.
 
 ![bokeh_charts](bokeh_charts.JPG)
 
-## API
-
-**Arguments**
-
-- `filename` - Make sure that you give filename as empty string ("") if there is no filename associated with this data and you want to use a dataframe, then use dfte to give the name of the dataframe. Otherwise, fill in the file name and leave dfte as empty string. Only one of these two is needed to load the data set.
-- `sep` - this is the separator in the file. It can be comma, semi-colon or tab or any value that you see in your file that separates each column.
-- `depVar` - target variable in your dataset. You can leave it as empty string if you don't have a target variable in your data.
-- `dfte` - this is the input dataframe in case you want to load a pandas dataframe to plot charts. In that case, leave filename as an empty string.
-- `header` - the row number of the header row in your file. If it is the first row, then this must be zero.
-- `verbose` - it has 3 acceptable values: 0, 1 or 2. With zero, you get all charts but limited info. With 1 you get all charts and more info. With 2, you will not see any charts but they will be quietly generated and save in your local current directory under the AutoViz_Plots directory which will be created. Make sure you delete this folder periodically, otherwise, you will have lots of charts saved here if you used verbose=2 option a lot.
-- `lowess` - this option is very nice for small datasets where you can see regression lines for each pair of continuous variable against the target variable. Don't use this for large data sets (that is over 100,000 rows)
-- `chart_format` - this can be `'svg', 'png', 'jpg'` or `'bokeh'` or `'server'` or `'html'`. You will get charts generated (inline with `verbose=0` or `1` option). Instead you can silently save them in multiple formats if you used `verbose=2` option. The latter options are useful for interactive charts.
-- `max_rows_analyzed` - limits the max number of rows that is used to display charts. If you have a very large data set with millions of rows, then use this option to limit the amount of time it takes to generate charts. We will take a statistically valid sample.
-- `max_cols_analyzed` - limits the number of continuous vars that can be analyzed
-- `save_plot_dir` - directory you want the plots to be saved. Default is None which means it is saved under the current directory under a sub-folder named `AutoViz_Plots`. If the `save_plot_dir` does not exist, it creates it.
+## Additional Notes
+<ul>
+  <li>AutoViz will visualize any sized file using a statistically valid sample.</li>
+  <li>COMMA is the default separator in the file, but you can change it.</li>
+  <li>Assumes the first row as the header in the file, but this can be changed.</li>
+</ul>
+
+<h3>Verbose Option</h3>
+<ol>
+  <li>Display minimal information but show charts in your notebook</li>
+  <li>Print extra information on the notebook and display charts</li>
+  <li>Do not display charts; save them locally under the AutoViz_Plots directory in your current working folder.</li>
+</ol>
+
+<h3>Chart Format Option</h3>
+<ul>
+  <li><code>'svg', 'jpg' or 'png'</code>: Display or save all charts, depending on the verbose option</li>
+  <li><code>'bokeh'</code>: Plot interactive charts using Bokeh in your Jupyter Notebook</li>
+  <li><code>'server'</code>: Display charts in your browser, with one chart type per tab</li>
+  <li><code>'html'</code>: Create interactive Bokeh charts and save them under the AutoViz_Plots directory or the directory specified in the save_plot_dir setting.</li>
+</ul>
 
 ![server_charts](server_charts.JPG)
 
-### Apr-2023 Update: AutoViz now creates scatter plots for categorical variables when data contains only cat variables
-From version 0.1.600 onwards, AutoViz now automatically draws `catscatter` plots for pairs of categorical variables in a data frame. A `catscatter` plot is a type of scatter plot that shows the frequency of each combination of categories in two variables. It can be useful for exploring the relationship between categorical variables and identifying patterns or outliers. It creates these plots only if the data contains no numeric variables. Otherwise, it doesn't create them since it would be unncessary.
+# Examples
+Here are some examples to help you get started with AutoViz:
+
+## Example 1: Visualize a CSV file with a target variable
 
 ```
-AutoViz is grateful to the cascatter implementation of Myr Barnés, 2020.
-You can see the original here: https://github.com/myrthings/catscatter/blob/master/catscatter.py
-# More info about this function here:
-# - https://towardsdatascience.com/visualize-categorical-relationships-with-catscatter-e60cdb164395
-# - https://github.com/myrthings/catscatter/blob/master/README.md
-```
+from autoviz import AutoViz_Class
+AV = AutoViz_Class()
 
-### Sep-2022 Update: AutoViz now provides data cleansing suggestions! #autoviz #datacleaning
-From version 0.1.50 onwards, AutoViz now automatically analyzes your dataset and provides suggestions for how to clean your  data set. It detects missing values, identifies rare categories, finds infinite values, detects mixed data types, and so much more. This will help you tremendously speed up your data cleaning activities. If you have suggestions to add more data cleaning steps please file an `Issue` in our GitHub and we will gladly consider it. Here is an example of how data cleaning suggestions look:<br>
-<img align="center" src="https://i.ibb.co/NKf1gdg/autoviz-data-cleaning.png">
+filename = "your_file.csv"
+target_variable = "your_target_variable"
 
-In order to get this latest function, you must upgrade autoviz to the latest version by:
-```
-pip install autoviz --upgrade
+dft = AV.AutoViz(
+    filename,
+    sep=",",
+    depVar=target_variable,
+    dfte=None,
+    header=0,
+    verbose=1,
+    lowess=False,
+    chart_format="svg",
+    max_rows_analyzed=150000,
+    max_cols_analyzed=30,
+    save_plot_dir=None
+)
 ```
 
-In the same version, you can also get data suggestions by using `AV.AutoViz(......, verbose=1)` or by simply importing it:<br>
+## Example 2: Visualize a Pandas DataFrame without a target variable:
 
 ```
-from autoviz import data_cleaning_suggestions
-data_cleaning_suggestions(df)
-```
+import pandas as pd
+from autoviz import AutoViz_Class
 
-### Dec-23-2021 Update: AutoViz now does Wordclouds! #autoviz #wordcloud
-AutoViz can now create Wordclouds automatically for your NLP variables in data. It detects NLP variables automatically and creates wordclouds for them. See Colab notebook for example: [AutoViz Demo with HTML setting](https://colab.research.google.com/drive/1r5QqESRZDY98FFfDOgVtMAVA_oaGtqqx?usp=sharing)
+AV = AutoViz_Class()
 
-<img align="center" src="https://i.postimg.cc/DyT466xP/wordclouds.png">
+data = {'col1': [1, 2, 3, 4, 5], 'col2': [5, 4, 3, 2, 1]}
+df = pd.DataFrame(data)
 
-### Dec 21, 2021: AutoViz now runs on Docker containers as part of MLOps pipelines. Check out Orchest.io
-We are excited to announce that AutoViz and Deep_AutoViML are now available as containerized applications on Docker. This means that you can build data pipelines using a fantastic tool like [orchest.io](orchest.io) to build MLOps pipelines visually. Here are two sample pipelines we have created:
+dft = AV.AutoViz(
+    "",
+    sep=",",
+    depVar="",
+    dfte=df,
+    header=0,
+    verbose=1,
+    lowess=False,
+    chart_format="svg",
+    max_rows_analyzed=150000,
+    max_cols_analyzed=30,
+    save_plot_dir=None
+)
+```
+
+## Example 3: Generate interactive Bokeh charts and save them as HTML files in a custom directory
 
-<b>AutoViz pipeline</b>: https://lnkd.in/g5uC-z66
-<b>Deep_AutoViML pipeline</b>: https://lnkd.in/gdnWTqCG
+```
+from autoviz import AutoViz_Class
+AV = AutoViz_Class()
 
-You can find more examples and a wonderful video on [orchest's web site](https://github.com/orchest/orchest-examples)
-![banner](https://github.com/rsesha/autoviz_pipeline/blob/main/autoviz_orchest.png)
+filename = "your_file.csv"
+target_variable = "your_target_variable"
+custom_plot_dir = "your_custom_plot_directory"
 
-### Dec-17-2021 AutoViz now uses HoloViews to display dashboards with Bokeh and save them as Dynamic HTML for web serving #HTML #Bokeh #Holoviews
-Now you can use AutoViz to create Interactive Bokeh charts and dashboards (see below) either in Jupyter Notebooks or in the browser. Use chart_format as follows:
-- `chart_format='bokeh'`: interactive Bokeh dashboards are plotted in Jupyter Notebooks.
-- `chart_format='server'`, dashboards will pop up for each kind of chart on your web browser.
-- `chart_format='html'`, interactive Bokeh charts will be silently saved as Dynamic HTML files under `AutoViz_Plots` directory
-<img align="center" src="https://i.postimg.cc/MTCZ6GzQ/Auto-Viz-HTML-dashboards.png" />
+dft = AV.AutoViz(
+    filename,
+    sep=",",
+    depVar=target_variable,
+    dfte=None,
+    header=0,
+    verbose=2,
+    lowess=False,
+    chart_format="html",
+    max_rows_analyzed=150000,
+    max_cols_analyzed=30,
+    save_plot_dir=custom_plot_dir
+)
+```
 
-## Maintainers
+These examples should give you an idea of how to use AutoViz with different scenarios and settings. By tailoring the options and settings, you can generate visualizations that best suit your needs, whether you're working with large datasets, interactive charts, or simply exploring the relationships between variables.
 
+# Maintainers
+AutoViz is actively maintained and improved by a team of dedicated developers. If you have any questions, suggestions or issues, feel free to reach out to the maintainers.
 * [@AutoViML](https://github.com/AutoViML)
 * [@morenoh149](https://github.com/morenoh149)
 * [@hironroy](https://github.com/hironroy)
 
-## Contributing
 
-See [the contributing file](contributing.md)!
+# Contributing
+We welcome contributions from the community! If you're interested in contributing to AutoViz, please follow these steps:
 
-PRs accepted.
+<h2>Fork the repository on GitHub</h2>
+<ol>
+  <li>Clone your fork and create a new branch for your feature or bugfix.</li>
+  <li>Commit your changes to the new branch, ensuring that you follow coding standards and write appropriate tests.</li>
+  <li>Push your changes to your fork on GitHub.</li>
+  <li>Submit a pull request to the main repository, detailing your changes and referencing any related issues.</li>
+</ol>
+
+See [the contributing file](contributing.md)!
 
-## License
+# License
+AutoViz is released under the Apache License, Version 2.0. By using AutoViz, you agree to the terms and conditions specified in the license.
 
-Apache License, Version 2.0
+# Tips
+<p>That covers the main aspects of AutoViz, but here are some additional tips and reminders to help you make the most of the library:</p>
+<ul>
+  <li>Make sure to regularly upgrade AutoViz to benefit from the <a href="https://github.com/AutoViML/AutoViz/blob/main/updates.md">latest features, bug fixes, and improvements</a>. You can update it using <code>pip install --upgrade autoviz</code>.</li>
+  <li>AutoViz is highly customizable, so don't hesitate to explore and experiment with various settings, such as <code>chart_format</code>, <code>verbose</code>, and <code>max_rows_analyzed</code>. This will allow you to create visualizations that better suit your specific needs and preferences.</li>
+  <li>Remember to delete the <code>AutoViz_Plots</code> directory (or any custom directory you specified) periodically if you used the <code>verbose=2</code> option, as it can accumulate a large number of saved charts over time.</li>
+  <li>For further guidance or inspiration, check out the <a href="https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad">Medium article on AutoViz</a>, as well as other online resources and tutorials.</li>
+  <li>If you encounter any issues, have questions, or want to suggest improvements, don't hesitate to engage with the AutoViz community through the <a href="https://github.com/AutoViML/AutoViz">GitHub repository</a> or other online platforms.</li>
+</ul>
+<p>By leveraging AutoViz's powerful and flexible features, you can streamline your data visualization process and gain valuable insights more efficiently. Happy visualizing!</p>
 
 ## DISCLAIMER
 This project is not an official Google project. It is not supported by Google and Google specifically disclaims all warranties as to its quality, merchantability, or fitness for a particular purpose.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `autoviz-0.1.601/autoviz/AutoViz_Class.py` & `autoviz-0.1.603/autoviz/AutoViz_Class.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.601/autoviz/AutoViz_Holo.py` & `autoviz-0.1.603/autoviz/AutoViz_Holo.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.601/autoviz/AutoViz_NLP.py` & `autoviz-0.1.603/autoviz/AutoViz_NLP.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.601/autoviz/AutoViz_Utils.py` & `autoviz-0.1.603/autoviz/AutoViz_Utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,21 +212,28 @@
             #color1 = random.choice(colormaps)
             color1 = "Set1"
             data = pd.DataFrame(dicti)
             x=dft[var1]
             ax1 = fig.add_subplot(rows,cols,counter)
             nocats = min(categorylimit,dft[var1].nunique())
             data = dft[var1].value_counts()
-            if problem_type != 'Binary_Classification' or problem_type != 'Multi_Classification':
-                sns.countplot(x=var1,
-                                data=dft,
-                                ax=ax1,
-                                order=dft[var1].value_counts().index,
-                                hue = depVar)
-                ax1.set_title('Distribution of %s by %s' %(var1, depVar),fontsize=12)
+            if problem_type in ['Binary_Classification', 'Multi_Classification']:
+                if dft[depVar].nunique() > 15:
+                    sns.countplot(x=var1,
+                                    data=dft,
+                                    ax=ax1,
+                                    order=dft[var1].value_counts().index,)
+                    ax1.set_title('Distribution of %s' %var1,fontsize=12)
+                else:
+                    sns.countplot(x=var1,
+                                    data=dft,
+                                    ax=ax1,
+                                    order=dft[var1].value_counts().index,
+                                    hue = depVar)
+                    ax1.set_title('Distribution of %s by %s' %(var1, depVar),fontsize=12)
             else:
                 sns.countplot(x=var1,
                                 data=dft,
                                 ax=ax1,
                                 order=dft[var1].value_counts().index,)
                 ax1.set_title('Distribution of %s' %var1,fontsize=12)
             ax1.set_xlabel(var1)
@@ -779,14 +786,15 @@
         #sns.color_palette("Set1")
         sns.set_palette("Set1")
         ##### First draw all the numeric variables in row after row #############
         if not len(conti) == 0:
             cols = 3
             rows = len(conti)
             fig, axes = plt.subplots(rows, cols, figsize=(width_size,rows*height_size))
+            fig.subplots_adjust(hspace=gap) ### This controls the space betwen rows            
             k = 1
             binsize = 30
             for each_conti in conti:
                 color1 = next(colors)
                 ax1 = plt.subplot(rows, cols, k)
                 dft[each_conti].hist(
                     bins=binsize, 
@@ -800,17 +808,17 @@
                 k += 1
                 ax3 = plt.subplot(rows, cols, k)
                 probplot(dft[each_conti], plot=ax3)
                 k += 1
                 skew_val=round(dft[each_conti].skew(), 1)
                 ax2.set_yticklabels([])
                 ax2.set_yticks([])
-                ax1.set_title(each_conti + " | Distplot")
-                ax2.set_title(each_conti + " | Boxplot")
-                ax3.set_title(each_conti + " | Probability Plot - Skew: "+str(skew_val))
+                ax1.set_title(each_conti + " | Distplot", fontsize=9)
+                ax2.set_title(each_conti + " | Boxplot", fontsize=9)
+                ax3.set_title(each_conti + " | Probability Plot - Skew: "+str(skew_val), fontsize=9)
             ###### Save the plots to disk if verbose = 2 ############
             if verbose == 2:
                 imgdata_list.append(save_image_data(fig, chart_format,
                                 plot_name+'_Numeric', dep, mk_dir))
                 image_count += 1
         #####  Now draw each of the categorical variable distributions in each subplot ####
         if not len(cats) == 0:
@@ -834,23 +842,23 @@
                 else:
                     dft[each_cat].value_counts(normalize=True, dropna=False)[:width_size].plot(kind='bar', 
                                             color=color2,
                                             ax=ax1,label='%s' %each_cat)
                     labels = dft[each_cat].value_counts(dropna=False)[:width_size].index.tolist()
                 k += 1
                 ax1.set_xticklabels(labels,**kwds);
-                ax1.set_title('Normalized distribution of %s (top %d categories only)' %(each_cat,width_size))
+                ax1.set_title('Norm. disti.of %s (top %d categories only)' %(each_cat,width_size), fontsize=9)
             fig.tight_layout();
             
             ########## This is where you end the logic for distplots ################
             if verbose == 2:
                 imgdata_list.append(save_image_data(fig, chart_format,
                                 plot_name+'_Cats', dep, mk_dir))
                 image_count += 1
-            fig.suptitle('Histograms and Normalized distribitions of all variables', fontsize=12,y=1.01)
+            fig.suptitle('Histograms and Normalized distribitions of all variables', fontsize=12, y=1.01)
             if verbose <= 1:
                 plt.show();
     else:
         ######### This is for Classification problems only ########
         #### Now you can draw both object and numeric variables using same conti variable
         #sns.color_palette("Set1")
         sns.set_palette("Set1")
@@ -1702,15 +1710,15 @@
     else:
         continuous_vars = var_df['continuous_vars']
     #### from now you can use wordclouds on discrete_string_vars ######################
     preds = [x for x in orig_preds if x not in IDcols+cols_delete]
     if len(IDcols+cols_delete) == 0:
         print('        No variables removed since no ID or low-information variables found in data set')
     else:
-        print('        %d variables removed since they were ID or low-information variables'
+        print('        %d variable(s) removed since they were ID or low-information variables'
                                 %len(IDcols+cols_delete))
         if verbose >= 1:
             print('        List of variables removed: %s' %(IDcols+cols_delete))
     #############    Sample data if too big and find problem type   #############################
     if dfte.shape[0]>= max_rows_analyzed:
         print('Since Number of Rows in data %d exceeds maximum, randomly sampling %d rows for EDA...' %(len(dfte),max_rows_analyzed))
         dft = dfte.sample(max_rows_analyzed, random_state=0)
@@ -1785,15 +1793,15 @@
             else:
                 continuous_vars = var_df['continuous_vars']
             date_vars = var_df['date_vars']
             preds = [x for x in important_features if x not in IDcols+cols_delete+discrete_string_vars]
             if len(IDcols+cols_delete+discrete_string_vars) == 0:
                 print('    No variables removed since no ID or low-information variables found in data')
             else:
-                print('    %d variables removed since they were ID or low-information variables'
+                print('    %d variable(s) removed since they were ID or low-information variables'
                                         %len(IDcols+cols_delete+discrete_string_vars))
             if verbose >= 1:
                 print('    List of variables removed: %s' %(IDcols+cols_delete+discrete_string_vars))
             dft = dft[preds+[depVar]]
         else:
             continuous_vars = continuous_vars[:max_cols_analyzed]
             print('%d numeric variables in data exceeds limit, taking top %d variables' %(len(
```

### Comparing `autoviz-0.1.601/autoviz/__init__.py` & `autoviz-0.1.603/autoviz/__init__.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.601/autoviz/classify_method.py` & `autoviz-0.1.603/autoviz/classify_method.py`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.601/autoviz.egg-info/PKG-INFO` & `autoviz-0.1.603/autoviz.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,214 +1,255 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.601
+Version: 0.1.603
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz
 Author: Ram Seshadri
 License: Apache License 2.0
-Description: # AutoViz
+Description: # AutoViz: The One-Line Automatic Data Visualization Library
         
-        Automatically Visualize any dataset, any size with a single line of code. Now you can save these interactive charts as HTML files automatically with the `"html"` setting.
+        ![logo](logo.png)
+        
+        Unlock the power of **AutoViz** to visualize any dataset, any size, with just a single line of code! Plus, now you can save these interactive charts as HTML files automatically with the `html` setting.
         
         [![Pepy Downloads](https://pepy.tech/badge/autoviz)](https://pepy.tech/project/autoviz)
         [![Pepy Downloads per week](https://pepy.tech/badge/autoviz/week)](https://pepy.tech/project/autoviz)
         [![Pepy Downloads per month](https://pepy.tech/badge/autoviz/month)](https://pepy.tech/project/autoviz)
         [![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg)](https://github.com/RichardLitt/standard-readme)
         [![Python Versions](https://img.shields.io/pypi/pyversions/autoviz.svg)](https://pypi.org/project/autoviz)
         [![PyPI Version](https://img.shields.io/pypi/v/autoviz.svg)](https://pypi.org/project/autoviz)
         [![PyPI License](https://img.shields.io/pypi/l/autoviz.svg)](https://github.com/AutoViML/AutoViz/blob/master/LICENSE)
         
-        AutoViz performs automatic visualization of any dataset with one line of code.
-        Give it any input file (CSV, txt or json format) of any size and AutoViz will visualize it, provided you set the `max_rows_analyzed` and `max_cols_analyzed` setting within the bounds of your machine's memory limit.
-        
-        AutoViz can now create charts in multiple  formats using the `chart_format` setting:
-        - If `chart_format ='png'` or `'svg'` or `'jpg'`: Matplotlib charts are plotted inline.
-            * Can be saved locally (using `verbose=2` setting) or displayed (`verbose=1`) in Jupyter Notebooks.
-            * This is the default behavior for AutoViz.
-        - If `chart_format='bokeh'`: Interactive Bokeh charts are plotted in Jupyter Notebooks.
-        - If `chart_format='server'`, dashboards will pop up for each kind of chart on your browser.
-        - If `chart_format='html'`, interactive Bokeh charts will be created and silently saved as HTML files under the `AutoViz_Plots` directory (under working folder) or any other directory that you specify using the `save_plot_dir` setting (during input).
+        With AutoViz, you can easily and quickly generate insightful visualizations for your data. Whether you're a beginner or an expert in data analysis, AutoViz can help you explore your data and uncover valuable insights. Try it out and see the power of automated visualization for yourself!
         
         ## Table of Contents
         
-        - [Install](#install)
-        - [Usage](#usage)
-        - [API](#api)
+        - [The purpose and motivation for AutoViz](#motivation)
+        - [How to install and setup AutoViz in your environment](#installation)
+        - [How to use AutoViz with various options and settings](#usage)
+        - [The API and available options](#api)
+        - [Examples to get you started](#examples)
         - [Maintainers](#maintainers)
-        - [Contributing](#contributing)
+        - [Contributing to the project](#contributing)
         - [License](#license)
+        - [Additional Tips before you start](#tips)
+        - [Disclaimer](#disclaimer)
         
-        ## Install
+        # Motivation
+        <p>The motivation to create AutoViz stems from the need for a more efficient, user-friendly, and automated approach to data visualization. Visualizing data is a crucial step in the data analysis process, as it helps users understand patterns, trends, and relationships in the data. However, creating insightful visualizations can be time-consuming and require specialized knowledge of various plotting libraries and techniques.</p>
         
-        **Prerequsites**
+        <p>AutoViz addresses these challenges by providing an easy-to-use, automated solution for generating meaningful visualizations with minimal effort. Its key motivation is to:</p>
         
-        - [Anaconda](https://docs.anaconda.com/anaconda/install/)
+        <ol>
+          <li><strong>Save time and effort</strong>: AutoViz simplifies the visualization process by requiring just a single line of code to generate multiple insightful plots, eliminating the need to write multiple lines of code for each chart.</li>
+          <li><strong>Handle large datasets</strong>: AutoViz is designed to work with datasets of any size, intelligently sampling the data when necessary to ensure that the visualizations are generated quickly and efficiently, without compromising on the insights.</li>
+          <li><strong>Accessibility</strong>: AutoViz makes data visualization accessible to a broader audience, including non-experts and beginners in data analysis, by abstracting away the complexities of various plotting libraries.</li>
+          <li><strong>Automate the visualization process</strong>: AutoViz intelligently selects the appropriate visualizations for the given data, taking into account the data types and relationships among variables, which helps users quickly gain insights without having to manually decide which plots to create.</li>
+          <li><strong>Customization and interactivity</strong>: AutoViz offers various options for customization, enabling users to tailor the generated visualizations to their specific needs and preferences. Moreover, with interactive chart formats like Bokeh, users can explore the data more dynamically.</li>
+        </ol>
         
-        To clone AutoViz, it's better to create a new environment, and install the required dependencies:
+        <p>In summary, the motivation behind AutoViz is to make data visualization more efficient, accessible, and automated, enabling users to quickly gain valuable insights from their data and focus on making data-driven decisions.</p>
         
-        To install from PyPi:
+        ## Installation
         
-        ```sh
-        conda create -n <your_env_name> python=3.7 anaconda
-        conda activate <your_env_name> # ON WINDOWS: `source activate <your_env_name>`
-        pip install autoviz
-        ```
+        **Prerequisites**
+        - [Anaconda](https://docs.anaconda.com/anaconda/install/)
         
-        To install from source:
+        Create a new environment and install the required dependencies to clone AutoViz:
         
+        **From PyPi:**
         ```sh
         cd <AutoViz_Destination>
         git clone git@github.com:AutoViML/AutoViz.git
         # or download and unzip https://github.com/AutoViML/AutoViz/archive/master.zip
         conda create -n <your_env_name> python=3.7 anaconda
         conda activate <your_env_name> # ON WINDOWS: `source activate <your_env_name>`
         cd AutoViz
         pip install -r requirements.txt
         ```
+        # Usage
+        Discover how to use AutoViz in this <a href="https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad?gi=822a01be6cd0">Medium article</a>.
         
-        ## Usage
-        
-        Read this Medium article to know how to use [AutoViz](https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad).
-        
-        In the AutoViz directory, open a Jupyter Notebook and use this line to instantiate the AutoViz_Class.<br>
-        <b>Alert!</b>: You no longer have to do: `from autoviz.AutoViz_Class import AutoViz_Class`. <br>
-        Instead, you can simply do<br>
+        In the AutoViz directory, open a Jupyter Notebook or on the command terminal and use this line to instantiate the AutoViz_Class. <b>Note: You no longer need to use from autoviz.AutoViz_Class import AutoViz_Class</b>. Instead, simply run:
         
-        ```py
+        ```
         from autoviz import AutoViz_Class
         AV = AutoViz_Class()
+        dft = AV.AutoViz(filename)
         ```
         
-        Load a dataset (any CSV or text file) into a Pandas dataframe or give the name of the path and filename you want to visualize.
-        If you don't have a filename, you can simply assign the filename argument `""` (empty string).
+        Feed AutoViz any input filename (in CSV, txt, or JSON format), and set `max_rows_analyzed` and `max_cols_analyzed` based on memory limitations in your environment, and watch the magic happen!
+        <p>AutoViz generates charts in multiple formats using the `chart_format` setting which can one of the following:
+        - `'png'`, `'svg'`, or `'jpg'`: Inline Matplotlib charts
+            * Save locally (`verbose=2`) or display in Jupyter Notebooks (`verbose=1`)
+            * Default AutoViz behavior
+        - `'bokeh'`: Interactive Bokeh charts in Jupyter Notebooks
+        - `'server'`: Browser-based dashboards with individual chart types
+        - `'html'`: Interactive Bokeh charts saved as HTML files under the `AutoViz_Plots` directory (working folder) or specified directory using the `save_plot_dir` setting
         
-        Call AutoViz method using the filename (or dataframe) along with the separator and the name of the target variable in the input.
-        
-        ```py
-        filename = ""
-        sep = ","
-        dft = AV.AutoViz(
-            filename,
-            sep=",",
-            depVar="",
-            dfte=None,
-            header=0,
-            verbose=0,
-            lowess=False,
-            chart_format="svg",
-            max_rows_analyzed=150000,
-            max_cols_analyzed=30,
-            save_plot_dir=None
-        )
-        ```
-        AutoViz will do the rest. You will see charts and plots on your screen.
+        AutoViz takes care of the rest. You'll see charts and plots on your screen.
         
         ![var_charts](var_charts.JPG)
         
-        `AV.AutoViz` is the main plotting function in AV. Depending on what `chart_format` you choose, AutoViz will automatically call either the `AutoViz_Main` function or `AutoViz_Holo` function.
+        AV.AutoViz is the main plotting function in AutoViz_Class (AV). Depending on the chart_format you choose, AutoViz will automatically call either the AutoViz_Main function or AutoViz_Holo function.
         
-        **Notes:**
+        # API
+        Arguments for AV.AutoViz() method:
         
-        * AutoViz will visualize any sized file using a statistically valid sample.
-        * `COMMA` is assumed as default separator in file. But you can change it.
-        * Assumes first row as header in file but you can change it.
-        - `verbose` option
-          - if 0, display minimal information but displays charts on your notebook
-          - if 1, print extra information on the notebook and also display charts
-          - if 2, will not display any charts, it will simply save them in your local machine under `AutoViz_Plots` directory under your current working folder.
-        
-        - `chart_format` option
-          - if `'svg','jpg' or 'png'`, displays all charts or saves them depending on verbose option.
-          - if `'bokeh'`, plots interactive charts using Bokeh on your Jupyter Notebook
-          - if `'server'`, will display charts on your browser with one chart type in each tab
-          - if `'html'`, will create bokeh interactive charts and silently save them under `AutoViz_Plots` directory or any directory you specify in the `save_plot_dir` setting.
+        - `filename`: Use an empty string ("") if there's no associated filename and you want to use a dataframe; set dfte as the dataframe name. Provide a filename and leave dfte empty to load the dataset.
+        - `sep`: File separator (comma, semi-colon, tab, or any column-separating value).
+        - `depVar`: Target variable in your dataset; leave empty if not applicable.
+        - `dfte`: Input dataframe for plotting charts; leave empty if providing a filename.
+        - `header`: Row number of the header row in your file (0 for the first row).
+        - `verbose`: 0 for minimal info and charts, 1 for more info and charts, or 2 for saving charts locally without display.
+        - `lowess`: Use regression lines for each pair of continuous variables against the target variable in small datasets; avoid using for large datasets (>100,000 rows).
+        - `chart_format`: `'svg', 'png', 'jpg', 'bokeh', 'server', or 'html'` for displaying or saving charts in various formats, depending on the `verbose` option.
+        - `max_rows_analyzed`: Limit the max number of rows for chart display, particularly useful for very large datasets (millions of rows) to reduce chart generation time. A statistically valid sample will be used.
+        - `max_cols_analyzed`: Limit the number of continuous variables to be analyzed.
+        - `save_plot_dir`: Directory for saving plots. Default is None, which saves plots under the current directory in a subfolder named AutoViz_Plots. If the save_plot_dir doesn't exist, it will be created.
         
         ![bokeh_charts](bokeh_charts.JPG)
         
-        ## API
-        
-        **Arguments**
-        
-        - `filename` - Make sure that you give filename as empty string ("") if there is no filename associated with this data and you want to use a dataframe, then use dfte to give the name of the dataframe. Otherwise, fill in the file name and leave dfte as empty string. Only one of these two is needed to load the data set.
-        - `sep` - this is the separator in the file. It can be comma, semi-colon or tab or any value that you see in your file that separates each column.
-        - `depVar` - target variable in your dataset. You can leave it as empty string if you don't have a target variable in your data.
-        - `dfte` - this is the input dataframe in case you want to load a pandas dataframe to plot charts. In that case, leave filename as an empty string.
-        - `header` - the row number of the header row in your file. If it is the first row, then this must be zero.
-        - `verbose` - it has 3 acceptable values: 0, 1 or 2. With zero, you get all charts but limited info. With 1 you get all charts and more info. With 2, you will not see any charts but they will be quietly generated and save in your local current directory under the AutoViz_Plots directory which will be created. Make sure you delete this folder periodically, otherwise, you will have lots of charts saved here if you used verbose=2 option a lot.
-        - `lowess` - this option is very nice for small datasets where you can see regression lines for each pair of continuous variable against the target variable. Don't use this for large data sets (that is over 100,000 rows)
-        - `chart_format` - this can be `'svg', 'png', 'jpg'` or `'bokeh'` or `'server'` or `'html'`. You will get charts generated (inline with `verbose=0` or `1` option). Instead you can silently save them in multiple formats if you used `verbose=2` option. The latter options are useful for interactive charts.
-        - `max_rows_analyzed` - limits the max number of rows that is used to display charts. If you have a very large data set with millions of rows, then use this option to limit the amount of time it takes to generate charts. We will take a statistically valid sample.
-        - `max_cols_analyzed` - limits the number of continuous vars that can be analyzed
-        - `save_plot_dir` - directory you want the plots to be saved. Default is None which means it is saved under the current directory under a sub-folder named `AutoViz_Plots`. If the `save_plot_dir` does not exist, it creates it.
+        ## Additional Notes
+        <ul>
+          <li>AutoViz will visualize any sized file using a statistically valid sample.</li>
+          <li>COMMA is the default separator in the file, but you can change it.</li>
+          <li>Assumes the first row as the header in the file, but this can be changed.</li>
+        </ul>
+        
+        <h3>Verbose Option</h3>
+        <ol>
+          <li>Display minimal information but show charts in your notebook</li>
+          <li>Print extra information on the notebook and display charts</li>
+          <li>Do not display charts; save them locally under the AutoViz_Plots directory in your current working folder.</li>
+        </ol>
+        
+        <h3>Chart Format Option</h3>
+        <ul>
+          <li><code>'svg', 'jpg' or 'png'</code>: Display or save all charts, depending on the verbose option</li>
+          <li><code>'bokeh'</code>: Plot interactive charts using Bokeh in your Jupyter Notebook</li>
+          <li><code>'server'</code>: Display charts in your browser, with one chart type per tab</li>
+          <li><code>'html'</code>: Create interactive Bokeh charts and save them under the AutoViz_Plots directory or the directory specified in the save_plot_dir setting.</li>
+        </ul>
         
         ![server_charts](server_charts.JPG)
         
-        ### Apr-2023 Update: AutoViz now creates scatter plots for categorical variables when data contains only cat variables
-        From version 0.1.600 onwards, AutoViz now automatically draws `catscatter` plots for pairs of categorical variables in a data frame. A `catscatter` plot is a type of scatter plot that shows the frequency of each combination of categories in two variables. It can be useful for exploring the relationship between categorical variables and identifying patterns or outliers. It creates these plots only if the data contains no numeric variables. Otherwise, it doesn't create them since it would be unncessary.
+        # Examples
+        Here are some examples to help you get started with AutoViz:
+        
+        ## Example 1: Visualize a CSV file with a target variable
         
         ```
-        AutoViz is grateful to the cascatter implementation of Myr Barnés, 2020.
-        You can see the original here: https://github.com/myrthings/catscatter/blob/master/catscatter.py
-        # More info about this function here:
-        # - https://towardsdatascience.com/visualize-categorical-relationships-with-catscatter-e60cdb164395
-        # - https://github.com/myrthings/catscatter/blob/master/README.md
-        ```
+        from autoviz import AutoViz_Class
+        AV = AutoViz_Class()
         
-        ### Sep-2022 Update: AutoViz now provides data cleansing suggestions! #autoviz #datacleaning
-        From version 0.1.50 onwards, AutoViz now automatically analyzes your dataset and provides suggestions for how to clean your  data set. It detects missing values, identifies rare categories, finds infinite values, detects mixed data types, and so much more. This will help you tremendously speed up your data cleaning activities. If you have suggestions to add more data cleaning steps please file an `Issue` in our GitHub and we will gladly consider it. Here is an example of how data cleaning suggestions look:<br>
-        <img align="center" src="https://i.ibb.co/NKf1gdg/autoviz-data-cleaning.png">
+        filename = "your_file.csv"
+        target_variable = "your_target_variable"
         
-        In order to get this latest function, you must upgrade autoviz to the latest version by:
-        ```
-        pip install autoviz --upgrade
+        dft = AV.AutoViz(
+            filename,
+            sep=",",
+            depVar=target_variable,
+            dfte=None,
+            header=0,
+            verbose=1,
+            lowess=False,
+            chart_format="svg",
+            max_rows_analyzed=150000,
+            max_cols_analyzed=30,
+            save_plot_dir=None
+        )
         ```
         
-        In the same version, you can also get data suggestions by using `AV.AutoViz(......, verbose=1)` or by simply importing it:<br>
+        ## Example 2: Visualize a Pandas DataFrame without a target variable:
         
         ```
-        from autoviz import data_cleaning_suggestions
-        data_cleaning_suggestions(df)
-        ```
+        import pandas as pd
+        from autoviz import AutoViz_Class
         
-        ### Dec-23-2021 Update: AutoViz now does Wordclouds! #autoviz #wordcloud
-        AutoViz can now create Wordclouds automatically for your NLP variables in data. It detects NLP variables automatically and creates wordclouds for them. See Colab notebook for example: [AutoViz Demo with HTML setting](https://colab.research.google.com/drive/1r5QqESRZDY98FFfDOgVtMAVA_oaGtqqx?usp=sharing)
+        AV = AutoViz_Class()
         
-        <img align="center" src="https://i.postimg.cc/DyT466xP/wordclouds.png">
+        data = {'col1': [1, 2, 3, 4, 5], 'col2': [5, 4, 3, 2, 1]}
+        df = pd.DataFrame(data)
         
-        ### Dec 21, 2021: AutoViz now runs on Docker containers as part of MLOps pipelines. Check out Orchest.io
-        We are excited to announce that AutoViz and Deep_AutoViML are now available as containerized applications on Docker. This means that you can build data pipelines using a fantastic tool like [orchest.io](orchest.io) to build MLOps pipelines visually. Here are two sample pipelines we have created:
+        dft = AV.AutoViz(
+            "",
+            sep=",",
+            depVar="",
+            dfte=df,
+            header=0,
+            verbose=1,
+            lowess=False,
+            chart_format="svg",
+            max_rows_analyzed=150000,
+            max_cols_analyzed=30,
+            save_plot_dir=None
+        )
+        ```
+        
+        ## Example 3: Generate interactive Bokeh charts and save them as HTML files in a custom directory
         
-        <b>AutoViz pipeline</b>: https://lnkd.in/g5uC-z66
-        <b>Deep_AutoViML pipeline</b>: https://lnkd.in/gdnWTqCG
+        ```
+        from autoviz import AutoViz_Class
+        AV = AutoViz_Class()
         
-        You can find more examples and a wonderful video on [orchest's web site](https://github.com/orchest/orchest-examples)
-        ![banner](https://github.com/rsesha/autoviz_pipeline/blob/main/autoviz_orchest.png)
+        filename = "your_file.csv"
+        target_variable = "your_target_variable"
+        custom_plot_dir = "your_custom_plot_directory"
         
-        ### Dec-17-2021 AutoViz now uses HoloViews to display dashboards with Bokeh and save them as Dynamic HTML for web serving #HTML #Bokeh #Holoviews
-        Now you can use AutoViz to create Interactive Bokeh charts and dashboards (see below) either in Jupyter Notebooks or in the browser. Use chart_format as follows:
-        - `chart_format='bokeh'`: interactive Bokeh dashboards are plotted in Jupyter Notebooks.
-        - `chart_format='server'`, dashboards will pop up for each kind of chart on your web browser.
-        - `chart_format='html'`, interactive Bokeh charts will be silently saved as Dynamic HTML files under `AutoViz_Plots` directory
-        <img align="center" src="https://i.postimg.cc/MTCZ6GzQ/Auto-Viz-HTML-dashboards.png" />
+        dft = AV.AutoViz(
+            filename,
+            sep=",",
+            depVar=target_variable,
+            dfte=None,
+            header=0,
+            verbose=2,
+            lowess=False,
+            chart_format="html",
+            max_rows_analyzed=150000,
+            max_cols_analyzed=30,
+            save_plot_dir=custom_plot_dir
+        )
+        ```
         
-        ## Maintainers
+        These examples should give you an idea of how to use AutoViz with different scenarios and settings. By tailoring the options and settings, you can generate visualizations that best suit your needs, whether you're working with large datasets, interactive charts, or simply exploring the relationships between variables.
         
+        # Maintainers
+        AutoViz is actively maintained and improved by a team of dedicated developers. If you have any questions, suggestions or issues, feel free to reach out to the maintainers.
         * [@AutoViML](https://github.com/AutoViML)
         * [@morenoh149](https://github.com/morenoh149)
         * [@hironroy](https://github.com/hironroy)
         
-        ## Contributing
         
-        See [the contributing file](contributing.md)!
+        # Contributing
+        We welcome contributions from the community! If you're interested in contributing to AutoViz, please follow these steps:
         
-        PRs accepted.
+        <h2>Fork the repository on GitHub</h2>
+        <ol>
+          <li>Clone your fork and create a new branch for your feature or bugfix.</li>
+          <li>Commit your changes to the new branch, ensuring that you follow coding standards and write appropriate tests.</li>
+          <li>Push your changes to your fork on GitHub.</li>
+          <li>Submit a pull request to the main repository, detailing your changes and referencing any related issues.</li>
+        </ol>
+        
+        See [the contributing file](contributing.md)!
         
-        ## License
+        # License
+        AutoViz is released under the Apache License, Version 2.0. By using AutoViz, you agree to the terms and conditions specified in the license.
         
-        Apache License, Version 2.0
+        # Tips
+        <p>That covers the main aspects of AutoViz, but here are some additional tips and reminders to help you make the most of the library:</p>
+        <ul>
+          <li>Make sure to regularly upgrade AutoViz to benefit from the <a href="https://github.com/AutoViML/AutoViz/blob/main/updates.md">latest features, bug fixes, and improvements</a>. You can update it using <code>pip install --upgrade autoviz</code>.</li>
+          <li>AutoViz is highly customizable, so don't hesitate to explore and experiment with various settings, such as <code>chart_format</code>, <code>verbose</code>, and <code>max_rows_analyzed</code>. This will allow you to create visualizations that better suit your specific needs and preferences.</li>
+          <li>Remember to delete the <code>AutoViz_Plots</code> directory (or any custom directory you specified) periodically if you used the <code>verbose=2</code> option, as it can accumulate a large number of saved charts over time.</li>
+          <li>For further guidance or inspiration, check out the <a href="https://towardsdatascience.com/autoviz-a-new-tool-for-automated-visualization-ec9c1744a6ad">Medium article on AutoViz</a>, as well as other online resources and tutorials.</li>
+          <li>If you encounter any issues, have questions, or want to suggest improvements, don't hesitate to engage with the AutoViz community through the <a href="https://github.com/AutoViML/AutoViz">GitHub repository</a> or other online platforms.</li>
+        </ul>
+        <p>By leveraging AutoViz's powerful and flexible features, you can streamline your data visualization process and gain valuable insights more efficiently. Happy visualizing!</p>
         
         ## DISCLAIMER
         This project is not an official Google project. It is not supported by Google and Google specifically disclaims all warranties as to its quality, merchantability, or fitness for a particular purpose.
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `autoviz-0.1.601/setup.py` & `autoviz-0.1.603/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autoviz",
-    version="0.1.601",
+    version="0.1.603",
     author="Ram Seshadri",
     # author_email="author@example.com",
     description="Automatically Visualize any dataset, any size with a single line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/AutoViz",
```

