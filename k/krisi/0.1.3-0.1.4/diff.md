# Comparing `tmp/krisi-0.1.3.tar.gz` & `tmp/krisi-0.1.4.tar.gz`

## Comparing `krisi-0.1.3.tar` & `krisi-0.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-0.1.3/.flake8
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-0.1.3/.isort.cfg
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 krisi-0.1.3/mkdocs.yaml
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-0.1.3/.vscode/launch.json
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 krisi-0.1.3/.vscode/settings.json
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/analyse/__init__.py
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/analyse/correlations.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/analyse/dataset.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/analyse/utils.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/__init__.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/assertions.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/compare.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/group.py
--rw-r--r--   0        0        0     7415 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/metric.py
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/score.py
--rw-r--r--   0        0        0    21175 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/scorecard.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/type.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/library/__init__.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/library/default_metrics_classification.py
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/library/default_metrics_regression.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/library/diagrams.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/evaluate/library/metric_wrappers.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/__init__.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/console.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/graph.py
--rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/interactive.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/pdf.py
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/report.py
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/type.py
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/vizualise.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/library/console/diagrams.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/library/pdf_layouts/scorecard/report.css
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/report/library/pdf_layouts/scorecard/report.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/console_plot.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/data.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/environment.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/io.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/iterable_helpers.py
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/printing.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 krisi-0.1.3/src/krisi/utils/devutils/timing.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 krisi-0.1.3/.gitignore
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-0.1.3/LICENSE
--rw-r--r--   0        0        0    27691 2020-02-02 00:00:00.000000 krisi-0.1.3/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 krisi-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    32477 2020-02-02 00:00:00.000000 krisi-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 krisi-0.1.4/.flake8
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 krisi-0.1.4/.isort.cfg
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 krisi-0.1.4/mkdocs.yaml
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 krisi-0.1.4/.vscode/launch.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 krisi-0.1.4/.vscode/settings.json
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/analyse/__init__.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/analyse/correlations.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/analyse/dataset.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/analyse/utils.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/evaluate/__init__.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/evaluate/assertions.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/evaluate/compare.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/evaluate/group.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/evaluate/metric.py
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/evaluate/score.py
+-rw-r--r--   0        0        0    21550 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/evaluate/scorecard.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/evaluate/type.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/evaluate/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/evaluate/library/__init__.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/evaluate/library/default_metrics_classification.py
+-rw-r--r--   0        0        0     5532 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/evaluate/library/default_metrics_regression.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/evaluate/library/diagrams.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/evaluate/library/metric_wrappers.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/report/__init__.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/report/console.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/report/graph.py
+-rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/report/interactive.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/report/pdf.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/report/report.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/report/type.py
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/report/vizualise.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/report/library/console/diagrams.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/report/library/pdf_layouts/scorecard/report.css
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/report/library/pdf_layouts/scorecard/report.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/utils/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/utils/console_plot.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/utils/data.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/utils/environment.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/utils/io.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/utils/iterable_helpers.py
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/utils/printing.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 krisi-0.1.4/src/krisi/utils/devutils/timing.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 krisi-0.1.4/.gitignore
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 krisi-0.1.4/LICENSE
+-rw-r--r--   0        0        0    61743 2020-02-02 00:00:00.000000 krisi-0.1.4/README.md
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 krisi-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    66529 2020-02-02 00:00:00.000000 krisi-0.1.4/PKG-INFO
```

### Comparing `krisi-0.1.3/mkdocs.yaml` & `krisi-0.1.4/mkdocs.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
       accent: deep orange
 
 nav:
     - Home: 'index.md'
     - Concepts:
       - ScoreCard: 'concepts/scorecard.md'
     - Walkthroughs: 
-      - Start Here: 'walkthroughs/walkthrough.md'
+      - Start Here: 'walkthroughs/a_full_rundown_notebook.md'
     - Examples: generated/gallery
     - API: 
       - 'api/index.md'
       - Evaluate: 'api/evaluate.md'
       - Scorecard & Metric: 'api/scorecard.md'
       - Default Metric Library: 'api/library.md'
       - Detaset helpers: 'api/dataset.md'
