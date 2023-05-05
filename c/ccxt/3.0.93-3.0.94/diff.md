# Comparing `tmp/ccxt-3.0.93.tar.gz` & `tmp/ccxt-3.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ccxt-3.0.93.tar", last modified: Fri May  5 11:54:10 2023, max compression
+gzip compressed data, was "dist/ccxt-3.0.94.tar", last modified: Fri May  5 16:10:46 2023, max compression
```

## Comparing `ccxt-3.0.93.tar` & `ccxt-3.0.94.tar`

### file list

```diff
@@ -1,487 +1,487 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 11:54:10.753984 ccxt-3.0.93/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2023-05-05 11:53:54.000000 ccxt-3.0.93/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-05-05 11:28:26.000000 ccxt-3.0.93/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)   113274 2023-05-05 11:54:10.757984 ccxt-3.0.93/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2023-05-05 11:28:26.000000 ccxt-3.0.93/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 11:54:10.677979 ccxt-3.0.93/ccxt/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15626 2023-05-05 11:53:53.000000 ccxt-3.0.93/ccxt/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 11:54:10.697980 ccxt-3.0.93/ccxt/abstract/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/abstract/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1861 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11071 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2347 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19171 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2443 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitforex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17077 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2659 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8966 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8653 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2919 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3648 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22372 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1987 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitstamp1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9337 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7439 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bkex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      849 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5594 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/btcex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/btctradeua.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1403 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    71684 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9017 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14759 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2182 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/coinfalcon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5354 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2504 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3736 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21126 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7452 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3128 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9386 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27864 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27864 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6840 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10949 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2596 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2266 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2867 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20600 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20893 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19005 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1474 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6930 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/lbank2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3566 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23203 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23203 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2565 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25825 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/okex5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2752 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12172 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6301 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4575 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1849 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10639 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/stex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1953 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/tidex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3463 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18450 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2130 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7934 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7689 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25850 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/xt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-05-05 11:32:32.000000 ccxt-3.0.93/ccxt/abstract/zonda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41329 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33161 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   127668 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 11:54:10.729982 ccxt-3.0.93/ccxt/async_support/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15429 2023-05-05 11:53:53.000000 ccxt-3.0.93/ccxt/async_support/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41553 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33307 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   128282 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 11:54:10.733982 ccxt-3.0.93/ccxt/async_support/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   128268 2023-05-05 11:53:53.000000 ccxt-3.0.93/ccxt/async_support/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/base/throttler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 11:54:10.733982 ccxt-3.0.93/ccxt/async_support/base/ws/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/base/ws/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4999 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/base/ws/aiohttp_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6085 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/base/ws/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/base/ws/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3733 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/base/ws/fast_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1495 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/base/ws/functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      249 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/base/ws/future.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/base/ws/order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6079 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/base/ws/order_book_side.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62726 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   374663 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2165 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35688 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39268 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      462 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46227 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      481 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69752 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   111979 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38049 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28522 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitforex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   204693 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42790 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   131902 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   120028 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    63629 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87760 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88471 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68835 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82612 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17931 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitstamp1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    93903 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77171 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74597 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bkex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16351 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47523 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35438 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22683 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   111410 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/btcex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48897 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22323 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/btctradeua.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35602 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45959 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/buda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   394329 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65248 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   125230 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1233 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74293 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34414 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   191811 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39252 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/coinfalcon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39813 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34679 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81496 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18912 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   108492 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80021 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    84440 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119560 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152866 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    89266 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1252 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   221908 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      459 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69449 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62675 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   117197 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69616 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   357192 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87087 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      586 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    67772 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30046 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42709 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35208 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/itbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101946 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82058 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   160977 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    98228 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37998 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70399 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33953 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    98405 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/lbank2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40781 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48763 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34881 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   210181 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   106630 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62006 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37393 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   178258 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/okex5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   265343 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22933 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   192396 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88811 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75472 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    67101 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47585 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/ripio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   118368 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/stex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42655 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/tidex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65784 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119594 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75965 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103947 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35792 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92578 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95037 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   188966 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/xt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51652 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28959 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   184533 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/zb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74326 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/async_support/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 11:54:10.733982 ccxt-3.0.93/ccxt/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/base/decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3401 2023-05-05 11:40:14.000000 ccxt-3.0.93/ccxt/base/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   169537 2023-05-05 11:53:53.000000 ccxt-3.0.93/ccxt/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/base/precise.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1071 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/base/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1136 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62340 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   373477 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2151 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35482 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39008 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45973 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      467 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69312 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   111509 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37741 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28316 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitforex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   203843 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42572 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   131264 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119564 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    63261 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87308 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88097 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68449 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82190 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17785 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitstamp1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    93397 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76761 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74167 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bkex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16241 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47095 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35160 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22489 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   110784 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/btcex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48547 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22177 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/btctradeua.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35384 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    45591 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/buda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   392459 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    64922 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   124586 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    73787 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34208 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   190913 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38956 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/coinfalcon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39565 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34455 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81092 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18778 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   107966 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79629 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    84060 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119018 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152160 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88724 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   221082 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69001 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62241 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   116511 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69194 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   355886 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    86605 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      572 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    67332 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29810 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42437 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34960 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/itbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101404 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    81756 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   160363 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    97782 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37750 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70007 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33717 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    97857 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/lbank2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40473 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48461 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34639 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   209135 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   106106 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    61638 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37055 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   177794 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      434 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/okex5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   264325 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22745 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   191812 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88311 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75104 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/poloniexfutures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 11:54:10.745983 ccxt-3.0.93/ccxt/pro/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6039 2023-05-05 11:53:53.000000 ccxt-3.0.93/ccxt/pro/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26668 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34553 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77193 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      724 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2016 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      914 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24762 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41903 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    44698 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24486 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    55606 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12557 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16235 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20784 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36705 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26009 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    31132 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/btcex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    60648 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    44892 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1121 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29075 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40578 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22975 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22087 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33925 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24397 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41718 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      391 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25142 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15160 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21786 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    85533 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23052 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      400 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28068 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11059 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    44317 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52058 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34128 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27781 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12175 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41886 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      388 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22655 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30234 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      382 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35657 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    59743 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22635 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12104 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/ripio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9473 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29862 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34279 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25030 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21557 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/pro/zb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    66751 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47325 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/ripio.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 11:54:10.745983 ccxt-3.0.93/ccxt/static_dependencies/
--rw-rw-r--   0 travis    (2000) travis    (2000)       30 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/static_dependencies/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 11:54:10.749984 ccxt-3.0.93/ccxt/static_dependencies/ecdsa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/static_dependencies/ecdsa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/static_dependencies/ecdsa/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/static_dependencies/ecdsa/curves.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/static_dependencies/ecdsa/der.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/static_dependencies/ecdsa/ecdsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/static_dependencies/ecdsa/ellipticcurve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/static_dependencies/ecdsa/keys.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/static_dependencies/ecdsa/numbertheory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/static_dependencies/ecdsa/rfc6979.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/static_dependencies/ecdsa/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 11:54:10.749984 ccxt-3.0.93/ccxt/static_dependencies/keccak/
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/static_dependencies/keccak/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/static_dependencies/keccak/keccak.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   117868 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/stex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 11:54:10.749984 ccxt-3.0.93/ccxt/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/test/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 11:54:10.753984 ccxt-3.0.93/ccxt/test/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1745 2023-05-05 11:40:18.000000 ccxt-3.0.93/ccxt/test/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      922 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_account.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2110 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_balance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1705 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_borrow_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1362 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_borrow_rate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/test/base/test_calculate_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2023-05-05 11:40:17.000000 ccxt-3.0.93/ccxt/test/base/test_crypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2145 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_currency.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5234 2023-05-05 11:40:15.000000 ccxt-3.0.93/ccxt/test/base/test_datetime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/test/base/test_decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/test/base/test_deep_extend.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1957 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_deposit_withdrawal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/test/base/test_exchange_datetime_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1140 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_funding_rate_history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2155 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_ledger_entry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/test/base/test_ledger_item.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_leverage_tier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1551 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_margin_modification.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5671 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_market.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22034 2023-05-05 11:40:15.000000 ccxt-3.0.93/ccxt/test/base/test_number.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2025 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_ohlcv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1327 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_open_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3392 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_order.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2983 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3526 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_position.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10987 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_shared_methods.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1226 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/test/base/test_throttle.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4935 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_ticker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1850 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_trade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2023-05-05 11:41:26.000000 ccxt-3.0.93/ccxt/test/base/test_trading_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/test/base/test_transaction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26500 2023-05-05 11:40:18.000000 ccxt-3.0.93/ccxt/test/test_async.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26096 2023-05-05 11:40:18.000000 ccxt-3.0.93/ccxt/test/test_sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42407 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/tidex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65452 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119250 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75531 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103453 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35544 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92126 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    94453 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   187865 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/xt.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51368 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28777 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   183857 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/zb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74036 2023-05-05 11:28:26.000000 ccxt-3.0.93/ccxt/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 11:54:10.677979 ccxt-3.0.93/ccxt.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)   113274 2023-05-05 11:54:10.000000 ccxt-3.0.93/ccxt.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    11640 2023-05-05 11:54:10.000000 ccxt-3.0.93/ccxt.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 11:54:10.000000 ccxt-3.0.93/ccxt.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-05-05 11:54:10.000000 ccxt-3.0.93/ccxt.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2023-05-05 11:54:10.000000 ccxt-3.0.93/ccxt.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     8459 2023-05-05 11:53:54.000000 ccxt-3.0.93/package.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2023-05-05 11:54:10.757984 ccxt-3.0.93/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2891 2023-05-05 11:28:26.000000 ccxt-3.0.93/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.430756 ccxt-3.0.94/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2023-05-05 16:10:30.000000 ccxt-3.0.94/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-05-05 15:55:39.000000 ccxt-3.0.94/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113274 2023-05-05 16:10:46.434757 ccxt-3.0.94/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2023-05-05 15:55:39.000000 ccxt-3.0.94/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.094733 ccxt-3.0.94/ccxt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15626 2023-05-05 16:10:28.000000 ccxt-3.0.94/ccxt/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.170738 ccxt-3.0.94/ccxt/abstract/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/abstract/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1861 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11071 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2347 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62883 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19171 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2443 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitforex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17077 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2659 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8966 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8653 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2919 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3648 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22372 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1987 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitstamp1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9337 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7439 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bkex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      849 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5594 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/btcex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/btctradeua.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1403 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    71684 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9017 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14759 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2182 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinfalcon.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5354 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2504 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3736 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21126 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7452 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3128 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9386 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27864 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27864 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6840 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10949 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2596 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2266 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2867 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20600 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20893 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19005 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1474 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6930 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/lbank2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3566 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23203 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23203 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2565 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25825 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/okex5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29716 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2752 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12172 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6301 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4575 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1849 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10639 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/stex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1953 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/tidex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3463 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18450 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2130 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7934 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7689 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25850 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/xt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-05-05 15:59:54.000000 ccxt-3.0.94/ccxt/abstract/zonda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41329 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33161 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   127668 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.318749 ccxt-3.0.94/ccxt/async_support/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15429 2023-05-05 16:10:28.000000 ccxt-3.0.94/ccxt/async_support/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41553 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33307 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   128282 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.322749 ccxt-3.0.94/ccxt/async_support/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   128268 2023-05-05 16:10:28.000000 ccxt-3.0.94/ccxt/async_support/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/throttler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.330749 ccxt-3.0.94/ccxt/async_support/base/ws/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4999 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/aiohttp_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6085 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3733 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/fast_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1495 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      249 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/future.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6079 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/base/ws/order_book_side.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62726 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   374663 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2165 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35688 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39268 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      462 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46227 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      481 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69752 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111979 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38049 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28522 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitforex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   204759 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42790 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   131902 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   120028 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63629 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87760 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88471 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68835 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82612 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17931 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitstamp1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    93903 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77171 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74597 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bkex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16351 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47523 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35438 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22683 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111410 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/btcex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48897 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22323 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/btctradeua.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35602 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45959 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/buda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   394329 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65248 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   125230 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1233 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74293 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34414 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   191811 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39252 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinfalcon.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39813 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34679 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81496 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18912 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   108492 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80021 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    84440 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119560 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152866 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89266 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1252 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   221908 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      459 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69449 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62675 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   117197 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69616 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   357192 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87087 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      586 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    67772 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30046 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42709 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35208 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/itbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101946 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82058 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   160977 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    98228 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37998 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70399 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33953 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    98405 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/lbank2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40781 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48763 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34881 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   210181 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   106630 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62006 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37393 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   178258 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/okex5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   265343 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22933 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   192396 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88811 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75472 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68946 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47585 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/ripio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   118368 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/stex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42655 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/tidex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65784 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119594 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75965 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103947 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35792 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92591 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95037 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   188966 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/xt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51652 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28959 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   184533 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/zb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74326 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/async_support/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.334750 ccxt-3.0.94/ccxt/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/base/decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3401 2023-05-05 16:07:38.000000 ccxt-3.0.94/ccxt/base/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   169537 2023-05-05 16:10:28.000000 ccxt-3.0.94/ccxt/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/base/precise.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1071 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/base/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1136 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62340 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   373477 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2151 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35482 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39008 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45973 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      467 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69312 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111509 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37741 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28316 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitforex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   203909 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42572 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   131264 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119564 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63261 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87308 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88097 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68449 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82190 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17785 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitstamp1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    93397 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76761 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74167 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bkex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16241 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47095 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35160 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22489 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   110784 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/btcex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48547 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22177 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/btctradeua.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35384 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    45591 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/buda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   392459 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    64922 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   124586 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    73787 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34208 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   190913 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38956 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinfalcon.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39565 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34455 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81092 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18778 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   107966 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79629 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    84060 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119018 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152160 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88724 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   221082 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69001 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62241 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   116511 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69194 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   355886 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    86605 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      572 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    67332 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29810 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42437 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34960 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/itbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101404 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    81756 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   160363 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    97782 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37750 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70007 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33717 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    97857 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/lbank2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40473 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48461 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34639 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   209135 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   106106 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    61638 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37055 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   177794 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      434 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/okex5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   264325 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22745 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   191812 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88311 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75104 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/poloniexfutures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.390754 ccxt-3.0.94/ccxt/pro/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6039 2023-05-05 16:10:28.000000 ccxt-3.0.94/ccxt/pro/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26668 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34553 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77193 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      724 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2016 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      914 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24762 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41903 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44698 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24486 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    55606 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12557 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16235 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20784 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36705 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26009 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31132 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/btcex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    60648 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44892 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1121 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29075 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40578 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22975 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22087 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33925 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24397 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41718 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      391 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25142 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15160 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21786 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    85533 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23052 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      400 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28068 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11059 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44317 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52058 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34128 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27781 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12175 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41886 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      388 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22655 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30234 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      382 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35657 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    59743 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22635 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12104 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/ripio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9473 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29862 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34279 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25030 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21557 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/pro/zb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68596 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47325 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/ripio.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.390754 ccxt-3.0.94/ccxt/static_dependencies/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       30 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.398754 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/curves.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/der.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/ecdsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/ellipticcurve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/keys.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/numbertheory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/rfc6979.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/ecdsa/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.398754 ccxt-3.0.94/ccxt/static_dependencies/keccak/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/keccak/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/static_dependencies/keccak/keccak.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   117868 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/stex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.402754 ccxt-3.0.94/ccxt/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.426756 ccxt-3.0.94/ccxt/test/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1745 2023-05-05 16:07:42.000000 ccxt-3.0.94/ccxt/test/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      922 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_account.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2110 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_balance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1705 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_borrow_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1362 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_borrow_rate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/base/test_calculate_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2023-05-05 16:07:41.000000 ccxt-3.0.94/ccxt/test/base/test_crypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2145 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_currency.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5234 2023-05-05 16:07:40.000000 ccxt-3.0.94/ccxt/test/base/test_datetime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/base/test_decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/base/test_deep_extend.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1957 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_deposit_withdrawal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/base/test_exchange_datetime_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1140 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_funding_rate_history.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2155 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_ledger_entry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/base/test_ledger_item.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1525 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_leverage_tier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1551 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_margin_modification.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5671 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_market.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22034 2023-05-05 16:07:40.000000 ccxt-3.0.94/ccxt/test/base/test_number.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2025 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_ohlcv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1327 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_open_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3392 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_order.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2983 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3526 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_position.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10987 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_shared_methods.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1226 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/base/test_throttle.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4935 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_ticker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1850 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_trade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2023-05-05 16:08:51.000000 ccxt-3.0.94/ccxt/test/base/test_trading_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/test/base/test_transaction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26500 2023-05-05 16:07:42.000000 ccxt-3.0.94/ccxt/test/test_async.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26096 2023-05-05 16:07:42.000000 ccxt-3.0.94/ccxt/test/test_sync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42407 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/tidex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65452 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119250 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75531 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103453 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35544 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92139 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    94453 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   187865 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/xt.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51368 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28777 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   183857 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/zb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74036 2023-05-05 15:55:39.000000 ccxt-3.0.94/ccxt/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-05 16:10:46.098733 ccxt-3.0.94/ccxt.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113274 2023-05-05 16:10:45.000000 ccxt-3.0.94/ccxt.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11640 2023-05-05 16:10:45.000000 ccxt-3.0.94/ccxt.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-05 16:10:45.000000 ccxt-3.0.94/ccxt.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-05-05 16:10:45.000000 ccxt-3.0.94/ccxt.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2023-05-05 16:10:45.000000 ccxt-3.0.94/ccxt.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8459 2023-05-05 16:10:29.000000 ccxt-3.0.94/package.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      205 2023-05-05 16:10:46.438757 ccxt-3.0.94/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2891 2023-05-05 15:55:39.000000 ccxt-3.0.94/setup.py
```

### Comparing `ccxt-3.0.93/LICENSE.txt` & `ccxt-3.0.94/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/PKG-INFO` & `ccxt-3.0.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 3.0.93
+Version: 3.0.94
 Summary: A JavaScript / Python / PHP cryptocurrency trading library with support for 130+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://docs.ccxt.com
