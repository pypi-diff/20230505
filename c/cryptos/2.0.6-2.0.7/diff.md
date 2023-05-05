# Comparing `tmp/cryptos-2.0.6.tar.gz` & `tmp/cryptos-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptos-2.0.6.tar", last modified: Mon Apr  3 17:26:12 2023, max compression
+gzip compressed data, was "cryptos-2.0.7.tar", last modified: Fri May  5 13:14:13 2023, max compression
```

## Comparing `cryptos-2.0.6.tar` & `cryptos-2.0.7.tar`

### file list

```diff
@@ -1,103 +1,115 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 17:26:12.980723 cryptos-2.0.6/
--rw-rw-rw-   0        0        0     1293 2022-10-03 10:19:24.000000 cryptos-2.0.6/LICENSE
--rw-rw-rw-   0        0        0       63 2022-10-03 10:19:24.000000 cryptos-2.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0    35590 2023-04-03 17:26:12.980723 cryptos-2.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    34875 2023-03-22 18:26:27.000000 cryptos-2.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 17:26:12.826139 cryptos-2.0.6/crypto_scripts/
--rw-rw-rw-   0        0        0        0 2023-03-22 18:26:27.000000 cryptos-2.0.6/crypto_scripts/__init__.py
--rw-rw-rw-   0        0        0      889 2023-03-22 18:26:27.000000 cryptos-2.0.6/crypto_scripts/broadcast.py
--rw-rw-rw-   0        0        0     1891 2023-03-22 18:26:27.000000 cryptos-2.0.6/crypto_scripts/convert_private_key.py
--rw-rw-rw-   0        0        0     1472 2023-03-22 18:26:27.000000 cryptos-2.0.6/crypto_scripts/create_private_key.py
--rw-rw-rw-   0        0        0     2987 2023-03-22 18:26:27.000000 cryptos-2.0.6/crypto_scripts/cryptosend.py
--rw-rw-rw-   0        0        0     8917 2023-03-22 18:26:27.000000 cryptos-2.0.6/crypto_scripts/explorer.py
--rw-rw-rw-   0        0        0     1088 2023-03-22 18:26:27.000000 cryptos-2.0.6/crypto_scripts/get_block_sizes.py
--rw-rw-rw-   0        0        0     3471 2023-03-22 18:26:27.000000 cryptos-2.0.6/crypto_scripts/subscribe.py
--rw-rw-rw-   0        0        0     3637 2023-03-22 18:26:27.000000 cryptos-2.0.6/crypto_scripts/view_private_key_addresses.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:26:12.875753 cryptos-2.0.6/cryptos/
--rw-rw-rw-   0        0        0      275 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/__init__.py
--rw-rw-rw-   0        0        0     3131 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/blocks.py
--rw-rw-rw-   0        0        0     6798 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/cashaddr.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:26:12.908744 cryptos-2.0.6/cryptos/coins/
--rw-rw-rw-   0        0        0      153 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/coins/__init__.py
--rw-rw-rw-   0        0        0    16705 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/coins/base.py
--rw-rw-rw-   0        0        0      162 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/coins/bitcoin.py
--rw-rw-rw-   0        0        0      183 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/coins/bitcoin_cash.py
--rw-rw-rw-   0        0        0      147 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/coins/dash.py
--rw-rw-rw-   0        0        0      151 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/coins/dogecoin.py
--rw-rw-rw-   0        0        0      167 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/coins/litecoin.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:26:12.909245 cryptos-2.0.6/cryptos/coins_async/
--rw-rw-rw-   0        0        0      124 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/coins_async/__init__.py
--rw-rw-rw-   0        0        0    50159 2023-04-03 17:25:43.000000 cryptos-2.0.6/cryptos/coins_async/base.py
--rw-rw-rw-   0        0        0     1252 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/coins_async/bitcoin.py
--rw-rw-rw-   0        0        0     1352 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/coins_async/bitcoin_cash.py
--rw-rw-rw-   0        0        0      746 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/coins_async/dash.py
--rw-rw-rw-   0        0        0      931 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/coins_async/dogecoin.py
--rw-rw-rw-   0        0        0      976 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/coins_async/litecoin.py
--rw-rw-rw-   0        0        0     1657 2022-10-03 10:19:24.000000 cryptos-2.0.6/cryptos/composite.py
--rw-rw-rw-   0        0        0      402 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/constants.py
--rw-rw-rw-   0        0        0     8911 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/deterministic.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:26:12.925857 cryptos-2.0.6/cryptos/electrumx_client/
--rw-rw-rw-   0        0        0       37 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/electrumx_client/__init__.py
--rw-rw-rw-   0        0        0    22725 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/electrumx_client/client.py
--rw-rw-rw-   0        0        0     2400 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/electrumx_client/types.py
--rw-rw-rw-   0        0        0    15164 2022-10-03 10:19:24.000000 cryptos-2.0.6/cryptos/english.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 17:26:12.948876 cryptos-2.0.6/cryptos/explorers/
--rw-rw-rw-   0        0        0      644 2022-10-03 10:19:24.000000 cryptos-2.0.6/cryptos/explorers/__init__.py
--rw-rw-rw-   0        0        0     3268 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/explorers/base_insight.py
--rw-rw-rw-   0        0        0      338 2022-10-03 10:19:24.000000 cryptos-2.0.6/cryptos/explorers/bitpay.py
--rw-rw-rw-   0        0        0     4045 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/explorers/blockchain.py
--rw-rw-rw-   0        0        0     1074 2022-10-03 10:19:24.000000 cryptos-2.0.6/cryptos/explorers/blockcypher.py
--rw-rw-rw-   0        0        0     1280 2022-10-03 10:19:24.000000 cryptos-2.0.6/cryptos/explorers/blockdozer.py
--rw-rw-rw-   0        0        0     1264 2022-10-03 10:19:24.000000 cryptos-2.0.6/cryptos/explorers/btg_explorer.py
--rw-rw-rw-   0        0        0     1242 2022-10-03 10:19:24.000000 cryptos-2.0.6/cryptos/explorers/dash_siampm.py
--rw-rw-rw-   0        0        0     3047 2022-10-03 10:19:24.000000 cryptos-2.0.6/cryptos/explorers/sochain.py
--rw-rw-rw-   0        0        0      559 2022-10-03 10:19:24.000000 cryptos-2.0.6/cryptos/explorers/utils.py
--rw-rw-rw-   0        0        0    18584 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/keystore.py
--rw-rw-rw-   0        0        0    19302 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/main.py
--rw-rw-rw-   0        0        0     8436 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/mnemonic.py
--rw-rw-rw-   0        0        0     2838 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/opcodes.py
--rw-rw-rw-   0        0        0     3494 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/py3specials.py
--rw-rw-rw-   0        0        0    15159 2022-10-03 10:19:24.000000 cryptos-2.0.6/cryptos/ripemd.py
--rw-rw-rw-   0        0        0      364 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/script_utils.py
--rw-rw-rw-   0        0        0     6099 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/segwit_addr.py
--rw-rw-rw-   0        0        0     3777 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/stealth.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:26:12.948876 cryptos-2.0.6/cryptos/testing/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/testing/__init__.py
--rw-rw-rw-   0        0        0    33902 2023-04-03 12:02:39.000000 cryptos-2.0.6/cryptos/testing/testcases.py
--rw-rw-rw-   0        0        0    56461 2023-04-03 12:02:39.000000 cryptos-2.0.6/cryptos/testing/testcases_async.py
--rw-rw-rw-   0        0        0    21694 2023-04-03 17:25:43.000000 cryptos-2.0.6/cryptos/transaction.py
--rw-rw-rw-   0        0        0     2414 2023-04-03 17:25:43.000000 cryptos-2.0.6/cryptos/types.py
--rw-rw-rw-   0        0        0     2040 2023-03-24 21:15:30.000000 cryptos-2.0.6/cryptos/utils.py
--rw-rw-rw-   0        0        0    12253 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/wallet.py
--rw-rw-rw-   0        0        0     6746 2023-03-22 13:46:57.000000 cryptos-2.0.6/cryptos/wallet_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:26:12.892219 cryptos-2.0.6/cryptos.egg-info/
--rw-rw-rw-   0        0        0    35590 2023-04-03 17:26:12.000000 cryptos-2.0.6/cryptos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2547 2023-04-03 17:26:12.000000 cryptos-2.0.6/cryptos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 17:26:12.000000 cryptos-2.0.6/cryptos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      438 2023-04-03 17:26:12.000000 cryptos-2.0.6/cryptos.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       80 2023-04-03 17:26:12.000000 cryptos-2.0.6/cryptos.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-03 17:26:12.000000 cryptos-2.0.6/cryptos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-03 17:26:12.996365 cryptos-2.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1801 2023-04-03 17:25:58.000000 cryptos-2.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:26:12.964450 cryptos-2.0.6/tests/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.6/tests/__init__.py
--rw-rw-rw-   0        0        0     5596 2023-03-22 13:46:57.000000 cryptos-2.0.6/tests/electrum_subscribe_mock_server.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:26:12.964450 cryptos-2.0.6/tests/test_coins/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.6/tests/test_coins/__init__.py
--rw-rw-rw-   0        0        0    13157 2023-04-03 13:33:46.000000 cryptos-2.0.6/tests/test_coins/test_bitcoin_testnet.py
-drwxrwxrwx   0        0        0        0 2023-04-03 17:26:12.980723 cryptos-2.0.6/tests/test_coins_async/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.6/tests/test_coins_async/__init__.py
--rw-rw-rw-   0        0        0    16130 2023-04-03 17:25:43.000000 cryptos-2.0.6/tests/test_coins_async/test_bitcoin.py
--rw-rw-rw-   0        0        0    11403 2023-03-24 22:06:15.000000 cryptos-2.0.6/tests/test_coins_async/test_bitcoin_cash.py
--rw-rw-rw-   0        0        0     8815 2023-03-22 13:46:57.000000 cryptos-2.0.6/tests/test_coins_async/test_bitcoin_cash_testnet.py
--rw-rw-rw-   0        0        0    10667 2023-04-03 12:02:39.000000 cryptos-2.0.6/tests/test_coins_async/test_bitcoin_testnet.py
--rw-rw-rw-   0        0        0     5932 2023-03-22 13:46:57.000000 cryptos-2.0.6/tests/test_coins_async/test_dash.py
--rw-rw-rw-   0        0        0     5829 2023-04-03 12:02:39.000000 cryptos-2.0.6/tests/test_coins_async/test_dash_testnet.py
--rw-rw-rw-   0        0        0     7355 2023-03-22 13:46:57.000000 cryptos-2.0.6/tests/test_coins_async/test_dogecoin.py
--rw-rw-rw-   0        0        0     5694 2023-03-22 13:46:57.000000 cryptos-2.0.6/tests/test_coins_async/test_dogecoin_testnet.py
--rw-rw-rw-   0        0        0    13843 2023-03-22 13:46:57.000000 cryptos-2.0.6/tests/test_coins_async/test_litecoin.py
--rw-rw-rw-   0        0        0     9245 2023-03-22 13:46:57.000000 cryptos-2.0.6/tests/test_coins_async/test_litecoin_testnet.py
--rw-rw-rw-   0        0        0    26157 2023-03-22 13:46:57.000000 cryptos-2.0.6/tests/test_electrum_client.py
--rw-rw-rw-   0        0        0    28702 2023-03-22 13:46:57.000000 cryptos-2.0.6/tests/test_general.py
--rw-rw-rw-   0        0        0     4366 2023-03-22 13:46:57.000000 cryptos-2.0.6/tests/test_stealth.py
--rw-rw-rw-   0        0        0    32352 2023-03-22 13:46:57.000000 cryptos-2.0.6/tests/test_wallet.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.229498 cryptos-2.0.7/
+-rw-rw-rw-   0        0        0     1293 2022-10-03 10:19:24.000000 cryptos-2.0.7/LICENSE
+-rw-rw-rw-   0        0        0      112 2023-05-05 12:53:53.000000 cryptos-2.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    36041 2023-05-05 13:14:13.227497 cryptos-2.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    35326 2023-05-05 13:08:32.000000 cryptos-2.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.046558 cryptos-2.0.7/crypto_scripts/
+-rw-rw-rw-   0        0        0        0 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/__init__.py
+-rw-rw-rw-   0        0        0      889 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/broadcast.py
+-rw-rw-rw-   0        0        0     1891 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/convert_private_key.py
+-rw-rw-rw-   0        0        0     1472 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/create_private_key.py
+-rw-rw-rw-   0        0        0     2987 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/cryptosend.py
+-rw-rw-rw-   0        0        0     8917 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/explorer.py
+-rw-rw-rw-   0        0        0     1088 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/get_block_sizes.py
+-rw-rw-rw-   0        0        0     3471 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/subscribe.py
+-rw-rw-rw-   0        0        0     3637 2023-03-22 18:26:27.000000 cryptos-2.0.7/crypto_scripts/view_private_key_addresses.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.091058 cryptos-2.0.7/cryptos/
+-rw-rw-rw-   0        0        0      275 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/__init__.py
+-rw-rw-rw-   0        0        0     3131 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/blocks.py
+-rw-rw-rw-   0        0        0     6798 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/cashaddr.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.120321 cryptos-2.0.7/cryptos/coins/
+-rw-rw-rw-   0        0        0      153 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins/__init__.py
+-rw-rw-rw-   0        0        0    16705 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins/base.py
+-rw-rw-rw-   0        0        0      162 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins/bitcoin.py
+-rw-rw-rw-   0        0        0      183 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins/bitcoin_cash.py
+-rw-rw-rw-   0        0        0      147 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins/dash.py
+-rw-rw-rw-   0        0        0      151 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins/dogecoin.py
+-rw-rw-rw-   0        0        0      167 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins/litecoin.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.136436 cryptos-2.0.7/cryptos/coins_async/
+-rw-rw-rw-   0        0        0      124 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins_async/__init__.py
+-rw-rw-rw-   0        0        0    50159 2023-04-03 17:25:43.000000 cryptos-2.0.7/cryptos/coins_async/base.py
+-rw-rw-rw-   0        0        0     1252 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins_async/bitcoin.py
+-rw-rw-rw-   0        0        0     1352 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins_async/bitcoin_cash.py
+-rw-rw-rw-   0        0        0      746 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins_async/dash.py
+-rw-rw-rw-   0        0        0      931 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins_async/dogecoin.py
+-rw-rw-rw-   0        0        0      976 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/coins_async/litecoin.py
+-rw-rw-rw-   0        0        0     1657 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/composite.py
+-rw-rw-rw-   0        0        0      402 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/constants.py
+-rw-rw-rw-   0        0        0     8911 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/deterministic.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.142500 cryptos-2.0.7/cryptos/electrumx_client/
+-rw-rw-rw-   0        0        0       37 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/__init__.py
+-rw-rw-rw-   0        0        0    22725 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/client.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.162771 cryptos-2.0.7/cryptos/electrumx_client/servers/
+-rw-rw-rw-   0        0        0    10969 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/bitcoin.json
+-rw-rw-rw-   0        0        0     3618 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/bitcoin_cash.json
+-rw-rw-rw-   0        0        0     1093 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/bitcoin_cash_testnet.json
+-rw-rw-rw-   0        0        0      936 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/bitcoin_testnet.json
+-rw-rw-rw-   0        0        0      384 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/dash.json
+-rw-rw-rw-   0        0        0      486 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/dash_testnet.json
+-rw-rw-rw-   0        0        0      254 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/doge.json
+-rw-rw-rw-   0        0        0      254 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/doge_testnet.json
+-rw-rw-rw-   0        0        0      973 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/litecoin.json
+-rw-rw-rw-   0        0        0      283 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/litecoin_testnet.json
+-rw-rw-rw-   0        0        0      257 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/servers/testing.json
+-rw-rw-rw-   0        0        0     2400 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/electrumx_client/types.py
+-rw-rw-rw-   0        0        0    15164 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/english.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.182148 cryptos-2.0.7/cryptos/explorers/
+-rw-rw-rw-   0        0        0      644 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/explorers/base_insight.py
+-rw-rw-rw-   0        0        0      338 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/bitpay.py
+-rw-rw-rw-   0        0        0     4045 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/explorers/blockchain.py
+-rw-rw-rw-   0        0        0     1074 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/blockcypher.py
+-rw-rw-rw-   0        0        0     1280 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/blockdozer.py
+-rw-rw-rw-   0        0        0     1264 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/btg_explorer.py
+-rw-rw-rw-   0        0        0     1242 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/dash_siampm.py
+-rw-rw-rw-   0        0        0     3047 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/sochain.py
+-rw-rw-rw-   0        0        0      559 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/explorers/utils.py
+-rw-rw-rw-   0        0        0    18584 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/keystore.py
+-rw-rw-rw-   0        0        0    19302 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/main.py
+-rw-rw-rw-   0        0        0     8436 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/mnemonic.py
+-rw-rw-rw-   0        0        0     2838 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/opcodes.py
+-rw-rw-rw-   0        0        0     3494 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/py3specials.py
+-rw-rw-rw-   0        0        0    15159 2022-10-03 10:19:24.000000 cryptos-2.0.7/cryptos/ripemd.py
+-rw-rw-rw-   0        0        0      364 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/script_utils.py
+-rw-rw-rw-   0        0        0     6099 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/segwit_addr.py
+-rw-rw-rw-   0        0        0     3777 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/stealth.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.187822 cryptos-2.0.7/cryptos/testing/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/testing/__init__.py
+-rw-rw-rw-   0        0        0    33902 2023-04-03 12:02:39.000000 cryptos-2.0.7/cryptos/testing/testcases.py
+-rw-rw-rw-   0        0        0    56461 2023-04-03 12:02:39.000000 cryptos-2.0.7/cryptos/testing/testcases_async.py
+-rw-rw-rw-   0        0        0    21694 2023-04-03 17:25:43.000000 cryptos-2.0.7/cryptos/transaction.py
+-rw-rw-rw-   0        0        0     2414 2023-04-03 17:25:43.000000 cryptos-2.0.7/cryptos/types.py
+-rw-rw-rw-   0        0        0     2040 2023-03-24 21:15:30.000000 cryptos-2.0.7/cryptos/utils.py
+-rw-rw-rw-   0        0        0    12253 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/wallet.py
+-rw-rw-rw-   0        0        0     6746 2023-03-22 13:46:57.000000 cryptos-2.0.7/cryptos/wallet_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.105193 cryptos-2.0.7/cryptos.egg-info/
+-rw-rw-rw-   0        0        0    36041 2023-05-05 13:14:12.000000 cryptos-2.0.7/cryptos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3093 2023-05-05 13:14:12.000000 cryptos-2.0.7/cryptos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 13:14:12.000000 cryptos-2.0.7/cryptos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      438 2023-05-05 13:14:12.000000 cryptos-2.0.7/cryptos.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       80 2023-05-05 13:14:12.000000 cryptos-2.0.7/cryptos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-05-05 13:14:12.000000 cryptos-2.0.7/cryptos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 13:14:13.229498 cryptos-2.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1801 2023-05-05 12:51:31.000000 cryptos-2.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.199933 cryptos-2.0.7/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     5596 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/electrum_subscribe_mock_server.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.204117 cryptos-2.0.7/tests/test_coins/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins/__init__.py
+-rw-rw-rw-   0        0        0    13157 2023-04-03 13:33:46.000000 cryptos-2.0.7/tests/test_coins/test_bitcoin_testnet.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:14:13.224498 cryptos-2.0.7/tests/test_coins_async/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins_async/__init__.py
+-rw-rw-rw-   0        0        0    16130 2023-04-03 17:25:43.000000 cryptos-2.0.7/tests/test_coins_async/test_bitcoin.py
+-rw-rw-rw-   0        0        0    11403 2023-03-24 22:06:15.000000 cryptos-2.0.7/tests/test_coins_async/test_bitcoin_cash.py
+-rw-rw-rw-   0        0        0     8815 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins_async/test_bitcoin_cash_testnet.py
+-rw-rw-rw-   0        0        0    10667 2023-04-03 12:02:39.000000 cryptos-2.0.7/tests/test_coins_async/test_bitcoin_testnet.py
+-rw-rw-rw-   0        0        0     5932 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins_async/test_dash.py
+-rw-rw-rw-   0        0        0     5829 2023-04-03 12:02:39.000000 cryptos-2.0.7/tests/test_coins_async/test_dash_testnet.py
+-rw-rw-rw-   0        0        0     7355 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins_async/test_dogecoin.py
+-rw-rw-rw-   0        0        0     5694 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins_async/test_dogecoin_testnet.py
+-rw-rw-rw-   0        0        0    13843 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins_async/test_litecoin.py
+-rw-rw-rw-   0        0        0     9245 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_coins_async/test_litecoin_testnet.py
+-rw-rw-rw-   0        0        0    26157 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_electrum_client.py
+-rw-rw-rw-   0        0        0    28702 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_general.py
+-rw-rw-rw-   0        0        0     4366 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_stealth.py
+-rw-rw-rw-   0        0        0    32352 2023-03-22 13:46:57.000000 cryptos-2.0.7/tests/test_wallet.py
```

### Comparing `cryptos-2.0.6/LICENSE` & `cryptos-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/PKG-INFO` & `cryptos-2.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptos
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python Crypto Coin Tools
 Home-page: http://github.com/primal100/pybitcointools
 Author: Paul Martin
 Author-email: greatestloginnameever@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pycryptotools, Python library for Crypto coins signatures and transactions
 
 This is a fork of Vitalik Buterin's original [pybitcointools](https://github.com/vbuterin/pybitcointools) library.
 
