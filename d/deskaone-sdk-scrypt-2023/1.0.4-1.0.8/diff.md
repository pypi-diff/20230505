# Comparing `tmp/deskaone_sdk_scrypt_2023-1.0.4.tar.gz` & `tmp/deskaone_sdk_scrypt_2023-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deskaone_sdk_scrypt_2023-1.0.4.tar", max compression
+gzip compressed data, was "deskaone_sdk_scrypt_2023-1.0.8.tar", max compression
```

## Comparing `deskaone_sdk_scrypt_2023-1.0.4.tar` & `deskaone_sdk_scrypt_2023-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      734 2023-05-04 07:01:57.726064 deskaone_sdk_scrypt_2023-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.0.4/README.md
--rw-r--r--   0        0        0      388 2023-05-02 07:28:00.336409 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/__init__.py
--rw-r--r--   0        0        0     5993 2023-05-04 07:01:51.651028 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Client/__init__.py
--rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Database/__init__.py
--rw-r--r--   0        0        0      823 2023-03-29 02:19:26.852041 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
--rw-r--r--   0        0        0     2939 2023-05-02 07:26:37.562775 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
--rw-r--r--   0        0        0      477 2023-05-04 07:02:02.501461 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
--rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
--rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Color.py
--rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
--rw-r--r--   0        0        0     1901 2023-03-27 01:24:30.967144 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
--rw-r--r--   0        0        0    17776 2023-05-04 06:49:07.198058 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
--rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Random.py
--rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
--rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
--rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
--rw-r--r--   0        0        0     3613 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
--rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
--rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.0.4/setup.py
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      734 2023-05-05 20:11:43.612179 deskaone_sdk_scrypt_2023-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.0.8/README.md
+-rw-r--r--   0        0        0      388 2023-05-02 07:28:00.336409 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/__init__.py
+-rw-r--r--   0        0        0     5993 2023-05-04 07:01:51.651028 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Client/__init__.py
+-rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Database/__init__.py
+-rw-r--r--   0        0        0      823 2023-03-29 02:19:26.852041 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
+-rw-r--r--   0        0        0     2939 2023-05-02 07:26:37.562775 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
+-rw-r--r--   0        0        0      491 2023-05-05 20:11:44.588051 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
+-rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
+-rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/Color.py
+-rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
+-rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
+-rw-r--r--   0        0        0    26122 2023-05-05 20:11:15.157841 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
+-rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/Random.py
+-rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
+-rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
+-rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
+-rw-r--r--   0        0        0     3613 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
+-rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
+-rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
+-rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.0.8/setup.py
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.0.8/PKG-INFO
```

### Comparing `deskaone_sdk_scrypt_2023-1.0.4/pyproject.toml` & `deskaone_sdk_scrypt_2023-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deskaone-sdk-scrypt-2023"
-version = "1.0.4"
+version = "1.0.8"
 description = ""
 authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "deskaone_sdk_scrypt_2023", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Client/__init__.py` & `deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Database/__init__.py` & `deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py` & `deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Internal/__init__.py` & `deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Internal/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py` & `deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py` & `deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py` & `deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from .Color import Color
 from .Typer import Typer
 import random
 
 class ProgressBar:
     
     def __init__(self, iteration: int, total: int, prefix = '', suffix = '', decimals = 1, length = 100, fill = '█', printEnd = "\r", ending = '\n') -> None:        