@@ -227,21 +227,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@3.0.93/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@3.0.93/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@3.0.94/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@3.0.94/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@3.0.93/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@3.0.94/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-3.0.93/README.rst` & `ccxt-3.0.94/README.rst`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/__init__.py` & `ccxt-3.0.94/ccxt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # ----------------------------------------------------------------------------
 
-__version__ = '3.0.93'
+__version__ = '3.0.94'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.base.exchange import Exchange                     # noqa: F401
 from ccxt.base.precise import Precise                       # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
```

### Comparing `ccxt-3.0.93/ccxt/abstract/ace.py` & `ccxt-3.0.94/ccxt/abstract/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/alpaca.py` & `ccxt-3.0.94/ccxt/abstract/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/ascendex.py` & `ccxt-3.0.94/ccxt/abstract/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bequant.py` & `ccxt-3.0.94/ccxt/abstract/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bigone.py` & `ccxt-3.0.94/ccxt/abstract/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/binance.py` & `ccxt-3.0.94/ccxt/abstract/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/binancecoinm.py` & `ccxt-3.0.94/ccxt/abstract/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/binanceus.py` & `ccxt-3.0.94/ccxt/abstract/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/binanceusdm.py` & `ccxt-3.0.94/ccxt/abstract/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bit2c.py` & `ccxt-3.0.94/ccxt/abstract/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitbank.py` & `ccxt-3.0.94/ccxt/abstract/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitbay.py` & `ccxt-3.0.94/ccxt/abstract/bitbay.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitbns.py` & `ccxt-3.0.94/ccxt/abstract/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitcoincom.py` & `ccxt-3.0.94/ccxt/abstract/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitfinex.py` & `ccxt-3.0.94/ccxt/abstract/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitfinex2.py` & `ccxt-3.0.94/ccxt/abstract/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitflyer.py` & `ccxt-3.0.94/ccxt/abstract/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitforex.py` & `ccxt-3.0.94/ccxt/abstract/bitforex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitget.py` & `ccxt-3.0.94/ccxt/abstract/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bithumb.py` & `ccxt-3.0.94/ccxt/abstract/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitmart.py` & `ccxt-3.0.94/ccxt/abstract/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitmex.py` & `ccxt-3.0.94/ccxt/abstract/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitopro.py` & `ccxt-3.0.94/ccxt/abstract/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitpanda.py` & `ccxt-3.0.94/ccxt/abstract/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitrue.py` & `ccxt-3.0.94/ccxt/abstract/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitso.py` & `ccxt-3.0.94/ccxt/abstract/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitstamp.py` & `ccxt-3.0.94/ccxt/abstract/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitstamp1.py` & `ccxt-3.0.94/ccxt/abstract/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bittrex.py` & `ccxt-3.0.94/ccxt/abstract/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bitvavo.py` & `ccxt-3.0.94/ccxt/abstract/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bkex.py` & `ccxt-3.0.94/ccxt/abstract/bkex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bl3p.py` & `ccxt-3.0.94/ccxt/abstract/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/blockchaincom.py` & `ccxt-3.0.94/ccxt/abstract/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/btcalpha.py` & `ccxt-3.0.94/ccxt/abstract/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/btcbox.py` & `ccxt-3.0.94/ccxt/abstract/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/btcex.py` & `ccxt-3.0.94/ccxt/abstract/btcex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/btcmarkets.py` & `ccxt-3.0.94/ccxt/abstract/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/btctradeua.py` & `ccxt-3.0.94/ccxt/abstract/btctradeua.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/btcturk.py` & `ccxt-3.0.94/ccxt/abstract/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/bybit.py` & `ccxt-3.0.94/ccxt/abstract/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/cex.py` & `ccxt-3.0.94/ccxt/abstract/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/coinbase.py` & `ccxt-3.0.94/ccxt/abstract/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/coinbaseprime.py` & `ccxt-3.0.94/ccxt/abstract/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/coinbasepro.py` & `ccxt-3.0.94/ccxt/abstract/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/coincheck.py` & `ccxt-3.0.94/ccxt/abstract/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/coinex.py` & `ccxt-3.0.94/ccxt/abstract/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/coinfalcon.py` & `ccxt-3.0.94/ccxt/abstract/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/coinmate.py` & `ccxt-3.0.94/ccxt/abstract/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/coinone.py` & `ccxt-3.0.94/ccxt/abstract/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/coinsph.py` & `ccxt-3.0.94/ccxt/abstract/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/coinspot.py` & `ccxt-3.0.94/ccxt/abstract/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/cryptocom.py` & `ccxt-3.0.94/ccxt/abstract/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/currencycom.py` & `ccxt-3.0.94/ccxt/abstract/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/delta.py` & `ccxt-3.0.94/ccxt/abstract/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/deribit.py` & `ccxt-3.0.94/ccxt/abstract/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/digifinex.py` & `ccxt-3.0.94/ccxt/abstract/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/exmo.py` & `ccxt-3.0.94/ccxt/abstract/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/fmfwio.py` & `ccxt-3.0.94/ccxt/abstract/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/gate.py` & `ccxt-3.0.94/ccxt/abstract/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/gateio.py` & `ccxt-3.0.94/ccxt/abstract/gateio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/gemini.py` & `ccxt-3.0.94/ccxt/abstract/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/hitbtc.py` & `ccxt-3.0.94/ccxt/abstract/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/hitbtc3.py` & `ccxt-3.0.94/ccxt/abstract/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/hollaex.py` & `ccxt-3.0.94/ccxt/abstract/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/huobi.py` & `ccxt-3.0.94/ccxt/abstract/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/huobijp.py` & `ccxt-3.0.94/ccxt/abstract/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/huobipro.py` & `ccxt-3.0.94/ccxt/abstract/huobipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/idex.py` & `ccxt-3.0.94/ccxt/abstract/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/independentreserve.py` & `ccxt-3.0.94/ccxt/abstract/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/indodax.py` & `ccxt-3.0.94/ccxt/abstract/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/kraken.py` & `ccxt-3.0.94/ccxt/abstract/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/krakenfutures.py` & `ccxt-3.0.94/ccxt/abstract/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/kucoin.py` & `ccxt-3.0.94/ccxt/abstract/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/kucoinfutures.py` & `ccxt-3.0.94/ccxt/abstract/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/kuna.py` & `ccxt-3.0.94/ccxt/abstract/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/latoken.py` & `ccxt-3.0.94/ccxt/abstract/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/lbank.py` & `ccxt-3.0.94/ccxt/abstract/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/lbank2.py` & `ccxt-3.0.94/ccxt/abstract/lbank2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/luno.py` & `ccxt-3.0.94/ccxt/abstract/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/lykke.py` & `ccxt-3.0.94/ccxt/abstract/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/mercado.py` & `ccxt-3.0.94/ccxt/abstract/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/mexc.py` & `ccxt-3.0.94/ccxt/abstract/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/mexc3.py` & `ccxt-3.0.94/ccxt/abstract/mexc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/ndax.py` & `ccxt-3.0.94/ccxt/abstract/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/novadax.py` & `ccxt-3.0.94/ccxt/abstract/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/oceanex.py` & `ccxt-3.0.94/ccxt/abstract/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/okcoin.py` & `ccxt-3.0.94/ccxt/abstract/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/okex.py` & `ccxt-3.0.94/ccxt/abstract/okex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/okex5.py` & `ccxt-3.0.94/ccxt/abstract/okex5.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/okx.py` & `ccxt-3.0.94/ccxt/abstract/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/paymium.py` & `ccxt-3.0.94/ccxt/abstract/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/phemex.py` & `ccxt-3.0.94/ccxt/abstract/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/poloniex.py` & `ccxt-3.0.94/ccxt/abstract/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/poloniexfutures.py` & `ccxt-3.0.94/ccxt/abstract/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/probit.py` & `ccxt-3.0.94/ccxt/abstract/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/stex.py` & `ccxt-3.0.94/ccxt/abstract/stex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/tidex.py` & `ccxt-3.0.94/ccxt/abstract/tidex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/timex.py` & `ccxt-3.0.94/ccxt/abstract/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/tokocrypto.py` & `ccxt-3.0.94/ccxt/abstract/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/upbit.py` & `ccxt-3.0.94/ccxt/abstract/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/wavesexchange.py` & `ccxt-3.0.94/ccxt/abstract/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/wazirx.py` & `ccxt-3.0.94/ccxt/abstract/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/whitebit.py` & `ccxt-3.0.94/ccxt/abstract/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/woo.py` & `ccxt-3.0.94/ccxt/abstract/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/xt.py` & `ccxt-3.0.94/ccxt/abstract/xt.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/yobit.py` & `ccxt-3.0.94/ccxt/abstract/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/zaif.py` & `ccxt-3.0.94/ccxt/abstract/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/abstract/zonda.py` & `ccxt-3.0.94/ccxt/abstract/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/ace.py` & `ccxt-3.0.94/ccxt/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/alpaca.py` & `ccxt-3.0.94/ccxt/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/ascendex.py` & `ccxt-3.0.94/ccxt/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/__init__.py` & `ccxt-3.0.94/ccxt/async_support/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '3.0.93'
+__version__ = '3.0.94'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.async_support.base.exchange import Exchange                   # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
 from ccxt.base.decimal_to_precision import TRUNCATE              # noqa: F401
```

### Comparing `ccxt-3.0.93/ccxt/async_support/ace.py` & `ccxt-3.0.94/ccxt/async_support/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/alpaca.py` & `ccxt-3.0.94/ccxt/async_support/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/ascendex.py` & `ccxt-3.0.94/ccxt/async_support/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/base/exchange.py` & `ccxt-3.0.94/ccxt/async_support/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # -----------------------------------------------------------------------------
 
-__version__ = '3.0.93'
+__version__ = '3.0.94'
 
 # -----------------------------------------------------------------------------
 
 import asyncio
 import concurrent.futures
 import socket
 import certifi
