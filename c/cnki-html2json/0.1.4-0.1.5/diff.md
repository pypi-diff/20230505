# Comparing `tmp/cnki_html2json-0.1.4.tar.gz` & `tmp/cnki_html2json-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnki_html2json-0.1.4.tar", last modified: Tue Apr 25 04:38:40 2023, max compression
+gzip compressed data, was "cnki_html2json-0.1.5.tar", last modified: Fri May  5 17:58:22 2023, max compression
```

## Comparing `cnki_html2json-0.1.4.tar` & `cnki_html2json-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:38:40.169607 cnki_html2json-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-04-25 04:38:40.169607 cnki_html2json-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:38:40.165607 cnki_html2json-0.1.4/cnki_html2json/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/cnki_html2json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/cnki_html2json/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/cnki_html2json/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11899 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/cnki_html2json/html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/cnki_html2json/parse_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/cnki_html2json/recognize_slider_coordinate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:38:40.169607 cnki_html2json-0.1.4/cnki_html2json.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-04-25 04:38:40.000000 cnki_html2json-0.1.4/cnki_html2json.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-25 04:38:40.000000 cnki_html2json-0.1.4/cnki_html2json.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:38:40.000000 cnki_html2json-0.1.4/cnki_html2json.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 04:38:40.000000 cnki_html2json-0.1.4/cnki_html2json.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-25 04:38:40.000000 cnki_html2json-0.1.4/cnki_html2json.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 04:38:40.000000 cnki_html2json-0.1.4/cnki_html2json.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 04:38:40.169607 cnki_html2json-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:38:40.169607 cnki_html2json-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/tests/test_html2json.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-25 04:38:29.000000 cnki_html2json-0.1.4/tests/test_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:58:22.071276 cnki_html2json-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-05-05 17:58:22.071276 cnki_html2json-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:58:22.071276 cnki_html2json-0.1.5/cnki_html2json/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/cnki_html2json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/cnki_html2json/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/cnki_html2json/crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/cnki_html2json/html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/cnki_html2json/parse_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/cnki_html2json/recognize_slider_coordinate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:58:22.071276 cnki_html2json-0.1.5/cnki_html2json.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-05-05 17:58:22.000000 cnki_html2json-0.1.5/cnki_html2json.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-05 17:58:22.000000 cnki_html2json-0.1.5/cnki_html2json.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:58:22.000000 cnki_html2json-0.1.5/cnki_html2json.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 17:58:22.000000 cnki_html2json-0.1.5/cnki_html2json.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 17:58:22.000000 cnki_html2json-0.1.5/cnki_html2json.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 17:58:22.000000 cnki_html2json-0.1.5/cnki_html2json.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:58:22.071276 cnki_html2json-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:58:22.071276 cnki_html2json-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/tests/test_html2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-05 17:58:10.000000 cnki_html2json-0.1.5/tests/test_metadata.py
```

### Comparing `cnki_html2json-0.1.4/LICENSE` & `cnki_html2json-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.4/PKG-INFO` & `cnki_html2json-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki_html2json
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Intended Audience :: Developers
@@ -22,57 +22,56 @@
 License-File: LICENSE
 
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
 
 最近更新：  
-- 从 `0.04` 版本开始，支持 `raw` 模式，可以保留章节文本中的参考文献标签；
+- `v0.15` 对解析论文html的方式进行重构，提高了解析的准确率；
 
 核心功能：
 - 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
 - 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
 - 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
   - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
-  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，例如[1,2]；
-  - `plain` 导出纯文本，不包含任何章节标题和参考文献索引；
-  - 以上三种模式都包含参考文献文献，可以参考 [examples](examples) 文件夹中给出的样例；
+  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，如[1,2]，以及换行符；
+  - `plain` 导出纯文本，不包含章节标题和参考文献索引；
+  - 以上三种模式都包含参考文献，可以参考 [examples](examples) 文件夹中给出的样例；
 
 <!-- 使用场景：
 - 对中文期刊论文进行全文获取和分析，为下游任务提供支持；
 - 对中文期刊论文进行引文分析； -->
 
 使用限制：
 - 确保你所在的网络环境能正常使用知网；
 - 仅能提取 <b>期刊论文</b> 的文本，其他文献类型未做测试；
