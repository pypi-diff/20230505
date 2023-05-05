# Comparing `tmp/notion_api-0.5.0.tar.gz` & `tmp/notion_api-0.5.1.tar.gz`

## Comparing `notion_api-0.5.0.tar` & `notion_api-0.5.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    12785 2020-02-02 00:00:00.000000 notion_api-0.5.0/README.md
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/py.typed
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/__init__.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/_about.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/_pkgv.py
--rw-r--r--   0        0        0     5950 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/blockmixin.py
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/client.py
--rw-r--r--   0        0        0    30361 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/notionblock.py
--rw-r--r--   0        0        0    25951 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/notiondatabase.py
--rw-r--r--   0        0        0    20093 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/notionpage.py
--rw-r--r--   0        0        0    15457 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/notionworkspace.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/block_ext/__init__.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/block_ext/code.py
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/block_ext/equation.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/block_ext/richtext.py
--rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/block_ext/table.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/api/block_ext/todo.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/exceptions/__init__.py
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/exceptions/errors.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/exceptions/validate.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/__init__.py
--rw-r--r--   0        0        0    15294 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/blocktypes.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/build.py
--rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/common.py
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/files.py
--rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/options.py
--rw-r--r--   0        0        0    14699 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/propertyobjects.py
--rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/propertyvalues.py
--rw-r--r--   0        0        0     7878 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/properties/richtext.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/propertyitems/__init__.py
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/propertyitems/base.py
--rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/propertyitems/call.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/query/__init__.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/query/compound.py
--rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/query/conditions.py
--rw-r--r--   0        0        0     7493 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/query/propfilter.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/query/sort.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 notion_api-0.5.0/notion/query/timestamp.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 notion_api-0.5.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 notion_api-0.5.0/LICENSE
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 notion_api-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    14249 2020-02-02 00:00:00.000000 notion_api-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    13237 2020-02-02 00:00:00.000000 notion_api-0.5.1/README.md
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/py.typed
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/api/__init__.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/api/_about.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/api/_pkgv.py
+-rw-r--r--   0        0        0     5950 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/api/blockmixin.py
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/api/client.py
+-rw-r--r--   0        0        0    30358 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/api/notionblock.py
+-rw-r--r--   0        0        0    25951 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/api/notiondatabase.py
+-rw-r--r--   0        0        0    20093 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/api/notionpage.py
+-rw-r--r--   0        0        0    13799 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/api/notionworkspace.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/api/block_ext/__init__.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/api/block_ext/code.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/api/block_ext/equation.py
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/api/block_ext/richtext.py
+-rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/api/block_ext/table.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/api/block_ext/todo.py
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/exceptions/__init__.py
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/exceptions/errors.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/exceptions/validate.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/properties/__init__.py
+-rw-r--r--   0        0        0    15294 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/properties/blocktypes.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/properties/build.py
+-rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/properties/common.py
+-rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/properties/files.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/properties/options.py
+-rw-r--r--   0        0        0    14699 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/properties/propertyobjects.py
+-rw-r--r--   0        0        0    14347 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/properties/propertyvalues.py
+-rw-r--r--   0        0        0     7878 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/properties/richtext.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/propertyitems/__init__.py
+-rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/propertyitems/base.py
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/propertyitems/call.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/query/__init__.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/query/compound.py
+-rw-r--r--   0        0        0     4019 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/query/conditions.py
+-rw-r--r--   0        0        0     7493 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/query/propfilter.py
+-rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/query/sort.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 notion_api-0.5.1/notion/query/timestamp.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 notion_api-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 notion_api-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 notion_api-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    14701 2020-02-02 00:00:00.000000 notion_api-0.5.1/PKG-INFO
```

### Comparing `notion_api-0.5.0/README.md` & `notion_api-0.5.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 </p>
 
 __Disclaimer: This is an _unofficial_ package and has no affiliation with Notion.so__  
 
 A wrapper for Notion's API, aiming to simplify the dynamic nature of interacting with Notion.  
 README contains examples of the main functionality, including: creating Pages/Databases/Blocks, adding/removing/editing properties, retrieving property values, and database queries.  