-After a lot of work, the library is finally active again and being actively updated.
+After a lot of work, the library is finally active again and being actively updated. This took a lot of work and unfortunately some backward imcompatible changes may have been introduced in v2. If you run into issues after upgrading open an issue and will try to help. If it's reasonable to do so we can consider restoring the previous behaviour in v2, otherwise will assist with migration.
 
 Installation:
 
 ```bash
 pip install cryptos
 ```
 
@@ -80,15 +80,15 @@
 
 ### Disadvantages:
 
 * Not a full node, has no idea what blocks are
 
 ### Example usage - the long way (best way to learn :) ):
 
-WARNING: While it's fun to mess around with this on the testnet, do not do the following procedure on the mainnet you really know what you are doing. Any value in the inputs not included in the outputs will be lost.
+WARNING: While it's fun to mess around with this on the testnet, do not do the following procedure on the mainnet unless you really know what you are doing. Any value in the inputs not included in the outputs will be lost.
 So if the total inputs value is 1 BTC, and the total outputs amount to 0.6 BTC, 0.4 BTC will be given to the miners as a fee. The faster way, listed later in the README, ensures the difference between
 inputs and outputs is sent as change back to the sender (except for a small minter fee).
 If in doubt, before broadcasting a transaction, visit https://live.blockcypher.com/btc/decodetx/ and decode the raw tx
 and make sure it looks right. If you aren't familiar with how Bitcoin transactions work, you should run through
  this procedure a few times on the testnet before developing for mainnet.
 
 OTHER WARNING: If transactions are taking a long time to be confirmed, try increasing the fee from what the 
