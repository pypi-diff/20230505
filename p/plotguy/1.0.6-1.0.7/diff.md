# Comparing `tmp/plotguy-1.0.6.tar.gz` & `tmp/plotguy-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotguy-1.0.6.tar", last modified: Sat Apr 29 03:04:05 2023, max compression
+gzip compressed data, was "plotguy-1.0.7.tar", last modified: Fri May  5 07:13:11 2023, max compression
```

## Comparing `plotguy-1.0.6.tar` & `plotguy-1.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-29 03:04:05.431820 plotguy-1.0.6/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-04-29 03:04:05.431668 plotguy-1.0.6/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.0.6/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-29 03:04:05.430703 plotguy-1.0.6/plotguy/
--rw-r--r--   0 cmw        (501) staff       (20)    25461 2023-04-29 03:02:55.000000 plotguy-1.0.6/plotguy/__init__.py
--rw-r--r--   0 cmw        (501) staff       (20)    16762 2023-02-28 03:04:57.000000 plotguy-1.0.6/plotguy/aggregate.py
--rw-r--r--   0 cmw        (501) staff       (20)    63231 2023-04-18 03:28:10.000000 plotguy-1.0.6/plotguy/components.py
--rw-r--r--   0 cmw        (501) staff       (20)    37694 2023-04-18 03:32:08.000000 plotguy-1.0.6/plotguy/equity_curves.py
--rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.0.6/plotguy/signals.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-04-29 03:04:05.431481 plotguy-1.0.6/plotguy.egg-info/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-04-29 03:04:05.000000 plotguy-1.0.6/plotguy.egg-info/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)      279 2023-04-29 03:04:05.000000 plotguy-1.0.6/plotguy.egg-info/SOURCES.txt
--rw-r--r--   0 cmw        (501) staff       (20)        1 2023-04-29 03:04:05.000000 plotguy-1.0.6/plotguy.egg-info/dependency_links.txt
--rw-r--r--   0 cmw        (501) staff       (20)      124 2023-04-29 03:04:05.000000 plotguy-1.0.6/plotguy.egg-info/requires.txt
--rw-r--r--   0 cmw        (501) staff       (20)        8 2023-04-29 03:04:05.000000 plotguy-1.0.6/plotguy.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-04-29 03:04:05.431871 plotguy-1.0.6/setup.cfg
--rw-r--r--   0 cmw        (501) staff       (20)      814 2023-04-29 03:03:27.000000 plotguy-1.0.6/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-05 07:13:11.752160 plotguy-1.0.7/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-05-05 07:13:11.751918 plotguy-1.0.7/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.0.7/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-05 07:13:11.750527 plotguy-1.0.7/plotguy/
+-rw-r--r--   0 cmw        (501) staff       (20)    24678 2023-05-05 07:11:41.000000 plotguy-1.0.7/plotguy/__init__.py
+-rw-r--r--   0 cmw        (501) staff       (20)    16762 2023-02-28 03:04:57.000000 plotguy-1.0.7/plotguy/aggregate.py
+-rw-r--r--   0 cmw        (501) staff       (20)    63231 2023-04-18 03:28:10.000000 plotguy-1.0.7/plotguy/components.py
+-rw-r--r--   0 cmw        (501) staff       (20)    37694 2023-04-18 03:32:08.000000 plotguy-1.0.7/plotguy/equity_curves.py
+-rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.0.7/plotguy/signals.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-05 07:13:11.751639 plotguy-1.0.7/plotguy.egg-info/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-05-05 07:13:11.000000 plotguy-1.0.7/plotguy.egg-info/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)      279 2023-05-05 07:13:11.000000 plotguy-1.0.7/plotguy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        1 2023-05-05 07:13:11.000000 plotguy-1.0.7/plotguy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmw        (501) staff       (20)      131 2023-05-05 07:13:11.000000 plotguy-1.0.7/plotguy.egg-info/requires.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        8 2023-05-05 07:13:11.000000 plotguy-1.0.7/plotguy.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-05-05 07:13:11.752237 plotguy-1.0.7/setup.cfg
+-rw-r--r--   0 cmw        (501) staff       (20)      832 2023-05-05 07:12:29.000000 plotguy-1.0.7/setup.py
```

### Comparing `plotguy-1.0.6/plotguy/__init__.py` & `plotguy-1.0.7/plotguy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 import itertools
 import multiprocessing as mp
 import zlib
 import requests
 from bs4 import BeautifulSoup
 import pandas as pd
+import polars as pl
 import numpy as np
-# import polars as pl
 
 from .equity_curves import *
 from .signals import *
 from .aggregate import *
 
+
 def multi_process(function, parameters, number_of_core=8):
     pool = mp.Pool(processes=number_of_core)
     pool.map(function, parameters)
     pool.close()
 
 
 def filename_only(para_combination):