```

#### html2text {}

```diff
@@ -4,33 +4,33 @@
 features: - navigation.indexes - search.suggest - toc.follow - navigation.top -
 content.code.copy palette: - media: "(prefers-color-scheme: light)" scheme:
 default toggle: icon: material/toggle-switch name: Switch to dark mode primary:
 amber accent: deep orange - media: "(prefers-color-scheme: dark)" scheme: slate
 toggle: icon: material/toggle-switch-off-outline name: Switch to light mode
 primary: amber accent: deep orange nav: - Home: 'index.md' - Concepts: -
 ScoreCard: 'concepts/scorecard.md' - Walkthroughs: - Start Here: 'walkthroughs/
-walkthrough.md' - Examples: generated/gallery - API: - 'api/index.md' -
-Evaluate: 'api/evaluate.md' - Scorecard & Metric: 'api/scorecard.md' - Default
-Metric Library: 'api/library.md' - Detaset helpers: 'api/dataset.md' - Product,
-Licencing & Roadmap: - License: product/license.md - Roadmap: 'product/
-roadmap.md' markdown_extensions: - tables - attr_list - pymdownx.emoji:
-emoji_index: !!python/name:materialx.emoji.twemoji emoji_generator: !!python/
-name:materialx.emoji.to_svg - pymdownx.highlight: anchor_linenums: true
-line_spans: __span pygments_lang_class: true - pymdownx.inlinehilite -
-pymdownx.snippets - pymdownx.superfences plugins: - search - include-markdown -
-glightbox: touchNavigation: true loop: true zoomable: true auto_caption: true -
-autorefs - gallery: examples_dirs: docs/examples # path to your example scripts
-gallery_dirs: docs/generated/gallery # where to save generated gallery -
-mkdocstrings: handlers: python: paths: [src] options: show_source: false
-separate_signature: true show_submodules: true show_signature_annotations: true
-docstring_style: 'numpy' show_root_toc_entry: false group_by_category: true
-show_root_heading: true show_category_heading: false import: - https://
-docs.python-requests.org/en/master/objects.inv extra: analytics: provider:
-google property: G-FBLB9N9026 feedback: title: Was this page helpful? ratings:
-- icon: material/emoticon-happy-outline name: This page was helpful data: 1
-note: >- Thanks for your feedback! - icon: material/emoticon-sad-outline name:
-This page could be improved data: 0 note: >- Thanks for your feedback! Help us
-improve this page by using our feedback_form. consent: title: Cookie consent
-description: >- We use cookies to recognize your repeated visits and
-preferences, as well as to measure the effectiveness of our documentation and
-whether users find what they're searching for. With your consent, you're
-helping us to make our documentation better.
+a_full_rundown_notebook.md' - Examples: generated/gallery - API: - 'api/
+index.md' - Evaluate: 'api/evaluate.md' - Scorecard & Metric: 'api/
+scorecard.md' - Default Metric Library: 'api/library.md' - Detaset helpers:
+'api/dataset.md' - Product, Licencing & Roadmap: - License: product/license.md
+- Roadmap: 'product/roadmap.md' markdown_extensions: - tables - attr_list -
+pymdownx.emoji: emoji_index: !!python/name:materialx.emoji.twemoji
+emoji_generator: !!python/name:materialx.emoji.to_svg - pymdownx.highlight:
+anchor_linenums: true line_spans: __span pygments_lang_class: true -
+pymdownx.inlinehilite - pymdownx.snippets - pymdownx.superfences plugins: -
+search - include-markdown - glightbox: touchNavigation: true loop: true
+zoomable: true auto_caption: true - autorefs - gallery: examples_dirs: docs/
+examples # path to your example scripts gallery_dirs: docs/generated/gallery #
+where to save generated gallery - mkdocstrings: handlers: python: paths: [src]
+options: show_source: false separate_signature: true show_submodules: true
+show_signature_annotations: true docstring_style: 'numpy' show_root_toc_entry:
+false group_by_category: true show_root_heading: true show_category_heading:
+false import: - https://docs.python-requests.org/en/master/objects.inv extra:
+analytics: provider: google property: G-FBLB9N9026 feedback: title: Was this
+page helpful? ratings: - icon: material/emoticon-happy-outline name: This page
+was helpful data: 1 note: >- Thanks for your feedback! - icon: material/
+emoticon-sad-outline name: This page could be improved data: 0 note: >- Thanks
+for your feedback! Help us improve this page by using our feedback_form.
+consent: title: Cookie consent description: >- We use cookies to recognize your
+repeated visits and preferences, as well as to measure the effectiveness of our
+documentation and whether users find what they're searching for. With your
+consent, you're helping us to make our documentation better.
```

### Comparing `krisi-0.1.3/.vscode/settings.json` & `krisi-0.1.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/analyse/correlations.py` & `krisi-0.1.4/src/krisi/analyse/correlations.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,88 +1,72 @@
 from functools import reduce