-Some more in-depth walkthroughs can be be found in `examples/`    
+Some more in-depth walkthroughs can be be found in [`examples/`](https://github.com/ayvi-0001/notion-api/tree/main/examples)    
 This package is not complete - new features will continue to be added, and current features may change.
 
 <br>
 
 <div border="0" align="center">
     <table>
         <tr>
@@ -93,15 +93,15 @@
 #             "synced_property_name": "blocked",
 #             "synced_property_id": "wx%7DQ"
 #         }
 #     }
 # }
 ```
 
-**_See usage of retrieving values from a page in examples/retrieving-property-items.md_**  
+**_See usage of retrieving values from a page in [examples/retrieving-property-items.md](https://github.com/ayvi-0001/notion-api/blob/main/examples/retrieving-property-items.md)_**  
 
 Below is a brief example if we were wanting to get the page id from the above property `dependencies` in `homepage`.
 
 ```py
 from notion import propertyitems
 
 related_id: list[str] = propertyitems.relation(homepage.dependencies)
@@ -114,15 +114,15 @@
 
 ```py
 homepage.title = "new page"
 homepage.cover = "https://www.notion.so/images/page-cover/webb1.jpg"
 homepage.icon = "https://www.notion.so/icons/alien-pixel_purple.svg"
 ```
 
-<p align="center"> <img src="examples/images/new_page.png"> </p>
+<p align="center"> <img src="https://github.com/ayvi-0001/notion-api/blob/main/examples/images/new_page.png?raw=true"> </p>
 
 <br>
 
 ## Creating Pages/Databases/Blocks
 
 The current version of the Notion api does not allow pages to be created to the parent `workspace`.  
 Create objects by passing an existing Page/Database instance as an arg to the `create` classmethods.
@@ -153,20 +153,20 @@
 # Referencing the synced block in a new page.
 notion.Block.duplicate_synced_block(new_page, original_synced_block.id)
 ```
 
 <br>
 
 There are few extensions to the `Block` class that have specific functions unique to their block-type.  
-Below is an example using `CodeBlock`. The others are `TableBlock`, `EquationBlock`, `RichTextBlock`, and `ToDoBlock`. You can see usage for them in `examples/block_extensions.md`.
+Below is an example using `CodeBlock`. The others are `TableBlock`, `EquationBlock`, `RichTextBlock`, and `ToDoBlock`. You can see usage for them in [`examples/block_extensions.md`](https://github.com/ayvi-0001/notion-api/blob/main/examples/block_extensions.md).
 
 ```py
 code_block = notion.CodeBlock("84c5721d8a954667902a757f0033f9e0")
 
-class_diagram = r"""
+git_graph = r"""
 %%{init: { 'logLevel': 'debug', 'theme': 'default' , 'themeVariables': { 'darkMode':'true', 'git0': '#ff0000', 'git1': '#00ff00', 'git2': '#0000ff', 'git3': '#ff00ff', 'git4': '#00ffff', 'git5': '#ffff00', 'git6': '#ff00ff', 'git7': '#00ffff' } } }%%
 gitGraph
        commit
        branch develop
        commit tag:"v1.0.0"
        commit
        checkout main
@@ -175,20 +175,20 @@
        merge develop
        commit
        branch featureA
        commit
 """
 
 code_block.language = prop.CodeBlockLang.mermaid
-code_block.code = class_diagram
-code_block.caption = "Example from https://mermaid.js.org/syntax/classDiagram.html#syntax"
+code_block.code = git_graph
+code_block.caption = "Example from https://mermaid.js.org/syntax/gitgraph.html"
 ```
 
 <p align="center">
-    <img src="examples/images/code_commit_diagram.png">
+    <img src="https://github.com/ayvi-0001/notion-api/blob/main/examples/images/code_commit_diagram.png?raw=true">
 </p>
 
 <br>
 
 **_Example Function: Using `notion.Workspace()` to retrieve a user, and appending blocks in a page to mention user/date._**
 
 ```py
@@ -222,15 +222,15 @@
 ```
 
 ```py
 >>> homepage = notion.Page("0b9eccfa890e4c3390175ee10c664a35")
 >>> inline_mention(page=homepage, message="example", user_name="AYVI")
 ```
 <p align="center">
-    <img src="examples/images/example_function_reminder.png">
+    <img src="https://github.com/ayvi-0001/notion-api/blob/main/examples/images/example_function_reminder.png?raw=true">
 </p>
 
 <br>
 
 ## Add, Set, & Delete: Page property values | Database property objects
 
 The first argument for all database property methods is the name of the property,  
@@ -343,14 +343,14 @@
  - `NotionInternalServerError`
  - `NotionServiceUnavailable`
  - `NotionDatabaseConnectionUnavailable`
 
 A common error to look out for is `NotionObjectNotFound`. This error is often raised because your bot has not been added as a connection to the page. 
 
 <p align="center">
-    <img src="examples/images/directory_add_connections.png">  
+    <img src="https://github.com/ayvi-0001/notion-api/blob/main/examples/images/directory_add_connections.png?raw=true">  
 </p>
 
 By default, a bot will have access to the children of any Parent object it has access too. Be sure to double check this connection when moving pages.  
 If you're working on a page that your token has access to via its parent page/database, but you never explicitly granted access to the child page -  and you later move that child page out, then it will lose access.
 
 ---
```

### Comparing `notion_api-0.5.0/notion/__init__.py` & `notion_api-0.5.1/notion/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 #### Queries:
 >>> from notion import query
 
 #### Properties:
 >>> from notion import properties as prop
 
 #### Block Extensions:
->>> notion.CodeBlock | notion.ToDoBlock | notion.EquationBlock | notion.ParagraphBlock
+>>> notion.CodeBlock | notion.ToDoBlock | notion.EquationBlock | notion.RichTextBlock
 
 ---
 
 Uncomment `check_for_pkg_update` method to enable auto-update check.
 
 """
 from typing import Sequence
```

### Comparing `notion_api-0.5.0/notion/api/__init__.py` & `notion_api-0.5.1/notion/api/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/api/_about.py` & `notion_api-0.5.1/notion/api/_about.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "__package_url__",
     "__package_json__",
 )
 
 __notion_version__: Final[str] = "2022-06-28"
 __content_type__: Final[str] = "application/json"
 __base_url__: Final[str] = "https://api.notion.com/v1/"
-__version__: Final[str] = "0.5.0"
+__version__: Final[str] = "0.5.1"
 __package_url__: Final[str] = "https://pypi.org/pypi/notion-api/"
 __package_json__: Final[str] = "https://pypi.org/pypi/notion-api/json"
 
 
 # Notion API Changlog
 # https://developers.notion.com/page/changelog
```

### Comparing `notion_api-0.5.0/notion/api/_pkgv.py` & `notion_api-0.5.1/notion/api/_pkgv.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/api/blockmixin.py` & `notion_api-0.5.1/notion/api/blockmixin.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/api/client.py` & `notion_api-0.5.1/notion/api/client.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/api/notionblock.py` & `notion_api-0.5.1/notion/api/notionblock.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-""" 
+"""
 A block object represents content within Notion. Blocks can be text, lists, media, and more. A page is a type of block, too.
-Some blocks have more content nested inside them. Some examples are indented paragraphs, lists, and toggles. 
+Some blocks have more content nested inside them. Some examples are indented paragraphs, lists, and toggles.
 The nested content is called children, and children are blocks, too.
 
 Block types which support children are:
-    "paragraph", "bulleted_list_item", "numbered_list_item", "toggle", "to_do", "quote", "callout", 
-    "synced_block", "column", "child_page", "child_database", and "table". 
+    "paragraph", "bulleted_list_item", "numbered_list_item", "toggle", "to_do", "quote", "callout",
+    "synced_block", "column", "child_page", "child_database", and "table".
     All heading blocks ("heading_1", "heading_2", and "heading_3") support children when the is_toggleable property is true.
 
 NOTE: The link_preview block will only be returned as part of a response. It cannot be created via the API.
 NOTE: As of March 27, 2023, Notion is no longer supporting the creation of template blocks. They are not included in this module.
 
 https://developers.notion.com/reference/block
 """
@@ -90,15 +90,15 @@
 class Block(_TokenBlockMixin):
     """A block object represents content within Notion.
     Blocks can be text, lists, media, and more. A page is a type of block, too.
 
     These are the individual 'nodes' in a page that you typically interact with in Notion.
     Some blocks have more content nested inside them.
     Some examples are indented paragraphs, lists, and toggles.
-    The nested content is called children, and children are blocks, too. 
+    The nested content is called children, and children are blocks, too.
 
     ---
     ### Versioning:
     To use a previous version of the API, set the envrionment variable `NOTION_VERSION`.
     For more info see: https://developers.notion.com/reference/versioning
 
     ---
@@ -769,9 +769,10 @@
         """Creates a newline break."""
         block_mapping = parent_object._append(BlockChildren([NewLineBreak]))
         newline_block = cls(_result_id(block_mapping))
         return newline_block
 
     # Column blocks are not currently supported.
 
+
 def _result_id(block_mapping: MutableMapping[str, Any]) -> str:
     return cast(str, block_mapping["results"][0]["id"])
```

### Comparing `notion_api-0.5.0/notion/api/notiondatabase.py` & `notion_api-0.5.1/notion/api/notiondatabase.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/api/notionpage.py` & `notion_api-0.5.1/notion/api/notionpage.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/api/notionworkspace.py` & `notion_api-0.5.1/notion/api/notionworkspace.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,32 +16,41 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from typing import Any, MutableMapping, Optional, Sequence, Union, cast
+from typing import Any, MutableMapping, Optional, Sequence, cast
 
 from notion.api._about import __base_url__
 from notion.api.client import _NotionClient
 from notion.api.notionblock import Block
 from notion.api.notionpage import Page
 from notion.properties.build import NotionObject, build_payload
 from notion.properties.common import Parent, UserObject
 from notion.properties.richtext import Mention, RichText
-from notion.query.sort import EntryTimestampSort, SortFilter
+from notion.query.sort import EntryTimestampSort
 
 __all__: Sequence[str] = ["Workspace"]
 
 
 class Workspace(_NotionClient):
