# Comparing `tmp/accompanist-1.0.4-py3-none-any.whl.zip` & `tmp/accompanist-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,21 @@
-Zip file size: 37147 bytes, number of entries: 16
--rw-r--r--  2.0 unx     3685 b- defN 23-Mar-23 16:21 accompanist/draw_histgram.py
--rw-r--r--  2.0 unx     2545 b- defN 23-Mar-23 16:23 accompanist/draw_pi_chart.py
--rw-r--r--  2.0 unx     2317 b- defN 23-Mar-26 07:38 accompanist/draw_table.py
--rw-r--r--  2.0 unx     3350 b- defN 23-Mar-29 13:55 accompanist/listen.py
--rw-r--r--  2.0 unx      204 b- defN 23-Mar-26 10:13 accompanist/main.py
--rw-r--r--  2.0 unx     1551 b- defN 23-Apr-03 05:18 accompanist/play.py
--rw-r--r--  2.0 unx     3450 b- defN 23-Apr-03 05:20 accompanist/utility_module.py
--rw-r--r--  2.0 unx      742 b- defN 23-Apr-03 05:37 accompanist/write_front_cover.py
+Zip file size: 42155 bytes, number of entries: 19
+-rw-r--r--  2.0 unx     1423 b- defN 23-May-05 12:22 accompanist/cmd_init.py
+-rw-r--r--  2.0 unx     5229 b- defN 23-May-05 08:48 accompanist/cmd_listen.py
+-rw-r--r--  2.0 unx     2968 b- defN 23-May-05 06:29 accompanist/cmd_play.py
+-rw-r--r--  2.0 unx      732 b- defN 23-May-04 15:46 accompanist/main.py
+-rw-r--r--  2.0 unx       22 b- defN 23-May-03 12:20 accompanist/version.py
+-rw-r--r--  2.0 unx     3945 b- defN 23-May-02 14:21 accompanist/report/draw_histgram.py
+-rw-r--r--  2.0 unx     3593 b- defN 23-May-03 12:19 accompanist/report/draw_pie_chart.py
+-rw-r--r--  2.0 unx     3375 b- defN 23-May-05 08:48 accompanist/report/draw_table.py
+-rw-r--r--  2.0 unx     2907 b- defN 23-May-05 12:37 accompanist/report/utility_module.py
+-rw-r--r--  2.0 unx     1419 b- defN 23-May-05 12:21 accompanist/report/write_comment.py
+-rw-r--r--  2.0 unx     1317 b- defN 23-May-03 16:29 accompanist/report/write_front_cover.py
 -rw-r--r--  2.0 unx    19193 b- defN 23-Mar-26 08:39 accompanist/resource/logo_trans.png
 -rw-r--r--  2.0 unx     6761 b- defN 23-Mar-26 08:25 accompanist/resource/logo_trans_small.png
--rw-r--r--  2.0 unx     1063 b- defN 23-Apr-06 11:59 accompanist-1.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2182 b- defN 23-Apr-06 11:59 accompanist-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-06 11:59 accompanist-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Apr-06 11:59 accompanist-1.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-06 11:59 accompanist-1.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1351 b- defN 23-Apr-06 11:59 accompanist-1.0.4.dist-info/RECORD
-16 files, 48551 bytes uncompressed, 34909 bytes compressed:  28.1%
+-rw-r--r--  2.0 unx     1063 b- defN 23-May-05 13:16 accompanist-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3477 b- defN 23-May-05 13:16 accompanist-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 13:16 accompanist-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-May-05 13:16 accompanist-1.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       31 b- defN 23-May-05 13:16 accompanist-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1645 b- defN 23-May-05 13:16 accompanist-1.1.0.dist-info/RECORD
+19 files, 59245 bytes uncompressed, 39441 bytes compressed:  33.4%
```

## zipnote {}

```diff
@@ -1,49 +1,58 @@
-Filename: accompanist/draw_histgram.py
+Filename: accompanist/cmd_init.py
 Comment: 
 
-Filename: accompanist/draw_pi_chart.py
+Filename: accompanist/cmd_listen.py
 Comment: 
 
-Filename: accompanist/draw_table.py
+Filename: accompanist/cmd_play.py
 Comment: 
 
-Filename: accompanist/listen.py
+Filename: accompanist/main.py
 Comment: 
 