```

### Comparing `ccxt-3.0.93/ccxt/async_support/base/throttler.py` & `ccxt-3.0.94/ccxt/async_support/base/throttler.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/base/ws/__init__.py` & `ccxt-3.0.94/ccxt/async_support/base/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/base/ws/aiohttp_client.py` & `ccxt-3.0.94/ccxt/async_support/base/ws/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/base/ws/cache.py` & `ccxt-3.0.94/ccxt/async_support/base/ws/cache.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/base/ws/client.py` & `ccxt-3.0.94/ccxt/async_support/base/ws/client.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/base/ws/fast_client.py` & `ccxt-3.0.94/ccxt/async_support/base/ws/fast_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/base/ws/functions.py` & `ccxt-3.0.94/ccxt/async_support/base/ws/functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/base/ws/order_book.py` & `ccxt-3.0.94/ccxt/async_support/base/ws/order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/base/ws/order_book_side.py` & `ccxt-3.0.94/ccxt/async_support/base/ws/order_book_side.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bequant.py` & `ccxt-3.0.94/ccxt/async_support/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bigone.py` & `ccxt-3.0.94/ccxt/async_support/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/binance.py` & `ccxt-3.0.94/ccxt/async_support/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/binancecoinm.py` & `ccxt-3.0.94/ccxt/async_support/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/binanceus.py` & `ccxt-3.0.94/ccxt/async_support/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/binanceusdm.py` & `ccxt-3.0.94/ccxt/async_support/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bit2c.py` & `ccxt-3.0.94/ccxt/async_support/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitbank.py` & `ccxt-3.0.94/ccxt/async_support/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitbns.py` & `ccxt-3.0.94/ccxt/async_support/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitfinex.py` & `ccxt-3.0.94/ccxt/async_support/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitfinex2.py` & `ccxt-3.0.94/ccxt/async_support/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitflyer.py` & `ccxt-3.0.94/ccxt/async_support/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitforex.py` & `ccxt-3.0.94/ccxt/async_support/bitforex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitget.py` & `ccxt-3.0.94/ccxt/async_support/bitget.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,28 +112,26 @@
                 'setLeverage': True,
                 'setMarginMode': True,
                 'setPositionMode': True,
                 'transfer': True,
                 'withdraw': False,
             },
             'timeframes': {
-                '1m': '1m',
-                '3m': '3m',
-                '5m': '5m',
-                '15m': '15m',
-                '30m': '30m',
+                '1m': '1min',
+                '5m': '5min',
+                '15m': '15min',
+                '30m': '30min',
                 '1h': '1h',
-                '2h': '2h',
                 '4h': '4h',
-                '6h': '6h',
-                '12h': '12h',
-                '1d': '1d',
-                '3d': '3d',
-                '1w': '1w',
-                '1M': '1M',
+                '6h': '6Hutc',
+                '12h': '12Hutc',
+                '1d': '1Dutc',
+                '3d': '3Dutc',
+                '1w': '1Wutc',
+                '1M': '1Mutc',
             },
             'hostname': 'bitget.com',
             'urls': {
                 'logo': 'https://user-images.githubusercontent.com/1294454/195989417-4253ddb0-afbe-4a1c-9dea-9dbcd121fa5d.jpg',
                 'api': {
                     'spot': 'https://api.{hostname}',
                     'mix': 'https://api.{hostname}',
@@ -821,18 +819,18 @@
             'precisionMode': TICK_SIZE,
             'commonCurrencies': {
                 'JADE': 'Jade Protocol',
             },
             'options': {
                 'timeframes': {
                     'spot': {
-                        '1m': '1m',
-                        '5m': '5m',
-                        '15m': '15m',
-                        '30m': '30m',
+                        '1m': '1min',
+                        '5m': '5min',
+                        '15m': '15min',
+                        '30m': '30min',
                         '1h': '1h',
                         '4h': '4h',
                         '6h': '6Hutc',
                         '12h': '12Hutc',
                         '1d': '1Dutc',
                         '3d': '3Dutc',
                         '1w': '1Wutc',
@@ -2077,14 +2075,15 @@
             self.safe_number_2(ohlcv, 5, 'baseVol'),
         ]
 
     async def fetch_ohlcv(self, symbol: str, timeframe='1m', since: Optional[int] = None, limit: Optional[int] = None, params={}):
         """
         fetches historical candlestick data containing the open, high, low, and close price, and the volume of a market
         see https://bitgetlimited.github.io/apidoc/en/mix/#get-candle-data
+        see https://bitgetlimited.github.io/apidoc/en/spot/#candlestick-line-timeframe
         :param str symbol: unified symbol of the market to fetch OHLCV data for
         :param str timeframe: the length of time each candle represents
         :param int|None since: timestamp in ms of the earliest candle to fetch
         :param int|None limit: the maximum amount of candles to fetch
         :param dict params: extra parameters specific to the bitget api endpoint
         :param int|None params['until']: timestamp in ms of the latest candle to fetch
         :returns [[int]]: A list of candles ordered, open, high, low, close, volume
@@ -2092,15 +2091,16 @@
         await self.load_markets()
         market = self.market(symbol)
         request = {
             'symbol': market['id'],
         }
         until = self.safe_integer_2(params, 'until', 'till')
         if limit is None:
-            limit = 100
+            limit = 1000
+        request['limit'] = limit
         marketType = 'spot' if market['spot'] else 'swap'
         timeframes = self.options['timeframes'][marketType]
         selectedTimeframe = self.safe_string(timeframes, timeframe, timeframe)
         duration = self.parse_timeframe(timeframe)
         if market['spot']:
             request['period'] = selectedTimeframe
             request['limit'] = limit
@@ -2110,18 +2110,18 @@
                     request['before'] = self.sum(since, limit * duration * 1000)
             if until is not None:
                 request['before'] = until
         elif market['contract']:
             request['granularity'] = selectedTimeframe
             now = self.milliseconds()
             if since is None:
-                request['startTime'] = now - (limit - 1) * (duration * 1000)
+                request['startTime'] = now - limit * (duration * 1000)
                 request['endTime'] = now
             else:
-                request['startTime'] = self.sum(since, duration * 1000)
+                request['startTime'] = since
                 if until is not None:
                     request['endTime'] = until
                 else:
                     request['endTime'] = self.sum(since, limit * duration * 1000)
         ommitted = self.omit(params, ['until', 'till'])
         extended = self.extend(request, ommitted)
         response = None
```

### Comparing `ccxt-3.0.93/ccxt/async_support/bithumb.py` & `ccxt-3.0.94/ccxt/async_support/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitmart.py` & `ccxt-3.0.94/ccxt/async_support/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitmex.py` & `ccxt-3.0.94/ccxt/async_support/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitopro.py` & `ccxt-3.0.94/ccxt/async_support/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitpanda.py` & `ccxt-3.0.94/ccxt/async_support/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitrue.py` & `ccxt-3.0.94/ccxt/async_support/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitso.py` & `ccxt-3.0.94/ccxt/async_support/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitstamp.py` & `ccxt-3.0.94/ccxt/async_support/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitstamp1.py` & `ccxt-3.0.94/ccxt/async_support/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bittrex.py` & `ccxt-3.0.94/ccxt/async_support/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bitvavo.py` & `ccxt-3.0.94/ccxt/async_support/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bkex.py` & `ccxt-3.0.94/ccxt/async_support/bkex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bl3p.py` & `ccxt-3.0.94/ccxt/async_support/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/blockchaincom.py` & `ccxt-3.0.94/ccxt/async_support/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/btcalpha.py` & `ccxt-3.0.94/ccxt/async_support/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/btcbox.py` & `ccxt-3.0.94/ccxt/async_support/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/btcex.py` & `ccxt-3.0.94/ccxt/async_support/btcex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/btcmarkets.py` & `ccxt-3.0.94/ccxt/async_support/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/btctradeua.py` & `ccxt-3.0.94/ccxt/async_support/btctradeua.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/btcturk.py` & `ccxt-3.0.94/ccxt/async_support/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/buda.py` & `ccxt-3.0.94/ccxt/async_support/buda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/bybit.py` & `ccxt-3.0.94/ccxt/async_support/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/cex.py` & `ccxt-3.0.94/ccxt/async_support/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/coinbase.py` & `ccxt-3.0.94/ccxt/async_support/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/coinbaseprime.py` & `ccxt-3.0.94/ccxt/async_support/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/coinbasepro.py` & `ccxt-3.0.94/ccxt/async_support/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/coincheck.py` & `ccxt-3.0.94/ccxt/async_support/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/coinex.py` & `ccxt-3.0.94/ccxt/async_support/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/coinfalcon.py` & `ccxt-3.0.94/ccxt/async_support/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/coinmate.py` & `ccxt-3.0.94/ccxt/async_support/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/coinone.py` & `ccxt-3.0.94/ccxt/async_support/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/coinsph.py` & `ccxt-3.0.94/ccxt/async_support/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/coinspot.py` & `ccxt-3.0.94/ccxt/async_support/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/cryptocom.py` & `ccxt-3.0.94/ccxt/async_support/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/currencycom.py` & `ccxt-3.0.94/ccxt/async_support/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/delta.py` & `ccxt-3.0.94/ccxt/async_support/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/deribit.py` & `ccxt-3.0.94/ccxt/async_support/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/digifinex.py` & `ccxt-3.0.94/ccxt/async_support/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/exmo.py` & `ccxt-3.0.94/ccxt/async_support/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/flowbtc.py` & `ccxt-3.0.94/ccxt/async_support/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/fmfwio.py` & `ccxt-3.0.94/ccxt/async_support/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/gate.py` & `ccxt-3.0.94/ccxt/async_support/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/gemini.py` & `ccxt-3.0.94/ccxt/async_support/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/hitbtc.py` & `ccxt-3.0.94/ccxt/async_support/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/hitbtc3.py` & `ccxt-3.0.94/ccxt/async_support/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/hollaex.py` & `ccxt-3.0.94/ccxt/async_support/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/huobi.py` & `ccxt-3.0.94/ccxt/async_support/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/huobijp.py` & `ccxt-3.0.94/ccxt/async_support/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/huobipro.py` & `ccxt-3.0.94/ccxt/async_support/huobipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/idex.py` & `ccxt-3.0.94/ccxt/async_support/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/independentreserve.py` & `ccxt-3.0.94/ccxt/async_support/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/indodax.py` & `ccxt-3.0.94/ccxt/async_support/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/itbit.py` & `ccxt-3.0.94/ccxt/async_support/itbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/kraken.py` & `ccxt-3.0.94/ccxt/async_support/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/krakenfutures.py` & `ccxt-3.0.94/ccxt/async_support/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/kucoin.py` & `ccxt-3.0.94/ccxt/async_support/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/kucoinfutures.py` & `ccxt-3.0.94/ccxt/async_support/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/kuna.py` & `ccxt-3.0.94/ccxt/async_support/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/latoken.py` & `ccxt-3.0.94/ccxt/async_support/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/lbank.py` & `ccxt-3.0.94/ccxt/async_support/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/lbank2.py` & `ccxt-3.0.94/ccxt/async_support/lbank2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/luno.py` & `ccxt-3.0.94/ccxt/async_support/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/lykke.py` & `ccxt-3.0.94/ccxt/async_support/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/mercado.py` & `ccxt-3.0.94/ccxt/async_support/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/mexc.py` & `ccxt-3.0.94/ccxt/async_support/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/ndax.py` & `ccxt-3.0.94/ccxt/async_support/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/novadax.py` & `ccxt-3.0.94/ccxt/async_support/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/oceanex.py` & `ccxt-3.0.94/ccxt/async_support/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/okcoin.py` & `ccxt-3.0.94/ccxt/async_support/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/okx.py` & `ccxt-3.0.94/ccxt/async_support/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/paymium.py` & `ccxt-3.0.94/ccxt/async_support/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/phemex.py` & `ccxt-3.0.94/ccxt/async_support/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/poloniex.py` & `ccxt-3.0.94/ccxt/async_support/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/poloniexfutures.py` & `ccxt-3.0.94/ccxt/async_support/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/probit.py` & `ccxt-3.0.94/ccxt/async_support/probit.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,15 +421,52 @@
             currency = currencies[i]
             id = self.safe_string(currency, 'id')
             code = self.safe_currency_code(id)
             displayName = self.safe_value(currency, 'display_name')
             name = self.safe_string(displayName, 'en-us')
             platforms = self.safe_value(currency, 'platform', [])
             platformsByPriority = self.sort_by(platforms, 'priority')
-            platform = self.safe_value(platformsByPriority, 0, {})
+            platform = None
+            networkList = {}
+            for j in range(0, len(platformsByPriority)):
+                network = platformsByPriority[j]
+                id = self.safe_string(network, 'id')
+                networkCode = self.network_id_to_code(id)
+                currentDepositSuspended = self.safe_value(network, 'deposit_suspended')
+                currentWithdrawalSuspended = self.safe_value(network, 'withdrawal_suspended')
+                currentDeposit = not currentDepositSuspended
+                currentWithdraw = not currentWithdrawalSuspended
+                currentActive = currentDeposit and currentWithdraw
+                if currentActive:
+                    platform = network
+                precision = self.safe_string(network, 'precision')
+                withdrawFee = self.safe_value(network, 'withdrawal_fee', [])
+                fee = self.safe_value(withdrawFee, 0, {})
+                networkList[networkCode] = {
+                    'id': id,
+                    'network': networkCode,
+                    'active': currentActive,
+                    'deposit': currentDeposit,
+                    'withdraw': currentWithdraw,
+                    'fee': self.safe_number(fee, 'amount'),
+                    'precision': self.parse_number(precision),
+                    'limits': {
+                        'withdraw': {
+                            'min': self.safe_number(network, 'min_withdrawal_amount'),
+                            'max': None,
+                        },
+                        'deposit': {
+                            'min': self.safe_number(network, 'min_deposit_amount'),
+                            'max': None,
+                        },
+                    },
+                    'info': network,
+                }
+            if platform is None:
+                platform = self.safe_value(platformsByPriority, 0, {})
             depositSuspended = self.safe_value(platform, 'deposit_suspended')
             withdrawalSuspended = self.safe_value(platform, 'withdrawal_suspended')
             deposit = not depositSuspended
             withdraw = not withdrawalSuspended
             active = deposit and withdraw
             withdrawalFees = self.safe_value(platform, 'withdrawal_fee', {})
             fees = []
@@ -464,15 +501,15 @@
                         'max': None,
                     },
                     'withdraw': {
                         'min': self.safe_number(platform, 'min_withdrawal_amount'),
                         'max': None,
                     },
                 },
-                'networks': {},
+                'networks': networkList,
             }
         return result
 
     def parse_balance(self, response):
         result = {
             'info': response,
             'timestamp': None,
```

### Comparing `ccxt-3.0.93/ccxt/async_support/ripio.py` & `ccxt-3.0.94/ccxt/async_support/ripio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/stex.py` & `ccxt-3.0.94/ccxt/async_support/stex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/tidex.py` & `ccxt-3.0.94/ccxt/async_support/tidex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/timex.py` & `ccxt-3.0.94/ccxt/async_support/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/tokocrypto.py` & `ccxt-3.0.94/ccxt/async_support/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/upbit.py` & `ccxt-3.0.94/ccxt/async_support/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/wavesexchange.py` & `ccxt-3.0.94/ccxt/async_support/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/wazirx.py` & `ccxt-3.0.94/ccxt/async_support/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/whitebit.py` & `ccxt-3.0.94/ccxt/async_support/whitebit.py`

 * *Files 0% similar despite different names*

```diff
@@ -5628,160 +5628,160 @@
 00015fb0: 7427 3a20 7265 7175 6573 742c 2027 6e6f  t': request, 'no
 00015fc0: 6e63 6527 3a20 6e6f 6e63 657d 2c20 7061  nce': nonce}, pa
 00015fd0: 7261 6d73 2929 0a20 2020 2020 2020 2020  rams)).         
 00015fe0: 2020 2070 6179 6c6f 6164 203d 2073 656c     payload = sel
 00015ff0: 662e 7374 7269 6e67 5f74 6f5f 6261 7365  f.string_to_base
 00016000: 3634 2862 6f64 7929 0a20 2020 2020 2020  64(body).       
 00016010: 2020 2020 2073 6967 6e61 7475 7265 203d       signature =
-00016020: 2073 656c 662e 686d 6163 2870 6179 6c6f   self.hmac(paylo
-00016030: 6164 2c20 7365 6372 6574 2c20 6861 7368  ad, secret, hash
-00016040: 6c69 622e 7368 6135 3132 290a 2020 2020  lib.sha512).    
-00016050: 2020 2020 2020 2020 6865 6164 6572 7320          headers 
-00016060: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-00016070: 2020 2020 2743 6f6e 7465 6e74 2d54 7970      'Content-Typ
-00016080: 6527 3a20 2761 7070 6c69 6361 7469 6f6e  e': 'application
-00016090: 2f6a 736f 6e27 2c0a 2020 2020 2020 2020  /json',.        
-000160a0: 2020 2020 2020 2020 2758 2d54 5843 2d41          'X-TXC-A
-000160b0: 5049 4b45 5927 3a20 7365 6c66 2e61 7069  PIKEY': self.api
-000160c0: 4b65 792c 0a20 2020 2020 2020 2020 2020  Key,.           
-000160d0: 2020 2020 2027 582d 5458 432d 5041 594c       'X-TXC-PAYL
-000160e0: 4f41 4427 3a20 7061 796c 6f61 642c 0a20  OAD': payload,. 
-000160f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00016100: 582d 5458 432d 5349 474e 4154 5552 4527  X-TXC-SIGNATURE'
-00016110: 3a20 7369 676e 6174 7572 652c 0a20 2020  : signature,.   
-00016120: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00016130: 2020 2072 6574 7572 6e20 7b27 7572 6c27     return {'url'
-00016140: 3a20 7572 6c2c 2027 6d65 7468 6f64 273a  : url, 'method':
-00016150: 206d 6574 686f 642c 2027 626f 6479 273a   method, 'body':
-00016160: 2062 6f64 792c 2027 6865 6164 6572 7327   body, 'headers'
-00016170: 3a20 6865 6164 6572 737d 0a0a 2020 2020  : headers}..    
-00016180: 6465 6620 6861 6e64 6c65 5f65 7272 6f72  def handle_error
-00016190: 7328 7365 6c66 2c20 636f 6465 2c20 7265  s(self, code, re
-000161a0: 6173 6f6e 2c20 7572 6c2c 206d 6574 686f  ason, url, metho
-000161b0: 642c 2068 6561 6465 7273 2c20 626f 6479  d, headers, body
-000161c0: 2c20 7265 7370 6f6e 7365 2c20 7265 7175  , response, requ
-000161d0: 6573 7448 6561 6465 7273 2c20 7265 7175  estHeaders, requ
-000161e0: 6573 7442 6f64 7929 3a0a 2020 2020 2020  estBody):.      
-000161f0: 2020 6966 2028 636f 6465 203d 3d20 3431    if (code == 41
-00016200: 3829 206f 7220 2863 6f64 6520 3d3d 2034  8) or (code == 4
-00016210: 3239 293a 0a20 2020 2020 2020 2020 2020  29):.           
-00016220: 2072 6169 7365 2044 446f 5350 726f 7465   raise DDoSProte
-00016230: 6374 696f 6e28 7365 6c66 2e69 6420 2b20  ction(self.id + 
-00016240: 2720 2720 2b20 7374 7228 636f 6465 2920  ' ' + str(code) 
-00016250: 2b20 2720 2720 2b20 7265 6173 6f6e 202b  + ' ' + reason +
-00016260: 2027 2027 202b 2062 6f64 7929 0a20 2020   ' ' + body).   
-00016270: 2020 2020 2069 6620 636f 6465 203d 3d20       if code == 
-00016280: 3430 343a 0a20 2020 2020 2020 2020 2020  404:.           
-00016290: 2072 6169 7365 2045 7863 6861 6e67 6545   raise ExchangeE
-000162a0: 7272 6f72 2873 656c 662e 6964 202b 2027  rror(self.id + '
-000162b0: 2027 202b 2073 7472 2863 6f64 6529 202b   ' + str(code) +
-000162c0: 2027 2065 6e64 706f 696e 7420 6e6f 7420   ' endpoint not 
-000162d0: 666f 756e 6427 290a 2020 2020 2020 2020  found').        
-000162e0: 6966 2072 6573 706f 6e73 6520 6973 206e  if response is n
-000162f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00016300: 2020 2020 2023 2046 6f72 2063 6173 6573       # For cases
-00016310: 2077 6865 7265 2077 6520 6861 7665 2061   where we have a
-00016320: 206d 6561 6e69 6e67 6675 6c20 7374 6174   meaningful stat
-00016330: 7573 0a20 2020 2020 2020 2020 2020 2023  us.            #
-00016340: 207b 2272 6573 706f 6e73 6522 3a6e 756c   {"response":nul
-00016350: 6c2c 2273 7461 7475 7322 3a34 3232 2c22  l,"status":422,"
-00016360: 6572 726f 7273 223a 7b22 6f72 6465 7249  errors":{"orderI
-00016370: 6422 3a5b 2246 696e 6973 6865 6420 6f72  d":["Finished or
-00016380: 6465 7220 6964 2034 3335 3435 3334 3534  der id 435453454
-00016390: 3533 3520 6e6f 7420 666f 756e 6420 6f6e  535 not found on
-000163a0: 2079 6f75 7220 6163 636f 756e 7422 5d7d   your account"]}
-000163b0: 2c22 6e6f 7469 6669 6361 7469 6f6e 223a  ,"notification":
-000163c0: 6e75 6c6c 2c22 7761 726e 696e 6722 3a22  null,"warning":"
-000163d0: 4669 6e69 7368 6564 206f 7264 6572 2069  Finished order i
-000163e0: 6420 3433 3534 3533 3435 3435 3335 206e  d 435453454535 n
-000163f0: 6f74 2066 6f75 6e64 206f 6e20 796f 7572  ot found on your
-00016400: 2061 6363 6f75 6e74 222c 225f 746f 6b65   account","_toke
-00016410: 6e22 3a6e 756c 6c7d 0a20 2020 2020 2020  n":null}.       
-00016420: 2020 2020 2073 7461 7475 7320 3d20 7365       status = se
-00016430: 6c66 2e73 6166 655f 7374 7269 6e67 2872  lf.safe_string(r
-00016440: 6573 706f 6e73 652c 2027 7374 6174 7573  esponse, 'status
-00016450: 2729 0a20 2020 2020 2020 2020 2020 2023  ').            #
-00016460: 207b 2263 6f64 6522 3a31 302c 226d 6573   {"code":10,"mes
-00016470: 7361 6765 223a 2255 6e61 7574 686f 7269  sage":"Unauthori
-00016480: 7a65 6420 7265 7175 6573 742e 227d 0a20  zed request."}. 
-00016490: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-000164a0: 6765 203d 2073 656c 662e 7361 6665 5f73  ge = self.safe_s
-000164b0: 7472 696e 6728 7265 7370 6f6e 7365 2c20  tring(response, 
-000164c0: 276d 6573 7361 6765 2729 0a20 2020 2020  'message').     
-000164d0: 2020 2020 2020 2023 2046 6f72 2074 6865         # For the
-000164e0: 7365 2063 6173 6573 2077 6865 7265 2077  se cases where w
-000164f0: 6520 6861 7665 2061 2067 656e 6572 6963  e have a generic
-00016500: 2063 6f64 6520 7661 7269 6162 6c65 2065   code variable e
-00016510: 7272 6f72 206b 6579 0a20 2020 2020 2020  rror key.       
-00016520: 2020 2020 2023 207b 2263 6f64 6522 3a30       # {"code":0
-00016530: 2c22 6d65 7373 6167 6522 3a22 5661 6c69  ,"message":"Vali
-00016540: 6461 7469 6f6e 2066 6169 6c65 6422 2c22  dation failed","
-00016550: 6572 726f 7273 223a 7b22 616d 6f75 6e74  errors":{"amount
-00016560: 223a 5b22 416d 6f75 6e74 206d 7573 7420  ":["Amount must 
-00016570: 6265 2067 7265 6174 6572 2074 6861 6e20  be greater than 
-00016580: 3022 5d7d 7d0a 2020 2020 2020 2020 2020  0"]}}.          
-00016590: 2020 636f 6465 4e65 7720 3d20 7365 6c66    codeNew = self
-000165a0: 2e73 6166 655f 696e 7465 6765 7228 7265  .safe_integer(re
-000165b0: 7370 6f6e 7365 2c20 2763 6f64 6527 290a  sponse, 'code').
-000165c0: 2020 2020 2020 2020 2020 2020 6861 7345              hasE
-000165d0: 7272 6f72 5374 6174 7573 203d 2073 7461  rrorStatus = sta
-000165e0: 7475 7320 6973 206e 6f74 204e 6f6e 6520  tus is not None 
-000165f0: 616e 6420 7374 6174 7573 2021 3d20 2732  and status != '2
-00016600: 3030 270a 2020 2020 2020 2020 2020 2020  00'.            
-00016610: 6966 2068 6173 4572 726f 7253 7461 7475  if hasErrorStatu
-00016620: 7320 6f72 2063 6f64 654e 6577 2069 7320  s or codeNew is 
-00016630: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00016640: 2020 2020 2020 2020 2020 6665 6564 6261            feedba
-00016650: 636b 203d 2073 656c 662e 6964 202b 2027  ck = self.id + '
-00016660: 2027 202b 2062 6f64 790a 2020 2020 2020   ' + body.      
-00016670: 2020 2020 2020 2020 2020 6572 726f 7249            errorI
-00016680: 6e66 6f20 3d20 6d65 7373 6167 650a 2020  nfo = message.  
-00016690: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000166a0: 2068 6173 4572 726f 7253 7461 7475 733a   hasErrorStatus:
-000166b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000166c0: 2020 2020 2065 7272 6f72 496e 666f 203d       errorInfo =
-000166d0: 2073 7461 7475 730a 2020 2020 2020 2020   status.        
-000166e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000166f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016700: 2020 6572 726f 724f 626a 6563 7420 3d20    errorObject = 
-00016710: 7365 6c66 2e73 6166 655f 7661 6c75 6528  self.safe_value(
-00016720: 7265 7370 6f6e 7365 2c20 2765 7272 6f72  response, 'error
-00016730: 7327 290a 2020 2020 2020 2020 2020 2020  s').            
-00016740: 2020 2020 2020 2020 6966 2065 7272 6f72          if error
-00016750: 4f62 6a65 6374 2069 7320 6e6f 7420 4e6f  Object is not No
-00016760: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00016770: 2020 2020 2020 2020 2020 2020 6572 726f              erro
-00016780: 724b 6579 203d 206c 6973 7428 6572 726f  rKey = list(erro
-00016790: 724f 626a 6563 742e 6b65 7973 2829 295b  rObject.keys())[
-000167a0: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
-000167b0: 2020 2020 2020 2020 2020 2065 7272 6f72             error
-000167c0: 4d65 7373 6167 6541 7272 6179 203d 2073  MessageArray = s
-000167d0: 656c 662e 7361 6665 5f76 616c 7565 2865  elf.safe_value(e
-000167e0: 7272 6f72 4f62 6a65 6374 2c20 6572 726f  rrorObject, erro
-000167f0: 724b 6579 2c20 5b5d 290a 2020 2020 2020  rKey, []).      
-00016800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016810: 2020 6572 726f 724d 6573 7361 6765 4c65    errorMessageLe
-00016820: 6e67 7468 203d 206c 656e 2865 7272 6f72  ngth = len(error
-00016830: 4d65 7373 6167 6541 7272 6179 290a 2020  MessageArray).  
-00016840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016850: 2020 2020 2020 6572 726f 7249 6e66 6f20        errorInfo 
-00016860: 3d20 6572 726f 724d 6573 7361 6765 4172  = errorMessageAr
-00016870: 7261 795b 305d 2069 6620 2865 7272 6f72  ray[0] if (error
-00016880: 4d65 7373 6167 654c 656e 6774 6820 3e20  MessageLength > 
-00016890: 3029 2065 6c73 6520 626f 6479 0a20 2020  0) else body.   
-000168a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000168b0: 662e 7468 726f 775f 6578 6163 746c 795f  f.throw_exactly_
-000168c0: 6d61 7463 6865 645f 6578 6365 7074 696f  matched_exceptio
-000168d0: 6e28 7365 6c66 2e65 7863 6570 7469 6f6e  n(self.exception
-000168e0: 735b 2765 7861 6374 275d 2c20 6572 726f  s['exact'], erro
-000168f0: 7249 6e66 6f2c 2066 6565 6462 6163 6b29  rInfo, feedback)
-00016900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016910: 2073 656c 662e 7468 726f 775f 6272 6f61   self.throw_broa
-00016920: 646c 795f 6d61 7463 6865 645f 6578 6365  dly_matched_exce
-00016930: 7074 696f 6e28 7365 6c66 2e65 7863 6570  ption(self.excep
-00016940: 7469 6f6e 735b 2762 726f 6164 275d 2c20  tions['broad'], 
-00016950: 626f 6479 2c20 6665 6564 6261 636b 290a  body, feedback).
-00016960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016970: 7261 6973 6520 4578 6368 616e 6765 4572  raise ExchangeEr
-00016980: 726f 7228 6665 6564 6261 636b 290a 2020  ror(feedback).  
-00016990: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-000169a0: 650a                                     e.
+00016020: 2073 656c 662e 686d 6163 2873 656c 662e   self.hmac(self.
+00016030: 656e 636f 6465 2870 6179 6c6f 6164 292c  encode(payload),
+00016040: 2073 6563 7265 742c 2068 6173 686c 6962   secret, hashlib
+00016050: 2e73 6861 3531 3229 0a20 2020 2020 2020  .sha512).       
+00016060: 2020 2020 2068 6561 6465 7273 203d 207b       headers = {
+00016070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016080: 2027 436f 6e74 656e 742d 5479 7065 273a   'Content-Type':
+00016090: 2027 6170 706c 6963 6174 696f 6e2f 6a73   'application/js
+000160a0: 6f6e 272c 0a20 2020 2020 2020 2020 2020  on',.           
+000160b0: 2020 2020 2027 582d 5458 432d 4150 494b       'X-TXC-APIK
+000160c0: 4559 273a 2073 656c 662e 6170 694b 6579  EY': self.apiKey
+000160d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000160e0: 2020 2758 2d54 5843 2d50 4159 4c4f 4144    'X-TXC-PAYLOAD
+000160f0: 273a 2070 6179 6c6f 6164 2c0a 2020 2020  ': payload,.    
+00016100: 2020 2020 2020 2020 2020 2020 2758 2d54              'X-T
+00016110: 5843 2d53 4947 4e41 5455 5245 273a 2073  XC-SIGNATURE': s
+00016120: 6967 6e61 7475 7265 2c0a 2020 2020 2020  ignature,.      
+00016130: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00016140: 7265 7475 726e 207b 2775 726c 273a 2075  return {'url': u
+00016150: 726c 2c20 276d 6574 686f 6427 3a20 6d65  rl, 'method': me
+00016160: 7468 6f64 2c20 2762 6f64 7927 3a20 626f  thod, 'body': bo
+00016170: 6479 2c20 2768 6561 6465 7273 273a 2068  dy, 'headers': h
+00016180: 6561 6465 7273 7d0a 0a20 2020 2064 6566  eaders}..    def
+00016190: 2068 616e 646c 655f 6572 726f 7273 2873   handle_errors(s
+000161a0: 656c 662c 2063 6f64 652c 2072 6561 736f  elf, code, reaso
+000161b0: 6e2c 2075 726c 2c20 6d65 7468 6f64 2c20  n, url, method, 
+000161c0: 6865 6164 6572 732c 2062 6f64 792c 2072  headers, body, r
+000161d0: 6573 706f 6e73 652c 2072 6571 7565 7374  esponse, request
+000161e0: 4865 6164 6572 732c 2072 6571 7565 7374  Headers, request
+000161f0: 426f 6479 293a 0a20 2020 2020 2020 2069  Body):.        i
+00016200: 6620 2863 6f64 6520 3d3d 2034 3138 2920  f (code == 418) 
+00016210: 6f72 2028 636f 6465 203d 3d20 3432 3929  or (code == 429)
+00016220: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00016230: 6973 6520 4444 6f53 5072 6f74 6563 7469  ise DDoSProtecti
+00016240: 6f6e 2873 656c 662e 6964 202b 2027 2027  on(self.id + ' '
+00016250: 202b 2073 7472 2863 6f64 6529 202b 2027   + str(code) + '
+00016260: 2027 202b 2072 6561 736f 6e20 2b20 2720   ' + reason + ' 
+00016270: 2720 2b20 626f 6479 290a 2020 2020 2020  ' + body).      
+00016280: 2020 6966 2063 6f64 6520 3d3d 2034 3034    if code == 404
+00016290: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+000162a0: 6973 6520 4578 6368 616e 6765 4572 726f  ise ExchangeErro
+000162b0: 7228 7365 6c66 2e69 6420 2b20 2720 2720  r(self.id + ' ' 
+000162c0: 2b20 7374 7228 636f 6465 2920 2b20 2720  + str(code) + ' 
+000162d0: 656e 6470 6f69 6e74 206e 6f74 2066 6f75  endpoint not fou
+000162e0: 6e64 2729 0a20 2020 2020 2020 2069 6620  nd').        if 
+000162f0: 7265 7370 6f6e 7365 2069 7320 6e6f 7420  response is not 
+00016300: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00016310: 2020 2320 466f 7220 6361 7365 7320 7768    # For cases wh
+00016320: 6572 6520 7765 2068 6176 6520 6120 6d65  ere we have a me
+00016330: 616e 696e 6766 756c 2073 7461 7475 730a  aningful status.
+00016340: 2020 2020 2020 2020 2020 2020 2320 7b22              # {"
+00016350: 7265 7370 6f6e 7365 223a 6e75 6c6c 2c22  response":null,"
+00016360: 7374 6174 7573 223a 3432 322c 2265 7272  status":422,"err
+00016370: 6f72 7322 3a7b 226f 7264 6572 4964 223a  ors":{"orderId":
+00016380: 5b22 4669 6e69 7368 6564 206f 7264 6572  ["Finished order
+00016390: 2069 6420 3433 3534 3533 3435 3435 3335   id 435453454535
+000163a0: 206e 6f74 2066 6f75 6e64 206f 6e20 796f   not found on yo
+000163b0: 7572 2061 6363 6f75 6e74 225d 7d2c 226e  ur account"]},"n
+000163c0: 6f74 6966 6963 6174 696f 6e22 3a6e 756c  otification":nul
+000163d0: 6c2c 2277 6172 6e69 6e67 223a 2246 696e  l,"warning":"Fin
+000163e0: 6973 6865 6420 6f72 6465 7220 6964 2034  ished order id 4
+000163f0: 3335 3435 3334 3534 3533 3520 6e6f 7420  35453454535 not 
+00016400: 666f 756e 6420 6f6e 2079 6f75 7220 6163  found on your ac
+00016410: 636f 756e 7422 2c22 5f74 6f6b 656e 223a  count","_token":
+00016420: 6e75 6c6c 7d0a 2020 2020 2020 2020 2020  null}.          
+00016430: 2020 7374 6174 7573 203d 2073 656c 662e    status = self.
+00016440: 7361 6665 5f73 7472 696e 6728 7265 7370  safe_string(resp
+00016450: 6f6e 7365 2c20 2773 7461 7475 7327 290a  onse, 'status').
+00016460: 2020 2020 2020 2020 2020 2020 2320 7b22              # {"
+00016470: 636f 6465 223a 3130 2c22 6d65 7373 6167  code":10,"messag
+00016480: 6522 3a22 556e 6175 7468 6f72 697a 6564  e":"Unauthorized
+00016490: 2072 6571 7565 7374 2e22 7d0a 2020 2020   request."}.    
+000164a0: 2020 2020 2020 2020 6d65 7373 6167 6520          message 
+000164b0: 3d20 7365 6c66 2e73 6166 655f 7374 7269  = self.safe_stri
+000164c0: 6e67 2872 6573 706f 6e73 652c 2027 6d65  ng(response, 'me
+000164d0: 7373 6167 6527 290a 2020 2020 2020 2020  ssage').        
+000164e0: 2020 2020 2320 466f 7220 7468 6573 6520      # For these 
+000164f0: 6361 7365 7320 7768 6572 6520 7765 2068  cases where we h
+00016500: 6176 6520 6120 6765 6e65 7269 6320 636f  ave a generic co
+00016510: 6465 2076 6172 6961 626c 6520 6572 726f  de variable erro
+00016520: 7220 6b65 790a 2020 2020 2020 2020 2020  r key.          
+00016530: 2020 2320 7b22 636f 6465 223a 302c 226d    # {"code":0,"m
+00016540: 6573 7361 6765 223a 2256 616c 6964 6174  essage":"Validat
+00016550: 696f 6e20 6661 696c 6564 222c 2265 7272  ion failed","err
+00016560: 6f72 7322 3a7b 2261 6d6f 756e 7422 3a5b  ors":{"amount":[
+00016570: 2241 6d6f 756e 7420 6d75 7374 2062 6520  "Amount must be 
+00016580: 6772 6561 7465 7220 7468 616e 2030 225d  greater than 0"]
+00016590: 7d7d 0a20 2020 2020 2020 2020 2020 2063  }}.            c
+000165a0: 6f64 654e 6577 203d 2073 656c 662e 7361  odeNew = self.sa
+000165b0: 6665 5f69 6e74 6567 6572 2872 6573 706f  fe_integer(respo
+000165c0: 6e73 652c 2027 636f 6465 2729 0a20 2020  nse, 'code').   
+000165d0: 2020 2020 2020 2020 2068 6173 4572 726f           hasErro
+000165e0: 7253 7461 7475 7320 3d20 7374 6174 7573  rStatus = status
+000165f0: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
+00016600: 2073 7461 7475 7320 213d 2027 3230 3027   status != '200'
+00016610: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00016620: 6861 7345 7272 6f72 5374 6174 7573 206f  hasErrorStatus o
+00016630: 7220 636f 6465 4e65 7720 6973 206e 6f74  r codeNew is not
+00016640: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00016650: 2020 2020 2020 2066 6565 6462 6163 6b20         feedback 
+00016660: 3d20 7365 6c66 2e69 6420 2b20 2720 2720  = self.id + ' ' 
+00016670: 2b20 626f 6479 0a20 2020 2020 2020 2020  + body.         
+00016680: 2020 2020 2020 2065 7272 6f72 496e 666f         errorInfo
+00016690: 203d 206d 6573 7361 6765 0a20 2020 2020   = message.     
+000166a0: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
+000166b0: 7345 7272 6f72 5374 6174 7573 3a0a 2020  sErrorStatus:.  
+000166c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166d0: 2020 6572 726f 7249 6e66 6f20 3d20 7374    errorInfo = st
+000166e0: 6174 7573 0a20 2020 2020 2020 2020 2020  atus.           
+000166f0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00016700: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00016710: 7272 6f72 4f62 6a65 6374 203d 2073 656c  rrorObject = sel
+00016720: 662e 7361 6665 5f76 616c 7565 2872 6573  f.safe_value(res
+00016730: 706f 6e73 652c 2027 6572 726f 7273 2729  ponse, 'errors')
+00016740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016750: 2020 2020 2069 6620 6572 726f 724f 626a       if errorObj
+00016760: 6563 7420 6973 206e 6f74 204e 6f6e 653a  ect is not None:
+00016770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016780: 2020 2020 2020 2020 2065 7272 6f72 4b65           errorKe
+00016790: 7920 3d20 6c69 7374 2865 7272 6f72 4f62  y = list(errorOb
+000167a0: 6a65 6374 2e6b 6579 7328 2929 5b30 5d0a  ject.keys())[0].
+000167b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167c0: 2020 2020 2020 2020 6572 726f 724d 6573          errorMes
+000167d0: 7361 6765 4172 7261 7920 3d20 7365 6c66  sageArray = self
+000167e0: 2e73 6166 655f 7661 6c75 6528 6572 726f  .safe_value(erro
+000167f0: 724f 626a 6563 742c 2065 7272 6f72 4b65  rObject, errorKe
+00016800: 792c 205b 5d29 0a20 2020 2020 2020 2020  y, []).         
+00016810: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00016820: 7272 6f72 4d65 7373 6167 654c 656e 6774  rrorMessageLengt
+00016830: 6820 3d20 6c65 6e28 6572 726f 724d 6573  h = len(errorMes
+00016840: 7361 6765 4172 7261 7929 0a20 2020 2020  sageArray).     
+00016850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016860: 2020 2065 7272 6f72 496e 666f 203d 2065     errorInfo = e
+00016870: 7272 6f72 4d65 7373 6167 6541 7272 6179  rrorMessageArray
+00016880: 5b30 5d20 6966 2028 6572 726f 724d 6573  [0] if (errorMes
+00016890: 7361 6765 4c65 6e67 7468 203e 2030 2920  sageLength > 0) 
+000168a0: 656c 7365 2062 6f64 790a 2020 2020 2020  else body.      
+000168b0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+000168c0: 6872 6f77 5f65 7861 6374 6c79 5f6d 6174  hrow_exactly_mat
+000168d0: 6368 6564 5f65 7863 6570 7469 6f6e 2873  ched_exception(s
+000168e0: 656c 662e 6578 6365 7074 696f 6e73 5b27  elf.exceptions['
+000168f0: 6578 6163 7427 5d2c 2065 7272 6f72 496e  exact'], errorIn
+00016900: 666f 2c20 6665 6564 6261 636b 290a 2020  fo, feedback).  
+00016910: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00016920: 6c66 2e74 6872 6f77 5f62 726f 6164 6c79  lf.throw_broadly
+00016930: 5f6d 6174 6368 6564 5f65 7863 6570 7469  _matched_excepti
+00016940: 6f6e 2873 656c 662e 6578 6365 7074 696f  on(self.exceptio
+00016950: 6e73 5b27 6272 6f61 6427 5d2c 2062 6f64  ns['broad'], bod
+00016960: 792c 2066 6565 6462 6163 6b29 0a20 2020  y, feedback).   
+00016970: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00016980: 7365 2045 7863 6861 6e67 6545 7272 6f72  se ExchangeError
+00016990: 2866 6565 6462 6163 6b29 0a20 2020 2020  (feedback).     
+000169a0: 2020 2072 6574 7572 6e20 4e6f 6e65 0a       return None.
```

### Comparing `ccxt-3.0.93/ccxt/async_support/woo.py` & `ccxt-3.0.94/ccxt/async_support/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/xt.py` & `ccxt-3.0.94/ccxt/async_support/xt.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/yobit.py` & `ccxt-3.0.94/ccxt/async_support/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/zaif.py` & `ccxt-3.0.94/ccxt/async_support/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/zb.py` & `ccxt-3.0.94/ccxt/async_support/zb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/async_support/zonda.py` & `ccxt-3.0.94/ccxt/async_support/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/base/__init__.py` & `ccxt-3.0.94/ccxt/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/base/decimal_to_precision.py` & `ccxt-3.0.94/ccxt/base/decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/base/errors.py` & `ccxt-3.0.94/ccxt/base/errors.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/base/exchange.py` & `ccxt-3.0.94/ccxt/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Base exchange class"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '3.0.93'
+__version__ = '3.0.94'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.base.errors import ExchangeError
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import AuthenticationError
```

### Comparing `ccxt-3.0.93/ccxt/base/precise.py` & `ccxt-3.0.94/ccxt/base/precise.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/base/types.py` & `ccxt-3.0.94/ccxt/base/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bequant.py` & `ccxt-3.0.94/ccxt/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bigone.py` & `ccxt-3.0.94/ccxt/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/binance.py` & `ccxt-3.0.94/ccxt/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/binancecoinm.py` & `ccxt-3.0.94/ccxt/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/binanceus.py` & `ccxt-3.0.94/ccxt/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/binanceusdm.py` & `ccxt-3.0.94/ccxt/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bit2c.py` & `ccxt-3.0.94/ccxt/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitbank.py` & `ccxt-3.0.94/ccxt/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitbns.py` & `ccxt-3.0.94/ccxt/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitfinex.py` & `ccxt-3.0.94/ccxt/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitfinex2.py` & `ccxt-3.0.94/ccxt/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitflyer.py` & `ccxt-3.0.94/ccxt/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitforex.py` & `ccxt-3.0.94/ccxt/bitforex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitget.py` & `ccxt-3.0.94/ccxt/bitget.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,28 +111,26 @@
                 'setLeverage': True,
                 'setMarginMode': True,
                 'setPositionMode': True,
                 'transfer': True,
                 'withdraw': False,
             },
             'timeframes': {
-                '1m': '1m',
-                '3m': '3m',
-                '5m': '5m',
-                '15m': '15m',
-                '30m': '30m',
+                '1m': '1min',
+                '5m': '5min',
+                '15m': '15min',
+                '30m': '30min',
                 '1h': '1h',
-                '2h': '2h',
                 '4h': '4h',
-                '6h': '6h',
-                '12h': '12h',
-                '1d': '1d',
-                '3d': '3d',
-                '1w': '1w',
-                '1M': '1M',
+                '6h': '6Hutc',
+                '12h': '12Hutc',
+                '1d': '1Dutc',
+                '3d': '3Dutc',
+                '1w': '1Wutc',
+                '1M': '1Mutc',
             },
             'hostname': 'bitget.com',
             'urls': {
                 'logo': 'https://user-images.githubusercontent.com/1294454/195989417-4253ddb0-afbe-4a1c-9dea-9dbcd121fa5d.jpg',
                 'api': {
                     'spot': 'https://api.{hostname}',
                     'mix': 'https://api.{hostname}',
@@ -820,18 +818,18 @@
             'precisionMode': TICK_SIZE,
             'commonCurrencies': {
                 'JADE': 'Jade Protocol',
             },
             'options': {
                 'timeframes': {
                     'spot': {
-                        '1m': '1m',
-                        '5m': '5m',
-                        '15m': '15m',
-                        '30m': '30m',
+                        '1m': '1min',
+                        '5m': '5min',
+                        '15m': '15min',
+                        '30m': '30min',
                         '1h': '1h',
                         '4h': '4h',
                         '6h': '6Hutc',
                         '12h': '12Hutc',
                         '1d': '1Dutc',
                         '3d': '3Dutc',
                         '1w': '1Wutc',
@@ -2076,14 +2074,15 @@
             self.safe_number_2(ohlcv, 5, 'baseVol'),
         ]
 
     def fetch_ohlcv(self, symbol: str, timeframe='1m', since: Optional[int] = None, limit: Optional[int] = None, params={}):
         """
         fetches historical candlestick data containing the open, high, low, and close price, and the volume of a market
         see https://bitgetlimited.github.io/apidoc/en/mix/#get-candle-data
+        see https://bitgetlimited.github.io/apidoc/en/spot/#candlestick-line-timeframe
         :param str symbol: unified symbol of the market to fetch OHLCV data for
         :param str timeframe: the length of time each candle represents
         :param int|None since: timestamp in ms of the earliest candle to fetch
         :param int|None limit: the maximum amount of candles to fetch
         :param dict params: extra parameters specific to the bitget api endpoint
         :param int|None params['until']: timestamp in ms of the latest candle to fetch
         :returns [[int]]: A list of candles ordered, open, high, low, close, volume
@@ -2091,15 +2090,16 @@
         self.load_markets()
         market = self.market(symbol)
         request = {
             'symbol': market['id'],
         }
         until = self.safe_integer_2(params, 'until', 'till')
         if limit is None:
-            limit = 100
+            limit = 1000
+        request['limit'] = limit
         marketType = 'spot' if market['spot'] else 'swap'
         timeframes = self.options['timeframes'][marketType]
         selectedTimeframe = self.safe_string(timeframes, timeframe, timeframe)
         duration = self.parse_timeframe(timeframe)
         if market['spot']:
             request['period'] = selectedTimeframe
             request['limit'] = limit
@@ -2109,18 +2109,18 @@
                     request['before'] = self.sum(since, limit * duration * 1000)
             if until is not None:
                 request['before'] = until
         elif market['contract']:
             request['granularity'] = selectedTimeframe
             now = self.milliseconds()
             if since is None:
-                request['startTime'] = now - (limit - 1) * (duration * 1000)
+                request['startTime'] = now - limit * (duration * 1000)
                 request['endTime'] = now
             else:
-                request['startTime'] = self.sum(since, duration * 1000)
+                request['startTime'] = since
                 if until is not None:
                     request['endTime'] = until
                 else:
                     request['endTime'] = self.sum(since, limit * duration * 1000)
         ommitted = self.omit(params, ['until', 'till'])
         extended = self.extend(request, ommitted)
         response = None
```

### Comparing `ccxt-3.0.93/ccxt/bithumb.py` & `ccxt-3.0.94/ccxt/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitmart.py` & `ccxt-3.0.94/ccxt/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitmex.py` & `ccxt-3.0.94/ccxt/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitopro.py` & `ccxt-3.0.94/ccxt/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitpanda.py` & `ccxt-3.0.94/ccxt/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitrue.py` & `ccxt-3.0.94/ccxt/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitso.py` & `ccxt-3.0.94/ccxt/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitstamp.py` & `ccxt-3.0.94/ccxt/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitstamp1.py` & `ccxt-3.0.94/ccxt/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bittrex.py` & `ccxt-3.0.94/ccxt/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bitvavo.py` & `ccxt-3.0.94/ccxt/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bkex.py` & `ccxt-3.0.94/ccxt/bkex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bl3p.py` & `ccxt-3.0.94/ccxt/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/blockchaincom.py` & `ccxt-3.0.94/ccxt/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/btcalpha.py` & `ccxt-3.0.94/ccxt/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/btcbox.py` & `ccxt-3.0.94/ccxt/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/btcex.py` & `ccxt-3.0.94/ccxt/btcex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/btcmarkets.py` & `ccxt-3.0.94/ccxt/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/btctradeua.py` & `ccxt-3.0.94/ccxt/btctradeua.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/btcturk.py` & `ccxt-3.0.94/ccxt/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/buda.py` & `ccxt-3.0.94/ccxt/buda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/bybit.py` & `ccxt-3.0.94/ccxt/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/cex.py` & `ccxt-3.0.94/ccxt/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/coinbase.py` & `ccxt-3.0.94/ccxt/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/coinbaseprime.py` & `ccxt-3.0.94/ccxt/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/coinbasepro.py` & `ccxt-3.0.94/ccxt/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/coincheck.py` & `ccxt-3.0.94/ccxt/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/coinex.py` & `ccxt-3.0.94/ccxt/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/coinfalcon.py` & `ccxt-3.0.94/ccxt/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/coinmate.py` & `ccxt-3.0.94/ccxt/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/coinone.py` & `ccxt-3.0.94/ccxt/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/coinsph.py` & `ccxt-3.0.94/ccxt/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/coinspot.py` & `ccxt-3.0.94/ccxt/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/cryptocom.py` & `ccxt-3.0.94/ccxt/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/currencycom.py` & `ccxt-3.0.94/ccxt/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/delta.py` & `ccxt-3.0.94/ccxt/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/deribit.py` & `ccxt-3.0.94/ccxt/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/digifinex.py` & `ccxt-3.0.94/ccxt/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/exmo.py` & `ccxt-3.0.94/ccxt/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/flowbtc.py` & `ccxt-3.0.94/ccxt/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/fmfwio.py` & `ccxt-3.0.94/ccxt/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/gate.py` & `ccxt-3.0.94/ccxt/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/gemini.py` & `ccxt-3.0.94/ccxt/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/hitbtc.py` & `ccxt-3.0.94/ccxt/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/hitbtc3.py` & `ccxt-3.0.94/ccxt/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/hollaex.py` & `ccxt-3.0.94/ccxt/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/huobi.py` & `ccxt-3.0.94/ccxt/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/huobijp.py` & `ccxt-3.0.94/ccxt/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/huobipro.py` & `ccxt-3.0.94/ccxt/huobipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/idex.py` & `ccxt-3.0.94/ccxt/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/independentreserve.py` & `ccxt-3.0.94/ccxt/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/indodax.py` & `ccxt-3.0.94/ccxt/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/itbit.py` & `ccxt-3.0.94/ccxt/itbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/kraken.py` & `ccxt-3.0.94/ccxt/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/krakenfutures.py` & `ccxt-3.0.94/ccxt/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/kucoin.py` & `ccxt-3.0.94/ccxt/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/kucoinfutures.py` & `ccxt-3.0.94/ccxt/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/kuna.py` & `ccxt-3.0.94/ccxt/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/latoken.py` & `ccxt-3.0.94/ccxt/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/lbank.py` & `ccxt-3.0.94/ccxt/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/lbank2.py` & `ccxt-3.0.94/ccxt/lbank2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/luno.py` & `ccxt-3.0.94/ccxt/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/lykke.py` & `ccxt-3.0.94/ccxt/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/mercado.py` & `ccxt-3.0.94/ccxt/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/mexc.py` & `ccxt-3.0.94/ccxt/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/ndax.py` & `ccxt-3.0.94/ccxt/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/novadax.py` & `ccxt-3.0.94/ccxt/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/oceanex.py` & `ccxt-3.0.94/ccxt/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/okcoin.py` & `ccxt-3.0.94/ccxt/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/okx.py` & `ccxt-3.0.94/ccxt/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/paymium.py` & `ccxt-3.0.94/ccxt/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/phemex.py` & `ccxt-3.0.94/ccxt/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/poloniex.py` & `ccxt-3.0.94/ccxt/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/poloniexfutures.py` & `ccxt-3.0.94/ccxt/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/__init__.py` & `ccxt-3.0.94/ccxt/pro/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # ----------------------------------------------------------------------------
 
-__version__ = '3.0.93'
+__version__ = '3.0.94'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.base.exchange import Exchange  # noqa: F401
 
 # CCXT Pro exchanges (now this is mainly used for importing exchanges in WS tests)
```

### Comparing `ccxt-3.0.93/ccxt/pro/alpaca.py` & `ccxt-3.0.94/ccxt/pro/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/ascendex.py` & `ccxt-3.0.94/ccxt/pro/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/bequant.py` & `ccxt-3.0.94/ccxt/pro/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/binance.py` & `ccxt-3.0.94/ccxt/pro/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/binancecoinm.py` & `ccxt-3.0.94/ccxt/pro/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/binanceus.py` & `ccxt-3.0.94/ccxt/pro/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/binanceusdm.py` & `ccxt-3.0.94/ccxt/pro/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/bitcoincom.py` & `ccxt-3.0.94/ccxt/pro/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/bitfinex.py` & `ccxt-3.0.94/ccxt/pro/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/bitfinex2.py` & `ccxt-3.0.94/ccxt/pro/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/bitget.py` & `ccxt-3.0.94/ccxt/pro/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/bitmart.py` & `ccxt-3.0.94/ccxt/pro/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/bitmex.py` & `ccxt-3.0.94/ccxt/pro/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/bitopro.py` & `ccxt-3.0.94/ccxt/pro/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/bitrue.py` & `ccxt-3.0.94/ccxt/pro/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/bitstamp.py` & `ccxt-3.0.94/ccxt/pro/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/bittrex.py` & `ccxt-3.0.94/ccxt/pro/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/bitvavo.py` & `ccxt-3.0.94/ccxt/pro/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/btcex.py` & `ccxt-3.0.94/ccxt/pro/btcex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/bybit.py` & `ccxt-3.0.94/ccxt/pro/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/cex.py` & `ccxt-3.0.94/ccxt/pro/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/coinbaseprime.py` & `ccxt-3.0.94/ccxt/pro/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/coinbasepro.py` & `ccxt-3.0.94/ccxt/pro/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/coinex.py` & `ccxt-3.0.94/ccxt/pro/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/cryptocom.py` & `ccxt-3.0.94/ccxt/pro/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/currencycom.py` & `ccxt-3.0.94/ccxt/pro/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/deribit.py` & `ccxt-3.0.94/ccxt/pro/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/exmo.py` & `ccxt-3.0.94/ccxt/pro/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/gate.py` & `ccxt-3.0.94/ccxt/pro/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/gemini.py` & `ccxt-3.0.94/ccxt/pro/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/hitbtc.py` & `ccxt-3.0.94/ccxt/pro/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/hollaex.py` & `ccxt-3.0.94/ccxt/pro/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/huobi.py` & `ccxt-3.0.94/ccxt/pro/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/huobijp.py` & `ccxt-3.0.94/ccxt/pro/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/idex.py` & `ccxt-3.0.94/ccxt/pro/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/independentreserve.py` & `ccxt-3.0.94/ccxt/pro/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/kraken.py` & `ccxt-3.0.94/ccxt/pro/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/krakenfutures.py` & `ccxt-3.0.94/ccxt/pro/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/kucoin.py` & `ccxt-3.0.94/ccxt/pro/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/kucoinfutures.py` & `ccxt-3.0.94/ccxt/pro/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/luno.py` & `ccxt-3.0.94/ccxt/pro/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/mexc.py` & `ccxt-3.0.94/ccxt/pro/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/ndax.py` & `ccxt-3.0.94/ccxt/pro/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/okcoin.py` & `ccxt-3.0.94/ccxt/pro/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/okx.py` & `ccxt-3.0.94/ccxt/pro/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/phemex.py` & `ccxt-3.0.94/ccxt/pro/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/probit.py` & `ccxt-3.0.94/ccxt/pro/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/ripio.py` & `ccxt-3.0.94/ccxt/pro/ripio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/upbit.py` & `ccxt-3.0.94/ccxt/pro/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/wazirx.py` & `ccxt-3.0.94/ccxt/pro/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/whitebit.py` & `ccxt-3.0.94/ccxt/pro/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/woo.py` & `ccxt-3.0.94/ccxt/pro/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/pro/zb.py` & `ccxt-3.0.94/ccxt/pro/zb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/probit.py` & `ccxt-3.0.94/ccxt/probit.py`

 * *Files 4% similar despite different names*

```diff
@@ -421,15 +421,52 @@
             currency = currencies[i]
             id = self.safe_string(currency, 'id')
             code = self.safe_currency_code(id)
             displayName = self.safe_value(currency, 'display_name')
             name = self.safe_string(displayName, 'en-us')
             platforms = self.safe_value(currency, 'platform', [])
             platformsByPriority = self.sort_by(platforms, 'priority')
-            platform = self.safe_value(platformsByPriority, 0, {})
+            platform = None
+            networkList = {}
+            for j in range(0, len(platformsByPriority)):
+                network = platformsByPriority[j]
+                id = self.safe_string(network, 'id')
+                networkCode = self.network_id_to_code(id)
+                currentDepositSuspended = self.safe_value(network, 'deposit_suspended')
+                currentWithdrawalSuspended = self.safe_value(network, 'withdrawal_suspended')
+                currentDeposit = not currentDepositSuspended
+                currentWithdraw = not currentWithdrawalSuspended
+                currentActive = currentDeposit and currentWithdraw
+                if currentActive:
+                    platform = network
+                precision = self.safe_string(network, 'precision')
+                withdrawFee = self.safe_value(network, 'withdrawal_fee', [])
+                fee = self.safe_value(withdrawFee, 0, {})
+                networkList[networkCode] = {
+                    'id': id,
+                    'network': networkCode,
+                    'active': currentActive,
+                    'deposit': currentDeposit,
+                    'withdraw': currentWithdraw,
+                    'fee': self.safe_number(fee, 'amount'),
+                    'precision': self.parse_number(precision),
+                    'limits': {
+                        'withdraw': {
+                            'min': self.safe_number(network, 'min_withdrawal_amount'),
+                            'max': None,
+                        },
+                        'deposit': {
+                            'min': self.safe_number(network, 'min_deposit_amount'),
+                            'max': None,
+                        },
+                    },
+                    'info': network,
+                }
+            if platform is None:
+                platform = self.safe_value(platformsByPriority, 0, {})
             depositSuspended = self.safe_value(platform, 'deposit_suspended')
             withdrawalSuspended = self.safe_value(platform, 'withdrawal_suspended')
             deposit = not depositSuspended
             withdraw = not withdrawalSuspended
             active = deposit and withdraw
             withdrawalFees = self.safe_value(platform, 'withdrawal_fee', {})
             fees = []
@@ -464,15 +501,15 @@
                         'max': None,
                     },
                     'withdraw': {
                         'min': self.safe_number(platform, 'min_withdrawal_amount'),
                         'max': None,
                     },
                 },
-                'networks': {},
+                'networks': networkList,
             }
         return result
 
     def parse_balance(self, response):
         result = {
             'info': response,
             'timestamp': None,
```

### Comparing `ccxt-3.0.93/ccxt/ripio.py` & `ccxt-3.0.94/ccxt/ripio.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/static_dependencies/ecdsa/__init__.py` & `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/static_dependencies/ecdsa/_version.py` & `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/static_dependencies/ecdsa/curves.py` & `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/curves.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/static_dependencies/ecdsa/der.py` & `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/der.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/static_dependencies/ecdsa/ecdsa.py` & `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/ecdsa.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/static_dependencies/ecdsa/ellipticcurve.py` & `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/ellipticcurve.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/static_dependencies/ecdsa/keys.py` & `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/keys.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/static_dependencies/ecdsa/numbertheory.py` & `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/numbertheory.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/static_dependencies/ecdsa/rfc6979.py` & `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/rfc6979.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/static_dependencies/ecdsa/util.py` & `ccxt-3.0.94/ccxt/static_dependencies/ecdsa/util.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/static_dependencies/keccak/keccak.py` & `ccxt-3.0.94/ccxt/static_dependencies/keccak/keccak.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/stex.py` & `ccxt-3.0.94/ccxt/stex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/__init__.py` & `ccxt-3.0.94/ccxt/test/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_account.py` & `ccxt-3.0.94/ccxt/test/base/test_account.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_balance.py` & `ccxt-3.0.94/ccxt/test/base/test_balance.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_borrow_interest.py` & `ccxt-3.0.94/ccxt/test/base/test_borrow_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_borrow_rate.py` & `ccxt-3.0.94/ccxt/test/base/test_borrow_rate.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_calculate_fee.py` & `ccxt-3.0.94/ccxt/test/base/test_calculate_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_crypto.py` & `ccxt-3.0.94/ccxt/test/base/test_crypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_currency.py` & `ccxt-3.0.94/ccxt/test/base/test_currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_datetime.py` & `ccxt-3.0.94/ccxt/test/base/test_datetime.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_decimal_to_precision.py` & `ccxt-3.0.94/ccxt/test/base/test_decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_deep_extend.py` & `ccxt-3.0.94/ccxt/test/base/test_deep_extend.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_deposit_withdrawal.py` & `ccxt-3.0.94/ccxt/test/base/test_deposit_withdrawal.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_exchange_datetime_functions.py` & `ccxt-3.0.94/ccxt/test/base/test_exchange_datetime_functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_funding_rate_history.py` & `ccxt-3.0.94/ccxt/test/base/test_funding_rate_history.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_ledger_entry.py` & `ccxt-3.0.94/ccxt/test/base/test_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_ledger_item.py` & `ccxt-3.0.94/ccxt/test/base/test_ledger_item.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_leverage_tier.py` & `ccxt-3.0.94/ccxt/test/base/test_leverage_tier.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_margin_modification.py` & `ccxt-3.0.94/ccxt/test/base/test_margin_modification.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_market.py` & `ccxt-3.0.94/ccxt/test/base/test_market.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_number.py` & `ccxt-3.0.94/ccxt/test/base/test_number.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_ohlcv.py` & `ccxt-3.0.94/ccxt/test/base/test_ohlcv.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_open_interest.py` & `ccxt-3.0.94/ccxt/test/base/test_open_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_order.py` & `ccxt-3.0.94/ccxt/test/base/test_order.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_order_book.py` & `ccxt-3.0.94/ccxt/test/base/test_order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_position.py` & `ccxt-3.0.94/ccxt/test/base/test_position.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_shared_methods.py` & `ccxt-3.0.94/ccxt/test/base/test_shared_methods.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_status.py` & `ccxt-3.0.94/ccxt/test/base/test_status.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_throttle.py` & `ccxt-3.0.94/ccxt/test/base/test_throttle.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_ticker.py` & `ccxt-3.0.94/ccxt/test/base/test_ticker.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_trade.py` & `ccxt-3.0.94/ccxt/test/base/test_trade.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_trading_fee.py` & `ccxt-3.0.94/ccxt/test/base/test_trading_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/base/test_transaction.py` & `ccxt-3.0.94/ccxt/test/base/test_transaction.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/test_async.py` & `ccxt-3.0.94/ccxt/test/test_async.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/test/test_sync.py` & `ccxt-3.0.94/ccxt/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/tidex.py` & `ccxt-3.0.94/ccxt/tidex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/timex.py` & `ccxt-3.0.94/ccxt/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/tokocrypto.py` & `ccxt-3.0.94/ccxt/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/upbit.py` & `ccxt-3.0.94/ccxt/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/wavesexchange.py` & `ccxt-3.0.94/ccxt/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/wazirx.py` & `ccxt-3.0.94/ccxt/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/whitebit.py` & `ccxt-3.0.94/ccxt/whitebit.py`

 * *Files 0% similar despite different names*

```diff
@@ -5600,159 +5600,160 @@
 00015df0: 7265 7175 6573 742c 2027 6e6f 6e63 6527  request, 'nonce'
 00015e00: 3a20 6e6f 6e63 657d 2c20 7061 7261 6d73  : nonce}, params
 00015e10: 2929 0a20 2020 2020 2020 2020 2020 2070  )).            p
 00015e20: 6179 6c6f 6164 203d 2073 656c 662e 7374  ayload = self.st
 00015e30: 7269 6e67 5f74 6f5f 6261 7365 3634 2862  ring_to_base64(b
 00015e40: 6f64 7929 0a20 2020 2020 2020 2020 2020  ody).           
 00015e50: 2073 6967 6e61 7475 7265 203d 2073 656c   signature = sel