@@ -24,15 +25,14 @@
     end_date = para_combination['end_date']
     py_filename = para_combination['py_filename']
     start_date_str = datetime.datetime.strptime(start_date, '%Y-%m-%d').strftime("%Y%m%d")
     end_date_str = datetime.datetime.strptime(end_date, '%Y-%m-%d').strftime("%Y%m%d")
     summary_mode = para_combination['summary_mode']
     freq = para_combination['freq']
 
-
     save_name = f'file={py_filename}&date={start_date_str}{end_date_str}&freq={freq}&summary_mode={summary_mode}&'
 
     for key in list(para_dict.keys()):
         para = para_combination[key]
         if key == 'code':
             if str(para).isdigit():
                 para = str(para).zfill(5)
@@ -48,31 +48,118 @@
 
 def path_reference_code(save_name):
     reference_code = str(zlib.crc32(bytes(save_name, 'UTF-8')))[:6]
     return reference_code
 
 
 def generate_filepath(para_combination, folder=''):
-
     file_format = para_combination['file_format']
 
     if not file_format == 'parquet':
         file_format = 'csv'
 
     save_name = filename_only(para_combination)
-
     reference_code = path_reference_code(save_name)
-    save_name = reference_code + '_' + save_name[:-1]     # position -1 to avoid '&' at the end
-
     output_folder = para_combination['output_folder']
-    filepath = os.path.join(folder,output_folder, f'{save_name}.{file_format}')
+    filepath = os.path.join(folder, output_folder, f'{para_combination["code"]}_{reference_code}.{file_format}')
 
     return filepath
 
 
+def apply_pnl(row):
+    # This is one line of backtest, i.e. one trade
+    # Purpose if this is to calculate unrealized pnl between open date and close date, aggreagte same day pnl with other trade,
+    # also save realized pnl
+
+    df_daily = apply_pnl.df_daily
+
+    open_date = row.open_date
+    close_date = row.date
+    now_close = df_daily.at[open_date, 'close']
+    dates = pd.date_range(start=open_date, end=close_date)
+    open_price = row.open_price
+    num_of_share = row.num_of_share
+    commission = row.commission
+    action = row.action
+    realized_pnl = row.realized_pnl
+
+    last_realized_capital = apply_pnl.last_realized_capital
+    multiplier = apply_pnl.multiplier
+
+    for date in dates:
+        if date == open_date:
+            # Unrealized pnl on the open date, record on df_daily
+            df_daily.at[open_date, 'action'] = 'open'
+            unrealized_pnl = num_of_share * multiplier * (now_close - open_price) - commission
+            unrealized_pnl = round(unrealized_pnl, 3)
+            df_daily.at[open_date, 'unrealized_pnl'] = unrealized_pnl
+
+            # print(open_date, 'Open!', open_price, now_close, num_of_share, unrealized_pnl)
+
+        elif date == close_date:  # close position on this date, end of this trade
+            # this is a same day trade
+            # clear the open unrealized pnl as open and close same day should not aggregate
+            # it should be record as realized pnl directly
+            if open_date == close_date:
+                df_daily.at[date, 'unrealized_pnl'] = None
+
+            # unrealized_pnl
+            if df_daily.at[date, 'unrealized_pnl']:  # if there is already unrealized_pnl, aggregate
+                df_daily.at[date, 'unrealized_pnl'] = df_daily.at[date, 'unrealized_pnl'] + realized_pnl
+            else:
+                df_daily.at[date, 'unrealized_pnl'] = realized_pnl
+
+            # realized pnl
+            if df_daily.at[date, 'realized_pnl']:  # if there is already realized_pnl, aggregate
+                df_daily.at[date, 'realized_pnl'] = df_daily.at[date, 'realized_pnl'] + realized_pnl
+            else:
+                df_daily.at[date, 'realized_pnl'] = realized_pnl
+
+            df_daily.at[date, 'action'] = action
+            df_daily.at[date, 'commission'] = commission
+            last_realized_capital = last_realized_capital + realized_pnl
+
+            # print(date, 'Close!', open_price, close_date, realized_pnl)
+            # print()
+
+        else:
+            try:
+                now_close = df_daily.at[date, 'close']
+                unrealized_pnl = num_of_share * multiplier * (now_close - open_price) - commission
+                unrealized_pnl = round(unrealized_pnl, 3)
+                if df_daily.at[date, 'unrealized_pnl']:
+                    df_daily.at[date, 'unrealized_pnl'] = df_daily.at[date, 'unrealized_pnl'] + unrealized_pnl
+                else:
+                    df_daily.at[date, 'unrealized_pnl'] = unrealized_pnl
+
+                # print(date, 'Not yet close', open_price, now_close, unrealized_pnl)
+
+            except:
+                pass
+                # print(date, 'Not yet close', 'Holiday!')
+
+    apply_pnl.df_daily = df_daily
+
+
+def df_daily_equity(row):
+    last_equity_value = df_daily_equity.last_equity_value
+    if row.name == 0:
+        return last_equity_value
+    else:
+        if not (row.realized_pnl == None):
+            equity_value = last_equity_value + row.realized_pnl
+            df_daily_equity.last_equity_value = equity_value
+        elif not (row.unrealized_pnl == None):
+            equity_value = last_equity_value + row.unrealized_pnl
+        else:
+            equity_value = None
+
+        return equity_value
+
+
 def mp_cal_performance(tuple_data):
     para_combination = tuple_data[0]
     manager_list = tuple_data[1]
 
     result = cal_performance(para_combination)
 
     # new