-Filename: accompanist/main.py
+Filename: accompanist/version.py
+Comment: 
+
+Filename: accompanist/report/draw_histgram.py
+Comment: 
+
+Filename: accompanist/report/draw_pie_chart.py
+Comment: 
+
+Filename: accompanist/report/draw_table.py
 Comment: 
 
-Filename: accompanist/play.py
+Filename: accompanist/report/utility_module.py
 Comment: 
 
-Filename: accompanist/utility_module.py
+Filename: accompanist/report/write_comment.py
 Comment: 
 
-Filename: accompanist/write_front_cover.py
+Filename: accompanist/report/write_front_cover.py
 Comment: 
 
 Filename: accompanist/resource/logo_trans.png
 Comment: 
 
 Filename: accompanist/resource/logo_trans_small.png
 Comment: 
 
-Filename: accompanist-1.0.4.dist-info/LICENSE
+Filename: accompanist-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: accompanist-1.0.4.dist-info/METADATA
+Filename: accompanist-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: accompanist-1.0.4.dist-info/WHEEL
+Filename: accompanist-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: accompanist-1.0.4.dist-info/entry_points.txt
+Filename: accompanist-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: accompanist-1.0.4.dist-info/top_level.txt
+Filename: accompanist-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: accompanist-1.0.4.dist-info/RECORD
+Filename: accompanist-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## accompanist/main.py

```diff
@@ -1,12 +1,20 @@
 import click
-from accompanist.listen import listen as listen_cmd
-from accompanist.play import play as play_cmd
+from accompanist.cmd_init import init as init_cmd
+from accompanist.cmd_listen import listen as listen_cmd
+from accompanist.cmd_play import play as play_cmd
 
 
-@click.group()
+@click.group(help="\
+        \"Accompanist\" is your accompanist on AWS WAF log analyses.               \
+        You can get an AWS WAF log analysis report by the following three commands.\
+        (1) $ accompanist init    # Configure CWL log group setting              \
+        (2) $ accompanist listen  # Get a WAF log file for analysis              \
+        (3) $ accompanist play    # Analysis WAF logs and generate a report")
+@click.version_option()
 def cmd():
     pass
 
 
+cmd.add_command(init_cmd)
 cmd.add_command(listen_cmd)
 cmd.add_command(play_cmd)
```

## Comparing `accompanist/draw_histgram.py` & `accompanist/report/draw_histgram.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,43 +6,45 @@
     def __init__(self):
         self._hours = 3
         self._bins = 0
         self._label_and_count = ""
         self._xlocation = []
         self._all_xlocation = []
         self._xlabel = []
-        self._jst_offset = 3600 * 9 * 1000
         self._1day_seconds = 3600 * 24 * 1000
         self._xlabel_threshold = 0
 
-    def histgram(self, ax, time, target, label, color):
+    def histgram(self, ax, time, target, label, color, utc_offset, y_limit):
         """
         Create settings for histgram
         """
-        self._calc_xticks_and_labels(time[0], time[len(time) - 1])
+        self._calc_xticks_and_labels(time[0], time[len(time) - 1], utc_offset)
         self._bins = int((self._last_xlocation - self._first_xlocation - self._1day_seconds)
                          / 1000 / (3600 * self._hours)) + 8  # margin = 8
         self._label_and_count = label + " (" + str(len(target)) + ")"
-        ax.axhspan(10, 20, color="gray", alpha=0.05)
-        ax.axhspan(30, 40, color="gray", alpha=0.05)
+        ax.grid(True)
+        # ax.yaxis.grid(False)
+        y_limit = int(y_limit)
+        ax.set_ylim(0, y_limit)
+        if label != "Third Party":  # a hack for preventing from drawing twice
+            ax.axhspan(y_limit / 5 * 1, y_limit / 5 * 2, color="gray", alpha=0.05)
+            ax.axhspan(y_limit / 5 * 3, y_limit / 5 * 4, color="gray", alpha=0.05)
         ax.hist(target, alpha=0.7, bins=self._bins, range=(self._first_xlocation, self._last_xlocation),
                 label=self._label_and_count, color=color, edgecolor="white", linewidth=0)
-        ax.grid(True)
-        ax.set_ylim(0, 50)
         ax.legend(loc="upper left", prop={"size": 12}, fancybox=True,
                   edgecolor="gray", facecolor="white", framealpha=1)
 