-    """
-    Workspace class is to provide general methods that are not specific to a single object.
-    Post/retrieve comments, retrieve users/bots, and search for pages/databases.
+    """The Workspace class is for general methods that are not specific to a single page/database/block object.
+
+    This covers the endpoints:
+        - [Users](https://developers.notion.com/reference/get-users)
+            - list all users
+            - retrieve a user
+            - retrieve your token bot's user
+        - [Search](https://developers.notion.com/reference/post-search)
+            - search workspace by title, page/database objects
+        - [Comments](https://developers.notion.com/reference/create-a-comment)
+            - create a comment
+            - retrieve comments
     """
 
     def __init__(
         self,
         token: Optional[str] = None,
     ) -> None:
         super().__init__(token=token)
@@ -76,45 +85,42 @@
             __base_url__,
             f"?block_id={block_id}" if block_id else "",
             f"&page_size={page_size}" if page_size else "",
             f"&start_cursor={start_cursor}" if start_cursor else "",
         )
 
     def retrieve_token_bot(self) -> MutableMapping[str, Any]:
-        """
-        Retrieves the bot User associated with the API token provided in the authorization header.
+        """Retrieves the bot User associated with the API token provided in the authorization header.
         The bot will have an owner field with information about the person who authorized the integration.
 
         https://developers.notion.com/reference/get-self
         """
         return self._get(self._workspace_endpoint(users=True, me=True))
 
     def list_all_users(
         self, *, page_size: Optional[int] = None, next_cursor: Optional[str] = None
     ) -> MutableMapping[str, Any]:
-        """
-        Returns a paginated list of Users for the workspace.
+        """Returns a paginated list of Users for the workspace.
         https://developers.notion.com/reference/get-users
         """
         if any([page_size, next_cursor]):
-            payload: NotionObject = NotionObject()
+            payload = NotionObject()
             if page_size:
                 payload.set("page_size", page_size)
             if next_cursor:
                 payload.set("next_cursor", next_cursor)
 
             return self._get(self._workspace_endpoint(users=True), payload=payload)
 
         return self._get(self._workspace_endpoint(users=True))
 
     def retrieve_user(
         self, *, user_name: Optional[str] = None, user_id: Optional[str] = None
     ) -> UserObject:
-        """
-        Retrieves a User using either the user name or ID specified.
+        """Retrieves a User using either the user name or ID specified.
 
         :param user_name: (1 of user_name or user_id required) User name in Notion.
         :param user_id: (1 of user_name or user_id required) Identifier for a Notion user
 
         https://developers.notion.com/reference/get-users
         """
         if not any([user_name, user_id]):
@@ -138,34 +144,34 @@
                 id=user["id"],
                 name=user["name"],
                 avatar_url=user["avatar_url"] if user["avatar_url"] else None,
                 email=user["person"]["email"] if user["person"]["email"] else None,
             )
         except KeyError:
             raise ValueError(
-                "%s. %s"
-                % (
-                    f"{self.__repr__()}: Could not find user with name: {user_name}",
-                    f"Only members and guests in the integration's workspace are visible.",
-                )
+                f"{self.__repr__()}: Could not find user with name: {user_name}. ",
+                "Only members and guests in the integration's workspace are visible.",
             )
 
     def retrieve_comments(
         self,
+        /,
+        thread: Page | Block | str,
         *,
-        thread: Union[Page, Block, str],
         page_size: Optional[int] = None,
         start_cursor: Optional[str] = None,
     ) -> MutableMapping[str, Any]:
-        """
-        When retrieving comments, one or more Comment objects will be returned in the form of an array,
+        """ When retrieving comments, one or more Comment objects will be returned in the form of an array,
         sorted in ascending chronological order.
 
-        Retrieving comments from a page parent will return all comments on the page, but not
-        comments from any blocks inside the page.
+        Retrieving comments from a page parent will return all comments on the page, 
+        but not comments from any blocks inside the page.
+
+        :param thread: (required) Either a `notion.Page`/`notion.Block` object, or the string of\
+                        a page/block/discussion_thread ID.
 
         https://developers.notion.com/reference/retrieve-a-comment
         """
         if isinstance(thread, Page) or isinstance(thread, Block):
             block_id = thread.id
         else:
             block_id = thread
@@ -173,46 +179,52 @@
         comments_endpoint = self._comments_endpoint(
             block_id=block_id, page_size=page_size, start_cursor=start_cursor
         )
         return self._get(comments_endpoint)
 
     def comment(
         self,
+        /,
+        comment: Sequence[RichText | Mention],
         *,
-        page: Optional[Union[Page, Block, str]] = None,
-        block: Optional[Union[Block, str]] = None,
+        page: Optional[Page | Block | str] = None,
+        block: Optional[Block | str] = None,
         discussion_id: Optional[str] = None,
-        comment: Sequence[Union[RichText, Mention]],
-    ) -> Union[MutableMapping[str, Any], None]:
-        """
+    ) -> MutableMapping[str, Any] | None:
+        """ Creates a comment in a page or existing discussion thread.
         There are two locations you can add a new comment to:
          - A page
          - An existing discussion thread
+        
+        If the intention is to add a new comment to a page, a parent object must be provided. 
+        Alternatively, if a new comment is being added to an existing discussion thread, the discussion_id string must be provided. 
+        **Exactly one** of these parameters must be provided.
+        
         Currently the API does not support starting a new comment thread on a block inside a page.
         Comments added will always appear as the newest comment in the thread.
-
+        
         ---
+        :param comment: (required) list containing Richtext/Mention objects.
         :param page: (1 of page/block/discussion_id required)\
                       either a string representing the id of a page, or a Page instance.\
                       - passing a string id of child block inside a page will raise NotionObjectNotFound\
                       - passing a Block instance to the page param will create a comment to the parent_id of the block.
         :param block: (1 of page/block/discussion_id required)\
                        either a string representing the id of a block, or a Block instance.\
                        Will search the block for an existing discussion thread,\
                         and comment in that thread if found.
         :param discussion_id: (1 of page/block/discussion_id required)\
                                a string representing the discussion_id of a comment object.
-        :param comment: (required) either a Richtext/Mention object.
 
         https://developers.notion.com/reference/create-a-comment
         """
         if len([k for k, v in locals().items() if v is not None]) > 3:
             raise ValueError("Only one of page/block/discussion_id can be provided.")
 
-        comment_object: NotionObject = NotionObject()
+        comment_object = NotionObject()
         comment_object.set("rich_text", comment)
 
         if page:
             if isinstance(page, Page):
                 payload = build_payload(Parent.page(page.id), comment_object)
             elif isinstance(page, Block):
                 payload = build_payload(Parent.page(page.parent_id), comment_object)
@@ -225,19 +237,16 @@
             if isinstance(block, Block):
                 comment_thread = self.retrieve_comments(thread=block.id).get("results")
             else:  # if str of block.id
                 comment_thread = self.retrieve_comments(thread=block).get("results")
 
             if not comment_thread:
                 raise ValueError(
-                    "%s %s"
-                    % (
-                        "Did not find a comment thread in this block.",
-                        f"Starting new comment threads on a block not supported.",
-                    )
+                    "Did not find a comment thread in this block. ",
+                    "Starting new comment threads on a block not supported.",
                 )
             # Regardless of which discussion_id in a comment thread is used,
             # The next comment will always appear last, so we only get the first discussion_id.
             thread_id = comment_thread[0]["discussion_id"]
             payload = build_payload({"discussion_id": thread_id}, comment_object)
             return self._post(self._comments_endpoint(), payload=payload)
 
@@ -256,60 +265,29 @@
         query: Optional[str] = None,
         filter_pages: Optional[bool] = False,
         filter_databases: Optional[bool] = False,
         start_cursor: Optional[str] = None,
         sort_ascending: Optional[bool] = None,
     ) -> MutableMapping[str, Any]:
         """
-        ### Searches all original pages, databases, and child pages/databases that are shared with the integration.
-        It will not return linked databases, since these duplicate their source databases.
-        The response may contain fewer than page_size of results.
-        See Pagination in api docs for details about how to use a cursor to iterate through the list.
-
-        ---------------
-        ### Limitations of search
-        The search endpoint works best when it's being used to query for pages and databases by name.
-        It is not optimized for the following use cases:
-         - Exhaustively enumerating through all the documents a bot has access to in a workspace.
-           Search is not guaranteed to return everything, and the index may change as your integration
-           is iterating through pages and databases resulting in unstable results.
-         - Searching or filtering within a particular database.
-           This use case is much better served by finding the database ID and using the Query a database endpoint.
-         - Immediate and complete results. Search indexing is not immediate.
-           If an integration performs a search quickly after a page is shared with the integration
-           (such as immediately after a user performs OAuth), the response may not contain the page.
-         - When an integration needs to present a user interface that depends on search results,
-           we recommend including a Refresh button to retry the search.
-           This will allow users to determine if the expected result is present or not, and give them a means to try again.
-
-        ---------------
-        ### Optimizations and recommended ways to use search
-         - Search tends to work best when the request is as specific as possible.
-         - Where possible, we recommend filtering by object (such as page or database) and providing a text query to help narrow down results.
-         - If search is very slow, specifying a smaller page_size can help. (The default page_size is 100.)
-         - Our implementation of the search endpoint includes an optimization where any pages or databases that are
-           directly shared with a bot (rather than shared via an ancestor) are guaranteed to be returned.
-         - If your use case requires pages or databases to immediately be available in search without an indexing delay,
-           we recommend that you share relevant pages/databases with your integration directly.
-
-        ---------------
-        #### Search Filter Object
-        Limitation: Currently the only filter allowed is object which will filter by type of object
-        (either page or database)
-
-        ---------------
-        #### Parameters
-        :param page_size: (optional) The number of items from the full list desired in the response. Maximum/Default: 100
-        :param query: (optional) When supplied, limits which pages are returned by comparing the query to the page title.\
-                       If the query parameter is not provided, the response will contain all pages (and child pages) in the results.
-        :param filter_pages: (optional) sets the `value` key in the Search Filter object to `page`
-        :param filter_databases:(optional)  sets the `value` key in the Search Filter object to `database`
-        :param sort_ascending: (optional) Limitation: Currently only a single sort is allowed and\
-                                is limited to last_edited_time. The default sort is by last_edited_time descending.\
-                                If sort_ascending is set to `True`, the default sort will be overridden.
+        Searches all parent or child pages and databases that have been shared with an integration.
+        Returns all pages or databases, excluding duplicated linked databases, that have titles that include the query param.
+        If no query param is provided, then the response contains all pages or databases that have been shared with the integration.
+        The results adhere to any limitations related to an integration's capabilities.
+        To limit the request to search only pages or to search only databases, use the filter param.
+
+        For more information on the limitations/optimizations of search,
+        see [Search optimizations and limitations](https://developers.notion.com/reference/post-search).
+
+        ---
+        :param page_size: (optional) The number of items from the full list to include in the response. Maximum: 100. Default: 100.
+        :param query: (optional) The text that the API compares page and database titles against.
+        :param filter_pages: (optional) If set to True, limits results to only `page` objects.
+        :param filter_databases:(optional) If set to True, limits results to only `database` objects.
+        :param sort_ascending: (optional) If sort is not provided, then default sort is last_edited_time descending.
         :param start_cursor: (optional) If supplied, will return a page of results starting after provided cursor.
 
         https://developers.notion.com/reference/post-search
         """
         payload: NotionObject = NotionObject()
         payload.set("page_size", page_size)
         if query:
@@ -319,10 +297,10 @@
             payload.nest("filter", "value", "page")
         if filter_databases:
             payload.nest("filter", "property", "object")
             payload.nest("filter", "value", "database")
         if start_cursor:
             payload.set("start_cursor", start_cursor)
         if sort_ascending:
-            payload |= SortFilter([EntryTimestampSort.last_edited_time_ascending()])
+            payload.set("sort", EntryTimestampSort.last_edited_time_ascending())
 
         return self._post(self._workspace_endpoint(search=True), payload=payload)
```

### Comparing `notion_api-0.5.0/notion/api/block_ext/code.py` & `notion_api-0.5.1/notion/api/block_ext/code.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/api/block_ext/equation.py` & `notion_api-0.5.1/notion/api/block_ext/equation.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/api/block_ext/richtext.py` & `notion_api-0.5.1/notion/api/block_ext/richtext.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/api/block_ext/table.py` & `notion_api-0.5.1/notion/api/block_ext/table.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/api/block_ext/todo.py` & `notion_api-0.5.1/notion/api/block_ext/todo.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,14 @@
 
 from notion.api.block_ext.richtext import RichTextBlock
 
 __all__: Sequence[str] = ["ToDoBlock"]
 
 
 class ToDoBlock(RichTextBlock):
-    """ """
-
     def __init__(self, id: str, /, *, token: Optional[str] = None) -> None:
         super().__init__(id, token=token)
 
         if self.type != "to_do":
             raise TypeError(
                 f"Block type must be 'to_do', not '{self.type}' for ToDoBlock."
             )