@@ -21,8 +22,18 @@
         filledLength = int(length * iteration // total)
         color = [Color.WHITE, Color.RED, Color.GREEN, Color.BLUE, Color.CYAN, Color.MAGENTA, Color.YELLOW]
         normal = ' ' * (length - filledLength)
         bar = f'{color[random.randint(0, len(color) - 1)]}{fill * filledLength}{normal}'
         Typer.Print(f'\r{prefix} |{bar}{Color.WHITE}| {Color.GREEN}{percent}% {Color.WHITE}Progress', Refresh=True) if printEnd == '\r' else Typer.Print(f'\r{prefix} |{bar}{Color.WHITE}| {Color.GREEN}{percent}% {Color.WHITE}Progress', Enter=True)
         if iteration == total: 
             bar = f'{Color.GREEN}{fill * filledLength}{normal}'
-            Typer.Print(f'\r{prefix} |{bar}{Color.WHITE}| {Color.GREEN}{percent}% {Color.WHITE}{suffix}', Refresh=True) if ending == '\r' else Typer.Print(f'\r{prefix} |{bar}{Color.WHITE}| {Color.GREEN}{percent}% {Color.WHITE}{suffix}', Enter=True)
+            Typer.Print(f'\r{prefix} |{bar}{Color.WHITE}| {Color.GREEN}{percent}% {Color.WHITE}{suffix}', Refresh=True) if ending == '\r' else Typer.Print(f'\r{prefix} |{bar}{Color.WHITE}| {Color.GREEN}{percent}% {Color.WHITE}{suffix}', Enter=True)
+
+class ProgressWait:
+    
+    def __init__(self, Random: bool, Start = 0, End = 60) -> None:
+        if Random is True: items = list(range(0, random.randint(Start, End)))
+        else: items = list(range(Start, End))
+        ProgressBar(0, len(items), prefix = 'Please wait:', suffix = 'Complete', length = 25, ending = '\r')
+        for i, item in enumerate(items):
+            ProgressBar(i + 1, len(items), prefix = 'Please wait:', suffix = 'Complete', length = 25, ending = '\r')
+            time.sleep(1)
```

### Comparing `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py` & `deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from typing import Optional, Tuple
+from typing import Optional
+from bs4 import BeautifulSoup
 import requests, json, random, os
 from requests.exceptions import ConnectionError, ConnectTimeout, SSLError, RequestException, HTTPError, ProxyError, Timeout, ReadTimeout, JSONDecodeError, TooManyRedirects, ChunkedEncodingError
-from .Typer import Typer, Color
-from bs4 import BeautifulSoup
+from ..Typer import Typer, Color
 
 class WebShare:
     
     def __init__(self, Authorization: str) -> None:
         self.BASE_URL   = 'https://proxy.webshare.io/api/v2/'
         self.HEADERS    = dict(Authorization = Authorization)
         self.Session    = requests.Session()
     
     @property
     def __proxy__(self) -> list:
         URL     = self.BASE_URL + 'proxy/list/?mode=direct&page=1&page_size=100'
         return self.Session.get(URL, headers=self.HEADERS).json().get('results')
     
-    def Main(self, New: bool) -> dict:
+    def __save__(self, New: bool) -> dict:
         if os.path.exists('MyProxy') is False:
             os.mkdir('MyProxy')
         if os.path.exists('MyProxy/__init__.json') is False or New is True:
             if os.path.exists('MyProxy/__init__.json') is True:Dict = dict(json.load(open('MyProxy/__init__.json')))
             else:Dict = dict()
             for Proxy in self.__proxy__:
                 USERNAME        = Proxy.get('username')
@@ -32,20 +32,51 @@
                         f'{IP}:{PORT}'  : dict(
                         PROXY = dict(
                             http    = f'http://{USERNAME}:{PASSWORD}@{IP}:{PORT}',
                             https   = f'http://{USERNAME}:{PASSWORD}@{IP}:{PORT}',
                         ),
                         IpPort  = f'{IP}:{PORT}',
                     )})
-                except TypeError:pass
+                except:pass
             json.dump(Dict, open('MyProxy/__init__.json', 'w'))
         else:
             Dict = dict(json.load(open('MyProxy/__init__.json')))
         return Dict
 
