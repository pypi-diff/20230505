# Comparing `tmp/openai_forward-0.1.5.tar.gz` & `tmp/openai_forward-0.1.6.tar.gz`

## Comparing `openai_forward-0.1.5.tar` & `openai_forward-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/__main__.py
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/_base.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/app.py
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/config.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/content/__init__.py
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/content/chat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/content/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/routers/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/routers/openai_v1.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openai_forward-0.1.5/openai_forward/routers/schemas.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 openai_forward-0.1.5/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.5/LICENSE
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 openai_forward-0.1.5/README.md
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 openai_forward-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 openai_forward-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/__init__.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/__main__.py
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/_base.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/app.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/config.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/content/chat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/content/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/routers/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/routers/openai_v1.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/routers/schemas.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 openai_forward-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.6/LICENSE
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 openai_forward-0.1.6/README.md
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 openai_forward-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 openai_forward-0.1.6/PKG-INFO
```

### Comparing `openai_forward-0.1.5/openai_forward/_base.py` & `openai_forward-0.1.6/openai_forward/_base.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.5/openai_forward/app.py` & `openai_forward-0.1.6/openai_forward/app.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.5/openai_forward/config.py` & `openai_forward-0.1.6/openai_forward/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,27 +21,30 @@
         frame, depth = logging.currentframe(), 2
         while frame.f_code.co_filename == logging.__file__:
             frame = frame.f_back
             depth += 1
         logger.opt(depth=depth, exception=record.exc_info).log(level, record.getMessage())
 
 
-def setting_log(log_name, multi_process=True, time_zone='Asia/Shanghai'):
+def setting_log(log_name, multi_process=True):
     # TODO 修复时区配置
+    time_zone = os.environ.get("TZ")
+    print(f"{time_zone=}")
     if time_zone == "Asia/Shanghai":
         import datetime
         tz = pytz.timezone(time_zone)
         loc_dt = tz.localize(datetime.datetime.now())
         offset = loc_dt.utcoffset()
         # tzname, offset = loc_dt.strftime("%Z::%z").split("::")
         # offset = loc_dt.strftime("%z")
         # os.environ['TZ'] = f"UTC-{offset}"
         os.environ['TZ'] = f"UTC-8"