+from pathlib import Path
 from typing import List, Optional, Tuple
 
 import matplotlib.pyplot as plt
 import pandas as pd
 from typing_extensions import Literal
 
+from krisi.evaluate.type import PathConst
+from krisi.report.graph import create_save_graphs
+
 from .utils import corr_without_symmetry, unroll
 
 
+def get_mean_corr_matrix(df_rolled_corr: List[pd.DataFrame]) -> pd.DataFrame:
+    df_rolled_summed = reduce(lambda x, y: x.add(y, fill_value=0), df_rolled_corr)
+    df_rolled_mean = df_rolled_summed / len(df_rolled_corr)
+
+    return df_rolled_mean
+
+
 def get_unrolled_correlation_over_time(
     df_rolled_corr: List[pd.DataFrame], start_indecies: List[pd.DatetimeIndex]
 ) -> pd.DataFrame:
     df_unrolled_in_time = pd.concat(
         [unroll(df_, start_indecies[i]) for i, df_ in enumerate(df_rolled_corr)],
         axis="columns",
     ).T
     df_unrolled_in_time.index = pd.to_datetime(df_unrolled_in_time.index)
     return df_unrolled_in_time
 
 
-def get_mean_corr_matrix(df_rolled_corr: List[pd.DataFrame]) -> pd.DataFrame:
-    df_rolled_summed = reduce(lambda x, y: x.add(y, fill_value=0), df_rolled_corr)
-    df_rolled_mean = df_rolled_summed / len(df_rolled_corr)
-
-    return df_rolled_mean
-
-
 def get_corr_rolled(
     df: pd.DataFrame, window: int, step: Optional[int] = None
 ) -> Tuple[List[pd.DataFrame], List[pd.DataFrame]]:
     if step is None or step == 1 or step == 0:
-        df_rolled = [df_ for df_ in df.rolling(window=window)][1:]
+        df_rolled = list(df.rolling(window=window))[1:]
     else:
-        df_rolled = [df_ for df_ in df.rolling(window=window, step=step)][1:]
+        df_rolled = list(df.rolling(window=window, step=step))[1:]
     df_rolled_corr = [corr_without_symmetry(df_) for df_ in df_rolled]
 
     return df_rolled_corr, df_rolled
 
 
-def create_rolled_correlation_metrics(
-    df_rolled_corr: List[pd.DataFrame],
-    start_indecies: List[pd.DatetimeIndex],
-    threshold: float = 0.25,
-) -> Tuple[
-    List[pd.DataFrame], pd.DataFrame, pd.DataFrame, pd.DataFrame, pd.Series, pd.Series
-]:
-    coor_unrolled_in_time = get_unrolled_correlation_over_time(
-        df_rolled_corr, start_indecies
-    )
-
-    # Correlations properties on unrolled correlation data
-    corr_std = coor_unrolled_in_time.std()
-    corr_mean = coor_unrolled_in_time.mean()
-
+def __corr_mean(df_rolled_corr: List[pd.DataFrame], threshold: float):
     # Mean correlations in a matrix for plotting into a network graph
     mean_corr_over_time = get_mean_corr_matrix(df_rolled_corr)
 
     mean_corr_over_time_treshold = mean_corr_over_time.where(
         mean_corr_over_time >= threshold, other=0.0
     )