+    
+    def Random(self, TIMEOUT: int, NEW: bool, IP_OLD_SAME: Optional[str] = None):
+        if os.path.exists('MyProxy/__init__.json') is True:os.unlink('MyProxy/__init__.json')
+        Proxys = self.__save__(NEW)
+        List = [v for k, v in zip(Proxys.keys(), Proxys.values())]
+        if len(List) != 0:
+            while True:
+                PROXY   = List[random.randint(0, len(List) - 1)]
+                if PROXY.get('IpPort') != IP_OLD_SAME or IP_OLD_SAME is None:
+                    try:
+                        API     = dict(requests.get("http://ip-api.com/json/%1s" % (PROXY.get('IpPort').split(":")[0])).json())
+                        Typer.Print(f'{Color.RED}=> {Color.WHITE}Mencoba Koneksi Proxy {Color.GREEN}{PROXY.get("IpPort")} {Color.WHITE}Country {Color.GREEN}{API.get("country")}', Refresh=True) 
+                        MYIP    = dict(requests.get("https://kin4u.com/test").json())
+                        S1 = requests.Session()
+                        CHECK   = dict(S1.get("https://kin4u.com/test", proxies=PROXY.get('PROXY'), timeout=TIMEOUT).json())
+                        if MYIP.get('HTTP_X_FORWARDED_FOR') != CHECK.get('HTTP_X_FORWARDED_FOR'):
+                            S1.close()
+                            return dict(
+                                PROXY   = PROXY.get('PROXY'),
+                                DATA    = API,
+                                IpPort  = PROXY.get('IpPort')
+                            )
+                    except ProxyError as e:pass
+                    except ConnectTimeout as e:pass
+                    except ConnectionError as e:pass
+                    except ReadTimeout as e:pass
+                    except JSONDecodeError:pass
+                    except TooManyRedirects as e:pass
+                    except Exception as e:pass
+        return None
+
 class ProxyScrape:
     
     def __init__(self) -> None:
         self.Session    = requests.Session()
     
     def __proxy__(self, Dict: dict):
         URL     = 'https://api.proxyscrape.com/v2/?request=displayproxies&protocol=http&timeout=5000&country=all&ssl=all&anonymity=all'
@@ -56,234 +87,88 @@
                     f'{Proxy}'  : dict(
                     PROXY = dict(
                         http    = f'http://{Proxy}',
                         https   = f'http://{Proxy}',
                     ),
                     IpPort  = f'{Proxy}',
                 )})
-            except TypeError:pass
+            except:pass
         
         URL     = 'https://api.proxyscrape.com/v2/?request=displayproxies&protocol=socks4&timeout=5000&country=all&ssl=all&anonymity=all'
         Result  = self.Session.get(URL).text
         for Proxy in Result.replace(' ', '').replace('\r', '').split('\n'):
             try:
                 Dict    = dict(**Dict, **{
                     f'{Proxy}'  : dict(
                     PROXY = dict(
                         http    = f'socks4://{Proxy}',
                         https   = f'socks4://{Proxy}',
                     ),
                     IpPort  = f'{Proxy}',
                 )}) 
-            except TypeError:pass
+            except:pass
         
         URL     = 'https://api.proxyscrape.com/v2/?request=displayproxies&protocol=socks5&timeout=5000&country=all&ssl=all&anonymity=all'
         Result  = self.Session.get(URL).text
         for Proxy in Result.replace(' ', '').replace('\r', '').split('\n'):
             try:
                 Dict    = dict(**Dict, **{
                     f'{Proxy}'  : dict(
                     PROXY = dict(
                         http    = f'socks5://{Proxy}',
                         https   = f'socks5://{Proxy}',
                     ),
                     IpPort  = f'{Proxy}',
                 )})