@@ -503,30 +503,29 @@
 The arguments are the private key of the sender, the receiver's address and the fee (default 10000). Change will be returned to the sender. 
 
 ### Listing of main coin-specific methods:
 
 * privtopub            : (privkey) -> pubkey
 * pubtoaddr            : (pubkey) -> address
 * privtoaddr           : (privkey) -> address
-* encode_privkey       : (privkey, format, script_type) -> privkey
+* encode_privkey       : (privkey, format, script_type="p2pkh") -> privkey
 * sign                 : (txobj, i, privkey) -> create digital signature of tx with privkey and add to input i
 * signall              : (txobj, privkey) -> create digital signature of tx with privkey for all inputs
-* history              : (address) -> tx history and balance of an address
-* unspent              : (address) -> unspent outputs for an addresses
+* history              : (address, merkle_proof=False) -> tx history and balance of an address
+* unspent              : (address, merkle_proof=False) -> unspent outputs for an addresses
 * pushtx               : (hex or bin tx) -> push a transaction to the blockchain
-* fetchtx              : (txhash) -> fetch a tx from the blockchain
-* txinputs             : (txhash) -> fetch inputs from a previous transaction in a format to be re-used as unspents             
-* send                 : (privkey, to, value, fee=10000, change_addr=None, segwit=False, addr=None) -> create and a push a simple transaction to send coins to an address and return change to the change address or sender
-* sendmultitx          : (privkey, to:value pairs, fee=10000, change_addr=None, segwit=False, addr=None) -> create and a push a transaction to send coins to multiple addresses and return change to the change address or sender
-* preparetx            : (frm, to, value, fee, change_addr=None, segwit=False): -> create unsigned txobj with change output
-* preparemultitx       : (frm, to:value pairs, fee, change_addr=None, segwit=False): -> create unsigned txobj with multiple outputs and additional change output
-* preparesignedtx      : (privkey, to, value, fee=10000, change_addr=None, segwit=False, addr=None) -> create signed txobj with change output
-* preparesignedmultitx : (privkey, *args, change_addr=None, segwit=False, addr=None) -> create signed txobj with multiple outputs and additional change output
-* mktx                 : (inputs, outputs) -> create unsigned txobj
-* mksend               : (inputs, outputs, change_addr, fee, segwit) -> create unsigned txobj
+* get_tx               : (txhash) -> fetch a tx from the blockchain
+* send                 : (privkey, frm, to, value, change_addr=None, fee=None, estimate_fee_blocks: int = 6) -> create and a push a simple transaction to send coins to an address and return change to the change address or sender
+* send_to_multiple_receivers_tx          : (privkey, addr outs:value pairs, change_addr=None,fee=10000,, estimate_fee_blocks: int = 6) -> create and a push a transaction to send coins to multiple addresses and return change to the change address or sender
+* preparetx            : (frm, to, value, fee, estimate_fee_blocks: int = 6,change_addr=None): -> create unsigned txobj with change output
+* preparemultitx       : (frm, outs:value pairs, change_addr=None, fee=None, estimate_fee_blocks: int = 6): -> create unsigned txobj with multiple outputs and additional change output
+* preparesignedtx      : (privkey, frm, to, value, change_addr=None, fee=10000, estimate_fee_blocks: int = 6) -> create signed txobj with change output
+* preparesignedmultirecipienttx : (privkey, frm, outs: value pairs, change_addr=None, fee=10000, estimate_fee_blocks: int = 6) -> create signed txobj with multiple outputs and additional change output
+* mktx                 : (inputs, outputs, locktime=0, sequence=0xFFFFFFFF) -> create unsigned txobj
+* mktx_with_change     : (inputs, outputs, change_addr=None, fee=None, estimate_fee_blocks=6, locktime=0, sequence=0xFFFFFFFF) -> create unsigned txobj
 * mk_multisig_address  : (pubkeys, M) -> Returns both M-of-N multsig script and address pubkeys
 * pubtop2w             : (pub) -> pay to witness script hash (segwit address)
 * privtop2w            : (priv) -> pay to witness script hash (segwit address)
 * is_address           : (addr) -> true if addr is a valid address for this network
 * is_p2sh              : (addr) -> true if addr is a pay to script hash for this network
 * is_segwit            : (priv, addr) -> true if priv-addr pair represent a pay to witness script hash
 * current_block_height : () -> Latest block height