@@ -108,120 +195,122 @@
             risk_free_rate = 2  # if network error, set rate to 2 %
             print('Network error. Risk free rate: {:.2f} %'.format(risk_free_rate))
     else:
         print('Risk free rate: {:.2f} %'.format(risk_free_rate))
 
     print('Backtest result is loading. Please wait patiently.')
 
-    manager_list = mp.Manager().list()# To save the result with index number
+    manager_list = mp.Manager().list()  # To save the result with index number
 
     cal_performance_list = []
     for para_combination in all_para_combination:
         para_combination['risk_free_rate'] = risk_free_rate
         cal_performance_list.append((para_combination, manager_list))
 
+    a = datetime.datetime.now()
+
     pool = mp.Pool(processes=number_of_core)
     pool.map(mp_cal_performance, cal_performance_list)
     pool.close()
 
+    b = datetime.datetime.now()
+    t = b - a
+    print('Process time:', t.total_seconds(), 's')
+
     pd.DataFrame(list(manager_list)).to_csv('backtest_result.csv')
 
 
 def plot_signal_analysis(py_filename, output_folder, start_date, end_date, para_dict, signal_settings):
-
-    app = signals.Signals(py_filename, output_folder, start_date, end_date, para_dict, generate_filepath, signal_settings)
+    app = signals.Signals(py_filename, output_folder, start_date, end_date, para_dict, generate_filepath,
+                          signal_settings)
 
     return app
 
 
-def plot(mode, all_para_combination={},  subchart_settings={}, number_of_curves=20, risk_free_rate='geometric_mean'):
-
-    if subchart_settings == {}: # subchart default setting
+def plot(mode, all_para_combination={}, subchart_settings={}, number_of_curves=20, risk_free_rate='geometric_mean'):
+    if subchart_settings == {}:  # subchart default setting
         subchart_settings = {
             'histogram_period': [1, 3, 5, 10, 20],
             'subchart_1': ['volume', 'line']
         }
 
     if mode == 'equity_curves':
         result_df = pd.read_csv('backtest_result.csv', index_col=0)
         app = equity_curves.Plot(all_para_combination, result_df, subchart_settings, number_of_curves)
 
     if mode == 'aggregate':
         app = aggregate.Aggregate(risk_free_rate)
 
-
     return app
 
 
 def get_latest_fed_fund_rate():
     url = "https://fred.stlouisfed.org/series/FEDFUNDS"
     page = requests.get(url)
     soup = BeautifulSoup(page.content, "html.parser")
 
     fed_funds_rate = soup.find("span", class_="series-meta-observation-value").text
     print("Latest Federal Funds Rate:", fed_funds_rate, '%')
     # fed_funds_rate = float(fed_funds_rate) / 100
-    fed_funds_rate = round( float(fed_funds_rate) ,2)
+    fed_funds_rate = round(float(fed_funds_rate), 2)
     return fed_funds_rate
 
 
-def get_geometric_mean_of_yearly_rate(start_year, end_year): # backtest period
+def get_geometric_mean_of_yearly_rate(start_year, end_year):  # backtest period
     url = "https://fred.stlouisfed.org/graph/fredgraph.csv?id=DTB3"
     response = requests.get(url)
     data = response.text.split("\n")[:-1]
     data = [row.split(",") for row in data]
     df = pd.DataFrame(data[1:], columns=data[0])
     df.columns = ["date", "risk_free_rate"]
     df["date"] = pd.to_datetime(df["date"])
     df["risk_free_rate"] = pd.to_numeric(df["risk_free_rate"], errors='coerce')
     df.dropna(subset=['risk_free_rate'], inplace=True)
 
     risk_free_rate_history_yearly = df.resample("A", on="date").mean()
     risk_free_rate_history_yearly = risk_free_rate_history_yearly.round(3)
 
     # show only start between start_year and end_year
-    risk_free_rate_history_yearly = risk_free_rate_history_yearly[risk_free_rate_history_yearly.index.year >= start_year]
+    risk_free_rate_history_yearly = risk_free_rate_history_yearly[
+        risk_free_rate_history_yearly.index.year >= start_year]
     risk_free_rate_history_yearly = risk_free_rate_history_yearly[risk_free_rate_history_yearly.index.year <= end_year]
 
     fed_fund_rate_geometric_mean = np.exp(np.log(risk_free_rate_history_yearly["risk_free_rate"]).mean())