-            except TypeError:pass
-        return Dict
-    
-    def Main(self, New: bool) -> dict:
-        if os.path.exists('MyProxy') is False:
-            os.mkdir('MyProxy')
-        if os.path.exists('MyProxy/__init__.json') is False or New is True:
-            if os.path.exists('MyProxy/__init__.json') is True:
-                Dict = self.__proxy__(dict(json.load(open('MyProxy/__init__.json'))))
-            else:
-                Dict = self.__proxy__(dict())
-            json.dump(Dict, open('MyProxy/__init__.json', 'w'))
-        else:
-            Dict = dict(json.load(open('MyProxy/__init__.json')))
-        return Dict
-    
-class Geonode:
-    
-    def __init__(self) -> None:
-        self.Session    = requests.Session()
-        self.BASE_URL   = 'https://proxylist.geonode.com/api/proxy-list?limit=500&page=1&sort_by=lastChecked&sort_type=desc&speed=medium&protocols=http%2Chttps%2Csocks4%2Csocks5'
-    
-    def Main(self, New: bool) -> dict:
-        if os.path.exists('MyProxy') is False:
-            os.mkdir('MyProxy')
-        if os.path.exists('MyProxy/__init__.json') is False or New is True:
-            if os.path.exists('MyProxy/__init__.json') is True:
-                Dict = self.__proxy__(dict(json.load(open('MyProxy/__init__.json'))))
-            else:
-                Dict = self.__proxy__(dict())
-            json.dump(Dict, open('MyProxy/__init__.json', 'w'))
-        else:
-            Dict = dict(json.load(open('MyProxy/__init__.json')))
-        return Dict
-    
-    def __proxy__(self, Dict: dict):
-        Result  = self.Session.get(self.BASE_URL).json()
-        data    = list(Result.get('data'))
-        for List in data:
-            IP      = List.get('ip')
-            PORT    = List.get('port')
-            SCHEMA  = List.get('protocols')[0]
-            try:
-                Dict    = dict(**Dict, **{
-                    f'{IP}:{PORT}'  : dict(
-                    PROXY = dict(
-                        http    = f'{SCHEMA.lower()}://{IP}:{PORT}',
-                        https   = f'{SCHEMA.lower()}://{IP}:{PORT}',
-                    ),
-                    IpPort  = f'{IP}:{PORT}',
-                )})
-            except TypeError:pass
-        return Dict
-    
-class FreeProxyList:
-    
-    def __init__(self) -> None:
-        self.Session    = requests.Session()
-        self.BASE_URL   = 'https://free-proxy-list.net/'
-    
-    def __proxy__(self, Dict: dict):
-        r  = self.Session.get(self.BASE_URL)
-        Result = BeautifulSoup(r.content, 'html5lib')
-        for row in Result.findAll('tbody')[0].findAll('tr'):
-            SPLIT   = str(row).split('td>')
-            IP      = SPLIT[1].split('</')[0]
-            PORT    = SPLIT[3].split('</')[0]
-            try:
-                Dict    = dict(**Dict, **{
-                    f'{IP}:{PORT}'  : dict(
-                    PROXY = dict(
-                        http    = f'http://{IP}:{PORT}',
-                        https   = f'http://{IP}:{PORT}',
-                    ),
-                    IpPort  = f'{IP}:{PORT}',
-                )})
-            except TypeError:pass
+            except:pass
         return Dict
     
-    def Main(self, New: bool) -> dict:
+    def __save__(self, New: bool) -> dict:
         if os.path.exists('MyProxy') is False:
             os.mkdir('MyProxy')
         if os.path.exists('MyProxy/__init__.json') is False or New is True:
             if os.path.exists('MyProxy/__init__.json') is True:
                 Dict = self.__proxy__(dict(json.load(open('MyProxy/__init__.json'))))
             else:
                 Dict = self.__proxy__(dict())
             json.dump(Dict, open('MyProxy/__init__.json', 'w'))
         else:
             Dict = dict(json.load(open('MyProxy/__init__.json')))
         return Dict
-    
-class ProxyList:
-    
-    def __init__(self) -> None:
-        self.Session    = requests.Session()
-        
-    def __http__(self, Dict: dict):
-        r  = self.Session.get('https://www.proxy-list.download/HTTP')
-        Result = BeautifulSoup(r.content, 'html5lib')
-        for row in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr'):
-            SPLIT   = str(row).split('td>')
-            IP      = SPLIT[1].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
-            PORT    = SPLIT[3].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
-            try:
-                Dict    = dict(**Dict, **{
-                    f'{IP}:{PORT}'  : dict(
-                    PROXY = dict(
-                        http    = f'http://{IP}:{PORT}',
-                        https   = f'http://{IP}:{PORT}',
-                    ),
-                    IpPort  = f'{IP}:{PORT}',
-                )})
-            except TypeError:pass
-        return Dict
-        
-    def __https__(self, Dict: dict):
-        r  = self.Session.get('https://www.proxy-list.download/HTTPS')
-        Result = BeautifulSoup(r.content, 'html5lib')
-        for row in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr'):
-            SPLIT   = str(row).split('td>')
-            IP      = SPLIT[1].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
-            PORT    = SPLIT[3].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
-            try:
-                Dict    = dict(**Dict, **{
-                    f'{IP}:{PORT}'  : dict(
-                    PROXY = dict(
-                        http    = f'http://{IP}:{PORT}',
-                        https   = f'http://{IP}:{PORT}',
-                    ),
-                    IpPort  = f'{IP}:{PORT}',
-                )})
-            except TypeError:pass
-        return Dict
         