```

### Comparing `notion_api-0.5.0/notion/exceptions/__init__.py` & `notion_api-0.5.1/notion/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/exceptions/errors.py` & `notion_api-0.5.1/notion/exceptions/errors.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/exceptions/validate.py` & `notion_api-0.5.1/notion/exceptions/validate.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/properties/__init__.py` & `notion_api-0.5.1/notion/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/properties/blocktypes.py` & `notion_api-0.5.1/notion/properties/blocktypes.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/properties/build.py` & `notion_api-0.5.1/notion/properties/build.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/properties/common.py` & `notion_api-0.5.1/notion/properties/common.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/properties/files.py` & `notion_api-0.5.1/notion/properties/files.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/properties/options.py` & `notion_api-0.5.1/notion/properties/options.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/properties/propertyobjects.py` & `notion_api-0.5.1/notion/properties/propertyobjects.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/properties/propertyvalues.py` & `notion_api-0.5.1/notion/properties/propertyvalues.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/properties/richtext.py` & `notion_api-0.5.1/notion/properties/richtext.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/propertyitems/__init__.py` & `notion_api-0.5.1/notion/propertyitems/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/propertyitems/base.py` & `notion_api-0.5.1/notion/propertyitems/base.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/propertyitems/call.py` & `notion_api-0.5.1/notion/propertyitems/call.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/query/__init__.py` & `notion_api-0.5.1/notion/query/__init__.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/query/compound.py` & `notion_api-0.5.1/notion/query/compound.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/query/conditions.py` & `notion_api-0.5.1/notion/query/conditions.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/query/propfilter.py` & `notion_api-0.5.1/notion/query/propfilter.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/notion/query/sort.py` & `notion_api-0.5.1/notion/query/sort.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
         :param sort_object: (required) A list containing PropertyValueSort/EntryTimestampSort\
                              The sort object listed first in the nested sort list takes precedence.
 
         https://developers.notion.com/reference/post-database-query-sort#sort-object
         """
         super().__init__()
-        self.set("sorts", sort_object)
+        self.set("sort", sort_object)
 
 
 class PropertyValueSort(NotionObject):
     __slots__: Sequence[str] = ()
 
     def __init__(self, property_name: str, /, *, direction: str) -> None:
         """
```

### Comparing `notion_api-0.5.0/notion/query/timestamp.py` & `notion_api-0.5.1/notion/query/timestamp.py`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/.gitignore` & `notion_api-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/LICENSE` & `notion_api-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/pyproject.toml` & `notion_api-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `notion_api-0.5.0/PKG-INFO` & `notion_api-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notion-api
-Version: 0.5.0
+Version: 0.5.1
 Summary: An unofficial wrapper for Notion's API, aiming to simplify the dynamic nature of interacting with Notion.
 Project-URL: Homepage, https://github.com/ayvi-0001/notion-api
 Project-URL: Source Code, https://github.com/ayvi-0001/notion-api
 Author-email: Alan Vickers <alan.k.vickers@gmail.com>
 License-File: LICENSE
 Keywords: notion-api,notion-version-2022-06-28,wrapper
 Classifier: Development Status :: 3 - Alpha
@@ -55,15 +55,15 @@
 
 </p>
 
 __Disclaimer: This is an _unofficial_ package and has no affiliation with Notion.so__  
 
 A wrapper for Notion's API, aiming to simplify the dynamic nature of interacting with Notion.  
 README contains examples of the main functionality, including: creating Pages/Databases/Blocks, adding/removing/editing properties, retrieving property values, and database queries.  