-    fed_fund_rate_geometric_mean = round(fed_fund_rate_geometric_mean,2)
-    print("Federal Funds Rate Geometric mean from {} to {}: {} %".format(start_year, end_year, fed_fund_rate_geometric_mean))
+    fed_fund_rate_geometric_mean = round(fed_fund_rate_geometric_mean, 2)
+    print("Federal Funds Rate Geometric mean from {} to {}: {} %".format(start_year, end_year,
+                                                                         fed_fund_rate_geometric_mean))
 
     return fed_fund_rate_geometric_mean
 
 
-def calculate_mdd(df_csv, col):
-    df = df_csv.copy()
+def calculate_mdd(df, col):
     roll_max = df[col].cummax()
     daily_drawdown = df[col] / roll_max - 1.0
     max_daily_drawdown = daily_drawdown.cummin()
 
     return min(list(max_daily_drawdown)), min(list(df[col] - roll_max))
 
 
-def calculate_win_rate_info(df_csv):
-    df = df_csv.copy()
+def calculate_win_rate_info(df):
     num_of_trade = list(df['action'] == 'open').count(True)
     num_of_loss = list(df['pnl'] < 0).count(True)
     num_of_win = num_of_trade - num_of_loss
 
     if num_of_trade > 0:
         win_rate = round(100 * num_of_win / num_of_trade, 2)
         loss_rate = round(100 * num_of_loss / num_of_trade, 2)
     else:
         win_rate = '--'
         loss_rate = '--'
 
-    # win_rate = str(int(round(100 * num_of_win / num_of_trade, 0))) if num_of_trade > 0 else '--'
-
     return num_of_trade, num_of_loss, num_of_win, win_rate, loss_rate
 
 
 def calculate_win_rate(df_csv):
-    df = df_csv.copy()
+    df = df_csv[['date', 'realized_pnl', 'action']].copy()
     df = df[df['action'].notnull()].reset_index(drop=True)
     df['date'] = pd.to_datetime(df['date'], format='%Y-%m-%d')
     df['pnl'] = df['realized_pnl'].shift(-1)
     df['year'] = pd.DatetimeIndex(df['date']).year
     year_list = list(set(df['year']))
     year_list.sort()
 
@@ -230,34 +319,34 @@
 
     for year in year_list:
         win_rate_dict[year] = calculate_win_rate_info(df.loc[df['year'] == year])
 
     return win_rate_dict
 
 
-def calculate_sharp_ratio(df_csv, col, risk_free_rate):
-    df = df_csv.copy()
+def calculate_sharp_ratio(df, col, risk_free_rate):
     holding_period_day = (df.loc[df.index[-1], 'date'] - df.loc[df.index[0], 'date']).days
     net_profit = df.at[df.index[-1], col] - df.at[df.index[0], col]
 
     initial_capital = df.loc[df.index[0], col]
 
     # To avoid power error below
     if net_profit < 0 and abs(net_profit) > initial_capital:
         net_profit = initial_capital * -1
 
     equity_value_pct_series = df[col].pct_change()
     equity_value_pct_series = equity_value_pct_series.dropna()
 
     return_on_capital = net_profit / initial_capital
-    annualized_return = (1 + return_on_capital) ** (365 / holding_period_day) - 1
+    annualized_return = (np.sign(1 + return_on_capital) * np.abs(1 + return_on_capital)) ** (
+                365 / holding_period_day) - 1
     annualized_std = equity_value_pct_series.std() * math.sqrt(365)
 
     if annualized_std > 0:
-        annualized_sr = (annualized_return - float(risk_free_rate)/100 ) / annualized_std
+        annualized_sr = (annualized_return - float(risk_free_rate) / 100) / annualized_std
     else:
         annualized_sr = 0
 
     return_on_capital = round(100 * return_on_capital, 2)
     annualized_return = round(100 * annualized_return, 2)
     annualized_std = round(100 * annualized_std, 2)
     annualized_sr = round(annualized_sr, 2)
@@ -266,218 +355,124 @@
 
 
 def resample_summary_to_daily(para_combination, folder=''):
     # Need to deal with the start date and date
 
     start_date = para_combination['start_date']
     end_date = para_combination['end_date']
+    start_date_datetime = datetime.datetime.strptime(start_date, '%Y-%m-%d')
+    end_date_datetime = datetime.datetime.strptime(end_date, '%Y-%m-%d')
 
     sec_profile = para_combination['sec_profile']
 
     sectype = sec_profile['sectype']
     lot_size_dict = sec_profile['lot_size_dict']
     code = para_combination['code']
     lot_size = lot_size_dict[code]
 
     intraday = para_combination['intraday']
     freq = para_combination['freq']
     file_format = para_combination['file_format']
     sec_profile = para_combination['sec_profile']
 