-    def __socks4__(self, Dict: dict):
-        r  = self.Session.get('https://www.proxy-list.download/SOCKS4')
-        Result = BeautifulSoup(r.content, 'html5lib')
-        for row in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr'):
-            SPLIT   = str(row).split('td>')
-            IP      = SPLIT[1].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
-            PORT    = SPLIT[3].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
-            try:
-                Dict    = dict(**Dict, **{
-                    f'{IP}:{PORT}'  : dict(
-                    PROXY = dict(
-                        http    = f'socks4://{IP}:{PORT}',
-                        https   = f'socks4://{IP}:{PORT}',
-                    ),
-                    IpPort  = f'{IP}:{PORT}',
-                )})
-            except TypeError:pass
-        return Dict
-        
-    def __socks5__(self, Dict: dict):
-        r  = self.Session.get('https://www.proxy-list.download/SOCKS5')
-        Result = BeautifulSoup(r.content, 'html5lib')
-        for row in Result.findAll('tbody', attrs={'id': 'tabli'})[0].findAll('tr'):
-            SPLIT   = str(row).split('td>')
-            IP      = SPLIT[1].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
-            PORT    = SPLIT[3].replace(' ', '').replace('\n', '').replace('\r', '').split('</')[0]
-            try:
-                Dict    = dict(**Dict, **{
-                    f'{IP}:{PORT}'  : dict(
-                    PROXY = dict(
-                        http    = f'socks5://{IP}:{PORT}',
-                        https   = f'socks5://{IP}:{PORT}',
-                    ),
-                    IpPort  = f'{IP}:{PORT}',
-                )})
-            except TypeError:pass
-        return Dict
-    
-    def __proxy__(self, Dict: dict):
-        Dict = self.__http__(Dict)
-        Dict = self.__https__(Dict)
-        Dict = self.__socks4__(Dict)
-        Dict = self.__socks5__(Dict)
-        return Dict
     
-    def Main(self, New: bool) -> dict:
-        if os.path.exists('MyProxy') is False:
-            os.mkdir('MyProxy')
-        if os.path.exists('MyProxy/__init__.json') is False or New is True:
-            if os.path.exists('MyProxy/__init__.json') is True:
-                Dict = self.__proxy__(dict(json.load(open('MyProxy/__init__.json'))))
-            else:
-                Dict = self.__proxy__(dict())
-            json.dump(Dict, open('MyProxy/__init__.json', 'w'))
-        else:
-            Dict = dict(json.load(open('MyProxy/__init__.json')))
-        return Dict
+    def Random(self, TIMEOUT: int, NEW: bool, IP_OLD_SAME: Optional[str] = None):
+        if os.path.exists('MyProxy/__init__.json') is True:os.unlink('MyProxy/__init__.json')
+        Proxys = self.__save__(NEW)
+        List = [v for k, v in zip(Proxys.keys(), Proxys.values())]
+        if len(List) != 0:
+            while True:
+                PROXY   = List[random.randint(0, len(List) - 1)]
+                if PROXY.get('IpPort') != IP_OLD_SAME or IP_OLD_SAME is None:
+                    try:
+                        API     = dict(requests.get("http://ip-api.com/json/%1s" % (PROXY.get('IpPort').split(":")[0])).json())
+                        Typer.Print(f'{Color.RED}=> {Color.WHITE}Mencoba Koneksi Proxy {Color.GREEN}{PROXY.get("IpPort")} {Color.WHITE}Country {Color.GREEN}{API.get("country")}', Refresh=True) 
+                        MYIP    = dict(requests.get("https://kin4u.com/test").json())
+                        S1 = requests.Session()
+                        CHECK   = dict(S1.get("https://kin4u.com/test", proxies=PROXY.get('PROXY'), timeout=TIMEOUT).json())
+                        if MYIP.get('HTTP_X_FORWARDED_FOR') != CHECK.get('HTTP_X_FORWARDED_FOR'):
+                            S1.close()
+                            return dict(
+                                PROXY   = PROXY.get('PROXY'),
+                                DATA    = API,
+                                IpPort  = PROXY.get('IpPort')
+                            )
+                    except ProxyError as e:pass
+                    except ConnectTimeout as e:pass
+                    except ConnectionError as e:pass
+                    except ReadTimeout as e:pass
+                    except JSONDecodeError:pass
+                    except TooManyRedirects as e:pass
+                    except Exception as e:pass
+        return None
 
 class HideMy:
     
     def First(self):
         URL = 'https://hidemy.name/en/proxy-list/'
         r = requests.get(URL, headers={'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36'})
         return BeautifulSoup(r.content, 'html5lib')