-        self._calc_xticks_and_labels(time[0], time[len(time) - 1])
         ax.set_xticks(self._xlocation)
         ax.set_xticklabels(self._xlabel)
         ax.tick_params(labelsize=10)
 
-    def _calc_xticks_and_labels(self, end_time, start_time):
-        self._last_xlocation = end_time - end_time % (self._1day_seconds) + self._1day_seconds - self._jst_offset
-        self._first_xlocation = start_time - start_time % (self._1day_seconds) - self._jst_offset
+    def _calc_xticks_and_labels(self, end_time, start_time, utc_offset):
+        tz_offset = 3600 * 1000 * utc_offset
+        self._last_xlocation = end_time - end_time % (self._1day_seconds) + self._1day_seconds - tz_offset
+        self._first_xlocation = start_time - start_time % (self._1day_seconds) - tz_offset
         self._number_of_labels = int((self._last_xlocation - self._first_xlocation) / self._1day_seconds) + 1
         self._all_xlocation = np.linspace(self._last_xlocation, self._first_xlocation, self._number_of_labels, dtype=int)
 
         self._xlabel_threshold = int(self._number_of_labels / 5) if (int(self._number_of_labels / 5)) > 2 else 2
 
         self._xlocation = []
         if self._number_of_labels > 7:
@@ -55,32 +57,32 @@
         self._xlabel = []
         for i in range(len(self._xlocation)):
             self._xlabel.append(datetime.datetime
                                 .fromtimestamp(self._xlocation[i] / 1000.0)
                                 .strftime("%m/%d(%a) %H:%M"))
 
 
-def draw_histgram(waf_log, fig):
+def draw_histgram(waf_log, fig, utc_offset, y_limit):
     """
     Draw two histgrams
     """
-    TITLE_OF_TOTAL = "Total Number of Access"
-    TITLE_OF_RULES = "AWS Managed Rule and Third Party Rule"
+    TITLE_OF_TOTAL = "Total Blocked / Counted Request"
+    TITLE_OF_RULES = "Breakdown of Requests by Rule Provider"
 
     fig.subplots_adjust(top=0.8, left=-0.5, hspace=0.2)
     ax_1 = fig.add_subplot(2, 1, 1)
     ax_2 = fig.add_subplot(2, 1, 2)
 
-    ax_1.set_position([0.1, 0.48, 0.8, 0.2])
-    ax_2.set_position([0.1, 0.14, 0.8, 0.2])
+    ax_1.set_position([0.099, 0.506, 0.8, 0.2])
+    ax_2.set_position([0.099, 0.14, 0.8, 0.2])
 
-    ax_1.set_title(TITLE_OF_TOTAL, loc="left", pad=10, fontsize="20", fontweight="bold", color="black")
-    ax_2.set_title(TITLE_OF_RULES, loc="left", pad=10, fontsize="20", fontweight="bold", color="black")
+    ax_1.set_title(TITLE_OF_TOTAL, loc="left", pad=18, fontsize="20", fontweight="bold", color="black")
+    ax_2.set_title(TITLE_OF_RULES, loc="left", pad=18, fontsize="20", fontweight="bold", color="black")
 
     aws_managed = waf_log[waf_log.rule.str.match('^AWS')]
     third_party = waf_log[waf_log.rule.str.match('^(?!AWS)')]
 
     draw = DrawHistgramClass()
 
-    draw.histgram(ax_1, waf_log["time"], waf_log["time"], "Total", "gray",)
-    draw.histgram(ax_2, waf_log["time"], aws_managed["time"], "AWS Managed", "indianred",)
-    draw.histgram(ax_2, waf_log["time"], third_party["time"], "Third Party", "skyblue",)
+    draw.histgram(ax_1, waf_log["time"], waf_log["time"], "Total", "gray", utc_offset, y_limit)
+    draw.histgram(ax_2, waf_log["time"], aws_managed["time"], "AWS", "indianred", utc_offset, y_limit)
+    draw.histgram(ax_2, waf_log["time"], third_party["time"], "Third Party", "skyblue", utc_offset, y_limit)
```

## Comparing `accompanist/draw_pi_chart.py` & `accompanist/report/draw_pie_chart.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,99 @@
 import pandas as pd