```

### Comparing `cryptos-2.0.6/README.md` & `cryptos-2.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Pycryptotools, Python library for Crypto coins signatures and transactions
 
 This is a fork of Vitalik Buterin's original [pybitcointools](https://github.com/vbuterin/pybitcointools) library.
 
-After a lot of work, the library is finally active again and being actively updated.
+After a lot of work, the library is finally active again and being actively updated. This took a lot of work and unfortunately some backward imcompatible changes may have been introduced in v2. If you run into issues after upgrading open an issue and will try to help. If it's reasonable to do so we can consider restoring the previous behaviour in v2, otherwise will assist with migration.
 
 Installation:
 
 ```bash
 pip install cryptos
 ```
 
@@ -61,15 +61,15 @@
 
 ### Disadvantages:
 
 * Not a full node, has no idea what blocks are
 
 ### Example usage - the long way (best way to learn :) ):
 
-WARNING: While it's fun to mess around with this on the testnet, do not do the following procedure on the mainnet you really know what you are doing. Any value in the inputs not included in the outputs will be lost.
+WARNING: While it's fun to mess around with this on the testnet, do not do the following procedure on the mainnet unless you really know what you are doing. Any value in the inputs not included in the outputs will be lost.
 So if the total inputs value is 1 BTC, and the total outputs amount to 0.6 BTC, 0.4 BTC will be given to the miners as a fee. The faster way, listed later in the README, ensures the difference between
 inputs and outputs is sent as change back to the sender (except for a small minter fee).
 If in doubt, before broadcasting a transaction, visit https://live.blockcypher.com/btc/decodetx/ and decode the raw tx
 and make sure it looks right. If you aren't familiar with how Bitcoin transactions work, you should run through
  this procedure a few times on the testnet before developing for mainnet.
 
 OTHER WARNING: If transactions are taking a long time to be confirmed, try increasing the fee from what the 
