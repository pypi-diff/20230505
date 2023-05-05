# Comparing `tmp/ds_caselaw_marklogic_api_client-6.1.0.tar.gz` & `tmp/ds_caselaw_marklogic_api_client-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds_caselaw_marklogic_api_client-6.1.0.tar", max compression
+gzip compressed data, was "ds_caselaw_marklogic_api_client-7.0.0.tar", max compression
```

## Comparing `ds_caselaw_marklogic_api_client-6.1.0.tar` & `ds_caselaw_marklogic_api_client-7.0.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0     1108 2023-05-02 09:30:24.624288 ds_caselaw_marklogic_api_client-6.1.0/LICENSE.md
--rw-r--r--   0        0        0     3139 2023-05-02 09:30:24.624288 ds_caselaw_marklogic_api_client-6.1.0/README.md
--rw-r--r--   0        0        0      926 2023-05-02 09:30:24.624288 ds_caselaw_marklogic_api_client-6.1.0/pyproject.toml
--rw-r--r--   0        0        0    28243 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/Client.py
--rw-r--r--   0        0        0        0 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/__init__.py
--rw-r--r--   0        0        0     2236 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/content_hash.py
--rw-r--r--   0        0        0     2318 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/errors.py
--rw-r--r--   0        0        0        0 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/models/__init__.py
--rw-r--r--   0        0        0     6157 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/models/judgments.py
--rw-r--r--   0        0        0     1341 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/models/utilities/__init__.py
--rw-r--r--   0        0        0     4098 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/models/utilities/aws.py
--rw-r--r--   0        0        0        0 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/py.typed
--rw-r--r--   0        0        0     3821 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xml_tools.py
--rw-r--r--   0        0        0      220 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/break_judgment_checkout.xqy
--rw-r--r--   0        0        0      197 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/checkin_judgment.xqy
--rw-r--r--   0        0        0      385 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/checkout_judgment.xqy
--rw-r--r--   0        0        0      318 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/copy_judgment.xqy
--rw-r--r--   0        0        0      302 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/delete_judgment.xqy
--rw-r--r--   0        0        0      715 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/get_judgment.xqy
--rw-r--r--   0        0        0      193 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/get_judgment_checkout_status.xqy
--rw-r--r--   0        0        0      292 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/get_judgment_version.xqy
--rw-r--r--   0        0        0      172 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/get_last_modified.xqy
--rw-r--r--   0        0        0      338 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/get_metadata_citation.xqy
--rw-r--r--   0        0        0      339 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/get_metadata_court.xqy
--rw-r--r--   0        0        0      221 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/get_metadata_name.xqy
--rw-r--r--   0        0        0      358 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/get_metadata_work_date.xqy
--rw-r--r--   0        0        0      594 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/get_properties_for_search_results.xqy
--rw-r--r--   0        0        0      209 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/get_property.xqy
--rw-r--r--   0        0        0      326 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/insert_judgment.xqy
--rw-r--r--   0        0        0      190 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/list_judgment_versions.xqy
--rw-r--r--   0        0        0      355 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/set_boolean_property.xqy
--rw-r--r--   0        0        0      659 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/set_metadata_citation.xqy
--rw-r--r--   0        0        0     1013 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/set_metadata_court.xqy
--rw-r--r--   0        0        0      756 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/set_metadata_name.xqy
--rw-r--r--   0        0        0     1762 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/set_metadata_this_uri.xqy
--rw-r--r--   0        0        0      939 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy
--rw-r--r--   0        0        0      343 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/set_property.xqy
--rw-r--r--   0        0        0      420 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/update_judgment.xqy
--rw-r--r--   0        0        0      556 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/update_locked_judgment.xqy
--rw-r--r--   0        0        0      371 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/user_has_privilege.xqy
--rw-r--r--   0        0        0      246 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/user_has_role.xqy
--rw-r--r--   0        0        0      156 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/validate_all_documents.xqy
--rw-r--r--   0        0        0      199 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/xslt.xqy
--rw-r--r--   0        0        0     1381 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/xslt_transform.xqy
--rw-r--r--   0        0        0     3455 2023-05-02 09:30:24.628288 ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery_type_dicts.py
--rw-r--r--   0        0        0     4193 1970-01-01 00:00:00.000000 ds_caselaw_marklogic_api_client-6.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/LICENSE.md
+-rw-r--r--   0        0        0     3128 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/README.md
+-rw-r--r--   0        0        0      926 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0    28845 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/Client.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/__init__.py
+-rw-r--r--   0        0        0     2236 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/content_hash.py
+-rw-r--r--   0        0        0     2526 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/errors.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/models/__init__.py
+-rw-r--r--   0        0        0     6376 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/models/judgments.py
+-rw-r--r--   0        0        0     1341 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/models/utilities/__init__.py
+-rw-r--r--   0        0        0     4098 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/models/utilities/aws.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/py.typed
+-rw-r--r--   0        0        0     3821 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xml_tools.py
+-rw-r--r--   0        0        0      220 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/break_judgment_checkout.xqy
+-rw-r--r--   0        0        0      197 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/checkin_judgment.xqy
+-rw-r--r--   0        0        0      385 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/checkout_judgment.xqy
+-rw-r--r--   0        0        0      318 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/copy_judgment.xqy
+-rw-r--r--   0        0        0      302 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/delete_judgment.xqy
+-rw-r--r--   0        0        0      715 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_judgment.xqy
+-rw-r--r--   0        0        0      193 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_judgment_checkout_status.xqy
+-rw-r--r--   0        0        0      292 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_judgment_version.xqy
+-rw-r--r--   0        0        0      172 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_last_modified.xqy
+-rw-r--r--   0        0        0      338 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_metadata_citation.xqy
+-rw-r--r--   0        0        0      339 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_metadata_court.xqy
+-rw-r--r--   0        0        0      221 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_metadata_name.xqy
+-rw-r--r--   0        0        0      358 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_metadata_work_date.xqy
+-rw-r--r--   0        0        0      594 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_properties_for_search_results.xqy
+-rw-r--r--   0        0        0      209 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_property.xqy
+-rw-r--r--   0        0        0      326 2023-05-05 14:07:33.669758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/insert_judgment.xqy
+-rw-r--r--   0        0        0       95 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/judgment_exists.xqy
+-rw-r--r--   0        0        0      190 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/list_judgment_versions.xqy
+-rw-r--r--   0        0        0      355 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_boolean_property.xqy
+-rw-r--r--   0        0        0      659 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_citation.xqy
+-rw-r--r--   0        0        0     1013 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_court.xqy
+-rw-r--r--   0        0        0      756 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_name.xqy
+-rw-r--r--   0        0        0     1762 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_this_uri.xqy
+-rw-r--r--   0        0        0      939 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy
+-rw-r--r--   0        0        0      343 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_property.xqy
+-rw-r--r--   0        0        0      420 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/update_judgment.xqy
+-rw-r--r--   0        0        0      556 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/update_locked_judgment.xqy
+-rw-r--r--   0        0        0      371 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/user_has_privilege.xqy
+-rw-r--r--   0        0        0      246 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/user_has_role.xqy
+-rw-r--r--   0        0        0      156 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/validate_all_documents.xqy
+-rw-r--r--   0        0        0      199 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/xslt.xqy
+-rw-r--r--   0        0        0     1381 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/xslt_transform.xqy
+-rw-r--r--   0        0        0     3536 2023-05-05 14:07:33.673758 ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery_type_dicts.py
+-rw-r--r--   0        0        0     4182 1970-01-01 00:00:00.000000 ds_caselaw_marklogic_api_client-7.0.0/PKG-INFO
```

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/LICENSE.md` & `ds_caselaw_marklogic_api_client-7.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/README.md` & `ds_caselaw_marklogic_api_client-7.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -74,16 +74,16 @@
 ```
 
 ## Testing
 
 To run the test suite:
 
 ```bash
-pip install -r requirements.txt
-python -m pytest
+poetry install
+poetry run pytest
 ```
 
 ## Making changes
 
 When making a change, update the [changelog](CHANGELOG.md) using the
 [Keep a Changelog 1.0.0](https://keepachangelog.com/en/1.0.0/) format. Pull
 requests should not be merged before any relevant updates are made.
@@ -94,15 +94,15 @@
 pull request.
 
 The package will **only** be released to PyPI if the branch is tagged. A merge
 to main alone will **not** trigger a release to PyPI.
 
 To create a release:
 
-0. Update the version number in `setup.cfg`
+0. Update the version number in `pyproject.toml`
 0. Create a branch `release/v{major}.{minor}.{patch}`
 0. Update `CHANGELOG.md` for the release
 0. Commit and push
 0. Open a PR from that branch to main
 0. Get approval on the PR
 0. Merge the PR to main and push
 0. Tag the merge commit on `main` with `v{major}.{minor}.{patch}` and push the tag
```

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/pyproject.toml` & `ds_caselaw_marklogic_api_client-7.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ds-caselaw-marklogic-api-client"
-version = "6.1.0"
+version = "7.0.0"
 description = "An API client for interacting with the underlying data in Find Caselaw."
 authors = ["The National Archives"]
 homepage = "https://github.com/nationalarchives/ds-caselaw-custom-api-client"
 keywords = ["national archives", "caselaw"]
 readme = "README.md"
 packages = [
     { include = "caselawclient", from = "src" },
```

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/Client.py` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/Client.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,16 +38,20 @@
 DEFAULT_XSL_TRANSFORM = "accessible-html.xsl"
 
 
 def decode_multipart(response: requests.Response) -> str:
     """Decode a multipart response and return just the text inside it.
     Note that it is possible for multiple responses to be returned, if
     multiple top-level returns exist in the XQuery."""
+
+    # Arguably, this should return None -- it occurs when there are no
+    # matching entries
     if not (response.content):
         return ""
+
     multipart_data = decoder.MultipartDecoder.from_response(response)
     part_count = len(multipart_data.parts)
     if part_count > 1:
         logging.warning(
             f"Throwing away multipart data ({part_count} items, expected 1)"
         )
     return str(multipart_data.parts[0].text)
@@ -155,14 +159,20 @@
     ) -> requests.Response:
         return self.eval(
             self._xquery_path(xquery_file_name),
             vars=json.dumps(vars),
             accept_header="application/xml",
         )
 
+    def _eval_and_decode(
+        self, vars: query_dicts.MarkLogicAPIDict, xquery_file_name: str
+    ) -> str:
+        response = self._send_to_eval(vars, xquery_file_name)
+        return decode_multipart(response)
+
     def prepare_request_kwargs(
         self,
         method: str,
         path: str,
         body: Optional[str] = None,
         data: Optional[dict[str, Any]] = None,
     ) -> dict[str, Any]:
@@ -198,14 +208,27 @@
 
     def POST(
         self, path: str, headers: dict[str, Any], **data: Any
     ) -> requests.Response:
         logging.warning("POST() is deprecated, use eval() or invoke()")
         return self.make_request("POST", path, headers, data)  # type: ignore
 
+    def judgment_exists(self, judgment_uri: str) -> bool:
+        uri = self._format_uri_for_marklogic(judgment_uri)
+        vars: query_dicts.JudgmentExistsDict = {
+            "uri": uri,
+        }
+        decoded_response = self._eval_and_decode(vars, "judgment_exists.xqy")
+
+        if decoded_response == "true":
+            return True
+        if decoded_response == "false":
+            return False
+        raise RuntimeError("Marklogic response was neither true nor false")
+
     def get_judgment_xml(
         self,
         judgment_uri: str,
         version_uri: Optional[str] = None,
         show_unpublished: bool = False,
     ) -> str:
         uri = self._format_uri_for_marklogic(judgment_uri)
@@ -214,37 +237,32 @@
             version_uri = f"/{version_uri.lstrip('/')}.xml"
         vars: query_dicts.GetJudgmentDict = {
             "uri": uri,
             "version_uri": version_uri,
             "show_unpublished": show_unpublished,
         }
 
-        response = self._send_to_eval(vars, "get_judgment.xqy")
-
-        if not response.text:
+        decoded_response = self._eval_and_decode(vars, "get_judgment.xqy")
+        if not decoded_response:
             raise MarklogicNotPermittedError(
                 "The document is not published and show_unpublished was not set"
             )
 
-        return decode_multipart(response)
+        return decoded_response
+
+        return self._eval_and_decode(vars, "get_judgment.xqy")
 
     def get_judgment_name(self, judgment_uri: str) -> str:
         uri = self._format_uri_for_marklogic(judgment_uri)
         vars: query_dicts.GetMetadataNameDict = {"uri": uri}
-
-        response = self._send_to_eval(vars, "get_metadata_name.xqy")
-        if not response.text:
-            return ""
-
-        return decode_multipart(response)
+        return self._eval_and_decode(vars, "get_metadata_name.xqy")
 
     def set_judgment_name(self, judgment_uri: str, content: str) -> requests.Response:
         uri = self._format_uri_for_marklogic(judgment_uri)
         vars: query_dicts.SetMetadataNameDict = {"uri": uri, "content": content}
-
         return self._send_to_eval(vars, "set_metadata_name.xqy")
 
     def set_judgment_date(self, judgment_uri: str, content: str) -> requests.Response:
         warnings.warn(
             "set_judgment_date() is deprecated, use set_judgment_work_expression_date()",
             DeprecationWarning,
             stacklevel=2,
@@ -540,21 +558,15 @@
 
     def get_property(self, judgment_uri: str, name: str) -> str:
         uri = self._format_uri_for_marklogic(judgment_uri)
         vars: query_dicts.GetPropertyDict = {
             "uri": uri,
             "name": name,
         }
-        response = self._send_to_eval(vars, "get_property.xqy")
-
-        if not response.text:
-            return ""
-
-        content = str(decoder.MultipartDecoder.from_response(response).parts[0].text)
-        return content
+        return self._eval_and_decode(vars, "get_property.xqy")
 
     def set_property(
         self, judgment_uri: str, name: str, value: str
     ) -> requests.Response:
         uri = f"/{judgment_uri.lstrip('/')}.xml"
         vars: query_dicts.SetPropertyDict = {
             "uri": uri,
```

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/content_hash.py` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/content_hash.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/errors.py` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,7 +67,13 @@
 
 class InvalidContentHashError(MarklogicAPIError):
     # This error does not come from Marklogic, but is an error raised by this API...
     status_code = 422
     default_message = (
         "The content hash in the document did not match the hash of the content"
     )
+
+
+class JudgmentNotFoundError(MarklogicAPIError):
+    # This error does not come from Marklogic, but is an error raised by this API...
+    status_code = 404
+    default_message = "The judgment was not found"
```

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/models/judgments.py` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/models/judgments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import datetime
 from functools import cached_property
+from typing import Optional
 
 from ds_caselaw_utils import neutral_url
 from requests_toolbelt.multipart import decoder
 
 from caselawclient.Client import MarklogicApiClient
+from caselawclient.errors import JudgmentNotFoundError
 
 from .utilities import VersionsDict, get_judgment_root, render_versions
 from .utilities.aws import (
     generate_docx_url,
     generate_pdf_url,
     notify_changed,
     publish_documents,
@@ -25,17 +27,19 @@
     pass
 
 
 class Judgment:
     def __init__(self, uri: str, api_client: MarklogicApiClient):
         self.uri = uri.strip("/")
         self.api_client = api_client
+        if not self.judgment_exists():
+            raise JudgmentNotFoundError(f"Judgment {self.uri} does not exist")
 
-        # As part of initialisation, we preload the NCN so we can generate a MarklogicResourceNotFoundError early
-        self.neutral_citation
+    def judgment_exists(self) -> bool:
+        return self.api_client.judgment_exists(self.uri)
 
     @property
     def public_uri(self) -> str:
         return "https://caselaw.nationalarchives.gov.uk/{uri}".format(uri=self.uri)
 
     @cached_property
     def neutral_citation(self) -> str:
@@ -112,15 +116,15 @@
             return render_versions(decoded_versions.parts)
         except AttributeError:
             return []
 
     def content_as_xml(self) -> str:
         return self.api_client.get_judgment_xml(self.uri, show_unpublished=True)
 
-    def content_as_html(self, version_uri: str) -> str:
+    def content_as_html(self, version_uri: Optional[str] = None) -> str:
         results = self.api_client.eval_xslt(
             self.uri, version_uri, show_unpublished=True
         )
         multipart_data = decoder.MultipartDecoder.from_response(results)
         return str(multipart_data.parts[0].text)
 
     @cached_property
@@ -199,14 +203,15 @@
         notify_changed(
             uri=self.uri,
             status="published",
             enrich=True,
         )
 
     def unpublish(self) -> None:
+        self.api_client.break_checkout(self.uri)
         unpublish_documents(uri_for_s3(self.uri))
         self.api_client.set_published(self.uri, False)
         notify_changed(
             uri=self.uri,
             status="not published",
             enrich=False,
         )
```

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/models/utilities/__init__.py` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/models/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/models/utilities/aws.py` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/models/utilities/aws.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xml_tools.py` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xml_tools.py`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/get_judgment.xqy` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_judgment.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/get_properties_for_search_results.xqy` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/get_properties_for_search_results.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/set_metadata_citation.xqy` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_citation.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/set_metadata_court.xqy` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_court.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/set_metadata_name.xqy` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_name.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/set_metadata_this_uri.xqy` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_this_uri.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/set_metadata_work_expression_date.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/update_locked_judgment.xqy` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/update_locked_judgment.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery/xslt_transform.xqy` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery/xslt_transform.xqy`

 * *Files identical despite different names*

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/src/caselawclient/xquery_type_dicts.py` & `ds_caselaw_marklogic_api_client-7.0.0/src/caselawclient/xquery_type_dicts.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,19 @@
 
 # insert_judgment.xqy
 class InsertJudgmentDict(MarkLogicAPIDict):
     judgment: str
     uri: str
 
 
+# judgment_exists.xqy
+class JudgmentExistsDict(MarkLogicAPIDict):
+    uri: str
+
+
 # list_judgment_versions.xqy
 class ListJudgmentVersionsDict(MarkLogicAPIDict):
     uri: str
 
 
 # set_boolean_property.xqy
 class SetBooleanPropertyDict(MarkLogicAPIDict):
```

### Comparing `ds_caselaw_marklogic_api_client-6.1.0/PKG-INFO` & `ds_caselaw_marklogic_api_client-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds-caselaw-marklogic-api-client
-Version: 6.1.0
+Version: 7.0.0
 Summary: An API client for interacting with the underlying data in Find Caselaw.
 Home-page: https://github.com/nationalarchives/ds-caselaw-custom-api-client
 Keywords: national archives,caselaw
 Author: The National Archives
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -99,16 +99,16 @@
 ```
 
 ## Testing
 
 To run the test suite:
 
 ```bash
-pip install -r requirements.txt
-python -m pytest
+poetry install
+poetry run pytest
 ```
 
 ## Making changes
 
 When making a change, update the [changelog](CHANGELOG.md) using the
 [Keep a Changelog 1.0.0](https://keepachangelog.com/en/1.0.0/) format. Pull
 requests should not be merged before any relevant updates are made.
@@ -119,15 +119,15 @@
 pull request.
 
 The package will **only** be released to PyPI if the branch is tagged. A merge
 to main alone will **not** trigger a release to PyPI.
 
 To create a release:
 
-0. Update the version number in `setup.cfg`
+0. Update the version number in `pyproject.toml`
 0. Create a branch `release/v{major}.{minor}.{patch}`
 0. Update `CHANGELOG.md` for the release
 0. Commit and push
 0. Open a PR from that branch to main
 0. Get approval on the PR
 0. Merge the PR to main and push
 0. Tag the merge commit on `main` with `v{major}.{minor}.{patch}` and push the tag
```