-Some more in-depth walkthroughs can be be found in `examples/`    
+Some more in-depth walkthroughs can be be found in [`examples/`](https://github.com/ayvi-0001/notion-api/tree/main/examples)    
 This package is not complete - new features will continue to be added, and current features may change.
 
 <br>
 
 <div border="0" align="center">
     <table>
         <tr>
@@ -127,15 +127,15 @@
 #             "synced_property_name": "blocked",
 #             "synced_property_id": "wx%7DQ"
 #         }
 #     }
 # }
 ```
 
-**_See usage of retrieving values from a page in examples/retrieving-property-items.md_**  
+**_See usage of retrieving values from a page in [examples/retrieving-property-items.md](https://github.com/ayvi-0001/notion-api/blob/main/examples/retrieving-property-items.md)_**  
 
 Below is a brief example if we were wanting to get the page id from the above property `dependencies` in `homepage`.
 
 ```py
 from notion import propertyitems
 
 related_id: list[str] = propertyitems.relation(homepage.dependencies)
@@ -148,15 +148,15 @@
 
 ```py
 homepage.title = "new page"
 homepage.cover = "https://www.notion.so/images/page-cover/webb1.jpg"
 homepage.icon = "https://www.notion.so/icons/alien-pixel_purple.svg"
 ```
 
-<p align="center"> <img src="examples/images/new_page.png"> </p>
+<p align="center"> <img src="https://github.com/ayvi-0001/notion-api/blob/main/examples/images/new_page.png?raw=true"> </p>
 
 <br>
 
 ## Creating Pages/Databases/Blocks
 
 The current version of the Notion api does not allow pages to be created to the parent `workspace`.  
 Create objects by passing an existing Page/Database instance as an arg to the `create` classmethods.
@@ -187,20 +187,20 @@
 # Referencing the synced block in a new page.
 notion.Block.duplicate_synced_block(new_page, original_synced_block.id)
 ```
 
 <br>
 
 There are few extensions to the `Block` class that have specific functions unique to their block-type.  
-Below is an example using `CodeBlock`. The others are `TableBlock`, `EquationBlock`, `RichTextBlock`, and `ToDoBlock`. You can see usage for them in `examples/block_extensions.md`.
+Below is an example using `CodeBlock`. The others are `TableBlock`, `EquationBlock`, `RichTextBlock`, and `ToDoBlock`. You can see usage for them in [`examples/block_extensions.md`](https://github.com/ayvi-0001/notion-api/blob/main/examples/block_extensions.md).
 
 ```py
 code_block = notion.CodeBlock("84c5721d8a954667902a757f0033f9e0")
 
-class_diagram = r"""
+git_graph = r"""
 %%{init: { 'logLevel': 'debug', 'theme': 'default' , 'themeVariables': { 'darkMode':'true', 'git0': '#ff0000', 'git1': '#00ff00', 'git2': '#0000ff', 'git3': '#ff00ff', 'git4': '#00ffff', 'git5': '#ffff00', 'git6': '#ff00ff', 'git7': '#00ffff' } } }%%
 gitGraph
        commit
        branch develop
        commit tag:"v1.0.0"
        commit
        checkout main
@@ -209,20 +209,20 @@
        merge develop
        commit
        branch featureA
        commit
 """
 
 code_block.language = prop.CodeBlockLang.mermaid
-code_block.code = class_diagram
-code_block.caption = "Example from https://mermaid.js.org/syntax/classDiagram.html#syntax"
+code_block.code = git_graph
+code_block.caption = "Example from https://mermaid.js.org/syntax/gitgraph.html"
 ```
 
 <p align="center">
-    <img src="examples/images/code_commit_diagram.png">
+    <img src="https://github.com/ayvi-0001/notion-api/blob/main/examples/images/code_commit_diagram.png?raw=true">
 </p>
 
 <br>
 
 **_Example Function: Using `notion.Workspace()` to retrieve a user, and appending blocks in a page to mention user/date._**
 
 ```py
@@ -256,15 +256,15 @@
 ```
 
 ```py
 >>> homepage = notion.Page("0b9eccfa890e4c3390175ee10c664a35")
 >>> inline_mention(page=homepage, message="example", user_name="AYVI")
 ```
 <p align="center">
-    <img src="examples/images/example_function_reminder.png">
+    <img src="https://github.com/ayvi-0001/notion-api/blob/main/examples/images/example_function_reminder.png?raw=true">
 </p>
 
 <br>
 
 ## Add, Set, & Delete: Page property values | Database property objects
 
 The first argument for all database property methods is the name of the property,  
@@ -377,14 +377,14 @@
  - `NotionInternalServerError`
  - `NotionServiceUnavailable`
  - `NotionDatabaseConnectionUnavailable`
 
 A common error to look out for is `NotionObjectNotFound`. This error is often raised because your bot has not been added as a connection to the page. 
 
 <p align="center">
-    <img src="examples/images/directory_add_connections.png">  
+    <img src="https://github.com/ayvi-0001/notion-api/blob/main/examples/images/directory_add_connections.png?raw=true">  
 </p>
 
 By default, a bot will have access to the children of any Parent object it has access too. Be sure to double check this connection when moving pages.  
 If you're working on a page that your token has access to via its parent page/database, but you never explicitly granted access to the child page -  and you later move that child page out, then it will lose access.
 
 ---
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: notion-api Version: 0.5.0 Summary: An unofficial
+Metadata-Version: 2.1 Name: notion-api Version: 0.5.1 Summary: An unofficial
 wrapper for Notion's API, aiming to simplify the dynamic nature of interacting
 with Notion. Project-URL: Homepage, https://github.com/ayvi-0001/notion-api
 Project-URL: Source Code, https://github.com/ayvi-0001/notion-api Author-email:
 Alan Vickers
 k.vickers@gmail.com> License-File: LICENSE Keywords: notion-api,notion-version-
 2022-06-28,wrapper Classifier: Development Status :: 3 - Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
@@ -24,16 +24,17 @@
    [notion_versioning]  
           [license:_MIT]   [code_style:_black]   [code_style:_black]
 __Disclaimer: This is an _unofficial_ package and has no affiliation with
 Notion.so__ A wrapper for Notion's API, aiming to simplify the dynamic nature
 of interacting with Notion. README contains examples of the main functionality,
 including: creating Pages/Databases/Blocks, adding/removing/editing properties,
 retrieving property values, and database queries. Some more in-depth
-walkthroughs can be be found in `examples/` This package is not complete - new
-features will continue to be added, and current features may change.
+walkthroughs can be be found in [`examples/`](https://github.com/ayvi-0001/
+notion-api/tree/main/examples) This package is not complete - new features will
+continue to be added, and current features may change.
                            Links: Notion API Updates
                            Notion_API_Changelog
 --- ## Install ``` pip install -U notion-api ``` ## Usage ```py import dotenv
 import notion # client will check env variables for 'NOTION_TOKEN'
 dotenv.load_dotenv() homepage = notion.Page('773b08ff38b44521b44b115827e850f2')
 parent_db = notion.Database(homepage.parent_id) # will also look for env var
 `TZ` to set the timezone for all notion objects. If not found, will default to
@@ -42,23 +43,25 @@
 homepage['dependencies'] # { # "id": "WYYq", # "type": "relation", #
 "relation": [ # { # "id": "7bcbc8e6-e237-434b-bd0d-6b56e044200b" # } # ], #
 "has_more": false # } parent_db['dependencies'] # { # "id": "WYYq", # "name":
 "dependencies", # "type": "relation", # "relation": { # "database_id":
 "f5984a7e-2257-4ab0-9d0a-23ea12324031", # "type": "dual_property", #
 "dual_property": { # "synced_property_name": "blocked", # "synced_property_id":
 "wx%7DQ" # } # } # } ``` **_See usage of retrieving values from a page in
-examples/retrieving-property-items.md_** Below is a brief example if we were
-wanting to get the page id from the above property `dependencies` in
-`homepage`. ```py from notion import propertyitems related_id: list[str] =
-propertyitems.relation(homepage.dependencies) ``` ```py >>> ["7bcbc8e6-e237-
-434b-bd0d-6b56e044200b"] ``` Both Page's and Database's have setters for title/
-icon/cover. ```py homepage.title = "new page" homepage.cover = "https://
-www.notion.so/images/page-cover/webb1.jpg" homepage.icon = "https://
-www.notion.so/icons/alien-pixel_purple.svg" ```
-                        [examples/images/new_page.png]
+[examples/retrieving-property-items.md](https://github.com/ayvi-0001/notion-
+api/blob/main/examples/retrieving-property-items.md)_** Below is a brief
+example if we were wanting to get the page id from the above property
+`dependencies` in `homepage`. ```py from notion import propertyitems
+related_id: list[str] = propertyitems.relation(homepage.dependencies) ``` ```py
+>>> ["7bcbc8e6-e237-434b-bd0d-6b56e044200b"] ``` Both Page's and Database's
+have setters for title/icon/cover. ```py homepage.title = "new page"
+homepage.cover = "https://www.notion.so/images/page-cover/webb1.jpg"
+homepage.icon = "https://www.notion.so/icons/alien-pixel_purple.svg" ```
+      [https://github.com/ayvi-0001/notion-api/blob/main/examples/images/
+                            new_page.png?raw=true]
 
 ## Creating Pages/Databases/Blocks The current version of the Notion api does
 not allow pages to be created to the parent `workspace`. Create objects by
 passing an existing Page/Database instance as an arg to the `create`
 classmethods. ```py new_database = notion.Database.create
 ( parent_instance=testpage, database_title="Example Database",
 name_column="page", # This is the column containing page names. Defaults to
@@ -74,25 +77,27 @@
 content to the synced block notion.Block.paragraph(original_synced_block,
 [prop.RichText("This is a synced block.")]) # Referencing the synced block in a
 new page. notion.Block.duplicate_synced_block(new_page,
 original_synced_block.id) ```
 There are few extensions to the `Block` class that have specific functions
 unique to their block-type. Below is an example using `CodeBlock`. The others
 are `TableBlock`, `EquationBlock`, `RichTextBlock`, and `ToDoBlock`. You can
-see usage for them in `examples/block_extensions.md`. ```py code_block =
-notion.CodeBlock("84c5721d8a954667902a757f0033f9e0") class_diagram = r""" %%
-{init: { 'logLevel': 'debug', 'theme': 'default' , 'themeVariables':
-{ 'darkMode':'true', 'git0': '#ff0000', 'git1': '#00ff00', 'git2': '#0000ff',
-'git3': '#ff00ff', 'git4': '#00ffff', 'git5': '#ffff00', 'git6': '#ff00ff',
-'git7': '#00ffff' } } }%% gitGraph commit branch develop commit tag:"v1.0.0"
-commit checkout main commit type: HIGHLIGHT commit merge develop commit branch
+see usage for them in [`examples/block_extensions.md`](https://github.com/ayvi-
+0001/notion-api/blob/main/examples/block_extensions.md). ```py code_block =
+notion.CodeBlock("84c5721d8a954667902a757f0033f9e0") git_graph = r""" %%{init:
+{ 'logLevel': 'debug', 'theme': 'default' , 'themeVariables': { 'darkMode':
+'true', 'git0': '#ff0000', 'git1': '#00ff00', 'git2': '#0000ff', 'git3':
+'#ff00ff', 'git4': '#00ffff', 'git5': '#ffff00', 'git6': '#ff00ff', 'git7':
+'#00ffff' } } }%% gitGraph commit branch develop commit tag:"v1.0.0" commit
+checkout main commit type: HIGHLIGHT commit merge develop commit branch
 featureA commit """ code_block.language = prop.CodeBlockLang.mermaid
-code_block.code = class_diagram code_block.caption = "Example from https://
-mermaid.js.org/syntax/classDiagram.html#syntax" ```
-                   [examples/images/code_commit_diagram.png]
+code_block.code = git_graph code_block.caption = "Example from https://
+mermaid.js.org/syntax/gitgraph.html" ```
+      [https://github.com/ayvi-0001/notion-api/blob/main/examples/images/
+                       code_commit_diagram.png?raw=true]
 
 **_Example Function: Using `notion.Workspace()` to retrieve a user, and
 appending blocks in a page to mention user/date._** ```py def inline_mention
 (page: notion.Page, message: str, user_name: str) -> None: mentionblock =
 notion.Block.paragraph( page, [ prop.Mention.user( notion.Workspace
 ().retrieve_user(user_name=user_name), annotations=prop.Annotations( code=True,
 bold=True, color=prop.BlockColor.purple ), ), prop.RichText(" - "),
@@ -100,15 +105,16 @@
 annotations=prop.Annotations( code=True, bold=True, italic=True,
 underline=True, color=prop.BlockColor.gray, ), ), prop.RichText(":"), ], ) #
 First method returned the newly created block that we append to here:
 notion.Block.paragraph(mentionblock, [prop.RichText(message)])
 notion.Block.divider(page) ``` ```py >>> homepage = notion.Page
 ("0b9eccfa890e4c3390175ee10c664a35") >>> inline_mention(page=homepage,
 message="example", user_name="AYVI") ```
-                [examples/images/example_function_reminder.png]
+      [https://github.com/ayvi-0001/notion-api/blob/main/examples/images/
+                    example_function_reminder.png?raw=true]
 
 ## Add, Set, & Delete: Page property values | Database property objects The
 first argument for all database property methods is the name of the property,
 If a property of that name does not exist, then a new property will be created.
 If a property of that name already exists, but it's a different type than the
 method used - then the API will overwrite this and change the property object
 to the new type. The original parameters will be saved if you decide to switch
@@ -157,13 +163,14 @@
 `NotionInvalidRequestUrl` - `NotionInvalidRequest` - `NotionValidationError` -
 `NotionMissingVersion` - `NotionUnauthorized` - `NotionRestrictedResource` -
 `NotionObjectNotFound` - `NotionConflictError` - `NotionRateLimited` -
 `NotionInternalServerError` - `NotionServiceUnavailable` -
 `NotionDatabaseConnectionUnavailable` A common error to look out for is
 `NotionObjectNotFound`. This error is often raised because your bot has not
 been added as a connection to the page.
-                [examples/images/directory_add_connections.png]
+      [https://github.com/ayvi-0001/notion-api/blob/main/examples/images/
+                    directory_add_connections.png?raw=true]
 By default, a bot will have access to the children of any Parent object it has
 access too. Be sure to double check this connection when moving pages. If
 you're working on a page that your token has access to via its parent page/
 database, but you never explicitly granted access to the child page - and you
 later move that child page out, then it will lose access. ---
```