+import matplotlib.lines as lines
 
 
 class CalcTop5Class:
     def __init__(self):
         self._data = []
         self._top5 = []
         self._dropped = []
 
     def count_top5(self, target_row):
         """
-        Top5のデータを集計する（上位6位以下の合計を計算し、Othersとする）
+        Calculate top 5 data
         """
         self._data = target_row.value_counts(sort=True) / target_row.value_counts().sum() * 100
         self._top5 = self._data[:5]
         self._dropped = self._data.drop(self._top5.index)
         self._top5["(Others)"] = pd.Series(self._dropped[0:].sum(), dtype="float64").to_string(index=False)
         return self._top5
 
 
-class DrawPiChartClass:
+class DrawpieChartClass:
     def __init__(self):
         self._colors = ["#2466a9", "#3f86bf", "#609fc6", "#88b5ce", "#bcd4e5", "#B2B2B2"]  # Blue palette
         self._wedgeprops = {"alpha": 0.9, "edgecolor": "white", "linewidth": 1, "width": 0.7}
-        self._textprops = {"weight": "bold", "color": "#ffff00", "fontsize": "12"}
+        self._textprops = {"weight": "bold", "color": "#ffff00", "fontsize": "14"}
 
-    def pi_chart(self, ax, data, title):
+    def pie_chart(self, ax, data, title):
         """
-        円グラフを描画する
+        Draw pie chart
         """
         ax.pie(data, colors=self._colors, startangle=90, counterclock=False,
                labels=data.index, pctdistance=0.7,
                autopct=lambda p: "{: .0f}%".format(p) if p >= 3 else "",
                wedgeprops=self._wedgeprops, textprops=self._textprops, labeldistance=None)
         ax.legend(loc="upper left", bbox_to_anchor=(1.3, 0.9),
-                  prop={"size": "14", "weight": "bold"}, frameon=False, ncol=1)
+                  prop={"size": "16", "weight": "bold"}, frameon=False, ncol=1)
         ax.set_title(title, loc="left", pad=10, fontsize="20", fontweight="bold", color="black")
 
 
-def draw_pi_chart(data_frame, fig_a, fig_b):
+def draw_pie_chart(data_frame, fig_a, fig_b, mask_ip):
     """
-    Draw pi chart for top 5
+    Draw pie chart for top 5
     """
     global top5
     top5 = [0] * 4
 
     calc = CalcTop5Class()
 
     for i in range(len(top5)):
         top5[i] = calc.count_top5(data_frame.iloc[:, i + 1])
 
+    if mask_ip:
+        top5[2] = (mask_ip_addresses(top5[2]))
+
     fig_a.subplots_adjust(top=0.8, left=-0.5, hspace=0.2)
     fig_b.subplots_adjust(top=0.8, left=-0.5, hspace=0.2)
 
+    # Add note for country code
+    fig_b.add_artist(lines.Line2D([0.66, 0.93], [0.16, 0.16], color="#eeeeee", linewidth=60, zorder=0))
+    cc_note = "Please refer to the following for the country code."
+    cc_link = "https://en.wikipedia.org/wiki/ISO_3166-2"
+    fig_b.text(0.64, 0.17, cc_note, fontsize=12, ha="left")
+    fig_b.text(0.64, 0.13, cc_link, fontsize=12, ha="left", color="blue",
+               url="https://en.wikipedia.org/wiki/ISO_3166-2")
+
     ax_a_1 = fig_a.add_subplot(2, 1, 1)
     ax_a_2 = fig_a.add_subplot(2, 1, 2)
     ax_b_1 = fig_b.add_subplot(2, 1, 1)
     ax_b_2 = fig_b.add_subplot(2, 1, 2)
 