-- 无法提取文献中的图片、公式等，因此提取的内容可能不完整；
+- 无法提取文献中的图片、表格等，因此提取的内容可能不完整；
 - 本工具已经尽力覆盖大多数情况，但不能保证每一篇文献都能正常提取；
 
 ## 快速开始
 本工具使用 Python 开发，请确保你的电脑上已经安装了 `Python3.8` 或以上版本。如果使用爬虫，需要提前配置好对应浏览器的驱动，例如chrome的驱动为 [chromedriver](https://chromedriver.chromium.org/downloads)
 
 ```console
 $ pip install cnki_html2json
 ```
 
 ## 使用方法
-1、调用 `html2json` 函数
+1、调用函数
 
 ```python
-from cnki_html2json import html2json
+from cnki_html2json.html2json import ExtractContent
 with open('paper.html', 'r', encoding='utf-8') as f:
-    html = f.read()
-print(html2json.extract(html, mode='structure'))
+    raw_html = f.read()
+print(ExtractContent(raw_html).extract(mode='raw',export_path=None))
 ```
-`html2json` 参数说明：
+`extract` 函数参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
-| `paper_html` | 一篇期刊论文的html字符串 |
-| `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `structure` |
+| `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `raw` |
 | `export_path` | 保存结果的路径，默认为 `None` ，则不保存为json文件 |
 
 > 函数返回值说明：参考 [examples](examples) 文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据
 
 2、使用命令行工具，启动一个selenium爬虫，然后在弹出的浏览器窗口(默认为Chrome)中进行检索
 ```console
 $ 无需设置任何参数，直接运行
@@ -87,45 +86,47 @@
 ```console
 $ 查看可选参数
 $ cnki-crawler --help
 ```
 
 命令行工具参数说明：
 |  | 参数 | 说明 |
-| :-: | :-- | -- |
+| --- | --- | --- |
 | -s | --start_paper_index | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
 | -e | --end_paper_index | 论文提取的终止索引，默认为 `None`，爬取到最后 |
-| -m | --mode | 模式，可选值为 `structure`， `plain`， `raw`，默认为 `structure` |
-| -b | --browser | 浏览器类型，Chrome(默认),可选Edge， Firefox， 不支持Safari |
-| -save | --save_path | 下载文件的保存路径，默认为当前目录的 `data` 文件夹 |
+| -m | --mode | 模式，可选值为 `raw(default)`、`structure`、`plain`|
+| -b | --browser | 浏览器类型，可选值为 `Chrome(default)`、`Edge`、`Firefox`|
+| -save | --save_path | 下载文件的保存路径，默认为当前目录的 `dataset` 文件夹 |
 | -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
-| -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，日志将保存在 `save_path` 下的 `log` 文件夹中 |
+| -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，</br>日志将保存在 `save_path` 下的 `log` 文件夹中 |
 
-> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `data` 文件夹下;  
-> 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (可以自动过滑块验证)
+> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `dataset` 文件夹下;  
+> 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (自动过滑块验证)
 
 ```python
 # 也可以在代码中调用爬虫，可选参数参考上方的参数说明
 from cnki_html2json.crawl import start_crawl
-start_crawl(start_paper_index=1,end_paper_index=100,mode='structure',log=True)
+start_crawl(start_paper_index=1,end_paper_index=100,mode='raw',log=True)
 ```
 
 ## json文件字段说明
-| 一级字段 | 二级字段 |三级字段| 说明 |
+| 一级字段 | 二级字段 | 三级字段 | 说明 |
 | --- | --- | --- | --- |
-| metadata | title |  |论文标题|
-|  | authors |  |论文作者|
-|  | orgs |  |作者所属机构|
-|  | abstract |  |论文摘要|
-|  | keywords |  |论文关键词|
-|  | funds |  |基金资助|
-|  | class_num |  |分类号|
-|  | source |  |发表期刊|
-|  | issue |  |发表刊号|
-| body_text | 0 |  |不包含章节标题的首段或没有篇章结构的全文|
-|  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) |reference对应本章节的参考文献索引；text对应本章节的文本|
-|  | 2.xxx | 2.1xxx ||
-|  | ...| ... ||
-| 参考文献 |  |  |参考文献|
+| metadata | title |  | 论文标题 |
+|  | authors |  | 论文作者 |
+|  | orgs |  | 作者所属机构 |
+|  | abstract |  | 论文摘要 |
+|  | keywords |  | 论文关键词 |
+|  | funds |  | 基金资助 |
+|  | class_num |  | 分类号 |
+|  | source |  | 来源期刊 |
+|  | issue |  | 刊号 |
+| body_text |  |  |  |
+|  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) | reference_index对应本章节的参考文献索引；text对应本章节的文本 |
+|  | 2.xxx | 2.1xxx |  |
+|  | ...| ... |  |
+| other | 作者贡献声明 |  |  |
+|  | 利益冲突声明 |  |  |
+|  | 参考文献 |  |  |
 
 ## 开源协议
 本项目使用 [MIT](LICENSE) 协议，具体可查看 [LICENSE](LICENSE) 文件。
```

### Comparing `cnki_html2json-0.1.4/README.md` & `cnki_html2json-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,54 @@
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
 
 最近更新：  
-- 从 `0.04` 版本开始，支持 `raw` 模式，可以保留章节文本中的参考文献标签；
+- `v0.15` 对解析论文html的方式进行重构，提高了解析的准确率；
 
 核心功能：
 - 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
 - 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
 - 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
   - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
-  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，例如[1,2]；
-  - `plain` 导出纯文本，不包含任何章节标题和参考文献索引；
-  - 以上三种模式都包含参考文献文献，可以参考 [examples](examples) 文件夹中给出的样例；
+  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，如[1,2]，以及换行符；
+  - `plain` 导出纯文本，不包含章节标题和参考文献索引；
+  - 以上三种模式都包含参考文献，可以参考 [examples](examples) 文件夹中给出的样例；
 
 <!-- 使用场景：
 - 对中文期刊论文进行全文获取和分析，为下游任务提供支持；
 - 对中文期刊论文进行引文分析； -->
 
 使用限制：
 - 确保你所在的网络环境能正常使用知网；
 - 仅能提取 <b>期刊论文</b> 的文本，其他文献类型未做测试；
-- 无法提取文献中的图片、公式等，因此提取的内容可能不完整；
+- 无法提取文献中的图片、表格等，因此提取的内容可能不完整；
 - 本工具已经尽力覆盖大多数情况，但不能保证每一篇文献都能正常提取；
 
 ## 快速开始
 本工具使用 Python 开发，请确保你的电脑上已经安装了 `Python3.8` 或以上版本。如果使用爬虫，需要提前配置好对应浏览器的驱动，例如chrome的驱动为 [chromedriver](https://chromedriver.chromium.org/downloads)
 
 ```console
 $ pip install cnki_html2json
 ```
 
 ## 使用方法
-1、调用 `html2json` 函数
+1、调用函数
 
 ```python
-from cnki_html2json import html2json
+from cnki_html2json.html2json import ExtractContent
 with open('paper.html', 'r', encoding='utf-8') as f:
-    html = f.read()
-print(html2json.extract(html, mode='structure'))
+    raw_html = f.read()
+print(ExtractContent(raw_html).extract(mode='raw',export_path=None))
 ```
-`html2json` 参数说明：
+`extract` 函数参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
-| `paper_html` | 一篇期刊论文的html字符串 |
-| `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `structure` |
+| `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `raw` |
 | `export_path` | 保存结果的路径，默认为 `None` ，则不保存为json文件 |
 
 > 函数返回值说明：参考 [examples](examples) 文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据
 
 2、使用命令行工具，启动一个selenium爬虫，然后在弹出的浏览器窗口(默认为Chrome)中进行检索
 ```console
 $ 无需设置任何参数，直接运行
@@ -64,45 +63,47 @@
 ```console
 $ 查看可选参数
 $ cnki-crawler --help
 ```
 
 命令行工具参数说明：
 |  | 参数 | 说明 |
-| :-: | :-- | -- |
+| --- | --- | --- |
 | -s | --start_paper_index | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
 | -e | --end_paper_index | 论文提取的终止索引，默认为 `None`，爬取到最后 |
-| -m | --mode | 模式，可选值为 `structure`， `plain`， `raw`，默认为 `structure` |
-| -b | --browser | 浏览器类型，Chrome(默认),可选Edge， Firefox， 不支持Safari |
-| -save | --save_path | 下载文件的保存路径，默认为当前目录的 `data` 文件夹 |
+| -m | --mode | 模式，可选值为 `raw(default)`、`structure`、`plain`|
+| -b | --browser | 浏览器类型，可选值为 `Chrome(default)`、`Edge`、`Firefox`|
+| -save | --save_path | 下载文件的保存路径，默认为当前目录的 `dataset` 文件夹 |
 | -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
-| -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，日志将保存在 `save_path` 下的 `log` 文件夹中 |
+| -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，</br>日志将保存在 `save_path` 下的 `log` 文件夹中 |
 
-> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `data` 文件夹下;  
-> 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (可以自动过滑块验证)
+> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `dataset` 文件夹下;  
+> 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (自动过滑块验证)
 
 ```python
 # 也可以在代码中调用爬虫，可选参数参考上方的参数说明
 from cnki_html2json.crawl import start_crawl
-start_crawl(start_paper_index=1,end_paper_index=100,mode='structure',log=True)
+start_crawl(start_paper_index=1,end_paper_index=100,mode='raw',log=True)
 ```
 
 ## json文件字段说明
-| 一级字段 | 二级字段 |三级字段| 说明 |
+| 一级字段 | 二级字段 | 三级字段 | 说明 |
 | --- | --- | --- | --- |
-| metadata | title |  |论文标题|
-|  | authors |  |论文作者|
-|  | orgs |  |作者所属机构|
-|  | abstract |  |论文摘要|
-|  | keywords |  |论文关键词|
-|  | funds |  |基金资助|
-|  | class_num |  |分类号|
-|  | source |  |发表期刊|
-|  | issue |  |发表刊号|
-| body_text | 0 |  |不包含章节标题的首段或没有篇章结构的全文|
-|  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) |reference对应本章节的参考文献索引；text对应本章节的文本|
-|  | 2.xxx | 2.1xxx ||
-|  | ...| ... ||
-| 参考文献 |  |  |参考文献|
+| metadata | title |  | 论文标题 |
+|  | authors |  | 论文作者 |
+|  | orgs |  | 作者所属机构 |
+|  | abstract |  | 论文摘要 |
+|  | keywords |  | 论文关键词 |
+|  | funds |  | 基金资助 |
+|  | class_num |  | 分类号 |
+|  | source |  | 来源期刊 |
+|  | issue |  | 刊号 |
+| body_text |  |  |  |
+|  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) | reference_index对应本章节的参考文献索引；text对应本章节的文本 |
+|  | 2.xxx | 2.1xxx |  |
+|  | ...| ... |  |
+| other | 作者贡献声明 |  |  |
+|  | 利益冲突声明 |  |  |
+|  | 参考文献 |  |  |
 
 ## 开源协议
 本项目使用 [MIT](LICENSE) 协议，具体可查看 [LICENSE](LICENSE) 文件。
```

### Comparing `cnki_html2json-0.1.4/cnki_html2json/crawl.py` & `cnki_html2json-0.1.5/cnki_html2json/crawl.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,19 +65,19 @@
         # 调用判断验证码函数
         recogize_count = process_slider(driver)
         
         if recogize_count > 0:
             logger.info(f'验证码识别{recogize_count}次后通过')
 
         paper_raw_html = driver.page_source
-        paper_dict = html2json._ExtractContent(paper_raw_html,mode).extract_all()
+        paper_dict = html2json.ExtractContent(paper_raw_html).extract(mode)
         driver.close()
         if not paper_dict:
             logger.error('无法解析html页面')
-        return concat_content(metadata,paper_dict)
+        return concat_content(metadata,paper_dict) # type: ignore
       
     finally:
         driver.switch_to.window(handles[0]) 
 
 def concat_content(metadata,paper_dict:dict)->dict:
     """将论文的元数据和正文内容合并"""
     return {**metadata,**paper_dict}
@@ -104,23 +104,23 @@
         else:
             driver.execute_script('window.scrollTo(0,0)')
             driver.find_element(By.XPATH,f'//a[@id="page{visible_page_index[-1]}"]').click()
             time.sleep(3)
             current_page = visible_page_index[-1]
 
         
-def start_crawl(start_paper_index=1,end_paper_index=None,mode='structure',browser_type='Chrome',log=True,save_path='data',wait_time=120):
+def start_crawl(start_paper_index=1,end_paper_index=None,mode='raw',browser_type='Chrome',log=True,save_path='dataset',wait_time=120):
     """爬取cnki网站的论文
     start_paper_index: 开始爬取的论文索引，默认为1
     end_paper_index: 结束爬取的论文索引，默认为None，即爬取到最后
-    mode: 模式，structure|plain|raw，默认为structure
-    save_path: 下载文件的保存路径，默认为当前目录的data文件夹
+    mode: 模式，structure|plain|raw，默认为raw
+    save_path: 下载文件的保存路径，默认为当前目录的<dataset>文件夹
     log: 是否保存日志，默认为True
     wait_time: 为检索预留的等待时间，单位为秒
-    browser_type: Chrome(默认)|Firefox|Edge|Safari
+    browser_type: Chrome(默认)|Firefox|Edge
     """
 
     if not os.path.exists(save_path):
         os.makedirs(save_path)
         logger.info(f'已创建{save_path}文件夹')
     else:
         save_path_files = [i for i in os.listdir(save_path) if i.endswith('.json')]
@@ -130,15 +130,15 @@
                 logger.warning(f'新下载的文件将覆盖{save_path}文件夹里的文件')
             else:
                 sys.exit('程序已退出')
     
     if log:
         if not os.path.exists(f'{save_path}/log'):
             os.mkdir(f'{save_path}/log')
-            logger.info(f'已在{save_path}文件夹下创建log文件夹')
+            logger.info(f'已创建{save_path}/log文件夹')
 
         current_time = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
         logger.add(f"{save_path}/log/{current_time}.log",format="{time} {level} {message}",level="INFO",mode='w')
         logger.info('本次任务记录日志')
     else:
         logger.info('本次任务不记录日志')
             
@@ -149,15 +149,15 @@
         driver = webdriver.Firefox()
     elif browser_type=='Edge':
         driver = webdriver.Edge()
     # elif browser_type=='Safari':
     #     driver = webdriver.Safari()
     else:
         logger.error('不支持的浏览器类型')
-        sys.exit('请选用合适的浏览器，程序已退出')
+        raise ValueError('请选用合适的浏览器，程序已退出')
 
     logger.info(f'已启动 {browser_type} 浏览器')
     driver.get('https://kns.cnki.net/kns8/AdvSearch')
     
     # 完成检索的等待时间
     time.sleep(wait_time)
     logger.info(f'请在弹出的浏览器窗口中完成检索，{wait_time}秒后将自动开始下载')
```

### Comparing `cnki_html2json-0.1.4/cnki_html2json/parse_metadata.py` & `cnki_html2json-0.1.5/cnki_html2json/parse_metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from lxml import html
+import re
 
 class Parse:
     
     def __init__(self,detail_html:str):
         """
         解析论文详情页的元数据
         detail_html:论文详情页html
         """
         self.content = detail_html
         self.tree = html.fromstring(self.content)
 
-    def _parse(self,xpath_expression:str): # ->str|None|list
+    def _parse(self,xpath_expression:str):
 
         parse_result = [i.strip() for i in self.tree.xpath(xpath_expression) if i.strip()!='']
         parse_result_length = len(parse_result)
     
         if parse_result_length == 0:
             return None
         elif parse_result_length == 1:
@@ -32,15 +33,20 @@
         orgs_xpath_list = ['//h3/a[@class="author"]/text()','//h3[@id="authorpart"]/following-sibling::h3[1]/span[1]/a[@class="author"]/text()','//h3[@id="authorpart"]/following-sibling::h3[1]/span/text()']
         for org_xpath in orgs_xpath_list:
             orgs = self._parse(org_xpath)
             if orgs:
                 break
         metadata['orgs'] = orgs
         
+        try:
+            funds = re.sub(r'\s','',self._parse('//p[@class="funds"]//text()')) # type: ignore
+        except:
+            funds = self._parse('//p[@class="funds"]//text()')
+        
         metadata['abstract'] = self._parse('//span[@id="ChDivSummary"]/text()')
         metadata['keywords'] = self._parse('//p[@class="keywords"]/a[@name="keyword"]/text()')
-        metadata['funds'] = self._parse('//p[@class="funds"]//text()')
+        metadata['funds'] = funds
         metadata['class_num'] = self._parse('//span[text()="分类号："]/following-sibling::p[1]/text()')
         metadata['source'] = self._parse('//div[@class="top-tip"]/span[1]/a[1][contains(@href,"journal")]/text()')
         metadata['issue'] = self._parse('//div[@class="top-tip"]/span[1]/a[2][contains(@href,"journal")]/text()')
         
         return {'metadata':metadata}
```

### Comparing `cnki_html2json-0.1.4/cnki_html2json/recognize_slider_coordinate.py` & `cnki_html2json-0.1.5/cnki_html2json/recognize_slider_coordinate.py`

 * *Files identical despite different names*

### Comparing `cnki_html2json-0.1.4/cnki_html2json.egg-info/PKG-INFO` & `cnki_html2json-0.1.5/cnki_html2json.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnki-html2json
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package to convert cnki html to json
 Home-page: https://github.com/doublessay/cnki-html2json
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: cnki,text-structure,crawler
 Classifier: Intended Audience :: Developers
@@ -22,57 +22,56 @@
 License-File: LICENSE
 
 # 从知网HTML格式的文献中提取结构化文本
 
 本仓库是一个从知网CNKI的HTML格式的 <b>期刊论文</b> 中提取结构化文本，然后导出 <b>JSON</b> 文件的工具，方便对中文期刊论文进行更细维度的分析。
 
 最近更新：  
-- 从 `0.04` 版本开始，支持 `raw` 模式，可以保留章节文本中的参考文献标签；
+- `v0.15` 对解析论文html的方式进行重构，提高了解析的准确率；
 
 核心功能：
 - 从文献的html字符串中解析出包含两级子章节标题的结构化文本；
 - 实现了一个基于 `selenium` 的爬虫，可以批量获取所需文献的结构化文本；
 - 提供三种模式，既可以导出结构化文本，也可以导出非结构化的纯文本；
   - `structure` 导出结构化文本，包含一级、二级子章节标题及对应的正文和参考文献索引；
-  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，例如[1,2]；
-  - `plain` 导出纯文本，不包含任何章节标题和参考文献索引；
-  - 以上三种模式都包含参考文献文献，可以参考 [examples](examples) 文件夹中给出的样例；
+  - `raw` 与 `structure` 模式相似，但是会在正文中保留参考文献标签，如[1,2]，以及换行符；
+  - `plain` 导出纯文本，不包含章节标题和参考文献索引；
+  - 以上三种模式都包含参考文献，可以参考 [examples](examples) 文件夹中给出的样例；
 
 <!-- 使用场景：
 - 对中文期刊论文进行全文获取和分析，为下游任务提供支持；
 - 对中文期刊论文进行引文分析； -->
 
 使用限制：
 - 确保你所在的网络环境能正常使用知网；
 - 仅能提取 <b>期刊论文</b> 的文本，其他文献类型未做测试；
-- 无法提取文献中的图片、公式等，因此提取的内容可能不完整；
+- 无法提取文献中的图片、表格等，因此提取的内容可能不完整；
 - 本工具已经尽力覆盖大多数情况，但不能保证每一篇文献都能正常提取；
 
 ## 快速开始
 本工具使用 Python 开发，请确保你的电脑上已经安装了 `Python3.8` 或以上版本。如果使用爬虫，需要提前配置好对应浏览器的驱动，例如chrome的驱动为 [chromedriver](https://chromedriver.chromium.org/downloads)
 
 ```console
 $ pip install cnki_html2json
 ```
 
 ## 使用方法
-1、调用 `html2json` 函数
+1、调用函数
 
 ```python
-from cnki_html2json import html2json
+from cnki_html2json.html2json import ExtractContent
 with open('paper.html', 'r', encoding='utf-8') as f:
-    html = f.read()
-print(html2json.extract(html, mode='structure'))
+    raw_html = f.read()
+print(ExtractContent(raw_html).extract(mode='raw',export_path=None))
 ```
-`html2json` 参数说明：
+`extract` 函数参数说明：
 
 | 参数 | 说明 |
 | --- | --- |
-| `paper_html` | 一篇期刊论文的html字符串 |
-| `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `structure` |
+| `mode` | 可选值为 `structure`, `plain`, `raw`，默认为 `raw` |
 | `export_path` | 保存结果的路径，默认为 `None` ，则不保存为json文件 |
 
 > 函数返回值说明：参考 [examples](examples) 文件夹中给出的样例，调用该函数得到的结果仅包含正文内容和参考文献，不包括文献元数据
 
 2、使用命令行工具，启动一个selenium爬虫，然后在弹出的浏览器窗口(默认为Chrome)中进行检索
 ```console
 $ 无需设置任何参数，直接运行
@@ -87,45 +86,47 @@
 ```console
 $ 查看可选参数
 $ cnki-crawler --help
 ```
 
 命令行工具参数说明：
 |  | 参数 | 说明 |
-| :-: | :-- | -- |
+| --- | --- | --- |
 | -s | --start_paper_index | 论文提取的起始索引，默认为 `1`，从第一篇开始下载 |
 | -e | --end_paper_index | 论文提取的终止索引，默认为 `None`，爬取到最后 |
-| -m | --mode | 模式，可选值为 `structure`， `plain`， `raw`，默认为 `structure` |
-| -b | --browser | 浏览器类型，Chrome(默认),可选Edge， Firefox， 不支持Safari |
-| -save | --save_path | 下载文件的保存路径，默认为当前目录的 `data` 文件夹 |
+| -m | --mode | 模式，可选值为 `raw(default)`、`structure`、`plain`|
+| -b | --browser | 浏览器类型，可选值为 `Chrome(default)`、`Edge`、`Firefox`|
+| -save | --save_path | 下载文件的保存路径，默认为当前目录的 `dataset` 文件夹 |
 | -wait | --wait_time | 为检索预留的等待时间，默认 `120` 秒 |
-| -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，日志将保存在 `save_path` 下的 `log` 文件夹中 |
+| -l | --log | 是否记录日志，指定该参数则保存日志，无需传值，</br>日志将保存在 `save_path` 下的 `log` 文件夹中 |
 
-> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `data` 文件夹下;  
-> 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (可以自动过滑块验证)
+> 如果未指定保存路径，将下载结果默认保存在当前目录下的 `dataset` 文件夹下;  
+> 由于提取的是文献正文，1分钟大概能下载3篇文献，可以放到夜间运行 (自动过滑块验证)
 
 ```python
 # 也可以在代码中调用爬虫，可选参数参考上方的参数说明
 from cnki_html2json.crawl import start_crawl
-start_crawl(start_paper_index=1,end_paper_index=100,mode='structure',log=True)
+start_crawl(start_paper_index=1,end_paper_index=100,mode='raw',log=True)
 ```
 
 ## json文件字段说明
-| 一级字段 | 二级字段 |三级字段| 说明 |
+| 一级字段 | 二级字段 | 三级字段 | 说明 |
 | --- | --- | --- | --- |
-| metadata | title |  |论文标题|
-|  | authors |  |论文作者|
-|  | orgs |  |作者所属机构|
-|  | abstract |  |论文摘要|
-|  | keywords |  |论文关键词|
-|  | funds |  |基金资助|
-|  | class_num |  |分类号|
-|  | source |  |发表期刊|
-|  | issue |  |发表刊号|
-| body_text | 0 |  |不包含章节标题的首段或没有篇章结构的全文|
-|  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) |reference对应本章节的参考文献索引；text对应本章节的文本|
-|  | 2.xxx | 2.1xxx ||
-|  | ...| ... ||
-| 参考文献 |  |  |参考文献|
+| metadata | title |  | 论文标题 |
+|  | authors |  | 论文作者 |
+|  | orgs |  | 作者所属机构 |
+|  | abstract |  | 论文摘要 |
+|  | keywords |  | 论文关键词 |
+|  | funds |  | 基金资助 |
+|  | class_num |  | 分类号 |
+|  | source |  | 来源期刊 |
+|  | issue |  | 刊号 |
+| body_text |  |  |  |
+|  | 1.xxx(一级章节标题) | 1.1xxx(二级章节标题) | reference_index对应本章节的参考文献索引；text对应本章节的文本 |
+|  | 2.xxx | 2.1xxx |  |
+|  | ...| ... |  |
+| other | 作者贡献声明 |  |  |
+|  | 利益冲突声明 |  |  |
+|  | 参考文献 |  |  |
 
 ## 开源协议
 本项目使用 [MIT](LICENSE) 协议，具体可查看 [LICENSE](LICENSE) 文件。
```

### Comparing `cnki_html2json-0.1.4/setup.py` & `cnki_html2json-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name="cnki_html2json",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.1.4",
+    version="0.1.5",
     description="A package to convert cnki html to json",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["cnki","text-structure","crawler"],
     license="MIT",
     url="https://github.com/doublessay/cnki-html2json",
     packages=["cnki_html2json"],
```

### Comparing `cnki_html2json-0.1.4/tests/test_html2json.py` & `cnki_html2json-0.1.5/tests/test_html2json.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from cnki_html2json import html2json
 
 def test_fulltext():
     with open('tests/fulltext.html','r') as f:
         content = f.read()
 
-    text_structure = html2json._ExtractContent(content,'structure').extract_all()
-    assert text_structure['body_text']['1 引言']['text'][:14] == '近年来，以Chat GPT('
-    assert text_structure['body_text']['1 引言']['reference'][0]==1
+    text_structure = html2json.ExtractContent(content).extract('structure')
+    assert text_structure['body_text']['1 引言']['text'][:14] == '近年来，以Chat GPT(' # type: ignore
+    assert text_structure['body_text']['1 引言']['reference_index'][0]==1 # type: ignore
 
-    text_plain = html2json._ExtractContent(content,'plain').extract_all()
-    assert text_plain['body_text'][:14] == '近年来，以Chat GPT('
+    text_plain = html2json.ExtractContent(content).extract('plain')
+    assert text_plain['body_text'][:14] == '近年来，以Chat GPT(' # type: ignore
 
-    text_raw = html2json._ExtractContent(content,'raw').extract_all()
-    assert '[1]' in text_raw['body_text']['1 引言']['text']
+    text_raw = html2json.ExtractContent(content).extract('raw')
+    assert '[1]' in text_raw['body_text']['1 引言']['text'] # type: ignore
 
 def test_fulltext_crawl():
     with open('tests/fulltext_crawl.html','r') as f:
         content = f.read()
 
-    text_structure = html2json._ExtractContent(content,'structure').extract_all()
-    assert text_structure['body_text']['1 引言']['text'][:14] == '近年来，以Chat GPT('
-    assert text_structure['body_text']['1 引言']['reference'][0]==1
+    text_structure = html2json.ExtractContent(content).extract('structure')
+    assert text_structure['body_text']['1 引言']['text'][:14] == '近年来，以Chat GPT(' # type: ignore
+    assert text_structure['body_text']['1 引言']['reference_index'][0]==1 # type: ignore
 
-    text_plain = html2json._ExtractContent(content,'plain').extract_all()
-    assert text_plain['body_text'][:14] == '近年来，以Chat GPT('
+    text_plain = html2json.ExtractContent(content).extract('plain')
+    assert text_plain['body_text'][:14] == '近年来，以Chat GPT(' # type: ignore
 
-    text_raw = html2json._ExtractContent(content,'raw').extract_all()
-    assert '[1]' in text_raw['body_text']['1 引言']['text']
+    text_raw = html2json.ExtractContent(content).extract('raw')
+    assert '[1]' in text_raw['body_text']['1 引言']['text'] # type: ignore
```