-        print(os.environ['TZ'])
-        time.tzset()
+        if hasattr(time, 'tzset'):
+            print(os.environ['TZ'])
+            time.tzset()
 
     logging.root.handlers = [InterceptHandler()]
     for name in logging.root.manager.loggerDict.keys():
         logging.getLogger(name).handlers = []
         logging.getLogger(name).propagate = True
     logger_config = {
         "handlers": [
```

### Comparing `openai_forward-0.1.5/openai_forward/openai.py` & `openai_forward-0.1.6/openai_forward/openai.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.5/openai_forward/content/chat.py` & `openai_forward-0.1.6/openai_forward/content/chat.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.5/openai_forward/routers/schemas.py` & `openai_forward-0.1.6/openai_forward/routers/schemas.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.5/.gitignore` & `openai_forward-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.5/LICENSE` & `openai_forward-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.5/README.md` & `openai_forward-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,21 +30,22 @@
     <a href="https://pypi.org/project/openai_forward/">
         <img alt="pypi downloads" src="https://img.shields.io/pypi/dm/openai_forward">
     </a>
 
 </p>
 This project is designed to solve the problem of some regions being unable to directly access OpenAI. The service is deployed on a server that can access the OpenAI API, and OpenAI requests are forwarded through the service, i.e. a reverse proxy service is set up. 
 
-Test access: https://caloi.top/v1/chat/completions is equivalent to https://api.openai.com/v1/chat/completions
+Test access: https://caloi.top/openai/v1/chat/completions is equivalent to https://api.openai.com/v1/chat/completions  
+Or, to put it another way, https://caloi.top/openai is equivalent to https://api.openai.com.
 
 # Table of Contents
 
 - [Features](#Features)
 - [Usage](#Usage)
-- [Service Deployment](#Service-Deployment)
+- [Deploy](#Deploy)
 - [Service Usage](#Service-Usage)
 - [Configuration](#Configuration)
 
 # Features
 
 - [x] Supports forwarding of all OpenAI interfaces
 - [x] Request IP verification
@@ -53,43 +54,43 @@
 - [x] pip installation and deployment
 - [x] Docker deployment
 - [x] Support for multiple worker processes
 - [x] Support for specifying the forwarding routing prefix
 
 # Usage
 
-> Here, the proxy address set up by the individual, https://caloi.top, is used as an example
+> Here, the proxy address set up by the individual, https://caloi.top/openai, is used as an example
 
 ### Using in a module
 
 
 **Python**
 
 ```diff
   import openai
-+ openai.api_base = "https://caloi.top/v1"
++ openai.api_base = "https://caloi.top/openai/v1"
   openai.api_key = "sk-******"
 ```
 
 **JS/TS**
 
 ```diff
   import { Configuration } from "openai";
   
   const configuration = new Configuration({
-+ basePath: "https://caloi.top/v1",
++ basePath: "https://caloi.top/openai/v1",
   apiKey: "sk-******",
   });
 ```
 
 
 ### Image Generation (DALL-E):
 
 ```bash 
-curl --location 'https://caloi.top/v1/images/generations' \ 
+curl --location 'https://caloi.top/openai/v1/images/generations' \ 
 --header 'Authorization: Bearer sk-******' \ 
 --header 'Content-Type: application/json' \ 
 --data '{ 
     "prompt": "A photo of a cat", 
     "n": 1, 
     "size": "512x512"
 }' 
@@ -97,28 +98,29 @@
 
 ### [chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web)
 
 Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/Chanzhaoyu/chatgpt-web#docker-compose) to the
 address of the proxy service we set up:
 
 ```bash 
-OPENAI_API_BASE_URL: https://caloi.top 
+OPENAI_API_BASE_URL: https://caloi.top/openai 
 ``` 
 
 ### [ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)
 
 Replace `BASE_URL` in the docker startup command with the address of the proxy service we set up:
 
 ```bash 
-docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="<your password>" -e BASE_URL="caloi.top" yidadaa/chatgpt-next-web 
+docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="<your password>" -e BASE_URL="caloi.top/openai" yidadaa/chatgpt-next-web 
 ``` 
 
-# Service Deployment
 
-Two service deployment methods are provided, choose one
+# Deploy
+
+Two deployment methods are provided, just choose one.
 
 ## Use `pip`  (recommended)
 
 **Installation**
 
 ```bash 
 pip install openai-forward
```

#### html2text {}

```diff
@@ -5,44 +5,46 @@
                         OpenAI API æ¥å£è½¬åæå¡
                 The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
                      image_size] [tests] [pypi_downloads]
 This project is designed to solve the problem of some regions being unable to
 directly access OpenAI. The service is deployed on a server that can access the
 OpenAI API, and OpenAI requests are forwarded through the service, i.e. a
-reverse proxy service is set up. Test access: https://caloi.top/v1/chat/
-completions is equivalent to https://api.openai.com/v1/chat/completions # Table
-of Contents - [Features](#Features) - [Usage](#Usage) - [Service Deployment]
-(#Service-Deployment) - [Service Usage](#Service-Usage) - [Configuration]
+reverse proxy service is set up. Test access: https://caloi.top/openai/v1/chat/
+completions is equivalent to https://api.openai.com/v1/chat/completions Or, to
+put it another way, https://caloi.top/openai is equivalent to https://
+api.openai.com. # Table of Contents - [Features](#Features) - [Usage](#Usage) -
+[Deploy](#Deploy) - [Service Usage](#Service-Usage) - [Configuration]
 (#Configuration) # Features - [x] Supports forwarding of all OpenAI interfaces
 - [x] Request IP verification - [x] Streaming Response - [x] Supports default
 API key (cyclic call with multiple API keys) - [x] pip installation and
 deployment - [x] Docker deployment - [x] Support for multiple worker processes
 - [x] Support for specifying the forwarding routing prefix # Usage > Here, the
-proxy address set up by the individual, https://caloi.top, is used as an
+proxy address set up by the individual, https://caloi.top/openai, is used as an
 example ### Using in a module **Python** ```diff import openai +
-openai.api_base = "https://caloi.top/v1" openai.api_key = "sk-******" ``` **JS/
-TS** ```diff import { Configuration } from "openai"; const configuration = new
-Configuration({ + basePath: "https://caloi.top/v1", apiKey: "sk-******", });
-``` ### Image Generation (DALL-E): ```bash curl --location 'https://caloi.top/
-v1/images/generations' \ --header 'Authorization: Bearer sk-******' \ --header
-'Content-Type: application/json' \ --data '{ "prompt": "A photo of a cat", "n":
-1, "size": "512x512" }' ``` ### [chatgpt-web](https://github.com/Chanzhaoyu/
-chatgpt-web) Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://
-github.com/Chanzhaoyu/chatgpt-web#docker-compose) to the address of the proxy
-service we set up: ```bash OPENAI_API_BASE_URL: https://caloi.top ``` ###
-[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web) Replace
-`BASE_URL` in the docker startup command with the address of the proxy service
-we set up: ```bash docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -
-e CODE="" -e BASE_URL="caloi.top" yidadaa/chatgpt-next-web ``` # Service
-Deployment Two service deployment methods are provided, choose one ## Use `pip`
-(recommended) **Installation** ```bash pip install openai-forward ``` **Run
-forwarding service** The port number can be specified through `--port`, which
-defaults to `8000`, and the number of worker processes can be specified through
-`--workers`, which defaults to `1`. ```bash openai_forward run --port=9999 --
+openai.api_base = "https://caloi.top/openai/v1" openai.api_key = "sk-******"
+``` **JS/TS** ```diff import { Configuration } from "openai"; const
+configuration = new Configuration({ + basePath: "https://caloi.top/openai/v1",
+apiKey: "sk-******", }); ``` ### Image Generation (DALL-E): ```bash curl --
+location 'https://caloi.top/openai/v1/images/generations' \ --header
+'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
+--data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` ###
+[chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web) Modify the
+`OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/Chanzhaoyu/
+chatgpt-web#docker-compose) to the address of the proxy service we set up:
+```bash OPENAI_API_BASE_URL: https://caloi.top/openai ``` ### [ChatGPT-Next-
+Web](https://github.com/Yidadaa/ChatGPT-Next-Web) Replace `BASE_URL` in the
+docker startup command with the address of the proxy service we set up: ```bash
+docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="" -
+e BASE_URL="caloi.top/openai" yidadaa/chatgpt-next-web ``` # Deploy Two
+deployment methods are provided, just choose one. ## Use `pip` (recommended)
+**Installation** ```bash pip install openai-forward ``` **Run forwarding
+service** The port number can be specified through `--port`, which defaults to
+`8000`, and the number of worker processes can be specified through `--
+workers`, which defaults to `1`. ```bash openai_forward run --port=9999 --
 workers=1 ``` The service is now set up, and the usage is to replace `https://
 api.openai.com` with the port number of the service `http://{ip}:{port}`. Of
 course, OPENAI_API_KEY can also be passed in as an environment variable as the
 default API key, so that the client does not need to pass in the Authorization
 in the header when requesting the relevant route. Startup command with default
 API key: ```bash OPENAI_API_KEY="sk-xxx" openai_forward run --port=9999 --
 workers=1 ``` Note: If both the default API key and the API key passed in the
```

### Comparing `openai_forward-0.1.5/pyproject.toml` & `openai_forward-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.5/PKG-INFO` & `openai_forward-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_forward
-Version: 0.1.5
+Version: 0.1.6
 Summary: 🚀 Openai api forward · OpenAI 接口转发服务 · streaming forward
 Project-URL: Homepage, https://github.com/beidongjiedeguang/openai-forward
 Project-URL: Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-forward
 Project-URL: Issues, https://github.com/beidongjiedeguang/openai-forward/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/openai-forward
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-File: LICENSE
@@ -63,21 +63,22 @@
     <a href="https://pypi.org/project/openai_forward/">
         <img alt="pypi downloads" src="https://img.shields.io/pypi/dm/openai_forward">
     </a>
 
 </p>
 This project is designed to solve the problem of some regions being unable to directly access OpenAI. The service is deployed on a server that can access the OpenAI API, and OpenAI requests are forwarded through the service, i.e. a reverse proxy service is set up. 
 
-Test access: https://caloi.top/v1/chat/completions is equivalent to https://api.openai.com/v1/chat/completions
+Test access: https://caloi.top/openai/v1/chat/completions is equivalent to https://api.openai.com/v1/chat/completions  
+Or, to put it another way, https://caloi.top/openai is equivalent to https://api.openai.com.
 
 # Table of Contents
 
 - [Features](#Features)
 - [Usage](#Usage)
-- [Service Deployment](#Service-Deployment)
+- [Deploy](#Deploy)
 - [Service Usage](#Service-Usage)
 - [Configuration](#Configuration)
 
 # Features
 
 - [x] Supports forwarding of all OpenAI interfaces
 - [x] Request IP verification
@@ -86,43 +87,43 @@
 - [x] pip installation and deployment
 - [x] Docker deployment
 - [x] Support for multiple worker processes
 - [x] Support for specifying the forwarding routing prefix
 
 # Usage
 
-> Here, the proxy address set up by the individual, https://caloi.top, is used as an example
+> Here, the proxy address set up by the individual, https://caloi.top/openai, is used as an example
 
 ### Using in a module
 
 
 **Python**
 
 ```diff
   import openai
-+ openai.api_base = "https://caloi.top/v1"
++ openai.api_base = "https://caloi.top/openai/v1"
   openai.api_key = "sk-******"
 ```
 
 **JS/TS**
 
 ```diff
   import { Configuration } from "openai";
   
   const configuration = new Configuration({
-+ basePath: "https://caloi.top/v1",
++ basePath: "https://caloi.top/openai/v1",
   apiKey: "sk-******",
   });
 ```
 
 
 ### Image Generation (DALL-E):
 
 ```bash 
-curl --location 'https://caloi.top/v1/images/generations' \ 
+curl --location 'https://caloi.top/openai/v1/images/generations' \ 
 --header 'Authorization: Bearer sk-******' \ 
 --header 'Content-Type: application/json' \ 
 --data '{ 
     "prompt": "A photo of a cat", 
     "n": 1, 
     "size": "512x512"
 }' 
@@ -130,28 +131,29 @@
 
 ### [chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web)
 
 Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/Chanzhaoyu/chatgpt-web#docker-compose) to the
 address of the proxy service we set up:
 
 ```bash 
-OPENAI_API_BASE_URL: https://caloi.top 
+OPENAI_API_BASE_URL: https://caloi.top/openai 
 ``` 
 
 ### [ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web)
 
 Replace `BASE_URL` in the docker startup command with the address of the proxy service we set up:
 
 ```bash 
-docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="<your password>" -e BASE_URL="caloi.top" yidadaa/chatgpt-next-web 
+docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="<your password>" -e BASE_URL="caloi.top/openai" yidadaa/chatgpt-next-web 
 ``` 
 
-# Service Deployment
 
-Two service deployment methods are provided, choose one
+# Deploy
+
+Two deployment methods are provided, just choose one.
 
 ## Use `pip`  (recommended)
 
 **Installation**
 
 ```bash 
 pip install openai-forward
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openai_forward Version: 0.1.5 Summary: ð Openai
+Metadata-Version: 2.1 Name: openai_forward Version: 0.1.6 Summary: ð Openai
 api forward Â· OpenAI æ¥å£è½¬åæå¡ Â· streaming forward Project-URL:
 Homepage, https://github.com/beidongjiedeguang/openai-forward Project-URL:
 Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-
 forward Project-URL: Issues, https://github.com/beidongjiedeguang/openai-
 forward/issues Project-URL: Source, https://github.com/beidongjiedeguang/
 openai-forward Author-email: kunyuan
 gmail.com> License-File: LICENSE Keywords:
@@ -23,44 +23,46 @@
                         OpenAI API æ¥å£è½¬åæå¡
                 The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
                      image_size] [tests] [pypi_downloads]
 This project is designed to solve the problem of some regions being unable to
 directly access OpenAI. The service is deployed on a server that can access the
 OpenAI API, and OpenAI requests are forwarded through the service, i.e. a
-reverse proxy service is set up. Test access: https://caloi.top/v1/chat/
-completions is equivalent to https://api.openai.com/v1/chat/completions # Table
-of Contents - [Features](#Features) - [Usage](#Usage) - [Service Deployment]
-(#Service-Deployment) - [Service Usage](#Service-Usage) - [Configuration]
+reverse proxy service is set up. Test access: https://caloi.top/openai/v1/chat/
+completions is equivalent to https://api.openai.com/v1/chat/completions Or, to
+put it another way, https://caloi.top/openai is equivalent to https://
+api.openai.com. # Table of Contents - [Features](#Features) - [Usage](#Usage) -
+[Deploy](#Deploy) - [Service Usage](#Service-Usage) - [Configuration]
 (#Configuration) # Features - [x] Supports forwarding of all OpenAI interfaces
 - [x] Request IP verification - [x] Streaming Response - [x] Supports default
 API key (cyclic call with multiple API keys) - [x] pip installation and
 deployment - [x] Docker deployment - [x] Support for multiple worker processes
 - [x] Support for specifying the forwarding routing prefix # Usage > Here, the
-proxy address set up by the individual, https://caloi.top, is used as an
+proxy address set up by the individual, https://caloi.top/openai, is used as an
 example ### Using in a module **Python** ```diff import openai +
-openai.api_base = "https://caloi.top/v1" openai.api_key = "sk-******" ``` **JS/
-TS** ```diff import { Configuration } from "openai"; const configuration = new
-Configuration({ + basePath: "https://caloi.top/v1", apiKey: "sk-******", });
-``` ### Image Generation (DALL-E): ```bash curl --location 'https://caloi.top/
-v1/images/generations' \ --header 'Authorization: Bearer sk-******' \ --header
-'Content-Type: application/json' \ --data '{ "prompt": "A photo of a cat", "n":
-1, "size": "512x512" }' ``` ### [chatgpt-web](https://github.com/Chanzhaoyu/
-chatgpt-web) Modify the `OPENAI_API_BASE_URL` in [Docker Compose](https://
-github.com/Chanzhaoyu/chatgpt-web#docker-compose) to the address of the proxy
-service we set up: ```bash OPENAI_API_BASE_URL: https://caloi.top ``` ###
-[ChatGPT-Next-Web](https://github.com/Yidadaa/ChatGPT-Next-Web) Replace
-`BASE_URL` in the docker startup command with the address of the proxy service
-we set up: ```bash docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -
-e CODE="" -e BASE_URL="caloi.top" yidadaa/chatgpt-next-web ``` # Service
-Deployment Two service deployment methods are provided, choose one ## Use `pip`
-(recommended) **Installation** ```bash pip install openai-forward ``` **Run
-forwarding service** The port number can be specified through `--port`, which
-defaults to `8000`, and the number of worker processes can be specified through
-`--workers`, which defaults to `1`. ```bash openai_forward run --port=9999 --
+openai.api_base = "https://caloi.top/openai/v1" openai.api_key = "sk-******"
+``` **JS/TS** ```diff import { Configuration } from "openai"; const
+configuration = new Configuration({ + basePath: "https://caloi.top/openai/v1",
+apiKey: "sk-******", }); ``` ### Image Generation (DALL-E): ```bash curl --
+location 'https://caloi.top/openai/v1/images/generations' \ --header
+'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
+--data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` ###
+[chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web) Modify the
+`OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/Chanzhaoyu/
+chatgpt-web#docker-compose) to the address of the proxy service we set up:
+```bash OPENAI_API_BASE_URL: https://caloi.top/openai ``` ### [ChatGPT-Next-
+Web](https://github.com/Yidadaa/ChatGPT-Next-Web) Replace `BASE_URL` in the
+docker startup command with the address of the proxy service we set up: ```bash
+docker run -d -p 3000:3000 -e OPENAI_API_KEY="sk-******" -e CODE="" -
+e BASE_URL="caloi.top/openai" yidadaa/chatgpt-next-web ``` # Deploy Two
+deployment methods are provided, just choose one. ## Use `pip` (recommended)
+**Installation** ```bash pip install openai-forward ``` **Run forwarding
+service** The port number can be specified through `--port`, which defaults to
+`8000`, and the number of worker processes can be specified through `--
+workers`, which defaults to `1`. ```bash openai_forward run --port=9999 --
 workers=1 ``` The service is now set up, and the usage is to replace `https://
 api.openai.com` with the port number of the service `http://{ip}:{port}`. Of
 course, OPENAI_API_KEY can also be passed in as an environment variable as the
 default API key, so that the client does not need to pass in the Authorization
 in the header when requesting the relevant route. Startup command with default
 API key: ```bash OPENAI_API_KEY="sk-xxx" openai_forward run --port=9999 --
 workers=1 ``` Note: If both the default API key and the API key passed in the
```