-    ax_a_1.set_position([0.02, 0.46, 0.4, 0.3])
-    ax_a_2.set_position([0.02, 0.06, 0.4, 0.3])
-    ax_b_1.set_position([0.02, 0.46, 0.4, 0.3])
-    ax_b_2.set_position([0.02, 0.06, 0.4, 0.3])
-
-    draw = DrawPiChartClass()
-
-    draw.pi_chart(ax_a_1, top5[0], "Terminating Rule Group")
-    draw.pi_chart(ax_a_2, top5[1], "URI")
-    draw.pi_chart(ax_b_1, top5[2], "IP Address")
-    draw.pi_chart(ax_b_2, top5[3], "Country")
+    ax_a_1.set_position([0.004, 0.42, 0.4, 0.3])
+    ax_a_2.set_position([0.004, 0.06, 0.4, 0.3])
+    ax_b_1.set_position([0.004, 0.42, 0.4, 0.3])
+    ax_b_2.set_position([0.004, 0.06, 0.4, 0.3])
+
+    draw = DrawpieChartClass()
+
+    draw.pie_chart(ax_a_1, top5[0], "Terminating Rule Group")
+    draw.pie_chart(ax_a_2, top5[1], "Path Name")
+    draw.pie_chart(ax_b_1, top5[2], "IP Address")
+    draw.pie_chart(ax_b_2, top5[3], "Country")
+
+
+def mask_ip_addresses(ip_dataframe):
+    """
+    Mask IP adress if the option was set
+    """
+    masked_ips = []
+    for i in range(len(ip_dataframe)):
+        ip_segments = str(ip_dataframe.index[i]).split(".")
+        if i != 5:
+            ip_segments[0] = "xxx"
+            ip_segments[1] = "xxx"
+        masked_ip = '.'.join(ip_segments)
+        masked_ips.append(masked_ip)
+    ip_dataframe.index = [masked_ips[0], masked_ips[1], masked_ips[2],
+                          masked_ips[3], masked_ips[4], masked_ips[5]]
+    return ip_dataframe
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `accompanist/draw_table.py` & `accompanist/report/draw_table.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import json
 import numpy as np
 
+CONFIG_FILE = "config.json"
 
 def draw_table(waf_log, fig):
     """
     Draw a table
     """
-    TABLE_TITLE = "Number of Requests per URI"
+    TABLE_TITLE = "Number of Requests per Path Name"
     uri_data = calc_count_of_uris(waf_log)
 
-    fig.subplots_adjust(top=0.8, left=0.2, right=0.8, hspace=0.1)
+    fig.subplots_adjust(top=0.64, left=0.04, right=0.82, hspace=0)
     ax = fig.add_subplot(1, 1, 1)
     ax.axis("off")
-    ax.set_title(TABLE_TITLE, loc="left", y=0.8, x=-0.14, fontsize="20",
+    ax.set_title(TABLE_TITLE, loc="left", y=1.17, x=0.07, fontsize="20",
                  fontweight="bold", color="black")
 
-    col_labels = ["No.", "URI", "Count"]
-    col_widths = [0.1, 0.7, 0.1]
-    col_colors = ["#000000", "#000000", "#000000"]
+    col_labels = ["No.", "Path Name", "Total Count"]
+    col_widths = [0.1, 0.6, 0.2]
+    col_colors = ["#3d3d3d", "#3d3d3d", "#3d3d3d"]
 
     cell_colors = np.full_like(uri_data, "", dtype=object)
     for i in range(len(uri_data)):
         if i % 2 == 0:
             for j in range(3):
                 cell_colors[i, j] = "#FFFFFF"
         else:
@@ -30,48 +31,74 @@
 
     uri_table = ax.table(cellText=uri_data,
                          cellColours=cell_colors,
                          colLabels=col_labels,
                          colColours=col_colors,
                          colWidths=col_widths,
                          colLoc="center",
-                         loc="center",
+                         loc="upper left",
+                         bbox=[0.1, 0.1, 0.9, 1.0]
                          )
+    # Cell Height contol
+    cellDict = uri_table.get_celld()
+    for j in range(0, len(col_labels)):
+        cellDict[(0, j)].set_height(1.2)
+        for i in range(1, len(uri_data) + 1):
+            cellDict[(i, j)].set_height(1)
 
     for i in range(1, len(uri_data) + 1):
         uri_table[i, 0]._text.set_horizontalalignment("center")
         uri_table[i, 1]._text.set_horizontalalignment("left")
         uri_table[i, 2]._text.set_horizontalalignment("right")
 
     for j in range(0, 3):
         uri_table[0, j]._text.set_color("white")
 
     for i in range(0, len(uri_data)):
-        if int(uri_data[i][2]) >= 10:
-            uri_table[i + 1, 2]._text.set_color("red")
-        elif int(uri_data[i][2]) >= 2:
-            uri_table[i + 1, 2]._text.set_color("orange")
+        if uri_data[i][2] != "":
+            if int(uri_data[i][2]) >= 10:
+                uri_table[i + 1, 2]._text.set_color("#F30100")
+            elif int(uri_data[i][2]) >= 1:
+                uri_table[i + 1, 2]._text.set_color("#F47A55")
 
-    uri_table.scale(1.44, 2.6)
     uri_table.auto_set_font_size(False)
-    uri_table.set_fontsize(20)
+    uri_table.set_fontsize(18)
+
+    for key, cell in uri_table.get_celld().items():
+        cell.set_linewidth(2)
+        cell.set_edgecolor("white")
+
+    note = "[Note] The total count is inaccurate if the COUNT action is chosen because one or more rules may count some requests."
+    ax.text(0.1, 0.01, note, color="black", fontsize=12)
 
 
 def calc_count_of_uris(waf_log):
     """
     Count the number of URIs
     """
 
-    f = open("./config.json", "r")
+    f = open(CONFIG_FILE, "r")
     settings_file = json.load(f)
     f.close()
 
     uris = settings_file["target_uri"]
     counted_uris = []
+    index = 0
     for uri in uris:
         count = 0
-        index = uris.index(uri) + 1
-        if uri in waf_log["uri"].values:
-            count = waf_log.groupby("uri").get_group(uri)["uri"].count()
-        counted_uris.append([index, uri, count])
+        index = index + 1
+        if index <= 12:
+            if uri in waf_log["uri"].values:
+                count = waf_log.groupby("uri").get_group(uri)["uri"].count()
+            counted_uris.append([index, uri, count])
+        else:
+            warning = "[Warning] Some paths can't be shown because the number of paths may be exceeded."
+            print("\033[33m" + warning + "\033[0m")
+            exit
+
+    if len(uris) < 12:
+        index = len(uris)
+        for i in range(12 - len(uris)):
+            index = index + 1
+            counted_uris.append([index, "", ""])
 
     return (counted_uris)
```

