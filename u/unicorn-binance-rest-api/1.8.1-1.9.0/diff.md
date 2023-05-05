# Comparing `tmp/unicorn-binance-rest-api-1.8.1.tar.gz` & `tmp/unicorn-binance-rest-api-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicorn-binance-rest-api-1.8.1.tar", last modified: Mon Apr  3 23:57:34 2023, max compression
+gzip compressed data, was "unicorn-binance-rest-api-1.9.0.tar", last modified: Wed Apr 12 20:56:41 2023, max compression
```

## Comparing `unicorn-binance-rest-api-1.8.1.tar` & `unicorn-binance-rest-api-1.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-03 23:57:34.386325 unicorn-binance-rest-api-1.8.1/
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     1286 2023-04-03 22:35:50.000000 unicorn-binance-rest-api-1.8.1/LICENSE
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    21067 2023-04-03 23:57:34.370602 unicorn-binance-rest-api-1.8.1/PKG-INFO
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    19273 2023-04-03 23:09:32.000000 unicorn-binance-rest-api-1.8.1/README.md
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)       38 2023-04-03 23:57:34.386325 unicorn-binance-rest-api-1.8.1/setup.cfg
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     4544 2023-04-03 22:35:51.000000 unicorn-binance-rest-api-1.8.1/setup.py
-drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-03 23:57:33.930591 unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api/
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)       68 2023-04-03 22:35:51.000000 unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api/__init__.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     3459 2023-04-03 22:35:51.000000 unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api/enums.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     4484 2023-04-03 22:35:51.000000 unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api/exceptions.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)     3325 2023-04-03 22:35:51.000000 unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api/helpers.py
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)   244640 2023-04-03 23:56:59.000000 unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api/manager.py
-drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-03 23:57:34.316976 unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api.egg-info/
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)    21067 2023-04-03 23:57:31.000000 unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api.egg-info/PKG-INFO
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)      447 2023-04-03 23:57:31.000000 unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)        1 2023-04-03 23:57:31.000000 unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)      113 2023-04-03 23:57:31.000000 unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api.egg-info/requires.txt
--rwxrwxrwx   0 oliver    (1000) oliver    (1000)       25 2023-04-03 23:57:31.000000 unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api.egg-info/top_level.txt
+drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-12 20:56:41.295342 unicorn-binance-rest-api-1.9.0/
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     1286 2023-04-03 22:35:50.000000 unicorn-binance-rest-api-1.9.0/LICENSE
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    21914 2023-04-12 20:56:41.291334 unicorn-binance-rest-api-1.9.0/PKG-INFO
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    20132 2023-04-12 12:35:46.000000 unicorn-binance-rest-api-1.9.0/README.md
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)       38 2023-04-12 20:56:41.296345 unicorn-binance-rest-api-1.9.0/setup.cfg
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     4544 2023-04-03 22:35:51.000000 unicorn-binance-rest-api-1.9.0/setup.py
+drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-12 20:56:41.109497 unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api/
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)       68 2023-04-03 22:35:51.000000 unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api/__init__.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     3459 2023-04-03 22:35:51.000000 unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api/enums.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     4484 2023-04-03 22:35:51.000000 unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api/exceptions.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)     3325 2023-04-03 22:35:51.000000 unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api/helpers.py
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)   249938 2023-04-12 20:55:55.000000 unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api/manager.py
+drwxrwxrwx   0 oliver    (1000) oliver    (1000)        0 2023-04-12 20:56:41.260419 unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api.egg-info/
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)    21914 2023-04-12 20:56:39.000000 unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)      447 2023-04-12 20:56:40.000000 unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)        1 2023-04-12 20:56:40.000000 unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)      113 2023-04-12 20:56:40.000000 unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api.egg-info/requires.txt
+-rwxrwxrwx   0 oliver    (1000) oliver    (1000)       25 2023-04-12 20:56:40.000000 unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api.egg-info/top_level.txt
```

### Comparing `unicorn-binance-rest-api-1.8.1/LICENSE` & `unicorn-binance-rest-api-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unicorn-binance-rest-api-1.8.1/PKG-INFO` & `unicorn-binance-rest-api-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicorn-binance-rest-api
-Version: 1.8.1
+Version: 1.9.0
 Summary: An unofficial Python API to use the Binance REST API`s (com+testnet, com-margin+testnet, com-isolated_margin+testnet, com-futures+testnet, us, tr) in a easy, fast, flexible, robust and fully-featured way. 
 Home-page: https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api
 Author: LUCIT Systems and Development
 Author-email: info@lucit.tech
 License: MIT License
 Project-URL: Howto, https://www.lucit.tech/unicorn-binance-rest-api.html#howto
 Project-URL: Documentation, https://unicorn-binance-rest-api.docs.lucit.tech/
@@ -104,23 +104,21 @@
 [Binance Margin](https://binance-docs.github.io/apidocs/spot/en/#user-data-streams) 
 ([+Testnet](https://testnet.binance.vision/)), 
 [Binance Isolated Margin](https://binance-docs.github.io/apidocs/spot/en/#listen-key-isolated-margin)
 ([+Testnet](https://testnet.binance.vision/)), 
 [Binance Futures](https://binance-docs.github.io/apidocs/futures/en/#websocket-market-streams) 
 ([+Testnet](https://testnet.binancefuture.com)), 
 [Binance COIN-M Futures](https://binance-docs.github.io/apidocs/delivery/en/#change-log),
-[Binance US](https://github.com/binance-us/binance-official-api-docs), 
-[Binance TR](https://www.trbinance.com/apidocs) and 
-[Binance JEX](https://jexapi.github.io/api-doc/spot.html#web-socket-streams) and needs to be used with a valid api_key and api_secret from the Binance Exchange 
+[Binance US](https://github.com/binance-us/binance-official-api-docs) and
+[Binance TR](https://www.trbinance.com/apidocs) and needs to be used with a valid api_key and api_secret from the Binance Exchange 
 [www.binance.com](https://www.binance.com/userCenter/createApi.html), 
-[testnet.binance.vision](https://testnet.binance.vision/), 
-[www.binance.us](https://www.binance.us/userCenter/createApi.html) or 
-[www.jex.com](https://www.jex.com/userCenter/createApi.html).
+[testnet.binance.vision](https://testnet.binance.vision/) or
+[www.binance.us](https://www.binance.us/userCenter/createApi.html).
 
-Be aware that the Binance REST API is request based. if you want to receive high frequency and high volume data, you can use the [UNICORN Binance Websocket API](https://www.lucit.tech/unicorn-binance-websocket-api.html) in combination. 
+Be aware that the Binance REST API is request based. if you want to send and receive high frequency and high volume data, you can use the [UNICORN Binance Websocket API](https://www.lucit.tech/unicorn-binance-websocket-api.html) in combination. 
 
 ### What are the benefits of the UNICORN Binance REST API?
 - Supported exchanges: 
 
 | Exchange                                                           | Exchange string                       | 
 |--------------------------------------------------------------------|---------------------------------------| 
 | [Binance](https://www.binance.com)                                 | `binance.com`                         |
@@ -134,14 +132,19 @@
 | [Binance Coin-M Futures](https://www.binance.com)                  | `binance.com-coin_futures`            |
 | [Binance US](https://www.binance.us)                               | `binance.us`                          |
 | [Binance TR](https://www.trbinance.com)                            | `trbinance.com`                       |
 
 - Helpful management features like 
 [`get_used_weight()`](https://unicorn-binance-rest-api.docs.lucit.tech/unicorn_binance_rest_api.html#unicorn_binance_rest_api.manager.BinanceRestApiManager.get_used_weight), 
 
+
+- Integration of [test cases](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/actions/workflows/unit-tests.yml) and [examples](#examples).
+
+- Customizable base URL and request timeout.
+
 - *Socks5 Proxy* support:
   ```
   ubra = BinanceRestApiManager(exchange="binance.com", socks5_proxy_server="127.0.0.1:9050") 
   ```
   Read the [docs](https://unicorn-binance-rest-api.docs.lucit.tech/unicorn_binance_rest_api.html#unicorn_binance_rest_api.manager.BinanceRestApiManager)
   or this [how to](https://medium.com/@oliverzehentleitner/how-to-connect-to-binance-com-rest-api-using-python-via-a-socks5-proxy-638dbbecacfd) 
   for more information or try 
@@ -205,14 +208,15 @@
 - [example_historical_data.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/blob/master/example_historical_data.py)
 - [example_logging.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/blob/master/example_logging.py)
 - [example_orders.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/blob/master/example_orders.py)
 - [example_socks5_proxy.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_socks5_proxy.py)
 - [example_version_of_this_package.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/blob/master/example_version_of_this_package.py)
 
 ## Howto
+- [Restful Binance Requests in Python with UNICORN Binance REST API](https://medium.lucit.tech/restful-binance-requests-in-python-with-unicorn-binance-rest-api-288f364e92a8)
 - [How to Download Klines from Binance using Python?](https://medium.lucit.tech/how-to-download-data-from-binance-using-python-8f1b6e8f19f3)
 - [How to Connect to binance.com REST API using Python via a SOCKS5 Proxy](https://medium.lucit.tech/how-to-connect-to-binance-com-rest-api-using-python-via-a-socks5-proxy-638dbbecacfd)
 
 ## Project Homepage
 [https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api)
 
 ## Wiki
@@ -234,15 +238,14 @@
 
 Follow us on [Twitter](https://twitter.com/LUCIT_SysDev) or on [Facebook](https://www.facebook.com/lucit.systems.and.development) for general news about the [unicorn-binance-suite](https://www.lucit.tech/unicorn-binance-suite.html)!
 
 To receive news (like inspection windows/maintenance) about the Binance API`s subscribe to their telegram groups: 
 
 - [https://t.me/binance_api_announcements](https://t.me/binance_api_announcements)
 - [https://t.me/binance_api_english](https://t.me/binance_api_english)
-- [https://t.me/Binance_JEX_EN](https://t.me/Binance_JEX_EN)
 - [https://t.me/Binance_USA](https://t.me/Binance_USA)
 - [https://t.me/TRBinanceTR](https://t.me/TRBinanceTR)
 - [https://t.me/BinanceDEXchange](https://t.me/BinanceDEXchange)
 - [https://t.me/BinanceExchange](https://t.me/BinanceExchange)
 
 ## How to report Bugs or suggest Improvements?
 [List of planned features](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement) - 
@@ -272,17 +275,26 @@
 ## Disclaimer
 This project is for informational purposes only. You should not construe this information or any other material as 
 legal, tax, investment, financial or other advice. Nothing contained herein constitutes a solicitation, recommendation, 
 endorsement or offer by us or any third party provider to buy or sell any securities or other financial instruments in 
 this or any other jurisdiction in which such solicitation or offer would be unlawful under the securities laws of such 
 jurisdiction.
 
-***If you intend to use real money, use it at your own risk.***
+### If you intend to use real money, use it at your own risk!
 
 Under no circumstances will we be responsible or liable for any claims, damages, losses, expenses, costs or liabilities 
 of any kind, including but not limited to direct or indirect damages for loss of profits.
 
+### SOCKS5 Proxy / Geoblocking
+We would like to explicitly point out that in our opinion US citizens are exclusively authorized to trade on Binance.US 
+and that this restriction must not be circumvented!
+
+The purpose of supporting a SOCKS5 proxy in the UNICORN Binance Suite and its modules is to allow non-US citizens to use 
+US services. For example, Github actions with UBS will not work without a SOCKS5 proxy, as they will inevitably run on 
+servers in the US and be blocked by Binance.com. Moreover, it also seems justified that traders, data scientists and 
+companies from the US analyze binance.com market data - as long as they do not trade there.
+
 ## Commercial Support
 
 [![Get professional and fast support](https://raw.githubusercontent.com/LUCIT-Systems-and-Development/unicorn-binance-suite/master/images/support/LUCIT-get-professional-and-fast-support.png)](https://www.lucit.tech/get-support.html)
 
 ***Do you need a developer, operator or consultant?*** [Contact us](https://www.lucit.tech/contact.html) for a non-binding initial consultation!
```

### Comparing `unicorn-binance-rest-api-1.8.1/README.md` & `unicorn-binance-rest-api-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,23 +68,21 @@
 [Binance Margin](https://binance-docs.github.io/apidocs/spot/en/#user-data-streams) 
 ([+Testnet](https://testnet.binance.vision/)), 
 [Binance Isolated Margin](https://binance-docs.github.io/apidocs/spot/en/#listen-key-isolated-margin)
 ([+Testnet](https://testnet.binance.vision/)), 
 [Binance Futures](https://binance-docs.github.io/apidocs/futures/en/#websocket-market-streams) 
 ([+Testnet](https://testnet.binancefuture.com)), 
 [Binance COIN-M Futures](https://binance-docs.github.io/apidocs/delivery/en/#change-log),
-[Binance US](https://github.com/binance-us/binance-official-api-docs), 
-[Binance TR](https://www.trbinance.com/apidocs) and 
-[Binance JEX](https://jexapi.github.io/api-doc/spot.html#web-socket-streams) and needs to be used with a valid api_key and api_secret from the Binance Exchange 
+[Binance US](https://github.com/binance-us/binance-official-api-docs) and
+[Binance TR](https://www.trbinance.com/apidocs) and needs to be used with a valid api_key and api_secret from the Binance Exchange 
 [www.binance.com](https://www.binance.com/userCenter/createApi.html), 
-[testnet.binance.vision](https://testnet.binance.vision/), 
-[www.binance.us](https://www.binance.us/userCenter/createApi.html) or 
-[www.jex.com](https://www.jex.com/userCenter/createApi.html).
+[testnet.binance.vision](https://testnet.binance.vision/) or
+[www.binance.us](https://www.binance.us/userCenter/createApi.html).
 
-Be aware that the Binance REST API is request based. if you want to receive high frequency and high volume data, you can use the [UNICORN Binance Websocket API](https://www.lucit.tech/unicorn-binance-websocket-api.html) in combination. 
+Be aware that the Binance REST API is request based. if you want to send and receive high frequency and high volume data, you can use the [UNICORN Binance Websocket API](https://www.lucit.tech/unicorn-binance-websocket-api.html) in combination. 
 
 ### What are the benefits of the UNICORN Binance REST API?
 - Supported exchanges: 
 
 | Exchange                                                           | Exchange string                       | 
 |--------------------------------------------------------------------|---------------------------------------| 
 | [Binance](https://www.binance.com)                                 | `binance.com`                         |
@@ -98,14 +96,19 @@
 | [Binance Coin-M Futures](https://www.binance.com)                  | `binance.com-coin_futures`            |
 | [Binance US](https://www.binance.us)                               | `binance.us`                          |
 | [Binance TR](https://www.trbinance.com)                            | `trbinance.com`                       |
 
 - Helpful management features like 
 [`get_used_weight()`](https://unicorn-binance-rest-api.docs.lucit.tech/unicorn_binance_rest_api.html#unicorn_binance_rest_api.manager.BinanceRestApiManager.get_used_weight), 
 
+
+- Integration of [test cases](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/actions/workflows/unit-tests.yml) and [examples](#examples).
+
+- Customizable base URL and request timeout.
+
 - *Socks5 Proxy* support:
   ```
   ubra = BinanceRestApiManager(exchange="binance.com", socks5_proxy_server="127.0.0.1:9050") 
   ```
   Read the [docs](https://unicorn-binance-rest-api.docs.lucit.tech/unicorn_binance_rest_api.html#unicorn_binance_rest_api.manager.BinanceRestApiManager)
   or this [how to](https://medium.com/@oliverzehentleitner/how-to-connect-to-binance-com-rest-api-using-python-via-a-socks5-proxy-638dbbecacfd) 
   for more information or try 
@@ -169,14 +172,15 @@
 - [example_historical_data.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/blob/master/example_historical_data.py)
 - [example_logging.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/blob/master/example_logging.py)
 - [example_orders.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/blob/master/example_orders.py)
 - [example_socks5_proxy.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_socks5_proxy.py)
 - [example_version_of_this_package.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/blob/master/example_version_of_this_package.py)
 
 ## Howto
+- [Restful Binance Requests in Python with UNICORN Binance REST API](https://medium.lucit.tech/restful-binance-requests-in-python-with-unicorn-binance-rest-api-288f364e92a8)
 - [How to Download Klines from Binance using Python?](https://medium.lucit.tech/how-to-download-data-from-binance-using-python-8f1b6e8f19f3)
 - [How to Connect to binance.com REST API using Python via a SOCKS5 Proxy](https://medium.lucit.tech/how-to-connect-to-binance-com-rest-api-using-python-via-a-socks5-proxy-638dbbecacfd)
 
 ## Project Homepage
 [https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api)
 
 ## Wiki
@@ -198,15 +202,14 @@
 
 Follow us on [Twitter](https://twitter.com/LUCIT_SysDev) or on [Facebook](https://www.facebook.com/lucit.systems.and.development) for general news about the [unicorn-binance-suite](https://www.lucit.tech/unicorn-binance-suite.html)!
 
 To receive news (like inspection windows/maintenance) about the Binance API`s subscribe to their telegram groups: 
 
 - [https://t.me/binance_api_announcements](https://t.me/binance_api_announcements)
 - [https://t.me/binance_api_english](https://t.me/binance_api_english)
-- [https://t.me/Binance_JEX_EN](https://t.me/Binance_JEX_EN)
 - [https://t.me/Binance_USA](https://t.me/Binance_USA)
 - [https://t.me/TRBinanceTR](https://t.me/TRBinanceTR)
 - [https://t.me/BinanceDEXchange](https://t.me/BinanceDEXchange)
 - [https://t.me/BinanceExchange](https://t.me/BinanceExchange)
 
 ## How to report Bugs or suggest Improvements?
 [List of planned features](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement) - 
@@ -236,17 +239,26 @@
 ## Disclaimer
 This project is for informational purposes only. You should not construe this information or any other material as 
 legal, tax, investment, financial or other advice. Nothing contained herein constitutes a solicitation, recommendation, 
 endorsement or offer by us or any third party provider to buy or sell any securities or other financial instruments in 
 this or any other jurisdiction in which such solicitation or offer would be unlawful under the securities laws of such 
 jurisdiction.
 
-***If you intend to use real money, use it at your own risk.***
+### If you intend to use real money, use it at your own risk!
 
 Under no circumstances will we be responsible or liable for any claims, damages, losses, expenses, costs or liabilities 
 of any kind, including but not limited to direct or indirect damages for loss of profits.
 
+### SOCKS5 Proxy / Geoblocking
+We would like to explicitly point out that in our opinion US citizens are exclusively authorized to trade on Binance.US 
+and that this restriction must not be circumvented!
+
+The purpose of supporting a SOCKS5 proxy in the UNICORN Binance Suite and its modules is to allow non-US citizens to use 
+US services. For example, Github actions with UBS will not work without a SOCKS5 proxy, as they will inevitably run on 
+servers in the US and be blocked by Binance.com. Moreover, it also seems justified that traders, data scientists and 
+companies from the US analyze binance.com market data - as long as they do not trade there.
+
 ## Commercial Support
 
 [![Get professional and fast support](https://raw.githubusercontent.com/LUCIT-Systems-and-Development/unicorn-binance-suite/master/images/support/LUCIT-get-professional-and-fast-support.png)](https://www.lucit.tech/get-support.html)
 
 ***Do you need a developer, operator or consultant?*** [Contact us](https://www.lucit.tech/contact.html) for a non-binding initial consultation!
```

### Comparing `unicorn-binance-rest-api-1.8.1/setup.py` & `unicorn-binance-rest-api-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api/enums.py` & `unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api/enums.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api/exceptions.py` & `unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api/helpers.py` & `unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api/helpers.py`

 * *Files identical despite different names*

### Comparing `unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api/manager.py` & `unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,27 +50,25 @@
 
 logger = logging.getLogger("unicorn_binance_rest_api")
 
 
 class BinanceRestApiManager(object):
     """
     An unofficial Python API to use the Binance REST API`s (com+testnet, com-margin+testnet,
-    com-isolated_margin+testnet, com-futures+testnet, us, jex) in a easy, fast, flexible,
+    com-isolated_margin+testnet, com-futures+testnet, us) in a easy, fast, flexible,
     robust and fully-featured way.
 
     Binance.com rest API documentation:
         -
     Binance.vision (Testnet) rest API documentation:
         -
     Binance.us rest API documentation:
         -
     TRBinance.com rest API documentation:
         - https://www.trbinance.com/apidocs/#api-document-description
-    Jex.com websocket API documentation:
-        - https://github.com/JexApi/jex-official-api-docs
 
     Binance API Client constructor
 
     :param api_key: Api Key
     :type api_key: str.
     :param api_secret: Api Secret
     :type api_secret: str.
@@ -78,16 +76,16 @@
     :type requests_params: dict.
     :param tld: Top Level Domain of the Binance endpoint, Default is False
     :type tld: str.
     :param warn_on_update: set to `False` to disable the update warning
     :type warn_on_update: bool
     :param exchange: Select binance.com, binance.com-testnet, binance.com-margin, binance.com-margin-testnet,
              binance.com-isolated_margin, binance.com-isolated_margin-testnet, binance.com-futures,
-             binance.com-futures-testnet, binance.com-coin-futures, binance.us, trbinance.com
-             or jex.com (default: binance.com) This overules parameter `tld`.
+             binance.com-futures-testnet, binance.com-coin-futures, binance.us or trbinance.com (default: binance.com)
+             This overrules parameter `tld`.
     :type exchange: str
     :param debug: If True the lib adds additional information to logging outputs
     :type debug:  bool
     :param disable_colorama: set to True to disable the use of `colorama <https://pypi.org/project/colorama/>`_
     :type disable_colorama: bool
     :param socks5_proxy_server: Set this to activate the usage of a socks5 proxy. Example: '127.0.0.1:9050'
     :type socks5_proxy_server:  str
@@ -199,15 +197,15 @@
                  socks5_proxy_server: Optional[str] = None,
                  socks5_proxy_user: Optional[str] = None,
                  socks5_proxy_pass: Optional[str] = None,
                  socks5_proxy_ssl_verification: Optional[bool] = True,
                  ):
 
         self.name = "unicorn-binance-rest-api"
-        self.version = "1.8.1"
+        self.version = "1.9.0"
         logger.info(f"New instance of {self.get_user_agent()} on {str(platform.system())} {str(platform.release())} "
                     f"for exchange {exchange} started ...")
         if disable_colorama is not True:
             logger.info(f"Initiating `colorama_{colorama.__version__}`")
             colorama.init()
         self.exchange = exchange
         self.debug = debug
@@ -328,23 +326,14 @@
             self.API_URL = "https://www.trbinance.com/api"
             self.MARGIN_API_URL = " https://api.trbinance.com/sapi"
             self.WEBSITE_URL = "https://www.trbinance.com"
             self.FUTURES_URL = "https://fapi.trbinance.com/fapi"
             self.FUTURES_DATA_URL = "https://fapi.trbinance.com/futures/data"
             self.FUTURES_COIN_URL = "https://fapi.trbinance.com/fapi"
             self.FUTURES_COIN_DATA_URL = "https://dapi.trbinance.com/futures/data"
-        elif self.exchange == "jex.com":
-            # Todo: Doesnt work!
-            self.API_URL = "https://www.jex.com/api"
-            self.MARGIN_API_URL = " https://www.jex.com/sapi"
-            self.WEBSITE_URL = "https://www.jex.com"
-            self.FUTURES_URL = "https://www.jex.com/fapi"
-            self.FUTURES_DATA_URL = "https://www.jex.com/futures/data"
-            self.FUTURES_COIN_URL = "https://www.jex.com/fapi"
-            self.FUTURES_COIN_DATA_URL = "https://www.jex.com/futures/data"
         elif self.exchange:
             # Unknown Exchange
             error_msg = f"Unknown exchange '{str(self.exchange)}'! Read the docs to see a list of supported " \
                         "exchanges: https://unicorn-binance-rest-api.docs.lucit.tech/unicorn_" \
                         "binance_rest_api.html#module-unicorn_binance_rest_api.unicorn_binance_rest_" \
                         "api_manager"
             logger.critical(error_msg)
@@ -6040,14 +6029,97 @@
         Get position mode for authenticated account
 
         https://binance-docs.github.io/apidocs/futures/en/#get-current-position-mode-user_data
         
         """
         return self._request_futures_api('get', 'positionSide/dual', True, data=params)
 
+    def futures_stream_get_listen_key(self, output="value", throw_exception=True):
+        """Start a new futures data stream and return the listen key
+        If a stream already exists it should return the same key.
+        If the stream becomes invalid a new key is returned.
+
+        Can be used to keep the stream alive.
+
+        https://binance-docs.github.io/apidocs/spot/en/#listen-key-margin
+
+        :param output: Set `output` to "raw_data" to receive the request resource, default is "value" which returns
+                        the plain listenKey.
+        :type output: str
+        :param throw_exception: Default `True`, if `False` the raw response will be returned.
+        :type throw_exception: bool
+        :returns: API response
+
+        .. code-block:: python
+
+            {
+                "listenKey": "pqia91ma19a5s61cv6a81va65sdf19v8a65a1a5s61cv6a81va65sdf19v8a65a1"
+            }
+
+        :raises: BinanceRequestException, BinanceAPIException
+
+        """
+        res = self._request_futures_api('post', 'listenKey', signed=False, data={}, throw_exception=throw_exception)
+        if output == "value":
+            return res['listenKey']
+        elif output == "raw_data":
+            return res
+        else:
+            return res['listenKey']
+
+    def futures_stream_keepalive(self, listenKey, throw_exception=True):
+        """PING a futures data stream to prevent a time out.
+
+        https://binance-docs.github.io/apidocs/spot/en/#listen-key-margin
+
+        :param listenKey: required
+        :type listenKey: str
+        :param throw_exception: Default `True`, if `False` the raw response will be returned.
+        :type throw_exception: bool
+
+        :returns: API response
+
+        .. code-block:: python
+
+            {}
+
+        :raises: BinanceRequestException, BinanceAPIException
+
+        """
+        params = {
+            'listenKey': listenKey
+        }
+        return self._request_futures_api('put', 'listenKey', signed=False, data=params,
+                                         throw_exception=throw_exception)
+
+    def futures_stream_close(self, listenKey, throw_exception=True):
+        """Close out a futures data stream.
+
+        https://binance-docs.github.io/apidocs/spot/en/#listen-key-margin
+
+        :param listenKey: required
+        :type listenKey: str
+        :param throw_exception: Default `True`, if `False` the raw response will be returned.
+        :type throw_exception: bool
+
+        :returns: API response
+
+        .. code-block:: python
+
+            {}
+
+        :raises: BinanceRequestException, BinanceAPIException
+
+        """
+        params = {
+            'listenKey': listenKey
+        }
+        return self._request_futures_api('delete', 'listenKey', signed=False, data=params,
+                                         throw_exception=throw_exception)
+
     # COIN Futures API
     def futures_coin_ping(self):
         """
         Test connectivity to the Rest API
 
         https://binance-docs.github.io/apidocs/delivery/en/#test-connectivity
 
@@ -6429,14 +6501,99 @@
         Get user's position mode (Hedge Mode or One-way Mode ) on EVERY symbol
 
         https://binance-docs.github.io/apidocs/delivery/en/#get-current-position-mode-user_data
 
         """
         return self._request_futures_coin_api("get", "positionSide/dual", True, data=params)
 
+    def futures_coin_stream_get_listen_key(self, output="value", throw_exception=True):
+        """Start a new coin futures data stream and return the listen key
+        If a stream already exists it should return the same key.
+        If the stream becomes invalid a new key is returned.
+
+        Can be used to keep the stream alive.
+
+        https://binance-docs.github.io/apidocs/spot/en/#listen-key-margin
+
+        :param output: Set `output` to "raw_data" to receive the request resource, default is "value" which returns
+                        the plain listenKey.
+        :type output: str
+        :param throw_exception: Default `True`, if `False` the raw response will be returned.
+        :type throw_exception: bool
+        :returns: API response
+
+        .. code-block:: python
+
+            {
+                "listenKey": "pqia91ma19a5s61cv6a81va65sdf19v8a65a1a5s61cv6a81va65sdf19v8a65a1"
+            }
+
+        :raises: BinanceRequestException, BinanceAPIException
+
+        """
+        res = self._request_futures_coin_api('post', 'listenKey', signed=False, data={},
+                                             throw_exception=throw_exception)
+        if output == "value":
+            return res['listenKey']
+        elif output == "raw_data":
+            return res
+        else:
+            return res['listenKey']
+
+    def futures_coin_stream_keepalive(self, listenKey, throw_exception=True):
+        """PING a coin futures data stream to prevent a time out.
+
+        https://binance-docs.github.io/apidocs/spot/en/#listen-key-margin
+
+        :param listenKey: required
+        :type listenKey: str
+        :param throw_exception: Default `True`, if `False` the raw response will be returned.
+        :type throw_exception: bool
+
+        :returns: API response
+
+        .. code-block:: python
+
+            {}
+
+        :raises: BinanceRequestException, BinanceAPIException
+
+        """
+        params = {
+            'listenKey': listenKey
+        }
+        return self._request_futures_coin_api('put', 'listenKey', signed=False, data=params,
+                                              throw_exception=throw_exception)
+
+    def futures_coin_stream_close(self, listenKey, throw_exception=True):
+        """Close out a coin futures data stream.
+
+        https://binance-docs.github.io/apidocs/spot/en/#listen-key-margin
+
+        :param listenKey: required
+        :type listenKey: str
+        :param throw_exception: Default `True`, if `False` the raw response will be returned.
+        :type throw_exception: bool
+
+        :returns: API response
+
+        .. code-block:: python
+
+            {}
+
+        :raises: BinanceRequestException, BinanceAPIException
+
+        """
+        params = {
+            'listenKey': listenKey
+        }
+        return self._request_futures_coin_api('delete', 'listenKey', signed=False, data=params,
+                                              throw_exception=throw_exception)
+
+
     def get_all_coins_info(self, **params):
         """
         Get information of coins (available for deposit and withdraw) for user.
 
         https://binance-docs.github.io/apidocs/spot/en/#all-coins-39-information-user_data
 
         :param recvWindow: optional
```

### Comparing `unicorn-binance-rest-api-1.8.1/unicorn_binance_rest_api.egg-info/PKG-INFO` & `unicorn-binance-rest-api-1.9.0/unicorn_binance_rest_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicorn-binance-rest-api
-Version: 1.8.1
+Version: 1.9.0
 Summary: An unofficial Python API to use the Binance REST API`s (com+testnet, com-margin+testnet, com-isolated_margin+testnet, com-futures+testnet, us, tr) in a easy, fast, flexible, robust and fully-featured way. 
 Home-page: https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api
 Author: LUCIT Systems and Development
 Author-email: info@lucit.tech
 License: MIT License
 Project-URL: Howto, https://www.lucit.tech/unicorn-binance-rest-api.html#howto
 Project-URL: Documentation, https://unicorn-binance-rest-api.docs.lucit.tech/
@@ -104,23 +104,21 @@
 [Binance Margin](https://binance-docs.github.io/apidocs/spot/en/#user-data-streams) 
 ([+Testnet](https://testnet.binance.vision/)), 
 [Binance Isolated Margin](https://binance-docs.github.io/apidocs/spot/en/#listen-key-isolated-margin)
 ([+Testnet](https://testnet.binance.vision/)), 
 [Binance Futures](https://binance-docs.github.io/apidocs/futures/en/#websocket-market-streams) 
 ([+Testnet](https://testnet.binancefuture.com)), 
 [Binance COIN-M Futures](https://binance-docs.github.io/apidocs/delivery/en/#change-log),
-[Binance US](https://github.com/binance-us/binance-official-api-docs), 
-[Binance TR](https://www.trbinance.com/apidocs) and 
-[Binance JEX](https://jexapi.github.io/api-doc/spot.html#web-socket-streams) and needs to be used with a valid api_key and api_secret from the Binance Exchange 
+[Binance US](https://github.com/binance-us/binance-official-api-docs) and
+[Binance TR](https://www.trbinance.com/apidocs) and needs to be used with a valid api_key and api_secret from the Binance Exchange 
 [www.binance.com](https://www.binance.com/userCenter/createApi.html), 
-[testnet.binance.vision](https://testnet.binance.vision/), 
-[www.binance.us](https://www.binance.us/userCenter/createApi.html) or 
-[www.jex.com](https://www.jex.com/userCenter/createApi.html).
+[testnet.binance.vision](https://testnet.binance.vision/) or
+[www.binance.us](https://www.binance.us/userCenter/createApi.html).
 
-Be aware that the Binance REST API is request based. if you want to receive high frequency and high volume data, you can use the [UNICORN Binance Websocket API](https://www.lucit.tech/unicorn-binance-websocket-api.html) in combination. 
+Be aware that the Binance REST API is request based. if you want to send and receive high frequency and high volume data, you can use the [UNICORN Binance Websocket API](https://www.lucit.tech/unicorn-binance-websocket-api.html) in combination. 
 
 ### What are the benefits of the UNICORN Binance REST API?
 - Supported exchanges: 
 
 | Exchange                                                           | Exchange string                       | 
 |--------------------------------------------------------------------|---------------------------------------| 
 | [Binance](https://www.binance.com)                                 | `binance.com`                         |
@@ -134,14 +132,19 @@
 | [Binance Coin-M Futures](https://www.binance.com)                  | `binance.com-coin_futures`            |
 | [Binance US](https://www.binance.us)                               | `binance.us`                          |
 | [Binance TR](https://www.trbinance.com)                            | `trbinance.com`                       |
 
 - Helpful management features like 
 [`get_used_weight()`](https://unicorn-binance-rest-api.docs.lucit.tech/unicorn_binance_rest_api.html#unicorn_binance_rest_api.manager.BinanceRestApiManager.get_used_weight), 
 
+
+- Integration of [test cases](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/actions/workflows/unit-tests.yml) and [examples](#examples).
+
+- Customizable base URL and request timeout.
+
 - *Socks5 Proxy* support:
   ```
   ubra = BinanceRestApiManager(exchange="binance.com", socks5_proxy_server="127.0.0.1:9050") 
   ```
   Read the [docs](https://unicorn-binance-rest-api.docs.lucit.tech/unicorn_binance_rest_api.html#unicorn_binance_rest_api.manager.BinanceRestApiManager)
   or this [how to](https://medium.com/@oliverzehentleitner/how-to-connect-to-binance-com-rest-api-using-python-via-a-socks5-proxy-638dbbecacfd) 
   for more information or try 
@@ -205,14 +208,15 @@
 - [example_historical_data.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/blob/master/example_historical_data.py)
 - [example_logging.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/blob/master/example_logging.py)
 - [example_orders.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/blob/master/example_orders.py)
 - [example_socks5_proxy.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-websocket-api/blob/master/example_socks5_proxy.py)
 - [example_version_of_this_package.py](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/blob/master/example_version_of_this_package.py)
 
 ## Howto
+- [Restful Binance Requests in Python with UNICORN Binance REST API](https://medium.lucit.tech/restful-binance-requests-in-python-with-unicorn-binance-rest-api-288f364e92a8)
 - [How to Download Klines from Binance using Python?](https://medium.lucit.tech/how-to-download-data-from-binance-using-python-8f1b6e8f19f3)
 - [How to Connect to binance.com REST API using Python via a SOCKS5 Proxy](https://medium.lucit.tech/how-to-connect-to-binance-com-rest-api-using-python-via-a-socks5-proxy-638dbbecacfd)
 
 ## Project Homepage
 [https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api)
 
 ## Wiki
@@ -234,15 +238,14 @@
 
 Follow us on [Twitter](https://twitter.com/LUCIT_SysDev) or on [Facebook](https://www.facebook.com/lucit.systems.and.development) for general news about the [unicorn-binance-suite](https://www.lucit.tech/unicorn-binance-suite.html)!
 
 To receive news (like inspection windows/maintenance) about the Binance API`s subscribe to their telegram groups: 
 
 - [https://t.me/binance_api_announcements](https://t.me/binance_api_announcements)
 - [https://t.me/binance_api_english](https://t.me/binance_api_english)
-- [https://t.me/Binance_JEX_EN](https://t.me/Binance_JEX_EN)
 - [https://t.me/Binance_USA](https://t.me/Binance_USA)
 - [https://t.me/TRBinanceTR](https://t.me/TRBinanceTR)
 - [https://t.me/BinanceDEXchange](https://t.me/BinanceDEXchange)
 - [https://t.me/BinanceExchange](https://t.me/BinanceExchange)
 
 ## How to report Bugs or suggest Improvements?
 [List of planned features](https://github.com/LUCIT-Systems-and-Development/unicorn-binance-rest-api/issues?q=is%3Aissue+is%3Aopen+label%3Aenhancement) - 
@@ -272,17 +275,26 @@
 ## Disclaimer
 This project is for informational purposes only. You should not construe this information or any other material as 
 legal, tax, investment, financial or other advice. Nothing contained herein constitutes a solicitation, recommendation, 
 endorsement or offer by us or any third party provider to buy or sell any securities or other financial instruments in 
 this or any other jurisdiction in which such solicitation or offer would be unlawful under the securities laws of such 
 jurisdiction.
 
-***If you intend to use real money, use it at your own risk.***
+### If you intend to use real money, use it at your own risk!
 
 Under no circumstances will we be responsible or liable for any claims, damages, losses, expenses, costs or liabilities 
 of any kind, including but not limited to direct or indirect damages for loss of profits.
 
+### SOCKS5 Proxy / Geoblocking
+We would like to explicitly point out that in our opinion US citizens are exclusively authorized to trade on Binance.US 
+and that this restriction must not be circumvented!
+
+The purpose of supporting a SOCKS5 proxy in the UNICORN Binance Suite and its modules is to allow non-US citizens to use 
+US services. For example, Github actions with UBS will not work without a SOCKS5 proxy, as they will inevitably run on 
+servers in the US and be blocked by Binance.com. Moreover, it also seems justified that traders, data scientists and 
+companies from the US analyze binance.com market data - as long as they do not trade there.
+
 ## Commercial Support
 
 [![Get professional and fast support](https://raw.githubusercontent.com/LUCIT-Systems-and-Development/unicorn-binance-suite/master/images/support/LUCIT-get-professional-and-fast-support.png)](https://www.lucit.tech/get-support.html)
 
 ***Do you need a developer, operator or consultant?*** [Contact us](https://www.lucit.tech/contact.html) for a non-binding initial consultation!
```