@@ -484,30 +484,29 @@
 The arguments are the private key of the sender, the receiver's address and the fee (default 10000). Change will be returned to the sender. 
 
 ### Listing of main coin-specific methods:
 
 * privtopub            : (privkey) -> pubkey
 * pubtoaddr            : (pubkey) -> address
 * privtoaddr           : (privkey) -> address
-* encode_privkey       : (privkey, format, script_type) -> privkey
+* encode_privkey       : (privkey, format, script_type="p2pkh") -> privkey
 * sign                 : (txobj, i, privkey) -> create digital signature of tx with privkey and add to input i
 * signall              : (txobj, privkey) -> create digital signature of tx with privkey for all inputs
-* history              : (address) -> tx history and balance of an address
-* unspent              : (address) -> unspent outputs for an addresses
+* history              : (address, merkle_proof=False) -> tx history and balance of an address
+* unspent              : (address, merkle_proof=False) -> unspent outputs for an addresses
 * pushtx               : (hex or bin tx) -> push a transaction to the blockchain
-* fetchtx              : (txhash) -> fetch a tx from the blockchain
-* txinputs             : (txhash) -> fetch inputs from a previous transaction in a format to be re-used as unspents             
-* send                 : (privkey, to, value, fee=10000, change_addr=None, segwit=False, addr=None) -> create and a push a simple transaction to send coins to an address and return change to the change address or sender
-* sendmultitx          : (privkey, to:value pairs, fee=10000, change_addr=None, segwit=False, addr=None) -> create and a push a transaction to send coins to multiple addresses and return change to the change address or sender
-* preparetx            : (frm, to, value, fee, change_addr=None, segwit=False): -> create unsigned txobj with change output
-* preparemultitx       : (frm, to:value pairs, fee, change_addr=None, segwit=False): -> create unsigned txobj with multiple outputs and additional change output
-* preparesignedtx      : (privkey, to, value, fee=10000, change_addr=None, segwit=False, addr=None) -> create signed txobj with change output
-* preparesignedmultitx : (privkey, *args, change_addr=None, segwit=False, addr=None) -> create signed txobj with multiple outputs and additional change output
-* mktx                 : (inputs, outputs) -> create unsigned txobj
-* mksend               : (inputs, outputs, change_addr, fee, segwit) -> create unsigned txobj
+* get_tx               : (txhash) -> fetch a tx from the blockchain
+* send                 : (privkey, frm, to, value, change_addr=None, fee=None, estimate_fee_blocks: int = 6) -> create and a push a simple transaction to send coins to an address and return change to the change address or sender
+* send_to_multiple_receivers_tx          : (privkey, addr outs:value pairs, change_addr=None,fee=10000,, estimate_fee_blocks: int = 6) -> create and a push a transaction to send coins to multiple addresses and return change to the change address or sender
+* preparetx            : (frm, to, value, fee, estimate_fee_blocks: int = 6,change_addr=None): -> create unsigned txobj with change output
+* preparemultitx       : (frm, outs:value pairs, change_addr=None, fee=None, estimate_fee_blocks: int = 6): -> create unsigned txobj with multiple outputs and additional change output
+* preparesignedtx      : (privkey, frm, to, value, change_addr=None, fee=10000, estimate_fee_blocks: int = 6) -> create signed txobj with change output
+* preparesignedmultirecipienttx : (privkey, frm, outs: value pairs, change_addr=None, fee=10000, estimate_fee_blocks: int = 6) -> create signed txobj with multiple outputs and additional change output
+* mktx                 : (inputs, outputs, locktime=0, sequence=0xFFFFFFFF) -> create unsigned txobj
+* mktx_with_change     : (inputs, outputs, change_addr=None, fee=None, estimate_fee_blocks=6, locktime=0, sequence=0xFFFFFFFF) -> create unsigned txobj
 * mk_multisig_address  : (pubkeys, M) -> Returns both M-of-N multsig script and address pubkeys
 * pubtop2w             : (pub) -> pay to witness script hash (segwit address)
 * privtop2w            : (priv) -> pay to witness script hash (segwit address)
 * is_address           : (addr) -> true if addr is a valid address for this network
 * is_p2sh              : (addr) -> true if addr is a pay to script hash for this network
 * is_segwit            : (priv, addr) -> true if priv-addr pair represent a pay to witness script hash
 * current_block_height : () -> Latest block height