-00015e60: 662e 686d 6163 2870 6179 6c6f 6164 2c20  f.hmac(payload, 
-00015e70: 7365 6372 6574 2c20 6861 7368 6c69 622e  secret, hashlib.
-00015e80: 7368 6135 3132 290a 2020 2020 2020 2020  sha512).        
-00015e90: 2020 2020 6865 6164 6572 7320 3d20 7b0a      headers = {.
-00015ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015eb0: 2743 6f6e 7465 6e74 2d54 7970 6527 3a20  'Content-Type': 
-00015ec0: 2761 7070 6c69 6361 7469 6f6e 2f6a 736f  'application/jso
-00015ed0: 6e27 2c0a 2020 2020 2020 2020 2020 2020  n',.            
-00015ee0: 2020 2020 2758 2d54 5843 2d41 5049 4b45      'X-TXC-APIKE
-00015ef0: 5927 3a20 7365 6c66 2e61 7069 4b65 792c  Y': self.apiKey,
-00015f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015f10: 2027 582d 5458 432d 5041 594c 4f41 4427   'X-TXC-PAYLOAD'
-00015f20: 3a20 7061 796c 6f61 642c 0a20 2020 2020  : payload,.     
-00015f30: 2020 2020 2020 2020 2020 2027 582d 5458             'X-TX
-00015f40: 432d 5349 474e 4154 5552 4527 3a20 7369  C-SIGNATURE': si
-00015f50: 676e 6174 7572 652c 0a20 2020 2020 2020  gnature,.       
-00015f60: 2020 2020 207d 0a20 2020 2020 2020 2072       }.        r
-00015f70: 6574 7572 6e20 7b27 7572 6c27 3a20 7572  eturn {'url': ur
-00015f80: 6c2c 2027 6d65 7468 6f64 273a 206d 6574  l, 'method': met
-00015f90: 686f 642c 2027 626f 6479 273a 2062 6f64  hod, 'body': bod
-00015fa0: 792c 2027 6865 6164 6572 7327 3a20 6865  y, 'headers': he
-00015fb0: 6164 6572 737d 0a0a 2020 2020 6465 6620  aders}..    def 
-00015fc0: 6861 6e64 6c65 5f65 7272 6f72 7328 7365  handle_errors(se
-00015fd0: 6c66 2c20 636f 6465 2c20 7265 6173 6f6e  lf, code, reason
-00015fe0: 2c20 7572 6c2c 206d 6574 686f 642c 2068  , url, method, h
-00015ff0: 6561 6465 7273 2c20 626f 6479 2c20 7265  eaders, body, re
-00016000: 7370 6f6e 7365 2c20 7265 7175 6573 7448  sponse, requestH
-00016010: 6561 6465 7273 2c20 7265 7175 6573 7442  eaders, requestB
-00016020: 6f64 7929 3a0a 2020 2020 2020 2020 6966  ody):.        if
-00016030: 2028 636f 6465 203d 3d20 3431 3829 206f   (code == 418) o
-00016040: 7220 2863 6f64 6520 3d3d 2034 3239 293a  r (code == 429):
-00016050: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00016060: 7365 2044 446f 5350 726f 7465 6374 696f  se DDoSProtectio
-00016070: 6e28 7365 6c66 2e69 6420 2b20 2720 2720  n(self.id + ' ' 
-00016080: 2b20 7374 7228 636f 6465 2920 2b20 2720  + str(code) + ' 
-00016090: 2720 2b20 7265 6173 6f6e 202b 2027 2027  ' + reason + ' '
-000160a0: 202b 2062 6f64 7929 0a20 2020 2020 2020   + body).       
-000160b0: 2069 6620 636f 6465 203d 3d20 3430 343a   if code == 404:
-000160c0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000160d0: 7365 2045 7863 6861 6e67 6545 7272 6f72  se ExchangeError
-000160e0: 2873 656c 662e 6964 202b 2027 2027 202b  (self.id + ' ' +
-000160f0: 2073 7472 2863 6f64 6529 202b 2027 2065   str(code) + ' e
-00016100: 6e64 706f 696e 7420 6e6f 7420 666f 756e  ndpoint not foun
-00016110: 6427 290a 2020 2020 2020 2020 6966 2072  d').        if r
-00016120: 6573 706f 6e73 6520 6973 206e 6f74 204e  esponse is not N
-00016130: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00016140: 2023 2046 6f72 2063 6173 6573 2077 6865   # For cases whe
-00016150: 7265 2077 6520 6861 7665 2061 206d 6561  re we have a mea
-00016160: 6e69 6e67 6675 6c20 7374 6174 7573 0a20  ningful status. 
-00016170: 2020 2020 2020 2020 2020 2023 207b 2272             # {"r
-00016180: 6573 706f 6e73 6522 3a6e 756c 6c2c 2273  esponse":null,"s
-00016190: 7461 7475 7322 3a34 3232 2c22 6572 726f  tatus":422,"erro
-000161a0: 7273 223a 7b22 6f72 6465 7249 6422 3a5b  rs":{"orderId":[
-000161b0: 2246 696e 6973 6865 6420 6f72 6465 7220  "Finished order 
-000161c0: 6964 2034 3335 3435 3334 3534 3533 3520  id 435453454535 
-000161d0: 6e6f 7420 666f 756e 6420 6f6e 2079 6f75  not found on you
-000161e0: 7220 6163 636f 756e 7422 5d7d 2c22 6e6f  r account"]},"no
-000161f0: 7469 6669 6361 7469 6f6e 223a 6e75 6c6c  tification":null
-00016200: 2c22 7761 726e 696e 6722 3a22 4669 6e69  ,"warning":"Fini
-00016210: 7368 6564 206f 7264 6572 2069 6420 3433  shed order id 43
-00016220: 3534 3533 3435 3435 3335 206e 6f74 2066  5453454535 not f
-00016230: 6f75 6e64 206f 6e20 796f 7572 2061 6363  ound on your acc
-00016240: 6f75 6e74 222c 225f 746f 6b65 6e22 3a6e  ount","_token":n
-00016250: 756c 6c7d 0a20 2020 2020 2020 2020 2020  ull}.           
-00016260: 2073 7461 7475 7320 3d20 7365 6c66 2e73   status = self.s
-00016270: 6166 655f 7374 7269 6e67 2872 6573 706f  afe_string(respo
-00016280: 6e73 652c 2027 7374 6174 7573 2729 0a20  nse, 'status'). 
-00016290: 2020 2020 2020 2020 2020 2023 207b 2263             # {"c
-000162a0: 6f64 6522 3a31 302c 226d 6573 7361 6765  ode":10,"message
-000162b0: 223a 2255 6e61 7574 686f 7269 7a65 6420  ":"Unauthorized 
-000162c0: 7265 7175 6573 742e 227d 0a20 2020 2020  request."}.     
-000162d0: 2020 2020 2020 206d 6573 7361 6765 203d         message =
-000162e0: 2073 656c 662e 7361 6665 5f73 7472 696e   self.safe_strin
-000162f0: 6728 7265 7370 6f6e 7365 2c20 276d 6573  g(response, 'mes
-00016300: 7361 6765 2729 0a20 2020 2020 2020 2020  sage').         
-00016310: 2020 2023 2046 6f72 2074 6865 7365 2063     # For these c
-00016320: 6173 6573 2077 6865 7265 2077 6520 6861  ases where we ha
-00016330: 7665 2061 2067 656e 6572 6963 2063 6f64  ve a generic cod
-00016340: 6520 7661 7269 6162 6c65 2065 7272 6f72  e variable error
-00016350: 206b 6579 0a20 2020 2020 2020 2020 2020   key.           
-00016360: 2023 207b 2263 6f64 6522 3a30 2c22 6d65   # {"code":0,"me
-00016370: 7373 6167 6522 3a22 5661 6c69 6461 7469  ssage":"Validati
-00016380: 6f6e 2066 6169 6c65 6422 2c22 6572 726f  on failed","erro
-00016390: 7273 223a 7b22 616d 6f75 6e74 223a 5b22  rs":{"amount":["
-000163a0: 416d 6f75 6e74 206d 7573 7420 6265 2067  Amount must be g
-000163b0: 7265 6174 6572 2074 6861 6e20 3022 5d7d  reater than 0"]}
-000163c0: 7d0a 2020 2020 2020 2020 2020 2020 636f  }.            co
-000163d0: 6465 4e65 7720 3d20 7365 6c66 2e73 6166  deNew = self.saf
-000163e0: 655f 696e 7465 6765 7228 7265 7370 6f6e  e_integer(respon
-000163f0: 7365 2c20 2763 6f64 6527 290a 2020 2020  se, 'code').    
-00016400: 2020 2020 2020 2020 6861 7345 7272 6f72          hasError
-00016410: 5374 6174 7573 203d 2073 7461 7475 7320  Status = status 
-00016420: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-00016430: 7374 6174 7573 2021 3d20 2732 3030 270a  status != '200'.
-00016440: 2020 2020 2020 2020 2020 2020 6966 2068              if h
-00016450: 6173 4572 726f 7253 7461 7475 7320 6f72  asErrorStatus or
-00016460: 2063 6f64 654e 6577 2069 7320 6e6f 7420   codeNew is not 
-00016470: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00016480: 2020 2020 2020 6665 6564 6261 636b 203d        feedback =
-00016490: 2073 656c 662e 6964 202b 2027 2027 202b   self.id + ' ' +
-000164a0: 2062 6f64 790a 2020 2020 2020 2020 2020   body.          
-000164b0: 2020 2020 2020 6572 726f 7249 6e66 6f20        errorInfo 
-000164c0: 3d20 6d65 7373 6167 650a 2020 2020 2020  = message.      
-000164d0: 2020 2020 2020 2020 2020 6966 2068 6173            if has
-000164e0: 4572 726f 7253 7461 7475 733a 0a20 2020  ErrorStatus:.   
-000164f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016500: 2065 7272 6f72 496e 666f 203d 2073 7461   errorInfo = sta
-00016510: 7475 730a 2020 2020 2020 2020 2020 2020  tus.            
-00016520: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00016530: 2020 2020 2020 2020 2020 2020 2020 6572                er
-00016540: 726f 724f 626a 6563 7420 3d20 7365 6c66  rorObject = self
-00016550: 2e73 6166 655f 7661 6c75 6528 7265 7370  .safe_value(resp
-00016560: 6f6e 7365 2c20 2765 7272 6f72 7327 290a  onse, 'errors').
-00016570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016580: 2020 2020 6966 2065 7272 6f72 4f62 6a65      if errorObje
-00016590: 6374 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ct is not None:.
-000165a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000165b0: 2020 2020 2020 2020 6572 726f 724b 6579          errorKey
-000165c0: 203d 206c 6973 7428 6572 726f 724f 626a   = list(errorObj
-000165d0: 6563 742e 6b65 7973 2829 295b 305d 0a20  ect.keys())[0]. 
-000165e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000165f0: 2020 2020 2020 2065 7272 6f72 4d65 7373         errorMess
-00016600: 6167 6541 7272 6179 203d 2073 656c 662e  ageArray = self.
-00016610: 7361 6665 5f76 616c 7565 2865 7272 6f72  safe_value(error
-00016620: 4f62 6a65 6374 2c20 6572 726f 724b 6579  Object, errorKey
-00016630: 2c20 5b5d 290a 2020 2020 2020 2020 2020  , []).          
-00016640: 2020 2020 2020 2020 2020 2020 2020 6572                er
-00016650: 726f 724d 6573 7361 6765 4c65 6e67 7468  rorMessageLength
-00016660: 203d 206c 656e 2865 7272 6f72 4d65 7373   = len(errorMess
-00016670: 6167 6541 7272 6179 290a 2020 2020 2020  ageArray).      
-00016680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016690: 2020 6572 726f 7249 6e66 6f20 3d20 6572    errorInfo = er
-000166a0: 726f 724d 6573 7361 6765 4172 7261 795b  rorMessageArray[
-000166b0: 305d 2069 6620 2865 7272 6f72 4d65 7373  0] if (errorMess
-000166c0: 6167 654c 656e 6774 6820 3e20 3029 2065  ageLength > 0) e
-000166d0: 6c73 6520 626f 6479 0a20 2020 2020 2020  lse body.       
-000166e0: 2020 2020 2020 2020 2073 656c 662e 7468           self.th
-000166f0: 726f 775f 6578 6163 746c 795f 6d61 7463  row_exactly_matc
-00016700: 6865 645f 6578 6365 7074 696f 6e28 7365  hed_exception(se
-00016710: 6c66 2e65 7863 6570 7469 6f6e 735b 2765  lf.exceptions['e
-00016720: 7861 6374 275d 2c20 6572 726f 7249 6e66  xact'], errorInf
-00016730: 6f2c 2066 6565 6462 6163 6b29 0a20 2020  o, feedback).   
-00016740: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00016750: 662e 7468 726f 775f 6272 6f61 646c 795f  f.throw_broadly_
-00016760: 6d61 7463 6865 645f 6578 6365 7074 696f  matched_exceptio
-00016770: 6e28 7365 6c66 2e65 7863 6570 7469 6f6e  n(self.exception
-00016780: 735b 2762 726f 6164 275d 2c20 626f 6479  s['broad'], body
-00016790: 2c20 6665 6564 6261 636b 290a 2020 2020  , feedback).    
-000167a0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000167b0: 6520 4578 6368 616e 6765 4572 726f 7228  e ExchangeError(
-000167c0: 6665 6564 6261 636b 290a 2020 2020 2020  feedback).      
-000167d0: 2020 7265 7475 726e 204e 6f6e 650a         return None.
+00015e60: 662e 686d 6163 2873 656c 662e 656e 636f  f.hmac(self.enco
+00015e70: 6465 2870 6179 6c6f 6164 292c 2073 6563  de(payload), sec
+00015e80: 7265 742c 2068 6173 686c 6962 2e73 6861  ret, hashlib.sha
+00015e90: 3531 3229 0a20 2020 2020 2020 2020 2020  512).           
+00015ea0: 2068 6561 6465 7273 203d 207b 0a20 2020   headers = {.   
+00015eb0: 2020 2020 2020 2020 2020 2020 2027 436f               'Co
+00015ec0: 6e74 656e 742d 5479 7065 273a 2027 6170  ntent-Type': 'ap
+00015ed0: 706c 6963 6174 696f 6e2f 6a73 6f6e 272c  plication/json',
+00015ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015ef0: 2027 582d 5458 432d 4150 494b 4559 273a   'X-TXC-APIKEY':
+00015f00: 2073 656c 662e 6170 694b 6579 2c0a 2020   self.apiKey,.  
+00015f10: 2020 2020 2020 2020 2020 2020 2020 2758                'X
+00015f20: 2d54 5843 2d50 4159 4c4f 4144 273a 2070  -TXC-PAYLOAD': p
+00015f30: 6179 6c6f 6164 2c0a 2020 2020 2020 2020  ayload,.        
+00015f40: 2020 2020 2020 2020 2758 2d54 5843 2d53          'X-TXC-S
+00015f50: 4947 4e41 5455 5245 273a 2073 6967 6e61  IGNATURE': signa
+00015f60: 7475 7265 2c0a 2020 2020 2020 2020 2020  ture,.          
+00015f70: 2020 7d0a 2020 2020 2020 2020 7265 7475    }.        retu
+00015f80: 726e 207b 2775 726c 273a 2075 726c 2c20  rn {'url': url, 
+00015f90: 276d 6574 686f 6427 3a20 6d65 7468 6f64  'method': method
+00015fa0: 2c20 2762 6f64 7927 3a20 626f 6479 2c20  , 'body': body, 
+00015fb0: 2768 6561 6465 7273 273a 2068 6561 6465  'headers': heade
+00015fc0: 7273 7d0a 0a20 2020 2064 6566 2068 616e  rs}..    def han
+00015fd0: 646c 655f 6572 726f 7273 2873 656c 662c  dle_errors(self,
+00015fe0: 2063 6f64 652c 2072 6561 736f 6e2c 2075   code, reason, u
+00015ff0: 726c 2c20 6d65 7468 6f64 2c20 6865 6164  rl, method, head
+00016000: 6572 732c 2062 6f64 792c 2072 6573 706f  ers, body, respo
+00016010: 6e73 652c 2072 6571 7565 7374 4865 6164  nse, requestHead
+00016020: 6572 732c 2072 6571 7565 7374 426f 6479  ers, requestBody
+00016030: 293a 0a20 2020 2020 2020 2069 6620 2863  ):.        if (c
+00016040: 6f64 6520 3d3d 2034 3138 2920 6f72 2028  ode == 418) or (
+00016050: 636f 6465 203d 3d20 3432 3929 3a0a 2020  code == 429):.  
+00016060: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00016070: 4444 6f53 5072 6f74 6563 7469 6f6e 2873  DDoSProtection(s
+00016080: 656c 662e 6964 202b 2027 2027 202b 2073  elf.id + ' ' + s
+00016090: 7472 2863 6f64 6529 202b 2027 2027 202b  tr(code) + ' ' +
+000160a0: 2072 6561 736f 6e20 2b20 2720 2720 2b20   reason + ' ' + 
+000160b0: 626f 6479 290a 2020 2020 2020 2020 6966  body).        if
+000160c0: 2063 6f64 6520 3d3d 2034 3034 3a0a 2020   code == 404:.  
+000160d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000160e0: 4578 6368 616e 6765 4572 726f 7228 7365  ExchangeError(se
+000160f0: 6c66 2e69 6420 2b20 2720 2720 2b20 7374  lf.id + ' ' + st
+00016100: 7228 636f 6465 2920 2b20 2720 656e 6470  r(code) + ' endp
+00016110: 6f69 6e74 206e 6f74 2066 6f75 6e64 2729  oint not found')
+00016120: 0a20 2020 2020 2020 2069 6620 7265 7370  .        if resp
+00016130: 6f6e 7365 2069 7320 6e6f 7420 4e6f 6e65  onse is not None
+00016140: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00016150: 466f 7220 6361 7365 7320 7768 6572 6520  For cases where 
+00016160: 7765 2068 6176 6520 6120 6d65 616e 696e  we have a meanin
+00016170: 6766 756c 2073 7461 7475 730a 2020 2020  gful status.    
+00016180: 2020 2020 2020 2020 2320 7b22 7265 7370          # {"resp
+00016190: 6f6e 7365 223a 6e75 6c6c 2c22 7374 6174  onse":null,"stat
+000161a0: 7573 223a 3432 322c 2265 7272 6f72 7322  us":422,"errors"
+000161b0: 3a7b 226f 7264 6572 4964 223a 5b22 4669  :{"orderId":["Fi
+000161c0: 6e69 7368 6564 206f 7264 6572 2069 6420  nished order id 
+000161d0: 3433 3534 3533 3435 3435 3335 206e 6f74  435453454535 not
+000161e0: 2066 6f75 6e64 206f 6e20 796f 7572 2061   found on your a
+000161f0: 6363 6f75 6e74 225d 7d2c 226e 6f74 6966  ccount"]},"notif
+00016200: 6963 6174 696f 6e22 3a6e 756c 6c2c 2277  ication":null,"w
+00016210: 6172 6e69 6e67 223a 2246 696e 6973 6865  arning":"Finishe
+00016220: 6420 6f72 6465 7220 6964 2034 3335 3435  d order id 43545
+00016230: 3334 3534 3533 3520 6e6f 7420 666f 756e  3454535 not foun
+00016240: 6420 6f6e 2079 6f75 7220 6163 636f 756e  d on your accoun
+00016250: 7422 2c22 5f74 6f6b 656e 223a 6e75 6c6c  t","_token":null
+00016260: 7d0a 2020 2020 2020 2020 2020 2020 7374  }.            st
+00016270: 6174 7573 203d 2073 656c 662e 7361 6665  atus = self.safe
+00016280: 5f73 7472 696e 6728 7265 7370 6f6e 7365  _string(response
+00016290: 2c20 2773 7461 7475 7327 290a 2020 2020  , 'status').    
+000162a0: 2020 2020 2020 2020 2320 7b22 636f 6465          # {"code
+000162b0: 223a 3130 2c22 6d65 7373 6167 6522 3a22  ":10,"message":"
+000162c0: 556e 6175 7468 6f72 697a 6564 2072 6571  Unauthorized req
+000162d0: 7565 7374 2e22 7d0a 2020 2020 2020 2020  uest."}.        
+000162e0: 2020 2020 6d65 7373 6167 6520 3d20 7365      message = se
+000162f0: 6c66 2e73 6166 655f 7374 7269 6e67 2872  lf.safe_string(r
+00016300: 6573 706f 6e73 652c 2027 6d65 7373 6167  esponse, 'messag
+00016310: 6527 290a 2020 2020 2020 2020 2020 2020  e').            
+00016320: 2320 466f 7220 7468 6573 6520 6361 7365  # For these case
+00016330: 7320 7768 6572 6520 7765 2068 6176 6520  s where we have 
+00016340: 6120 6765 6e65 7269 6320 636f 6465 2076  a generic code v
+00016350: 6172 6961 626c 6520 6572 726f 7220 6b65  ariable error ke
+00016360: 790a 2020 2020 2020 2020 2020 2020 2320  y.            # 
+00016370: 7b22 636f 6465 223a 302c 226d 6573 7361  {"code":0,"messa
+00016380: 6765 223a 2256 616c 6964 6174 696f 6e20  ge":"Validation 
+00016390: 6661 696c 6564 222c 2265 7272 6f72 7322  failed","errors"
+000163a0: 3a7b 2261 6d6f 756e 7422 3a5b 2241 6d6f  :{"amount":["Amo
+000163b0: 756e 7420 6d75 7374 2062 6520 6772 6561  unt must be grea
+000163c0: 7465 7220 7468 616e 2030 225d 7d7d 0a20  ter than 0"]}}. 
+000163d0: 2020 2020 2020 2020 2020 2063 6f64 654e             codeN
+000163e0: 6577 203d 2073 656c 662e 7361 6665 5f69  ew = self.safe_i
+000163f0: 6e74 6567 6572 2872 6573 706f 6e73 652c  nteger(response,
+00016400: 2027 636f 6465 2729 0a20 2020 2020 2020   'code').       
+00016410: 2020 2020 2068 6173 4572 726f 7253 7461       hasErrorSta
+00016420: 7475 7320 3d20 7374 6174 7573 2069 7320  tus = status is 
+00016430: 6e6f 7420 4e6f 6e65 2061 6e64 2073 7461  not None and sta
+00016440: 7475 7320 213d 2027 3230 3027 0a20 2020  tus != '200'.   
+00016450: 2020 2020 2020 2020 2069 6620 6861 7345           if hasE
+00016460: 7272 6f72 5374 6174 7573 206f 7220 636f  rrorStatus or co
+00016470: 6465 4e65 7720 6973 206e 6f74 204e 6f6e  deNew is not Non
+00016480: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00016490: 2020 2066 6565 6462 6163 6b20 3d20 7365     feedback = se
+000164a0: 6c66 2e69 6420 2b20 2720 2720 2b20 626f  lf.id + ' ' + bo
+000164b0: 6479 0a20 2020 2020 2020 2020 2020 2020  dy.             
+000164c0: 2020 2065 7272 6f72 496e 666f 203d 206d     errorInfo = m
+000164d0: 6573 7361 6765 0a20 2020 2020 2020 2020  essage.         
+000164e0: 2020 2020 2020 2069 6620 6861 7345 7272         if hasErr
+000164f0: 6f72 5374 6174 7573 3a0a 2020 2020 2020  orStatus:.      
+00016500: 2020 2020 2020 2020 2020 2020 2020 6572                er
+00016510: 726f 7249 6e66 6f20 3d20 7374 6174 7573  rorInfo = status
+00016520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016530: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00016540: 2020 2020 2020 2020 2020 2065 7272 6f72             error
+00016550: 4f62 6a65 6374 203d 2073 656c 662e 7361  Object = self.sa
+00016560: 6665 5f76 616c 7565 2872 6573 706f 6e73  fe_value(respons
+00016570: 652c 2027 6572 726f 7273 2729 0a20 2020  e, 'errors').   
+00016580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016590: 2069 6620 6572 726f 724f 626a 6563 7420   if errorObject 
+000165a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000165b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000165c0: 2020 2020 2065 7272 6f72 4b65 7920 3d20       errorKey = 
+000165d0: 6c69 7374 2865 7272 6f72 4f62 6a65 6374  list(errorObject
+000165e0: 2e6b 6579 7328 2929 5b30 5d0a 2020 2020  .keys())[0].    
+000165f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016600: 2020 2020 6572 726f 724d 6573 7361 6765      errorMessage
+00016610: 4172 7261 7920 3d20 7365 6c66 2e73 6166  Array = self.saf
+00016620: 655f 7661 6c75 6528 6572 726f 724f 626a  e_value(errorObj
+00016630: 6563 742c 2065 7272 6f72 4b65 792c 205b  ect, errorKey, [
+00016640: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00016650: 2020 2020 2020 2020 2020 2065 7272 6f72             error
+00016660: 4d65 7373 6167 654c 656e 6774 6820 3d20  MessageLength = 
+00016670: 6c65 6e28 6572 726f 724d 6573 7361 6765  len(errorMessage
+00016680: 4172 7261 7929 0a20 2020 2020 2020 2020  Array).         
+00016690: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000166a0: 7272 6f72 496e 666f 203d 2065 7272 6f72  rrorInfo = error
+000166b0: 4d65 7373 6167 6541 7272 6179 5b30 5d20  MessageArray[0] 
+000166c0: 6966 2028 6572 726f 724d 6573 7361 6765  if (errorMessage
+000166d0: 4c65 6e67 7468 203e 2030 2920 656c 7365  Length > 0) else
+000166e0: 2062 6f64 790a 2020 2020 2020 2020 2020   body.          
+000166f0: 2020 2020 2020 7365 6c66 2e74 6872 6f77        self.throw
+00016700: 5f65 7861 6374 6c79 5f6d 6174 6368 6564  _exactly_matched
+00016710: 5f65 7863 6570 7469 6f6e 2873 656c 662e  _exception(self.
+00016720: 6578 6365 7074 696f 6e73 5b27 6578 6163  exceptions['exac
+00016730: 7427 5d2c 2065 7272 6f72 496e 666f 2c20  t'], errorInfo, 
+00016740: 6665 6564 6261 636b 290a 2020 2020 2020  feedback).      
+00016750: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00016760: 6872 6f77 5f62 726f 6164 6c79 5f6d 6174  hrow_broadly_mat
+00016770: 6368 6564 5f65 7863 6570 7469 6f6e 2873  ched_exception(s
+00016780: 656c 662e 6578 6365 7074 696f 6e73 5b27  elf.exceptions['
+00016790: 6272 6f61 6427 5d2c 2062 6f64 792c 2066  broad'], body, f
+000167a0: 6565 6462 6163 6b29 0a20 2020 2020 2020  eedback).       
+000167b0: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+000167c0: 7863 6861 6e67 6545 7272 6f72 2866 6565  xchangeError(fee
+000167d0: 6462 6163 6b29 0a20 2020 2020 2020 2072  dback).        r
+000167e0: 6574 7572 6e20 4e6f 6e65 0a              eturn None.
```

### Comparing `ccxt-3.0.93/ccxt/woo.py` & `ccxt-3.0.94/ccxt/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/xt.py` & `ccxt-3.0.94/ccxt/xt.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/yobit.py` & `ccxt-3.0.94/ccxt/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/zaif.py` & `ccxt-3.0.94/ccxt/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/zb.py` & `ccxt-3.0.94/ccxt/zb.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt/zonda.py` & `ccxt-3.0.94/ccxt/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/ccxt.egg-info/PKG-INFO` & `ccxt-3.0.94/ccxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 3.0.93
+Version: 3.0.94
 Summary: A JavaScript / Python / PHP cryptocurrency trading library with support for 130+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://docs.ccxt.com
@@ -227,21 +227,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@3.0.93/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@3.0.93/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@3.0.94/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@3.0.94/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@3.0.93/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@3.0.94/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-3.0.93/ccxt.egg-info/SOURCES.txt` & `ccxt-3.0.94/ccxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccxt-3.0.93/package.json` & `ccxt-3.0.94/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'3.0.94'"}*

```diff
@@ -217,9 +217,9 @@
         "update-badges": "node build/update-badges",
         "update-links": "node build/update-links",
         "vss": "node build/vss"
     },
     "type": "module",
     "types": "./js/ccxt.d.ts",
     "unpkg": "dist/ccxt.browser.js",
-    "version": "3.0.93"
+    "version": "3.0.94"
 }
```

### Comparing `ccxt-3.0.93/setup.py` & `ccxt-3.0.94/setup.py`

 * *Files identical despite different names*