## Comparing `accompanist/utility_module.py` & `accompanist/report/utility_module.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,87 @@
 import datetime
 import json
 import site
 import os
 import matplotlib.lines as lines
 from PIL import Image
 
-# REPORT_MAIN_COLOR = "#883D1A"
-# MAIN_COLOR = "#56c3ed"
 LOGO_FILE = "logo_trans_small.png"
+SHEET_MUSIC_FILE = "sheet_music.json"
 
 
 class WriteHeaderFooterClass():
     """
     Write header and footer class
     """
 
     def __init__(self):
 
         self._dic_box = {
             "facecolor": "White",
-            "edgecolor": "#2b7700",
-            "boxstyle": "Square, pad=0.5",
+            "edgecolor": "#757575",
+            "boxstyle": "Round, pad=0.7",
             "linewidth": 3,
         }
 
     def header_footer(self, fig, page_number, term, color):
-        with open("./previous_music.json", mode="r") as f:
+        with open(SHEET_MUSIC_FILE, mode="r") as f:
             settings_dict = json.load(f)
 
         MAIN_COLOR = color
 
         # Header
-        page_title = "AWS WAF Log  ( Action: " + settings_dict["mode"] + " )"
-        web_acl = settings_dict["web_acl"].lstrip("aws-waf-logs-")
+        page_title = "AWS WAF Log  (Action: " + settings_dict["action"] + ")"
+        log_group = settings_dict["log_group"].replace("aws-waf-logs-", "")
+        if len(log_group) > 15:
+            log_group = log_group[:15] + "*****"
         fig.add_artist(lines.Line2D([0, 1], [0.94, 0.94], color=MAIN_COLOR, linewidth=80, zorder=0))
 
         fig.text(0.05, 0.91, page_title, color="#ffffff", fontsize=26, fontweight="bold")
-        fig.text(0.70, 0.8, "WebACL: " + web_acl, color="#2b7700", fontsize=16, fontweight="bold", bbox=self._dic_box)
-        fig.text(0.72, 0.74, term, color="black", fontsize=12)
+        fig.text(0.71, 0.82, "Log Group: " + log_group, color="#757575", fontsize=14, fontweight="bold", bbox=self._dic_box)
+        fig.text(0.7, 0.76, term, color="#757575", fontsize=14)
 
         # Footer
         fig.add_artist(lines.Line2D([0, 1], [0.0004, 0.0004], color=MAIN_COLOR, linewidth=80, zorder=0))