```

### Comparing `cryptos-2.0.6/crypto_scripts/broadcast.py` & `cryptos-2.0.7/crypto_scripts/broadcast.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/crypto_scripts/convert_private_key.py` & `cryptos-2.0.7/crypto_scripts/convert_private_key.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/crypto_scripts/create_private_key.py` & `cryptos-2.0.7/crypto_scripts/create_private_key.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/crypto_scripts/cryptosend.py` & `cryptos-2.0.7/crypto_scripts/cryptosend.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/crypto_scripts/explorer.py` & `cryptos-2.0.7/crypto_scripts/explorer.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/crypto_scripts/get_block_sizes.py` & `cryptos-2.0.7/crypto_scripts/get_block_sizes.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/crypto_scripts/subscribe.py` & `cryptos-2.0.7/crypto_scripts/subscribe.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/crypto_scripts/view_private_key_addresses.py` & `cryptos-2.0.7/crypto_scripts/view_private_key_addresses.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/blocks.py` & `cryptos-2.0.7/cryptos/blocks.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/cashaddr.py` & `cryptos-2.0.7/cryptos/cashaddr.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/coins/base.py` & `cryptos-2.0.7/cryptos/coins/base.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/coins_async/base.py` & `cryptos-2.0.7/cryptos/coins_async/base.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/coins_async/bitcoin.py` & `cryptos-2.0.7/cryptos/coins_async/bitcoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/coins_async/bitcoin_cash.py` & `cryptos-2.0.7/cryptos/coins_async/bitcoin_cash.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/coins_async/dash.py` & `cryptos-2.0.7/cryptos/coins_async/dash.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/coins_async/dogecoin.py` & `cryptos-2.0.7/cryptos/coins_async/dogecoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/coins_async/litecoin.py` & `cryptos-2.0.7/cryptos/coins_async/litecoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/composite.py` & `cryptos-2.0.7/cryptos/composite.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/deterministic.py` & `cryptos-2.0.7/cryptos/deterministic.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/electrumx_client/client.py` & `cryptos-2.0.7/cryptos/electrumx_client/client.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/electrumx_client/types.py` & `cryptos-2.0.7/cryptos/electrumx_client/types.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/english.txt` & `cryptos-2.0.7/cryptos/english.txt`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/explorers/__init__.py` & `cryptos-2.0.7/cryptos/explorers/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/explorers/base_insight.py` & `cryptos-2.0.7/cryptos/explorers/base_insight.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/explorers/blockchain.py` & `cryptos-2.0.7/cryptos/explorers/blockchain.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/explorers/blockcypher.py` & `cryptos-2.0.7/cryptos/explorers/blockcypher.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/explorers/blockdozer.py` & `cryptos-2.0.7/cryptos/explorers/blockdozer.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/explorers/btg_explorer.py` & `cryptos-2.0.7/cryptos/explorers/btg_explorer.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/explorers/dash_siampm.py` & `cryptos-2.0.7/cryptos/explorers/dash_siampm.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/explorers/sochain.py` & `cryptos-2.0.7/cryptos/explorers/sochain.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/explorers/utils.py` & `cryptos-2.0.7/cryptos/explorers/utils.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/keystore.py` & `cryptos-2.0.7/cryptos/keystore.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/main.py` & `cryptos-2.0.7/cryptos/main.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/mnemonic.py` & `cryptos-2.0.7/cryptos/mnemonic.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/opcodes.py` & `cryptos-2.0.7/cryptos/opcodes.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/py3specials.py` & `cryptos-2.0.7/cryptos/py3specials.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/ripemd.py` & `cryptos-2.0.7/cryptos/ripemd.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/segwit_addr.py` & `cryptos-2.0.7/cryptos/segwit_addr.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/stealth.py` & `cryptos-2.0.7/cryptos/stealth.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/testing/testcases.py` & `cryptos-2.0.7/cryptos/testing/testcases.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/testing/testcases_async.py` & `cryptos-2.0.7/cryptos/testing/testcases_async.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/transaction.py` & `cryptos-2.0.7/cryptos/transaction.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/types.py` & `cryptos-2.0.7/cryptos/types.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/utils.py` & `cryptos-2.0.7/cryptos/utils.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/wallet.py` & `cryptos-2.0.7/cryptos/wallet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos/wallet_utils.py` & `cryptos-2.0.7/cryptos/wallet_utils.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/cryptos.egg-info/PKG-INFO` & `cryptos-2.0.7/cryptos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptos
-Version: 2.0.6
+Version: 2.0.7
 Summary: Python Crypto Coin Tools
 Home-page: http://github.com/primal100/pybitcointools
 Author: Paul Martin
 Author-email: greatestloginnameever@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pycryptotools, Python library for Crypto coins signatures and transactions
 
 This is a fork of Vitalik Buterin's original [pybitcointools](https://github.com/vbuterin/pybitcointools) library.
 
-After a lot of work, the library is finally active again and being actively updated.
+After a lot of work, the library is finally active again and being actively updated. This took a lot of work and unfortunately some backward imcompatible changes may have been introduced in v2. If you run into issues after upgrading open an issue and will try to help. If it's reasonable to do so we can consider restoring the previous behaviour in v2, otherwise will assist with migration.
 
 Installation:
 
 ```bash
 pip install cryptos
 ```
 
@@ -80,15 +80,15 @@
 
 ### Disadvantages:
 
 * Not a full node, has no idea what blocks are
 
 ### Example usage - the long way (best way to learn :) ):
 
-WARNING: While it's fun to mess around with this on the testnet, do not do the following procedure on the mainnet you really know what you are doing. Any value in the inputs not included in the outputs will be lost.
+WARNING: While it's fun to mess around with this on the testnet, do not do the following procedure on the mainnet unless you really know what you are doing. Any value in the inputs not included in the outputs will be lost.
 So if the total inputs value is 1 BTC, and the total outputs amount to 0.6 BTC, 0.4 BTC will be given to the miners as a fee. The faster way, listed later in the README, ensures the difference between
 inputs and outputs is sent as change back to the sender (except for a small minter fee).
 If in doubt, before broadcasting a transaction, visit https://live.blockcypher.com/btc/decodetx/ and decode the raw tx
 and make sure it looks right. If you aren't familiar with how Bitcoin transactions work, you should run through
  this procedure a few times on the testnet before developing for mainnet.
 
 OTHER WARNING: If transactions are taking a long time to be confirmed, try increasing the fee from what the 
@@ -503,30 +503,29 @@
 The arguments are the private key of the sender, the receiver's address and the fee (default 10000). Change will be returned to the sender. 
 
 ### Listing of main coin-specific methods:
 
 * privtopub            : (privkey) -> pubkey
 * pubtoaddr            : (pubkey) -> address
 * privtoaddr           : (privkey) -> address
-* encode_privkey       : (privkey, format, script_type) -> privkey
+* encode_privkey       : (privkey, format, script_type="p2pkh") -> privkey
 * sign                 : (txobj, i, privkey) -> create digital signature of tx with privkey and add to input i
 * signall              : (txobj, privkey) -> create digital signature of tx with privkey for all inputs
-* history              : (address) -> tx history and balance of an address
-* unspent              : (address) -> unspent outputs for an addresses
+* history              : (address, merkle_proof=False) -> tx history and balance of an address
+* unspent              : (address, merkle_proof=False) -> unspent outputs for an addresses
 * pushtx               : (hex or bin tx) -> push a transaction to the blockchain
-* fetchtx              : (txhash) -> fetch a tx from the blockchain
-* txinputs             : (txhash) -> fetch inputs from a previous transaction in a format to be re-used as unspents             
-* send                 : (privkey, to, value, fee=10000, change_addr=None, segwit=False, addr=None) -> create and a push a simple transaction to send coins to an address and return change to the change address or sender
-* sendmultitx          : (privkey, to:value pairs, fee=10000, change_addr=None, segwit=False, addr=None) -> create and a push a transaction to send coins to multiple addresses and return change to the change address or sender
-* preparetx            : (frm, to, value, fee, change_addr=None, segwit=False): -> create unsigned txobj with change output
-* preparemultitx       : (frm, to:value pairs, fee, change_addr=None, segwit=False): -> create unsigned txobj with multiple outputs and additional change output
-* preparesignedtx      : (privkey, to, value, fee=10000, change_addr=None, segwit=False, addr=None) -> create signed txobj with change output
-* preparesignedmultitx : (privkey, *args, change_addr=None, segwit=False, addr=None) -> create signed txobj with multiple outputs and additional change output
-* mktx                 : (inputs, outputs) -> create unsigned txobj
-* mksend               : (inputs, outputs, change_addr, fee, segwit) -> create unsigned txobj
+* get_tx               : (txhash) -> fetch a tx from the blockchain
+* send                 : (privkey, frm, to, value, change_addr=None, fee=None, estimate_fee_blocks: int = 6) -> create and a push a simple transaction to send coins to an address and return change to the change address or sender
+* send_to_multiple_receivers_tx          : (privkey, addr outs:value pairs, change_addr=None,fee=10000,, estimate_fee_blocks: int = 6) -> create and a push a transaction to send coins to multiple addresses and return change to the change address or sender
+* preparetx            : (frm, to, value, fee, estimate_fee_blocks: int = 6,change_addr=None): -> create unsigned txobj with change output
+* preparemultitx       : (frm, outs:value pairs, change_addr=None, fee=None, estimate_fee_blocks: int = 6): -> create unsigned txobj with multiple outputs and additional change output
+* preparesignedtx      : (privkey, frm, to, value, change_addr=None, fee=10000, estimate_fee_blocks: int = 6) -> create signed txobj with change output
+* preparesignedmultirecipienttx : (privkey, frm, outs: value pairs, change_addr=None, fee=10000, estimate_fee_blocks: int = 6) -> create signed txobj with multiple outputs and additional change output
+* mktx                 : (inputs, outputs, locktime=0, sequence=0xFFFFFFFF) -> create unsigned txobj
+* mktx_with_change     : (inputs, outputs, change_addr=None, fee=None, estimate_fee_blocks=6, locktime=0, sequence=0xFFFFFFFF) -> create unsigned txobj
 * mk_multisig_address  : (pubkeys, M) -> Returns both M-of-N multsig script and address pubkeys
 * pubtop2w             : (pub) -> pay to witness script hash (segwit address)
 * privtop2w            : (priv) -> pay to witness script hash (segwit address)
 * is_address           : (addr) -> true if addr is a valid address for this network
 * is_p2sh              : (addr) -> true if addr is a pay to script hash for this network
 * is_segwit            : (priv, addr) -> true if priv-addr pair represent a pay to witness script hash
 * current_block_height : () -> Latest block height
```