@@ -316,74 +201,71 @@
                     URL = 'https://hidemy.name/en/proxy-list/?' + page.find('li', attrs = {'class':'next_array'}).a['href'].split('?')[1]
                     r = requests.get(URL, headers={'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36'})
                     SOUP = BeautifulSoup(r.content, 'html5lib')
                     Dict    = self.ParseTable(Dict)
             except:pass
         return Dict
     
-    def Main(self, New: bool) -> dict:
+    def __save__(self, New: bool) -> dict:
         if os.path.exists('MyProxy') is False:
             os.mkdir('MyProxy')
         if os.path.exists('MyProxy/__init__.json') is False or New is True:
             if os.path.exists('MyProxy/__init__.json') is True:
                 Dict = self.ParseTable(dict(json.load(open('MyProxy/__init__.json'))))
             else:
                 Dict = self.ParseTable(dict())
             json.dump(Dict, open('MyProxy/__init__.json', 'w'))
         else:
             Dict = dict(json.load(open('MyProxy/__init__.json')))
         return Dict
+    
+    def Random(self, TIMEOUT: int, NEW: bool, IP_OLD_SAME: Optional[str] = None):
+        if os.path.exists('MyProxy/__init__.json') is True:os.unlink('MyProxy/__init__.json')
+        Proxys = self.__save__(NEW)
+        List = [v for k, v in zip(Proxys.keys(), Proxys.values())]
+        if len(List) != 0:
+            while True:
+                PROXY   = List[random.randint(0, len(List) - 1)]
+                if PROXY.get('IpPort') != IP_OLD_SAME or IP_OLD_SAME is None:
+                    try:
+                        API     = dict(requests.get("http://ip-api.com/json/%1s" % (PROXY.get('IpPort').split(":")[0])).json())
+                        Typer.Print(f'{Color.RED}=> {Color.WHITE}Mencoba Koneksi Proxy {Color.GREEN}{PROXY.get("IpPort")} {Color.WHITE}Country {Color.GREEN}{API.get("country")}', Refresh=True) 
+                        MYIP    = dict(requests.get("https://kin4u.com/test").json())
+                        S1 = requests.Session()
+                        CHECK   = dict(S1.get("https://kin4u.com/test", proxies=PROXY.get('PROXY'), timeout=TIMEOUT).json())
+                        if MYIP.get('HTTP_X_FORWARDED_FOR') != CHECK.get('HTTP_X_FORWARDED_FOR'):
+                            S1.close()
+                            return dict(
+                                PROXY   = PROXY.get('PROXY'),
+                                DATA    = API,
+                                IpPort  = PROXY.get('IpPort')
+                            )
+                    except ProxyError as e:pass
+                    except ConnectTimeout as e:pass
+                    except ConnectionError as e:pass
+                    except ReadTimeout as e:pass
+                    except JSONDecodeError:pass
+                    except TooManyRedirects as e:pass
+                    except Exception as e:pass
+        return None
 
-class Proxy:
+class MyProxy:
+    
+    def __init__(self, TIMEOUT: int, NEW: bool, IP_OLD_SAME: Optional[str] = None, Authorization: Optional[str] = None) -> None:
+        RANDOM, WebShares = random.randint(0, 2), False
+        if RANDOM == 0:
+            if Authorization is not None:
+                Proxy = WebShare(Authorization=Authorization).Random(TIMEOUT, NEW, IP_OLD_SAME)
+                if Proxy is None:WebShares = False
+                else:self.Proxy, WebShares = Proxy, True
+        if WebShares is False:
+            if RANDOM == 1:
+                self.Proxy = ProxyScrape().Random(TIMEOUT, NEW, IP_OLD_SAME)
+            else:
+                self.Proxy = HideMy().Random(TIMEOUT, NEW, IP_OLD_SAME)
     