-
     if sectype == 'FUT':
         margin_req = sec_profile['margin_req']
         multiplier = sec_profile['multiplier']
     elif sectype == 'STK':
         multiplier = 1
 
-
     # Read backtest data
-    save_path = generate_filepath(para_combination=para_combination,folder=folder)
+    save_path = generate_filepath(para_combination=para_combination, folder=folder)
+
     if file_format == 'parquet':
-        df_backtest = pd.read_parquet(save_path) # Daraframe that may not be daily
-        ### parquet specific, All backtest force to treart as summary, # ie filter action only
-        # df_backtest = df_backtest.loc[df_backtest['action'] != ''].copy()
-        # df_backtest = df_backtest.loc[df_backtest['action'].isnull() == False].copy()
+        df = pl.read_parquet(save_path)
     else:
-        df_backtest = pd.read_csv(save_path, index_col=0)  # Daraframe that may not be daily
-        ### csv only specific, All backtest force to treart as summary, ie filter action only
-        # df_backtest = df_backtest.loc[df_backtest['action'] != ''].copy()
-        # df_backtest = df_backtest.loc[df_backtest['action'].isnull() == False].copy()
-
-    df_backtest = df_backtest.loc[df_backtest['action'] != ''].copy()
-    df_backtest = df_backtest.loc[df_backtest['action'].isnull() == False].copy()
-
-    df_backtest['date'] = pd.to_datetime(df_backtest['date'], format='%Y-%m-%d')
-    df_backtest = df_backtest.loc[(df_backtest['date'] >= start_date) & (df_backtest['date'] <= end_date)]
-    df_backtest = df_backtest.reset_index(drop=True)  # Reset Index
-
+        df = pl.read_csv(save_path, try_parse_dates=True)
 
-
-    df_daily = pd.DataFrame()  # Dataframe for Daily
-
-
-
-
-    # check if df_backtest 0 length:
-    if len(df_backtest) == 0:
+    # Calculate initial capital before trim the dataframe
+    if len(df) == 0:
+        # This would happen when it is summary mode and no trade for the strategy
+        # Note that in intra day but not summary mode, length of df of  no trade df_bakctest is still > 0
         initial_capital = sec_profile['initial_capital']
     else:
-        initial_capital = df_backtest.iloc[-1].equity_value - df_backtest['realized_pnl'].sum()
-    # initial_capital = df_backtest.iloc[-1].equity_value - df_backtest['realized_pnl'].sum()
+        if pl.sum(df.get_column('realized_pnl')) == None:  # when NOT summary mode but no trade
+            initial_capital = sec_profile['initial_capital']
+        else:
+            initial_capital = df.row(-1, named=True)['equity_value'] - pl.sum(df.get_column('realized_pnl'))
+
     last_realized_capital = initial_capital
 
+    df = (df.lazy()
+          .filter((pl.col('action') != '') &
+                  (pl.col('action').is_not_null()) &
+                  (pl.col('date') >= start_date_datetime) &
+                  (pl.col('date') <= end_date_datetime)
+                  )
+          .select(['date', 'action', 'open_price', 'close', 'commission', 'num_of_share', 'realized_pnl'])
+          .with_columns(pl.col('date').shift(1).alias('open_date'))
+          .with_columns(pl.col('open_price').shift(1).alias('open_price'))
+          .with_columns(pl.col('num_of_share').shift(1).alias('num_of_share'))
+          .filter(pl.col('action') != 'open')
+          .collect()
+          )
+
+    df_backtest = df.to_pandas()
 
     # Read source data
     data_folder = para_combination['data_folder']
     code = para_combination['code']
 
-
-    data_path = os.path.join(folder,data_folder, f'{code}_{freq}.{file_format}')
+    data_path = os.path.join(folder, data_folder, f'{code}_{freq}.{file_format}')
 
     if file_format == 'parquet':
-        df_csv = pd.read_parquet(data_path)
+        df = pl.read_parquet(data_path)
     else:
-        df_csv = pd.read_csv(data_path, index_col=0)
-
-
-    df_csv = df_csv.reset_index(drop=False)
-
-
-
-    df_daily['open'] = df_csv['open']
-    df_daily['high'] = df_csv['high']
-    df_daily['low'] = df_csv['low']
-    df_daily['close'] = df_csv['close']
-    df_daily['volume'] = df_csv['volume']
-    df_daily.index = pd.to_datetime(df_csv['datetime'], format='%Y-%m-%d %H:%M:%S')
-
-    if intraday:
-        df_daily = df_daily.resample('1D').agg({'open': 'first', 'high': 'max', 'low': 'min',
-                                                'close': 'last', 'volume': 'sum',
-                                                }).copy()
-
-    df_daily['date'] = df_daily.index
-    df_daily = df_daily.loc[(df_daily['date'] >= start_date) & (df_daily['date'] <= end_date)]
-    df_daily = df_daily.loc[df_daily['close'].isnull() == False].copy()  # Filter out non trading day
-    df_daily['bah'] = df_daily['close'] * (initial_capital / df_daily.iloc[0].close)  # Calculate all bah value
-    df_daily.at[df_daily.index[0], 'equity_value'] = initial_capital  # Set the equity value at the beginning
-    df_daily['action'] = None
-    df_daily['realized_pnl'] = None
-    df_daily['unrealized_pnl'] = None
-    df_daily['signal_value'] = None
-
-
-
-
-    trade_pair = zip(*(iter(list(df_backtest.index)),) * 2)  # Group df_backtest by 2
-
-
-    for i, j in trade_pair:
-        open_date = df_backtest.at[i, 'date']
-        close_date = df_backtest.at[j, 'date']
-        dates = pd.date_range(start=open_date, end=close_date)  # Determine days between open_date and close_date
-        now_close = df_daily.at[open_date, 'close']
-        # print(i, j)
-        # print(dates)
-        # print(df_backtest.at[i, 'date'], df_backtest.at[i, 'action'])
-        # print(df_backtest.at[j, 'date'], df_backtest.at[j, 'action'])
-
-
-        if sectype == 'STK':
-            num_of_share = lot_size * (last_realized_capital // (now_close * lot_size))
-        elif sectype == 'FUT':
-            num_of_share = last_realized_capital // margin_req
-
-        open_price = df_backtest.at[i, 'open_price']
-        commission = df_backtest.at[j, 'commission']
-
-        df_daily.at[open_date, 'signal_value'] = df_daily.at[open_date, 'bah']  # Mark the open for each trade_pair
-
-        # print(open_price, df_daily.at[open_date, 'bah'])
-
-        # If only one date in the dates (i.e. open and close at the same day), add one more to avoid error
-        if open_date == close_date:
-            dates = list(dates) + list(dates)
-            dates = pd.to_datetime(dates, format='%Y-%m-%d')
-
-        # For the situation that open and close is not the same day. If same, close pnl will replace this one
-        df_daily.at[open_date, 'action'] = 'open'
-        unrealized_pnl = num_of_share * multiplier * (now_close - open_price) - commission
-        unrealized_pnl = round(unrealized_pnl, 3)
-        df_daily.at[open_date, 'unrealized_pnl'] = unrealized_pnl
-        # print(open_date, 'Open!', open_price, now_close, unrealized_pnl)
-
-        ### record unrealised pnl and realized pnl and the same time
-        ### unrealised pnl for the equity value in between
-        for date in dates[1:]:
-            if date == close_date:  # close position on this date
-
-                # clear the open pnl as open and close same day should not aggregate
-                if open_date == close_date:
-                    df_daily.at[date, 'unrealized_pnl'] = None
-
-                # unrealized_pnl
-                if df_daily.at[date, 'unrealized_pnl']:  # if there is already unrealized_pnl, aggregate
-                    df_daily.at[date, 'unrealized_pnl'] = df_daily.at[date, 'unrealized_pnl'] + df_backtest.at[
-                        j, 'realized_pnl']
-                else:
-                    df_daily.at[date, 'unrealized_pnl'] = df_backtest.at[j, 'realized_pnl']
-
-                # realized pnl
-                if df_daily.at[date, 'realized_pnl']:  # if there is already realized_pnl, aggregate
-                    df_daily.at[date, 'realized_pnl'] = df_daily.at[date, 'realized_pnl'] + df_backtest.at[
-                        j, 'realized_pnl']
-                else:
-                    df_daily.at[date, 'realized_pnl'] = df_backtest.at[j, 'realized_pnl']
-
-                df_daily.at[date, 'action'] = df_backtest.at[j, 'action']
-                df_daily.at[date, 'commission'] = df_backtest.at[j, 'commission']
-                last_realized_capital = last_realized_capital + df_backtest.at[j, 'realized_pnl']
-
-                # print(date, 'Close!', open_price, df_backtest.at[j, 'close_price'], df_backtest.at[j, 'realized_pnl'])
-
-            else:
-                try:
-                    now_close = df_daily.at[date, 'close']
-                    unrealized_pnl = num_of_share * multiplier * (now_close - open_price) - commission
-                    unrealized_pnl = round(unrealized_pnl, 3)
-                    if df_daily.at[date, 'unrealized_pnl']:
-                        df_daily.at[date, 'unrealized_pnl'] = df_daily.at[date, 'unrealized_pnl'] + unrealized_pnl
-                    else:
-                        df_daily.at[date, 'unrealized_pnl'] = unrealized_pnl
-
-                    # print(date, 'Not yet close', open_price, now_close, unrealized_pnl)
-
-                except:
-                    pass
-                    # print(date, 'Not yet close', 'Holiday!')
-
-        # print()
-
-    last_equity_value = initial_capital
-
-    for i in df_daily.index[1:]:
-        if df_daily.at[i, 'realized_pnl']:
-            df_daily.at[i, 'equity_value'] = last_equity_value + df_daily.at[i, 'realized_pnl']
-            last_equity_value = df_daily.at[i, 'equity_value']
-
-        elif df_daily.at[i, 'unrealized_pnl']:
-            df_daily.at[i, 'equity_value'] = last_equity_value + df_daily.at[i, 'unrealized_pnl']
-
-    df_daily['equity_value'] = df_daily['equity_value'].fillna(method='ffill')  # Fill na for equity value only
+        df = pl.read_csv(data_path, try_parse_dates=True)
 
+    df = (df.lazy()
+          .select(['datetime', 'open', 'high', 'low', 'close', 'volume']).sort("datetime")
+          .sort("datetime")
+          .groupby_dynamic("datetime", every="1d").agg([
+        pl.col("open").first(),
+        pl.col("high").max(),
+        pl.col("low").min(),
+        pl.col("close").last(),
+        pl.col("volume").sum(),
+    ])  # ploars automatically filter out non-trading date (null close dates in the df_csv)
+          .filter((pl.col('datetime') >= start_date_datetime) & (pl.col('datetime') <= end_date_datetime))
+          .with_columns(pl.col('datetime').alias('date'))
+          .with_columns([
+        (pl.col('close') * (initial_capital / df.head(1)['close'][0])).alias('bah'),
+        pl.lit(None).alias('equity_value'),
+        pl.lit(None).alias('action'),
+        pl.lit(None).alias('realized_pnl'),
+        pl.lit(None).alias('unrealized_pnl'),
+    ])
+          .collect()
+          )
+
+    df_daily = df.to_pandas()
+    df_daily.index = pd.to_datetime(df_daily['datetime'], format='%Y-%m-%d')
+
+    # Apply apply_pnl on backtes here
+    apply_pnl.last_realized_capital = last_realized_capital
+    apply_pnl.multiplier = multiplier
+    apply_pnl.df_daily = df_daily
+    df_backtest.apply(apply_pnl, axis=1)
+
+    df_daily = apply_pnl.df_daily
+
+    df_daily = df_daily.reset_index(drop=True)
+    df_daily_equity.last_equity_value = initial_capital
+    df_daily['equity_value'] = df_daily.apply(df_daily_equity, axis=1).fillna(method='ffill')
 
     return df_daily
 
 
-
-
 def cal_performance(para_combination):
-
     start_date = para_combination['start_date']
     end_date = para_combination['end_date']
 
     risk_free_rate = para_combination['risk_free_rate']
 
     intraday = para_combination['intraday']
     summary_mode = para_combination['summary_mode']
@@ -492,39 +487,30 @@
             df_backtest = pd.read_parquet(save_path)  # Daraframe that may not be daily
         else:
             df_backtest = pd.read_csv(save_path, index_col=0)  # Daraframe that may not be daily
 
         df_backtest['date'] = pd.to_datetime(df_backtest['date'], format='%Y-%m-%d')
         df_backtest = df_backtest.loc[(df_backtest['date'] >= start_date) & (df_backtest['date'] <= end_date)]
         df_backtest = df_backtest.reset_index(drop=True)  # Reset Index
-        df_daily = df_backtest.copy()
-
-    df = df_daily.copy()
-
-
-
-    # end_time = time.time()
-    # elapsed_time = end_time - start_time
-    # print("Resample: {:.2f} seconds".format(elapsed_time))
-
+        df_daily = df_backtest
 
+    df = df_daily
 
     # Deter if equity_value unchange = no tade
     equity_value_column = df['equity_value'].to_numpy()
     no_trade = (equity_value_column[0] == equity_value_column).all()
 
     result_dict = {}
 
     # Determine years at the beginning
     start_date_year = datetime.datetime.strptime(start_date, '%Y-%m-%d').year
     end_date_year = datetime.datetime.strptime(end_date, '%Y-%m-%d').year
     year_list = list(range(start_date_year, end_date_year + 1))
     for y in year_list: result_dict[str(y)] = []
 
-
     # if length of backtest is zero, no trade, no performance
     if no_trade:
         return_on_capital = 0
         result_dict['holding_period_day'] = 0
         result_dict['total_commission'] = 0
         result_dict['net_profit'] = 0
         result_dict['return_on_capital'] = 0
@@ -535,27 +521,27 @@
         result_dict['mdd_pct'] = 0
         result_dict['num_of_trade'] = 0
         result_dict['win_rate'] = 0
         result_dict['loss_rate'] = 0
         result_dict['net_profit_to_mdd'] = np.inf
         result_dict['cov'] = 0
 
-
         # Win rate by year
         for year in year_list:
             result_dict[str(year)] = 0
             result_dict[f'{year}_win_rate'] = '--'
             result_dict[f'{year}_return'] = 0
 
     else:
         df['date'] = pd.to_datetime(df['date'], format='%Y-%m-%d')
         df['year'] = pd.DatetimeIndex(df['date']).year
 
         # Strategy Performance
-        net_profit, holding_period_day, return_on_capital, annualized_return, annualized_std, annualized_sr = calculate_sharp_ratio(df, 'equity_value', risk_free_rate)
+        net_profit, holding_period_day, return_on_capital, annualized_return, annualized_std, annualized_sr = calculate_sharp_ratio(
+            df, 'equity_value', risk_free_rate)
         mdd_pct, mdd_dollar = calculate_mdd(df, 'equity_value')
         mdd_pct = mdd_pct * -100
         mdd_dollar = mdd_dollar * -1
 
         # Win Rate (need to use df_backtest directly)
 
         save_path = generate_filepath(para_combination=para_combination)
@@ -585,15 +571,14 @@
         result_dict['loss_rate'] = loss_rate
 
         if mdd_dollar == 0:
             result_dict['net_profit_to_mdd'] = np.inf
         else:
             result_dict['net_profit_to_mdd'] = net_profit / mdd_dollar
 
-
         # Cov
         df3 = df[df['action'] == 'open']
         df3 = df3.set_index('date')
         signal_year_count = df3.groupby(lambda x: x.year).size()
 
         signal_year_std = np.std(signal_year_count)
         signal_year_mean = np.mean(signal_year_count)
@@ -608,42 +593,33 @@
                 result_dict[f'{year}_win_rate'] = win_rate_dict[year][3]
 
             except Exception as e:
                 # print(e)
                 result_dict[str(year)] = 0
                 result_dict[f'{year}_win_rate'] = '--'
 
-
         # Performance by year
         first_equity_value = 0
         last_equity_value = 0
         for year in year_list:
-            if not df.loc[df['year'] == year].empty: # if trade
-                if first_equity_value == 0: # if 1st year, set beginning as the first equity_value
+            if not df.loc[df['year'] == year].empty:  # if trade
+                if first_equity_value == 0:  # if 1st year, set beginning as the first equity_value
                     first_equity_value = df.loc[df['year'] == year].iloc[0].equity_value
                 last_equity_value = df.loc[df['year'] == year].iloc[-1].equity_value
                 yearly_return = (last_equity_value - first_equity_value) / first_equity_value
                 if np.isnan(yearly_return):
                     result_dict[f'{year}_return'] = 0
                 else:
-                    result_dict[f'{year}_return'] = int(yearly_return*100)
+                    result_dict[f'{year}_return'] = int(yearly_return * 100)
 
-            else: # no trade
+            else:  # no trade
                 result_dict[f'{year}_return'] = '-----'
 
             first_equity_value = last_equity_value
 
-
-
-    # end_time = time.time()
-    # elapsed_time = end_time - start_time
-    # print("No Trade: {:.2f} seconds".format(elapsed_time))
-
-
-
     result_dict['risk_free_rate'] = risk_free_rate
 
     # BaH Performance
     bah_net_return, holding_period_day, bah_return, \
     bah_annualized_return, bah_annualized_std, bah_annualized_sr = calculate_sharp_ratio(df, 'close',
                                                                                          risk_free_rate)
     initial_capital = df.loc[df.index[0], 'equity_value']
@@ -656,10 +632,9 @@
     result_dict['bah_annualized_return'] = bah_annualized_return
     result_dict['bah_annualized_std'] = bah_annualized_std
     result_dict['bah_annualized_sr'] = bah_annualized_sr
     result_dict['bah_mdd_dollar'] = bah_mdd_dollar
     result_dict['bah_mdd_pct'] = bah_mdd_pct
     result_dict['return_to_bah'] = return_on_capital - bah_return
 
-
     return result_dict
```

### Comparing `plotguy-1.0.6/plotguy/aggregate.py` & `plotguy-1.0.7/plotguy/aggregate.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.6/plotguy/components.py` & `plotguy-1.0.7/plotguy/components.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.6/plotguy/equity_curves.py` & `plotguy-1.0.7/plotguy/equity_curves.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.6/plotguy/signals.py` & `plotguy-1.0.7/plotguy/signals.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.6/setup.py` & `plotguy-1.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plotguy",
-    version="1.0.6",
+    version="1.0.7",
     author="Plotguy Team",
     author_email="plotguy.info@gmail.com",
     description="Plotguy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[         
         'pandas>=1.5.2',  
         'numpy>=1.24.1',  
         'hkfdb>=2.2', 
         'pyarrow',
+        'polars',
         'lxml',        
         'dash',
         'dash_bootstrap_components',
         'dash_daq',
         'dash_dangerously_set_inner_html',
     ],
     url="https://pypi.org/project/plotguy/",
```