-        fig.text(0.9, 0.025, page_number, color="#d3b734", fontsize=20, fontweight="bold")
+        fig.text(0.92, 0.02, page_number, color="#949494", fontsize=20, fontweight="bold")
 
         # Logo
         logo_path = "".join(site.getsitepackages()) + "/accompanist/resource/" + LOGO_FILE
         if os.path.isfile(logo_path):
-            fig.figimage(Image.open(logo_path), xo=500, yo=7)
+            fig.figimage(Image.open(logo_path), xo=500, yo=10)
         else:
             print("Logo file is not found.")
 
 
-def calc_term(time):
+def calc_term(time, utc_offset):
     """
     Show term
     """
-    with open("./previous_music.json", mode="r") as f:
+    with open(SHEET_MUSIC_FILE, mode="r") as f:
         settings_dict = json.load(f)
 
-    oldest_time = datetime.datetime.fromtimestamp(time[len(time) - 1] / 1000.0).strftime("%m/%d %H:%M")
-    latest_time = datetime.datetime.fromtimestamp(time[0] / 1000.0).strftime("%m/%d %H:%M")
+    offset = 3600 * utc_offset
+    print("[Info] The current UTC offset is \"" + str(utc_offset) + "\". You can change the offset with an option, --utc-offset N.")
+
+    oldest_time = datetime.datetime.fromtimestamp(time[len(time) - 1] / 1000.0 + offset, tz=datetime.timezone.utc).strftime("%m/%d %H:%M")
+    latest_time = datetime.datetime.fromtimestamp(time[0] / 1000.0 + offset, tz=datetime.timezone.utc).strftime("%m/%d %H:%M")
 
     days = str(settings_dict["days"])
-    return oldest_time + " - " + latest_time + " ( " + days + " days )"
+
+    if int(days) > 1:
+        term = days + " days (" + oldest_time + " - " + latest_time + ")"
+    else:
+        term = oldest_time + " - " + latest_time
+    return term
 
 
-def write_header_and_footer(waf_log_time, figs, color):
+def write_header_and_footer(waf_log_time, figs, utc_offset, color):
     """
     Add header and footer
     """
-    term = calc_term(waf_log_time)
+    term = calc_term(waf_log_time, utc_offset)
 
     write = WriteHeaderFooterClass()
 
     for fig in (figs):
         page_number = str(figs.index(fig) + 1) + " / " + str(len(figs))
         write.header_footer(fig, page_number, term, color)