-    def __init__(self, Authorization: Optional[str] = None, *args, **kwargs) -> None:
-        self.__get__(Authorization, True, **kwargs)
+    def __repr__(self) -> str:
+        return json.dumps(self.Proxy, indent=4)
     
-    def __get__(self, Authorization: Optional[str] = None, New = True, *args, **kwargs):
-        self.List   = list()
-        if Authorization is not None:
-            A1 = WebShare(Authorization).Main(New)
-            for k, v in zip(A1.keys(), A1.values()):self.List.append(v)
-        if kwargs.get('ProxyScrape') is True or kwargs.get('ProxyScrape') is None:
-            A2  = ProxyScrape().Main(New)
-            for k, v in zip(A2.keys(), A2.values()):self.List.append(v)
-        if kwargs.get('Geonode') is True or kwargs.get('Geonode') is None:
-            A3  = Geonode().Main(New)
-            for k, v in zip(A3.keys(), A3.values()):self.List.append(v)
-        if kwargs.get('FreeProxyList') is True or kwargs.get('FreeProxyList') is None:
-            A4  = FreeProxyList().Main(New)
-            for k, v in zip(A4.keys(), A4.values()):self.List.append(v)
-        if kwargs.get('ProxyList') is True or kwargs.get('ProxyList') is None:
-            A5  = ProxyList().Main(New)
-            for k, v in zip(A5.keys(), A5.values()):self.List.append(v)
-        if kwargs.get('HideMy') is True or kwargs.get('HideMy') is None:
-            A6  = HideMy().Main(New)
-            for k, v in zip(A6.keys(), A6.values()):self.List.append(v)
     
-    def __check__(self):
-        while True:
-            try:
-                PROXY   = self.List[random.randint(0, len(self.List) - 1)]
-                API     = dict(requests.get("http://ip-api.com/json/%1s" % (PROXY.get('IpPort').split(":")[0])).json())
-                Typer.Print(f'{Color.RED}=> {Color.WHITE}Check New Proxy {Color.GREEN}{PROXY.get("IpPort")} {Color.WHITE}Country {Color.GREEN}{API.get("country")}', Refresh=True) 
-                MYIP    = dict(requests.get("https://kin4u.com/test").json())
-                S1 = requests.Session()
-                CHECK   = dict(S1.get("https://kin4u.com/test", proxies=PROXY.get('PROXY'), timeout=15).json())
-                if MYIP.get('HTTP_X_FORWARDED_FOR') != CHECK.get('HTTP_X_FORWARDED_FOR'):
-                    S1.close()
-                    return dict(
-                        PROXY   = PROXY.get('PROXY'),
-                        DATA    = API,
-                        IpPort  = PROXY.get('IpPort')
-                    )
-            except ProxyError as e:pass
-            except ConnectTimeout as e:pass
-            except ConnectionError as e:pass
-            except ReadTimeout as e:pass
-            except JSONDecodeError:pass
-            except TooManyRedirects as e:pass
-            except Exception as e:pass
-    
-    def Generate(self) -> Tuple[bool, dict]:
-        if len(self.List) != 0:return True,  self.__check__()
-        return False, dict()
-                
+        
+
```

### Comparing `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Random.py` & `deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/Random.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Timer.py` & `deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/Timer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/Typer.py` & `deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/Typer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.4/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py` & `deskaone_sdk_scrypt_2023-1.0.8/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.0.4/setup.py` & `deskaone_sdk_scrypt_2023-1.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  'python-dotenv>=1.0.0,<2.0.0',
  'random-user-agent>=1.0.1,<2.0.0',
  'requests[socks]>=2.28.2,<3.0.0',
  'sqlalchemy==1.4.29']
 
 setup_kwargs = {
     'name': 'deskaone-sdk-scrypt-2023',
-    'version': '1.0.4',
+    'version': '1.0.8',
     'description': '',
     'long_description': 'xxxxxxxxxxxxxxxx',
     'author': 'Antoni Oktha Fernandes',
     'author_email': '37358597+DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `deskaone_sdk_scrypt_2023-1.0.4/PKG-INFO` & `deskaone_sdk_scrypt_2023-1.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deskaone-sdk-scrypt-2023
-Version: 1.0.4
+Version: 1.0.8
 Summary: 
 Author: Antoni Oktha Fernandes
 Author-email: 37358597+DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