### Comparing `cryptos-2.0.6/setup.py` & `cryptos-2.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 setup(name='cryptos',
-      version='2.0.6',
+      version='2.0.7',
       description='Python Crypto Coin Tools',
       long_description=open('README.md').read(),
       long_description_content_type='text/markdown',
       author='Paul Martin',
       author_email='greatestloginnameever@gmail.com',
       url='http://github.com/primal100/pybitcointools',
       packages=find_packages(),
```

### Comparing `cryptos-2.0.6/tests/electrum_subscribe_mock_server.py` & `cryptos-2.0.7/tests/electrum_subscribe_mock_server.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/tests/test_coins/test_bitcoin_testnet.py` & `cryptos-2.0.7/tests/test_coins/test_bitcoin_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/tests/test_coins_async/test_bitcoin.py` & `cryptos-2.0.7/tests/test_coins_async/test_bitcoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/tests/test_coins_async/test_bitcoin_cash.py` & `cryptos-2.0.7/tests/test_coins_async/test_bitcoin_cash.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/tests/test_coins_async/test_bitcoin_cash_testnet.py` & `cryptos-2.0.7/tests/test_coins_async/test_bitcoin_cash_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/tests/test_coins_async/test_bitcoin_testnet.py` & `cryptos-2.0.7/tests/test_coins_async/test_bitcoin_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/tests/test_coins_async/test_dash.py` & `cryptos-2.0.7/tests/test_coins_async/test_dash.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/tests/test_coins_async/test_dash_testnet.py` & `cryptos-2.0.7/tests/test_coins_async/test_dash_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/tests/test_coins_async/test_dogecoin.py` & `cryptos-2.0.7/tests/test_coins_async/test_dogecoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/tests/test_coins_async/test_dogecoin_testnet.py` & `cryptos-2.0.7/tests/test_coins_async/test_dogecoin_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/tests/test_coins_async/test_litecoin.py` & `cryptos-2.0.7/tests/test_coins_async/test_litecoin.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/tests/test_coins_async/test_litecoin_testnet.py` & `cryptos-2.0.7/tests/test_coins_async/test_litecoin_testnet.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/tests/test_electrum_client.py` & `cryptos-2.0.7/tests/test_electrum_client.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/tests/test_general.py` & `cryptos-2.0.7/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/tests/test_stealth.py` & `cryptos-2.0.7/tests/test_stealth.py`

 * *Files identical despite different names*

### Comparing `cryptos-2.0.6/tests/test_wallet.py` & `cryptos-2.0.7/tests/test_wallet.py`

 * *Files identical despite different names*