-    return (
-        df_rolled_corr,
-        mean_corr_over_time,
-        mean_corr_over_time_treshold,
-        coor_unrolled_in_time,
-        corr_std,
-        corr_mean,
-    )
+
+    return mean_corr_over_time, mean_corr_over_time_treshold
 
 
-def create_summaries(
+def __create_summary(
     corr_std: pd.Series,
     corr_mean: pd.Series,
     df_unrolled_in_time: pd.DataFrame,
     window: int,
     step: int,
     name: str,
-    save_or_display: List[Literal["save", "display"]] = ["display"],
-    save_location: str = "structured_data/plots",
-    top_k: int = 2,
+    save_or_display: List[Literal["save", "display"]],
+    save_location: str,
+    top_k: int,
 ) -> None:
     fig, ax = plt.subplots(2, 1)
     title = f"Summary of {name} | window - {window} ~ step - {step}"
     fig.suptitle(title)
 
     # ranking = corr_mean/corr_std
 
@@ -101,7 +85,78 @@
     print(result)
 
     if "save" in save_or_display:
         path_friendly = title.replace(" ", "_")
         plt.savefig(f"{save_location}/{path_friendly}.png", format="PNG")
     if "display" in save_or_display:
         plt.show()
+
+
+def get_rolled_corr_metrics(
+    df: pd.DataFrame,
+    window: int,
+    step: int = 1,
+) -> Tuple[pd.DataFrame, pd.Series, pd.Series]:
+    df_rolled_corr, df_rolled = get_corr_rolled(df, window, step)
+
+    start_indecies = [df_.index[0] for df_ in df_rolled]
+
+    coor_unrolled_in_time = get_unrolled_correlation_over_time(
+        df_rolled_corr, start_indecies
+    )
+
+    # Correlations properties on unrolled correlation data
+    corr_std = coor_unrolled_in_time.std()
+    corr_mean = coor_unrolled_in_time.mean()
+
+    return (
+        coor_unrolled_in_time,
+        corr_std,
+        corr_mean,
+    )
+
+
+def matrix_corr_over_time(
+    df: pd.DataFrame,
+    window: int,
+    step: int = 1,
+    threshold: float = 0.25,
+    save_location: Path = PathConst.default_analyse_output_path,
+    save_graphs: bool = False,
+):
+    df_rolled_corr, df_rolled = get_corr_rolled(df, window, step)
+    df_rolled_mean, df_rolled_mean_treshold = __corr_mean(
+        df_rolled_corr, threshold=threshold
+    )
+
+    if save_graphs:
+        create_save_graphs([df_rolled_mean_treshold], save_location)
+
+    return df_rolled_mean, df_rolled_mean_treshold
+
+
+def plot_corr_over_time(
+    df: pd.DataFrame,
+    window: int,
+    step: int = 1,
+    name: str = "",
+    save_or_display: List[Literal["save", "display"]] = ["display"],
+    save_location: str = "structured_data/plots",
+    top_k: int = 2,
+) -> None:
+    (
+        coor_unrolled_in_time,
+        corr_std,
+        corr_mean,
+    ) = get_rolled_corr_metrics(df, window, step)
+
+    __create_summary(
+        corr_std,
+        corr_mean,
+        coor_unrolled_in_time,
+        window,
+        step,
+        name=name,
+        save_or_display=save_or_display,
+        save_location=save_location,
+        top_k=top_k,
+    )
```

### Comparing `krisi-0.1.3/src/krisi/analyse/dataset.py` & `krisi-0.1.4/src/krisi/analyse/dataset.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/evaluate/assertions.py` & `krisi-0.1.4/src/krisi/evaluate/assertions.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/evaluate/compare.py` & `krisi-0.1.4/src/krisi/evaluate/compare.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/evaluate/group.py` & `krisi-0.1.4/src/krisi/evaluate/group.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/evaluate/metric.py` & `krisi-0.1.4/src/krisi/evaluate/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     func: Optional[MetricFunction] = None
     plot_funcs: Optional[List[Tuple[PlotFunction, Optional[Dict[str, Any]]]]] = None
     plot_func_rolling: Optional[Tuple[PlotFunction, Optional[Dict[str, Any]]]] = None
     info: str = ""
     restrict_to_sample: Optional[SampleTypes] = None
     comp_complexity: Optional[ComputationalComplexity] = None
     disable_rolling: bool = False
+    _from_group: bool = False
 
     def __post_init__(self):
         if self.key == "":
             self.key = string_to_id(self.name)
 
     def __setitem__(self, key: str, item: Any) -> None:
         setattr(self, key, item)
@@ -85,31 +86,34 @@
         return print_metric(self)
 
     def __repr__(self) -> str:
         print(print_metric(self, repr=True))
         return super().__repr__()
 
     def _evaluation(self, *args) -> "Metric":
+        if self._from_group:
+            return self
         try:
             result = self.func(*args, **self.parameters)
         except Exception as e:
             result = e
         self.__safe_set(result, key="result")
         return self
 
     def evaluate(self, y: Targets, predictions: Predictions) -> None:
         assert (
             self.func is not None
         ), "`func` has to be set on Metric to calculate result."
-
         self._evaluation(y, predictions)
 
     def _rolling_evaluation(self, *args, rolling_args: dict) -> "Metric":
+        if self._from_group:
+            return self
         if self.disable_rolling:
-            self._evaluation(*args)
+            return self
         else:
             _df = pd.concat(args, axis="columns")
             try:
                 df_rolled = (
                     _df.expanding()
                     if rolling_args["window"] is None
                     else _df.rolling(**rolling_args)
```

### Comparing `krisi-0.1.3/src/krisi/evaluate/score.py` & `krisi-0.1.4/src/krisi/evaluate/score.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/evaluate/scorecard.py` & `krisi-0.1.4/src/krisi/evaluate/scorecard.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Predictions,
     PrintMode,
     SampleTypes,
     SaveModes,
     ScoreCardMetadata,
     Targets,
 )
-from krisi.evaluate.utils import handle_unnamed
+from krisi.evaluate.utils import get_save_path, handle_unnamed
 from krisi.report.console import (
     get_large_metric_summary,
     get_minimal_summary,
     get_summary,
 )
 from krisi.report.report import create_report_from_scorecard
 from krisi.report.type import DisplayModes, InteractiveFigure
@@ -128,15 +128,14 @@
     predictions: Predictions
     sample_type: SampleTypes
     default_metrics_keys: List[str]
     custom_metrics_keys: List[str]
     classification: bool  # TODO: Support multilabel classification
     metadata: ScoreCardMetadata
     rolling_args: Dict[str, Any]
-    save_path: Path
 
     def __init__(
         self,
         y: Targets,
         predictions: Predictions,
         model_name: Optional[str] = None,
         model_description: str = "",
@@ -163,14 +162,15 @@
             else classification
         )
         model_name_, dataset_name_, project_name_ = handle_unnamed(
             y, predictions, model_name, dataset_name, project_name
         )
 
         self.__dict__["metadata"] = ScoreCardMetadata(
+            get_save_path(project_name_),
             project_name_,
             project_description,
             model_name_,
             model_description,
             dataset_name_,
             dataset_description,
         )
@@ -192,24 +192,14 @@
 
         for metric in default_metrics:
             self.__dict__[metric.key] = deepcopy(metric)
 
         for metric in custom_metrics:
             self.__dict__[metric.key] = deepcopy(metric)
 
-        self.__dict__["save_path"] = Path(
-            os.path.join(
-                PathConst.default_eval_output_path,
-                replace_if_None(
-                    self.metadata.project_name,
-                    f"{datetime.datetime.now().strftime('%d-%m')}_{self.metadata.model_name}_{self.metadata.dataset_name}",
-                ),
-            )
-        )
-
     def __setitem__(self, key: str, item: Any) -> None:
         self.__setattr__(key, item)
 
     def __getitem__(self, key: Union[str, List[str]]) -> Union["ScoreCard", Metric]:
         if isinstance(key, List):
             scorecard_copy = deepcopy(self)
             all_keys = list(scorecard_copy.__dict__.keys())
@@ -407,15 +397,22 @@
         ScoreCard
         """
 
         for metric in self.get_all_metrics(defaults=defaults):
             if metric.restrict_to_sample is not self.sample_type:
                 if isinstance(metric, Group):
                     for metric in metric.evaluate(self.y, self.predictions):
-                        self[metric.key] = metric
+                        if metric.key not in self.__dict__:
+                            metric._from_group = True
+                            self[metric.key] = metric
+                        else:
+                            self[metric.key] = {
+                                "result": metric.result,
+                                "_from_group": True,
+                            }
                 else:
                     metric.evaluate(self.y, self.predictions)
 
         return self
 
     def evaluate_over_time(self, defaults: bool = True) -> "ScoreCard":
         """
@@ -440,15 +437,22 @@
         """
         for metric in self.get_all_metrics(defaults=defaults):
             if metric.restrict_to_sample is not self.sample_type:
                 if isinstance(metric, Group):
                     for metric in metric.evaluate_over_time(
                         self.y, self.predictions, rolling_args=self.rolling_args
                     ):
-                        self[metric.key] = metric
+                        if metric.key not in self.__dict__:
+                            metric._from_group = True
+                            self[metric.key] = metric
+                        else:
+                            self[metric.key] = {
+                                "result_rolling": metric.result_rolling,
+                                "_from_group": True,
+                            }
                 else:
                     metric.evaluate_over_time(
                         self.y, self.predictions, rolling_args=self.rolling_args
                     )
         return self
 
     def print(
@@ -508,15 +512,15 @@
         ],
         override_base_path: Optional[Path] = None,
         timestamping: bool = True,
     ) -> "ScoreCard":
         path = replace_if_None(
             override_base_path,
             os.path.join(
-                self.save_path,
+                self.metadata.save_path,
                 f"scorecards/{datetime.datetime.now().strftime('%H-%M-%S-%f') if timestamping else 'scorecard'}",
             ),
         )
         ensure_path(path)
 
         if SaveModes.minimal in save_modes or SaveModes.minimal.value in save_modes:
             save_minimal_summary(self, path)
@@ -540,15 +544,15 @@
         ],
         html_template_url: Path = PathConst.html_report_template_url,
         css_template_url: Path = PathConst.css_report_template_url,
         author: str = "",
         report_title: Optional[str] = None,
         override_base_path: Optional[Path] = None,
     ) -> None:
-        save_path = replace_if_None(override_base_path, self.save_path)
+        save_path = replace_if_None(override_base_path, self.metadata.save_path)
         ensure_path(save_path)
 
         display_modes = [
             DisplayModes.from_str(mode) for mode in wrap_in_list(display_modes)
         ]
         report = create_report_from_scorecard(
             self,
```

### Comparing `krisi-0.1.3/src/krisi/evaluate/type.py` & `krisi-0.1.4/src/krisi/evaluate/type.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import os
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
-from typing import Callable, List, Tuple, TypeVar, Union
+from typing import Any, Callable, List, Tuple, TypeVar, Union
 
 import numpy as np
 import pandas as pd
 
 MetricResult = TypeVar(
     "MetricResult", bound=Union[float, int, str, List, Tuple, pd.DataFrame]
 )
@@ -43,33 +44,43 @@
     text = "text"
     obj = "obj"
     minimal = "minimal"
 
 
 class PathConst:
     default_eval_output_path: Path = Path("output/")
+    default_analyse_output_path: Path = Path("analyse/")
     html_report_template_url: Path = Path("library/pdf_layouts/scorecard/report.html")
     css_report_template_url: Path = Path("library/pdf_layouts/scorecard/report.css")
 
 
 class ComputationalComplexity(Enum):
     low = "low"
     medium = "medium"
     high = "high"
 
 
 @dataclass
 class ScoreCardMetadata:
+    save_path: Path
     project_name: str = ""
     project_description: str = ""
     model_name: str = ""
     model_description: str = ""
     dataset_name: str = ""
     dataset_description: str = ""
 
+    def __setattr__(self, key: str, item: Any) -> None:
+        if key == "project_name":
+            self.save_path = Path(
+                os.path.join(PathConst.default_eval_output_path, item)
+            )
+
+        super().__setattr__(key, item)
+
 
 class PrintMode(Enum):
     extended = "extended"
     minimal = "minimal"
     minimal_table = "minimal_table"
 
     @staticmethod
```

### Comparing `krisi-0.1.3/src/krisi/evaluate/utils.py` & `krisi-0.1.4/src/krisi/evaluate/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import datetime
+import os
 import uuid
+from pathlib import Path
 from typing import TYPE_CHECKING, List, Optional, Tuple
 
 import pandas as pd
 
-from krisi.evaluate.type import Predictions, Targets
+from krisi.evaluate.type import PathConst, Predictions, Targets
 
 if TYPE_CHECKING:
     from krisi.evaluate.scorecard import ScoreCard
 
 
 def handle_empty_metrics_to_display(
     scorecard: "ScoreCard", sort_by: Optional[str], metric_keys: Optional[List[str]]
@@ -54,7 +56,11 @@
         else:
             model_name = f"Model_{display_time+str(uuid.uuid4()).split('-')[0]}"
 
     if project_name is None:
         project_name = f"Project_{display_time+str(uuid.uuid4()).split('-')[0]}"
 
     return model_name, dataset_name, project_name
+
+
+def get_save_path(project_name: str) -> Path:
+    return Path(os.path.join(PathConst.default_eval_output_path, project_name))
```

### Comparing `krisi-0.1.3/src/krisi/evaluate/library/default_metrics_classification.py` & `krisi-0.1.4/src/krisi/evaluate/library/default_metrics_classification.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/evaluate/library/default_metrics_regression.py` & `krisi-0.1.4/src/krisi/evaluate/library/default_metrics_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,19 +110,24 @@
         (display_density_plot, dict(width=1500.0)),
         (display_time_series, dict(width=1500.0)),
     ],
     disable_rolling=True,
 )
 """ ~ """
 
+
+def dummy_func(res):
+    return res.mean()
+
+
 residuals_mean = Metric[float](
     name="Mean of the Residuals",
     key="residuals_mean",
     category=MetricCategories.residual,
-    func=lambda res: res.mean(),
+    func=dummy_func,  # lambda res: res.mean(),
     plot_funcs=[(display_single_value, dict(width=900.0))],
     plot_func_rolling=(display_time_series, dict(width=1500.0)),
 )
 """ ~ """
 
 residuals_std = Metric[float](
     name="Standard Deviation of the Residuals",
@@ -138,14 +143,15 @@
     name="Ljung Box Statistics",
     key="ljung_box_statistics",
     category=MetricCategories.residual,
     func=ljung_box,
     info="If p is larger than our significance level then we cannot dismiss the null-hypothesis that the residuals are a random walk.",
     restrict_to_sample=SampleTypes.insample,
     comp_complexity=ComputationalComplexity.high,
+    disable_rolling=True,
 )
 """ ~ """
 
 residual_group = Group(
     name="residual_group",
     key="residual_group",
     metrics=[residuals_mean, residuals_std],
```

### Comparing `krisi-0.1.3/src/krisi/evaluate/library/diagrams.py` & `krisi-0.1.4/src/krisi/evaluate/library/diagrams.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/report/console.py` & `krisi-0.1.4/src/krisi/report/console.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/report/graph.py` & `krisi-0.1.4/src/krisi/report/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+from pathlib import Path
 from typing import List
 
 import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
 import pandas as pd
 from typing_extensions import Literal
 
+from krisi.evaluate.type import PathConst
+from krisi.utils.io import ensure_path
+
 
 def create_save_graphs(
     df_rolled_corr: List[pd.DataFrame],
     save_or_display: List[Literal["save", "display"]] = ["save", "display"],
     corr_direction: Literal["positive", "negative"] = "positive",
     min_correlation: float = 0.01,
-    save_location: str = "output/analyse/correlations",
+    save_location: Path = PathConst.default_analyse_output_path,
 ) -> None:
+    ensure_path(save_location)
     for i, corr_df in enumerate(df_rolled_corr):
         __display_corr_graph(
             corr_df,
             save_or_display,
             corr_direction,
             min_correlation,
             save_location,
@@ -26,15 +31,15 @@
 
 
 def __display_corr_graph(
     corr: pd.DataFrame,
     save_or_display: List[Literal["save", "display"]],
     corr_direction: Literal["positive", "negative"],
     min_correlation: float,
-    save_location: str,
+    save_location: Path,
     file_name: str = "0",
 ) -> None:
     feature_node_names = corr.index.values
     matrix_array = np.array(corr)
     matrix_corr = np.matrix(matrix_array, copy=False, dtype=None)
 
     G = nx.Graph(matrix_corr)
@@ -51,15 +56,15 @@
     )
 
 
 def __create_corr_network(
     G: nx.Graph,
     corr_direction: Literal["positive", "negative"],
     min_correlation: float,
-    save_location: str,
+    save_location: Path,
     file_name: str,
     save_or_display: List[Literal["save", "display"]],
 ):
     # Creates a copy of the graph
     H = G.copy()
 
     # Checks all the edges and removes some based on corr_direction
```

### Comparing `krisi-0.1.3/src/krisi/report/interactive.py` & `krisi-0.1.4/src/krisi/report/interactive.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,10 +178,10 @@
             app.callback(
                 Output(component.id, "figure"),
                 [Input(input_.id, input_.value_name) for input_ in component.inputs]
                 + [Input(input_id, "value") for input_id in component.global_input_ids],
             )(component.get_figure)
 
     if isnotebook:
-        app.run_server(mode="inline", debug=True, threaded=True)
+        app.run_server(mode="inline", debug=False, threaded=True)
     else:
-        app.run(debug=True, threaded=True)
+        app.run(debug=False, threaded=True)
```

### Comparing `krisi-0.1.3/src/krisi/report/pdf.py` & `krisi-0.1.4/src/krisi/report/pdf.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/report/report.py` & `krisi-0.1.4/src/krisi/report/report.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/report/type.py` & `krisi-0.1.4/src/krisi/report/type.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/report/vizualise.py` & `krisi-0.1.4/src/krisi/report/vizualise.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/report/library/console/diagrams.py` & `krisi-0.1.4/src/krisi/report/library/console/diagrams.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/report/library/pdf_layouts/scorecard/report.css` & `krisi-0.1.4/src/krisi/report/library/pdf_layouts/scorecard/report.css`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/report/library/pdf_layouts/scorecard/report.html` & `krisi-0.1.4/src/krisi/report/library/pdf_layouts/scorecard/report.html`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/utils/console_plot.py` & `krisi-0.1.4/src/krisi/utils/console_plot.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/utils/data.py` & `krisi-0.1.4/src/krisi/utils/data.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/utils/environment.py` & `krisi-0.1.4/src/krisi/utils/environment.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/utils/io.py` & `krisi-0.1.4/src/krisi/utils/io.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/utils/iterable_helpers.py` & `krisi-0.1.4/src/krisi/utils/iterable_helpers.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/utils/printing.py` & `krisi-0.1.4/src/krisi/utils/printing.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/src/krisi/utils/devutils/timing.py` & `krisi-0.1.4/src/krisi/utils/devutils/timing.py`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/.gitignore` & `krisi-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/LICENSE` & `krisi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `krisi-0.1.3/pyproject.toml` & `krisi-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "krisi"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Mark Szulyovszky", email="mark@dreamfaster.ai" },
   { name="Daniel Szemerey", email="daniel@dreamfaster.ai" },
 ]
 description = "Testing and Reporting framework for Time Series Analysis"
 readme = "README.md"
 license = { file="LICENSE" }
@@ -135,15 +135,15 @@
   "src",
   ".",
 ]
 testpaths = ["tests"] 
 
 # bumpver command: ``bumpver update --patch``
 [tool.bumpver]
-current_version = "0.1.3"
+current_version = "0.1.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "chore(Release): Bump version from {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