-
-
-def write_comment(fig):
-    """
-    Add comment page (last page)
-    """
-    with open("config.json", mode="r") as f:
-        config_dict = json.load(f)
-
-    comment_item_1 = config_dict["comment"][0]
-    comment_item_2 = config_dict["comment"][1]
-    comment_item_3 = config_dict["comment"][2]
-    comment_item_4 = config_dict["comment"][3]
-    comment_item_5 = config_dict["comment"][4]
-
-    fig.text(0.1, 0.7, "Comment", color="black", fontsize=20, fontweight="bold")
-    fig.text(0.1, 0.6, comment_item_1, color="black", fontsize=20, wrap=True, fontfamily="YuGothic")
-    fig.text(0.1, 0.5, comment_item_2, color="black", fontsize=20, wrap=True, fontfamily="YuGothic")
-    fig.text(0.1, 0.4, comment_item_3, color="black", fontsize=20, wrap=True, fontfamily="YuGothic")
-    fig.text(0.1, 0.3, comment_item_4, color="black", fontsize=20, wrap=True, fontfamily="YuGothic")
-    fig.text(0.1, 0.2, comment_item_5, color="black", fontsize=20, wrap=True, fontfamily="YuGothic")
```

## Comparing `accompanist-1.0.4.dist-info/LICENSE` & `accompanist-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `accompanist-1.0.4.dist-info/RECORD` & `accompanist-1.1.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-accompanist/draw_histgram.py,sha256=kJhFAad1NKrQqpgdSi6NrqU2aK7BqyjzMAma-jGCyMY,3685
-accompanist/draw_pi_chart.py,sha256=P8j5EquO5ampocBwp6hUoJFduB20LmzYAc-MLNfeQA4,2545
-accompanist/draw_table.py,sha256=tzWnrBty7oeY9H1APpsfV8DJFnsjurFn3xNvR1Nv84k,2317
-accompanist/listen.py,sha256=uDtJs8ghrO2v9TLCank7UsyKCx52QxPmL2-X3l8YQqM,3350
-accompanist/main.py,sha256=KRXs-yQ7uIVllRk6haxqm-GbHIQOeeVpqJ3h9ZuPMfM,204
-accompanist/play.py,sha256=CzQDeRLUXGjXYTB4CwFN3cwOeliMlCEEPWCmvdLCogQ,1551
-accompanist/utility_module.py,sha256=UqtI_P2I2hdL5AwSCf9ISn7vkp5uWuV25PRB6YCeGXU,3450
-accompanist/write_front_cover.py,sha256=u6s6jA_qTBKG8rzKnOpeSU1tZ8oZSdDp70V5pzoyQuQ,742
+accompanist/cmd_init.py,sha256=OLo47_jHWs60veUjy2UwLOU4LnXzWE7OrPg792F06jw,1423
+accompanist/cmd_listen.py,sha256=bLEMLzyFMQYxZI06JvJVyyWBMP4KDMxC-9xLixPYrQg,5229
+accompanist/cmd_play.py,sha256=UUmb5vK0q4GwWBEya-8XfBzcAzWLtGaGr61P9cnWXdg,2968
+accompanist/main.py,sha256=xlbFfTD9O7s_6IOoOFjrXQs0EaT1M4pAFxSmCdmr_SA,732
+accompanist/version.py,sha256=LGVQyDsWifdACo7qztwb8RWWHds1E7uQ-ZqD8SAjyw4,22
+accompanist/report/draw_histgram.py,sha256=Pfx-Aeof53v3FsYF0kEeilmNAGi8NIppnX_SwPMHw-o,3945
+accompanist/report/draw_pie_chart.py,sha256=nbboVXR2--dCc65QyvfaHLgmb3Hk_fK17SM5ScC0Noc,3593
+accompanist/report/draw_table.py,sha256=Q8alH0uWr7E4dfobgyKQGZy0RdSOlHshAChyVE1Qa74,3375
+accompanist/report/utility_module.py,sha256=7bWcRuJNK7iNNvEmsm0LXeEqSB4SkVTXto33_o-oiKU,2907
+accompanist/report/write_comment.py,sha256=igcU0ZSAHwYGaq3itCtfIDXLAKNi-8fGiYxjWagh00Q,1419
+accompanist/report/write_front_cover.py,sha256=XbUTRbiBhn5qI4cM14rYAgvKPMJqtYhVQS_42GYMQNY,1317
 accompanist/resource/logo_trans.png,sha256=IbkfTLMa9qzSifN32YocbOdpDRecelHA7k8cLrBVK_4,19193
 accompanist/resource/logo_trans_small.png,sha256=SS9AlZGL3Ce-6BbD4EW5rbn7zuDcje7HkEXW_lHE2zs,6761
-accompanist-1.0.4.dist-info/LICENSE,sha256=EHImwl3uAjnXzz33MkVgnfcyDByFp0t6O-H4QaGLs4M,1063
-accompanist-1.0.4.dist-info/METADATA,sha256=-LivK1MKR5elP7zKKR_kBi3sRL_KrQLu5JXcGFSYcjo,2182
-accompanist-1.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-accompanist-1.0.4.dist-info/entry_points.txt,sha256=gLZwXDl7kf85kYQ1HNQZSxCe81vLub8Eb8wWqrThDeM,53
-accompanist-1.0.4.dist-info/top_level.txt,sha256=HMR4fV8gkGDO-4DjMdWJYDM6NtMypoCtBRNUiLC6Jpc,12
-accompanist-1.0.4.dist-info/RECORD,,
+accompanist-1.1.0.dist-info/LICENSE,sha256=EHImwl3uAjnXzz33MkVgnfcyDByFp0t6O-H4QaGLs4M,1063
+accompanist-1.1.0.dist-info/METADATA,sha256=9y2PTU9AvaZvtuf5Be_yz6OBfrbcFGMEZYNjgrFDX0U,3477
+accompanist-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+accompanist-1.1.0.dist-info/entry_points.txt,sha256=gLZwXDl7kf85kYQ1HNQZSxCe81vLub8Eb8wWqrThDeM,53
+accompanist-1.1.0.dist-info/top_level.txt,sha256=vUeFtOUVsBOaqJK8b1z7iVPvaRhz3jGN4Uw79o1o9Ck,31
+accompanist-1.1.0.dist-info/RECORD,,
```

