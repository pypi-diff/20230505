# Comparing `tmp/code_genie-0.2.1.dev0.tar.gz` & `tmp/code_genie-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_genie-0.2.1.dev0.tar", last modified: Tue May  2 05:53:02 2023, max compression
+gzip compressed data, was "code_genie-0.3.0.tar", last modified: Fri May  5 05:32:51 2023, max compression
```

## Comparing `code_genie-0.2.1.dev0.tar` & `code_genie-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,34 @@
--rw-r--r--   0        0        0      404 2023-05-02 05:52:48.260158 code_genie-0.2.1.dev0/.bumpversion.cfg
--rw-r--r--   0        0        0     1871 2023-04-29 16:20:39.492906 code_genie-0.2.1.dev0/.gitignore
--rw-r--r--   0        0        0      635 2023-04-27 10:15:39.147415 code_genie-0.2.1.dev0/.readthedocs.yaml
--rw-r--r--   0        0        0      251 2023-05-02 05:52:48.260947 code_genie-0.2.1.dev0/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-04-20 10:01:19.112941 code_genie-0.2.1.dev0/LICENSE
--rw-r--r--   0        0        0     1554 2023-05-02 05:52:48.261659 code_genie-0.2.1.dev0/README.md
--rw-r--r--   0        0        0      484 2023-04-30 09:58:38.245553 code_genie-0.2.1.dev0/TODO.md
--rw-r--r--   0        0        0      245 2023-05-02 05:52:48.262694 code_genie-0.2.1.dev0/code_genie/__init__.py
--rw-r--r--   0        0        0     3041 2023-04-29 16:20:39.495446 code_genie-0.2.1.dev0/code_genie/_cache.py
--rw-r--r--   0        0        0     1678 2023-04-29 16:20:39.496137 code_genie-0.2.1.dev0/code_genie/client.py
--rw-r--r--   0        0        0       89 2023-04-29 16:20:39.496555 code_genie-0.2.1.dev0/code_genie/genie/__init__.py
--rw-r--r--   0        0        0     4755 2023-05-02 05:52:48.263526 code_genie-0.2.1.dev0/code_genie/genie/base.py
--rw-r--r--   0        0        0      501 2023-04-29 16:20:39.497458 code_genie-0.2.1.dev0/code_genie/genie/genie.py
--rw-r--r--   0        0        0     3407 2023-04-29 16:20:39.497737 code_genie-0.2.1.dev0/code_genie/genie/pandas.py
--rw-r--r--   0        0        0      679 2023-04-27 10:15:39.149821 code_genie-0.2.1.dev0/docs/Makefile
--rw-r--r--   0        0        0       92 2023-04-27 10:15:39.151209 code_genie-0.2.1.dev0/docs/api.rst
--rw-r--r--   0        0        0     1492 2023-04-27 10:15:39.151752 code_genie-0.2.1.dev0/docs/conf.py
--rw-r--r--   0        0        0       81 2023-04-27 10:15:39.152197 code_genie-0.2.1.dev0/docs/examples.rst
--rw-r--r--   0        0        0      284 2023-04-27 10:15:39.153008 code_genie-0.2.1.dev0/docs/generated/code_genie.client.rst
--rw-r--r--   0        0        0      226 2023-04-27 10:15:39.153533 code_genie-0.2.1.dev0/docs/generated/code_genie.genie.rst
--rw-r--r--   0        0        0      123 2023-04-27 10:15:39.154001 code_genie-0.2.1.dev0/docs/genie.rst
--rw-r--r--   0        0        0     1110 2023-04-27 10:15:39.154405 code_genie-0.2.1.dev0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-04-27 10:15:39.155023 code_genie-0.2.1.dev0/docs/make.bat
--rw-r--r--   0        0        0    57086 2023-05-02 05:52:48.264496 code_genie-0.2.1.dev0/docs/notebooks/Starter.ipynb
--rw-r--r--   0        0        0     1695 2023-05-02 05:52:48.265032 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/_meta.json
--rw-r--r--   0        0        0      232 2023-05-02 05:52:48.265457 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/boxplots_of_salary_by_department_12125.py
--rw-r--r--   0        0        0      193 2023-05-02 05:52:48.265844 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/count_high_earners_61505.py
--rw-r--r--   0        0        0       80 2023-05-02 05:52:48.266223 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/count_missing_values_28317.py
--rw-r--r--   0        0        0      625 2023-05-02 05:52:48.266565 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/generate_employee_data_58297.py
--rw-r--r--   0        0        0      518 2023-05-02 05:52:48.266983 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/generate_employee_dataframe_96513.py
--rw-r--r--   0        0        0      318 2023-05-02 05:52:48.267382 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/make_salaries_missing_39233.py
--rw-r--r--   0        0        0      452 2023-05-02 05:52:48.267772 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/plot_salary_distribution_47385.py
--rw-r--r--   0        0        0      192 2023-05-02 05:52:48.268126 code_genie-0.2.1.dev0/docs/notebooks/_cache_starter/plot_salary_distribution_49433.py
--rw-r--r--   0        0        0       54 2023-04-27 10:15:39.156660 code_genie-0.2.1.dev0/docs/requirements.in
--rw-r--r--   0        0        0     3100 2023-04-27 10:15:39.156993 code_genie-0.2.1.dev0/docs/requirements.txt
--rw-r--r--   0        0        0     1212 2023-04-27 10:15:39.157311 code_genie-0.2.1.dev0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 05:29:52.448133 code_genie-0.2.1.dev0/tests/__init__.py
--rw-r--r--   0        0        0      475 2023-04-29 16:20:39.501753 code_genie-0.2.1.dev0/tests/conftest.py
--rw-r--r--   0        0        0     1559 2023-04-29 16:20:39.502197 code_genie-0.2.1.dev0/tests/test_cache.py
--rw-r--r--   0        0        0      776 2023-04-29 16:20:39.502598 code_genie-0.2.1.dev0/tests/test_genie.py
--rw-r--r--   0        0        0      839 2023-04-29 16:20:39.503091 code_genie-0.2.1.dev0/tox.ini
--rw-r--r--   0        0        0     3031 1970-01-01 00:00:00.000000 code_genie-0.2.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0      399 2023-05-05 05:32:36.162791 code_genie-0.3.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1871 2023-04-29 16:20:39.492906 code_genie-0.3.0/.gitignore
+-rw-r--r--   0        0        0      635 2023-04-27 10:15:39.147415 code_genie-0.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      448 2023-05-05 05:32:36.163481 code_genie-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-04-20 10:01:19.112941 code_genie-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1549 2023-05-05 05:32:36.164274 code_genie-0.3.0/README.md
+-rw-r--r--   0        0        0      484 2023-04-30 09:58:38.245553 code_genie-0.3.0/TODO.md
+-rw-r--r--   0        0        0      102 2023-05-05 05:32:36.165170 code_genie-0.3.0/code_genie/__init__.py
+-rw-r--r--   0        0        0     3431 2023-05-05 05:32:36.166104 code_genie-0.3.0/code_genie/_cache.py
+-rw-r--r--   0        0        0     1678 2023-04-29 16:20:39.496137 code_genie-0.3.0/code_genie/client.py
+-rw-r--r--   0        0        0     5723 2023-05-05 05:32:36.166922 code_genie-0.3.0/code_genie/genie.py
+-rw-r--r--   0        0        0      679 2023-04-27 10:15:39.149821 code_genie-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0       47 2023-05-05 05:32:36.167856 code_genie-0.3.0/docs/api.rst
+-rw-r--r--   0        0        0     1492 2023-04-27 10:15:39.151752 code_genie-0.3.0/docs/conf.py
+-rw-r--r--   0        0        0       81 2023-04-27 10:15:39.152197 code_genie-0.3.0/docs/examples.rst
+-rw-r--r--   0        0        0      284 2023-04-27 10:15:39.153008 code_genie-0.3.0/docs/generated/code_genie.client.rst
+-rw-r--r--   0        0        0      226 2023-04-27 10:15:39.153533 code_genie-0.3.0/docs/generated/code_genie.genie.rst
+-rw-r--r--   0        0        0     1154 2023-05-05 05:32:36.168709 code_genie-0.3.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-04-27 10:15:39.155023 code_genie-0.3.0/docs/make.bat
+-rw-r--r--   0        0        0    64979 2023-05-05 05:32:36.170025 code_genie-0.3.0/docs/notebooks/Starter.ipynb
+-rw-r--r--   0        0        0     1320 2023-05-05 05:32:36.171160 code_genie-0.3.0/docs/notebooks/_cache_starter/_meta.json
+-rw-r--r--   0        0        0      377 2023-05-05 05:32:36.171751 code_genie-0.3.0/docs/notebooks/_cache_starter/count_missing_values_57234.py
+-rw-r--r--   0        0        0      491 2023-05-05 05:32:36.172371 code_genie-0.3.0/docs/notebooks/_cache_starter/generate_employee_dataframe_16305.py
+-rw-r--r--   0        0        0      125 2023-05-05 05:32:36.172714 code_genie-0.3.0/docs/notebooks/_cache_starter/high_earners_26869.py
+-rw-r--r--   0        0        0      224 2023-05-05 05:32:36.173103 code_genie-0.3.0/docs/notebooks/_cache_starter/plot_salary_by_department_20090.py
+-rw-r--r--   0        0        0      372 2023-05-05 05:32:36.173421 code_genie-0.3.0/docs/notebooks/_cache_starter/plot_salary_distribution_88606.py
+-rw-r--r--   0        0        0       54 2023-04-27 10:15:39.156660 code_genie-0.3.0/docs/requirements.in
+-rw-r--r--   0        0        0     3100 2023-04-27 10:15:39.156993 code_genie-0.3.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1245 2023-05-05 05:32:36.173897 code_genie-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 05:29:52.448133 code_genie-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      475 2023-04-29 16:20:39.501753 code_genie-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1176 2023-05-05 05:32:36.174627 code_genie-0.3.0/tests/test_genie.py
+-rw-r--r--   0        0        0      839 2023-04-29 16:20:39.503091 code_genie-0.3.0/tox.ini
+-rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 code_genie-0.3.0/PKG-INFO
```

### Comparing `code_genie-0.2.1.dev0/.gitignore` & `code_genie-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.1.dev0/.readthedocs.yaml` & `code_genie-0.3.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.1.dev0/LICENSE` & `code_genie-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.1.dev0/README.md` & `code_genie-0.3.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # code-genie
 This library is your copilot for jupyter notebooks
 
-Latest version: 0.2.1-dev0
+Latest version: 0.3.0
 
 ## Documentation
 
 - [Starter Notebook](https://code-genie.readthedocs.io/en/main/notebooks/Starter.html)
 - [All Examples](https://code-genie.readthedocs.io/en/main/examples.html)
 - [API Documentation](https://code-genie.readthedocs.io/en/main/api.html)
```

### Comparing `code_genie-0.2.1.dev0/code_genie/_cache.py` & `code_genie-0.3.0/code_genie/_cache.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from pydantic import BaseModel
 
 logger = logging.getLogger(__name__)
 
 
 class _MetaValue(BaseModel):
-    filename: str
+    id: str
     fn_name: str
 
     class Config:
         frozen = True
 
     def toJson(self):
         return json.dumps(self, default=lambda o: o.__dict__)
@@ -28,17 +28,14 @@
 class _CacheManager:
     DEFAULT_NAME = "_genie_cache.json"
     META_NAME = "_meta.json"
     DEFAULT_CACHE_DIR = mkdtemp()
 
     def __init__(self, cache_dir: Optional[str] = None):
         self.cache_dir, self.meta_path = self._check_cache_dir(cache_dir or self.DEFAULT_CACHE_DIR)
-        self._cache_meta = self._load_meta()
-        if len(self._cache_meta) > 0:
-            logger.info(f"Loaded {len(self._cache_meta)} items from cache file {self.cache_dir}")
 
     @classmethod
     def _set_cache_dir(cls, cache_dir: str):
         cls.DEFAULT_CACHE_DIR = cache_dir
 
     @classmethod
     def reload(cls, filepath: str):
@@ -70,36 +67,54 @@
     def _load_meta(self) -> Dict[str, _MetaValue]:
         if not os.path.exists(self.meta_path):
             return {}
         with open(self.meta_path, "r") as f:
             meta_data: Dict[str, _MetaValue] = json.load(f, object_hook=self._json_decoder(_MetaValue))
         return meta_data
 
-    def _load_code(self, filename: str) -> str:
-        with open(os.path.join(self.cache_dir, filename), "r") as f:
+    def _load_code(self, id: str) -> str:
+        with open(self._get_filename(id), "r") as f:
             return f.read()
 
     @classmethod
     def _consistent_hash(cls, value: str) -> str:
         h = blake2b()
         h.update(bytes(value, "utf-8"))
         return h.hexdigest()
 
+    def _get_filename(self, id: str) -> str:
+        return os.path.join(self.cache_dir, f"{id}.py")
+
     def update(self, key: str, value: _CacheValue):
+        _cache_meta = self._load_meta()
         key_hash = self._consistent_hash(key)
-        self._cache_meta[key_hash] = value
+
+        # if key is present in, delete the file which is currently cashed
+        if key_hash in _cache_meta:
+            os.remove(self._get_filename(_cache_meta[key_hash].id))
+
+        # add new cash entry
+        _cache_meta[key_hash] = value
         # write to code file
-        with open(os.path.join(self.cache_dir, value.filename), "w") as f:
+        with open(self._get_filename(value.id), "w") as f:
             f.write(value.code)
         # update metadata
         with open(self.meta_path, "w") as f:
-            json.dump(self._cache_meta, f, indent=4, default=self._json_encoder)
+            json.dump(_cache_meta, f, indent=4, default=self._json_encoder)
 
     def get(self, key: str) -> Optional[_CacheValue]:
-        meta = self._cache_meta.get(self._consistent_hash(key), None)
+        _cache_meta = self._load_meta()
+        meta = _cache_meta.get(self._consistent_hash(key), None)
         if meta is not None:
-            code = self._load_code(meta.filename)
-            return _CacheValue(code=code, filename=meta.filename, fn_name=meta.fn_name)
+            code = self._load_code(meta.id)
+            return _CacheValue(code=code, id=meta.id, fn_name=meta.fn_name)
         return None
 
     def num_items(self):
-        return len(self._cache_meta)
+        return len(self._load_meta())
+
+    def get_all_code_segments(self) -> Dict[str, str]:
+        _cache_meta = self._load_meta()
+        code_segments = {}
+        for meta in _cache_meta.values():
+            code_segments[meta.id] = self._load_code(meta.id)
+        return code_segments
```

### Comparing `code_genie-0.2.1.dev0/code_genie/client.py` & `code_genie-0.3.0/code_genie/client.py`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.1.dev0/docs/Makefile` & `code_genie-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.1.dev0/docs/conf.py` & `code_genie-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.1.dev0/docs/index.rst` & `code_genie-0.3.0/docs/index.rst`

 * *Files 16% similar despite different names*

```diff
@@ -14,18 +14,19 @@
    API <api>
    Examples <examples>
 
 code-genie will help you bring the power of chatGPT technology to your notebooks.
 
 Look how easy it is to use::
 
-   from code_genie import PandasGenie
+   from code_genie import Genie
    df = load_your_df()
-   genie = PandasGenie(instructions="create a dataframe with number of missing values per column")
-   df_missing = genie(df)
+   genie = Genie(inputs={"df": df})
+   df_missing = genie.plz("create a dataframe with number of missing values per column")
+   genie.plz("make scatter plot of col1 vs col2")
 
 Find more examples in the `examples` folder.
 
 Installation
 ------------
 
 Install code-genie by running:
```

### Comparing `code_genie-0.2.1.dev0/docs/make.bat` & `code_genie-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.1.dev0/docs/notebooks/Starter.ipynb` & `code_genie-0.3.0/docs/notebooks/Starter.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9643687307098765%*

 * *Differences: {"'cells'": '{6: {\'source\': [\'CACHE_DIR = "./_cache_starter"\']}, 8: {\'source\': [\'from '*

 * *            "code_genie import Genie']}, 9: {'execution_count': 6, 'outputs': {0: {'text': ['Genie "*

 * *            "cached with id: generate_employee_dataframe_16305\\n']}}, 'source': ['df = "*

 * *            'Genie(cache_dir=CACHE_DIR).plz(\\n\', \'    ["generate a pandas dataframe containing '*

 * *            '100 rows with employee information with following columns id, name, salary (salary '*

 * *            'per annum in US […]*

```diff
@@ -85,16 +85,15 @@
         {
             "cell_type": "code",
             "execution_count": 4,
             "id": "8a18da38-ec68-4ecc-95bc-58c8ecdfda51",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from code_genie import set_cache_dir\n",
-                "set_cache_dir(\"./_cache_starter\")"
+                "CACHE_DIR = \"./_cache_starter\""
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b3dc2f0a-ca73-41e8-9a50-0672d1a58bc7",
             "metadata": {},
             "source": [
@@ -106,65 +105,61 @@
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "d5bfbd38-e760-468b-8d14-11d18f183da8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from code_genie.genie import Genie, PandasGenie"
+                "from code_genie import Genie"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 6,
             "id": "91de25d6-84dd-4019-bfd9-60fe3582d169",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Executor saved to cache file generate_employee_data_58297.py\n"
+                        "Genie cached with id: generate_employee_dataframe_16305\n"
                     ]
                 }
             ],
             "source": [
-                "data_gen = Genie(instructions=[\"generate a pandas dataframe containing 100 rows with employee information with following columns:\",\n",
-                "                               \"id: random employee id\",\n",
-                "                               \"name: employee name\",\n",
-                "                               \"salary: salary per annum in USD\",\n",
-                "                               \"department: should be either engineering or product\"],\n",
-                "                 override=True)"
+                "df = Genie(cache_dir=CACHE_DIR).plz(\n",
+                "    [\"generate a pandas dataframe containing 100 rows with employee information with following columns id, name, salary (salary per annum in USD), department (should be either engineering or product)\", \n",
+                "     \"make salaries for around 10% of the employees missing\"], override=True)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 7,
             "id": "e7f67149-b53f-4c7f-9b4b-fc7e1972391f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "(100, 4)"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "df = data_gen()\n",
                 "df.shape"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 8,
             "id": "9c4897c3-19f0-41ba-80c1-57b2b5aef90d",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
@@ -190,125 +185,78 @@
                             "      <th>salary</th>\n",
                             "      <th>department</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
-                            "      <td>391</td>\n",
-                            "      <td>Employee_0</td>\n",
-                            "      <td>80288</td>\n",
-                            "      <td>engineering</td>\n",
+                            "      <td>1</td>\n",
+                            "      <td>Employee_1</td>\n",
+                            "      <td>49669.0</td>\n",
+                            "      <td>product</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
-                            "      <td>289</td>\n",
-                            "      <td>Employee_1</td>\n",
-                            "      <td>74477</td>\n",
+                            "      <td>2</td>\n",
+                            "      <td>Employee_2</td>\n",
+                            "      <td>115165.0</td>\n",
                             "      <td>engineering</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
-                            "      <td>817</td>\n",
-                            "      <td>Employee_2</td>\n",
-                            "      <td>134461</td>\n",
+                            "      <td>3</td>\n",
+                            "      <td>Employee_3</td>\n",
+                            "      <td>NaN</td>\n",
                             "      <td>product</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
-                            "      <td>828</td>\n",
-                            "      <td>Employee_3</td>\n",
-                            "      <td>58336</td>\n",
-                            "      <td>product</td>\n",
+                            "      <td>4</td>\n",
+                            "      <td>Employee_4</td>\n",
+                            "      <td>86308.0</td>\n",
+                            "      <td>engineering</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
-                            "      <td>139</td>\n",
-                            "      <td>Employee_4</td>\n",
-                            "      <td>111504</td>\n",
-                            "      <td>engineering</td>\n",
+                            "      <td>5</td>\n",
+                            "      <td>Employee_5</td>\n",
+                            "      <td>52598.0</td>\n",
+                            "      <td>product</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "    id        name  salary   department\n",
-                            "0  391  Employee_0   80288  engineering\n",
-                            "1  289  Employee_1   74477  engineering\n",
-                            "2  817  Employee_2  134461      product\n",
-                            "3  828  Employee_3   58336      product\n",
-                            "4  139  Employee_4  111504  engineering"
+                            "   id        name    salary   department\n",
+                            "0   1  Employee_1   49669.0      product\n",
+                            "1   2  Employee_2  115165.0  engineering\n",
+                            "2   3  Employee_3       NaN      product\n",
+                            "3   4  Employee_4   86308.0  engineering\n",
+                            "4   5  Employee_5   52598.0      product"
                         ]
                     },
-                    "execution_count": 11,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df.head()"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "08e9d70d-f8eb-43e3-bec5-a549f0c64a90",
-            "metadata": {},
-            "source": [
-                "### add missing values"
-            ]
-        },
-        {
             "cell_type": "code",
-            "execution_count": 12,
-            "id": "9b04199c-2abe-4de4-a74f-eda4b14f572a",
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "Executor saved to cache file make_salaries_missing_39233.py\n"
-                    ]
-                }
-            ],
-            "source": [
-                "data_gen_add_missing = PandasGenie(\"make salaries for around 10% of the employees missing\",\n",
-                "                                   columns=list(df.columns))"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 13,
-            "id": "1a408205-c16d-4799-b6a2-1ff0071972cc",
+            "execution_count": 9,
+            "id": "5d223450-bc51-4060-94eb-0301f850a106",
             "metadata": {},
             "outputs": [],
             "source": [
-                "df_missing = data_gen_add_missing(df)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 14,
-            "id": "d47d0c97-f170-4ff5-a011-d975ffebfb2a",
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "10"
-                        ]
-                    },
-                    "execution_count": 14,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "df_missing[\"salary\"].isnull().sum()"
+                "# create genie instance on this df\n",
+                "genie = Genie(inputs={\"df\": df}, cache_dir=CACHE_DIR)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "228545bc-062d-4129-9003-15cac860e7bf",
             "metadata": {},
             "source": [
@@ -321,303 +269,215 @@
             "metadata": {},
             "source": [
                 "### find number of missing values in each column"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 10,
             "id": "934df451-afaf-458c-a36c-a0c0277969b2",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Executor saved to cache file count_missing_values_28317.py\n"
+                        "Genie cached with id: count_missing_values_57234\n"
                     ]
-                }
-            ],
-            "source": [
-                "num_missing = PandasGenie(\"find number of missing values in each column\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 16,
-            "id": "5ad11b01-bffc-45ae-ae68-ce9d971d5c51",
-            "metadata": {},
-            "outputs": [
+                },
                 {
                     "data": {
                         "text/plain": [
                             "id             0\n",
                             "name           0\n",
                             "salary        10\n",
                             "department     0\n",
                             "dtype: int64"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 10,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "num_missing(df_missing)"
+                "genie.plz(\"find number of missing values in each column\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4fb0ba20-a031-452e-a989-7e9a32c62ef8",
             "metadata": {},
             "source": [
                 "### plot distribution of salary"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 11,
             "id": "2b9d7bf3-1638-41e9-a44f-a138f1b4294e",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Executor saved to cache file plot_salary_distribution_49433.py\n"
+                        "Genie cached with id: plot_salary_distribution_88606\n"
                     ]
-                }
-            ],
-            "source": [
-                "dist_salary = PandasGenie(\"plot distribution of salary, create bins of 10K each\", columns=df_missing.columns,\n",
-                "                          override=True)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 21,
-            "id": "465c1afb-4fa8-4644-8fcf-48c25f44a31b",
-            "metadata": {},
-            "outputs": [
+                },
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAjMAAAGwCAYAAABcnuQpAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/NK7nSAAAACXBIWXMAAA9hAAAPYQGoP6dpAAA+OElEQVR4nO3deXxU9b3/8fcsyWSfhIRskIRF1oDsUMRWqCgCbtW6XaSov1qtKCK9lHIVt15FrbVYS6V6b0VvVbQVqHXBIoJIZRFCZAt7JCGQhJB9myzz/f2BTI3sMcnMCa/n4zGPMOd853w/30kyeXPO95xjM8YYAQAAWJTd3wUAAAB8F4QZAABgaYQZAABgaYQZAABgaYQZAABgaYQZAABgaYQZAABgaU5/F9DavF6vDh06pMjISNlsNn+XAwAAzoIxRhUVFUpOTpbdfvp9L+0+zBw6dEgpKSn+LgMAADRDbm6uOnfufNo27T7MREZGSjr2ZkRFRfm5GgAAcDbKy8uVkpLi+zt+Ou0+zBw/tBQVFUWYAQDAYs5miggTgAEAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKURZgAAgKU5/V0AgBPl5OSoqKiozfuNi4tTampqm/cLAN8FYQYIMDk5Oerdp49qqqvbvO/QsDDtzMoi0ACwFMIMEGCKiopUU12tSbN+o4TU7m3Wb0HOPr3+9EwVFRURZgBYCmEGCFAJqd3VuUe6v8sAgIDHBGAAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBphBkAAGBpfg0zq1ev1lVXXaXk5GTZbDYtXbr0hDZZWVm6+uqr5Xa7FR4ermHDhiknJ6ftiwUAAAHJr2GmqqpKAwYM0Pz580+6ft++fbr44ovVu3dvrVq1Slu2bNGcOXMUEhLSxpUCAIBA5fRn5+PHj9f48eNPuf7BBx/UhAkT9Mwzz/iWde/e/bTb9Hg88ng8vufl5eXfvVAAABCwAnbOjNfr1fvvv6+ePXtq3Lhxio+P14gRI056KOqb5s6dK7fb7XukpKS0TcEAAMAvAjbMFBYWqrKyUk899ZSuuOIK/fOf/9SPfvQjXXfddfr0009P+brZs2errKzM98jNzW3DqgEAQFvz62Gm0/F6vZKka665Rg888IAkaeDAgfr888+1YMECXXLJJSd9ncvlksvlarM6AQCAfwXsnpm4uDg5nU717du3yfI+ffpwNhMAAPAJ2DATHBysYcOGadeuXU2W7969W2lpaX6qCgAABBq/HmaqrKzU3r17fc+zs7OVmZmpDh06KDU1VTNnztRNN92kH/zgBxozZoyWLVumf/zjH1q1apX/igYAAAHFr2Fm48aNGjNmjO/5jBkzJElTpkzRwoUL9aMf/UgLFizQ3LlzNW3aNPXq1UvvvPOOLr74Yn+VDAAAAoxfw8zo0aNljDltmzvuuEN33HFHG1UEAACsJmDnzAAAAJwNwgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0v4aZ1atX66qrrlJycrJsNpuWLl16yrZ33323bDab5s2b12b1AQCAwOfXMFNVVaUBAwZo/vz5p223ZMkSrVu3TsnJyW1UGQAAsAqnPzsfP368xo8ff9o2eXl5uu+++/TRRx9p4sSJbVQZAACwCr+GmTPxer2aPHmyZs6cqfT09LN6jcfjkcfj8T0vLy9vrfIAAEAACOgJwE8//bScTqemTZt21q+ZO3eu3G6375GSktKKFQIAAH8L2DCzadMmPf/881q4cKFsNttZv2727NkqKyvzPXJzc1uxSgAA4G8BG2Y+++wzFRYWKjU1VU6nU06nUwcOHNAvfvELdenS5ZSvc7lcioqKavIAAADtV8DOmZk8ebLGjh3bZNm4ceM0efJk3X777X6qCgAABBq/hpnKykrt3bvX9zw7O1uZmZnq0KGDUlNTFRsb26R9UFCQEhMT1atXr7YuFQAABCi/hpmNGzdqzJgxvuczZsyQJE2ZMkULFy70U1UAAMBK/BpmRo8eLWPMWbf/6quvWq8YAABgSQE7ARgAAOBsEGYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAIClEWYAAICl+TXMrF69WldddZWSk5Nls9m0dOlS37r6+nrNmjVL/fv3V3h4uJKTk/WTn/xEhw4d8l/BAAAg4Pg1zFRVVWnAgAGaP3/+Ceuqq6uVkZGhOXPmKCMjQ4sXL9auXbt09dVX+6FSAAAQqJz+7Hz8+PEaP378Sde53W4tX768ybI//OEPGj58uHJycpSamnrS13k8Hnk8Ht/z8vLylisYAAAEHEvNmSkrK5PNZlN0dPQp28ydO1dut9v3SElJabsCAQBAm7NMmKmtrdWsWbN0yy23KCoq6pTtZs+erbKyMt8jNze3DasEAABtza+Hmc5WfX29brzxRhlj9OKLL562rcvlksvlaqPKAACAvwV8mDkeZA4cOKBPPvnktHtlAADA+Segw8zxILNnzx6tXLlSsbGx/i4JAAAEGL+GmcrKSu3du9f3PDs7W5mZmerQoYOSkpL04x//WBkZGXrvvffU2Nio/Px8SVKHDh0UHBzsr7IBAEAA8WuY2bhxo8aMGeN7PmPGDEnSlClT9Oijj+rdd9+VJA0cOLDJ61auXKnRo0e3VZkAACCA+TXMjB49WsaYU64/3ToAAADJQqdmAwAAnAxhBgAAWBphBgAAWBphBgAAWBphBgAAWBphBgAAWBphBgAAWBphBgAAWBphBgAAWBphBgAAWBphBgAAWBphBgAAWJpfbzQJAGg7OTk5KioqavN+4+LilJqa2ub94vxBmAGA80BOTo569+mjmurqNu87NCxMO7OyCDRoNYQZADgPFBUVqaa6WpNm/UYJqd3brN+CnH16/emZKioqIsyg1RBmAOA8kpDaXZ17pPu7DKBFMQEYAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYGmEGAABYml/DzOrVq3XVVVcpOTlZNptNS5cubbLeGKOHH35YSUlJ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AwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALC3gw8zcuXM1bNgwRUZGKj4+Xtdee6127drl77IAAECACPgw8+mnn2rq1Klat26dli9frvr6el1++eWqqqryd2kAACAAOP1dwJksW7asyfOFCxcqPj5emzZt0g9+8IMT2ns8Hnk8Ht/z8vLyVq8RAAD4T8Dvmfm2srIySVKHDh1Oun7u3Llyu92+R0pKSluWBwAA2pilwozX69X06dM1atQo9evX76RtZs+erbKyMt8jNze3jasEAABtKeAPM33T1KlTtW3bNq1Zs+aUbVwul1wuVxtWBQAA/MkyYebee+/Ve++9p9WrV6tz587+LgcAAASIgA8zxhjdd999WrJkiVatWqWuXbv6uyQAABBAAj7MTJ06VW+88Yb+/ve/KzIyUvn5+ZIkt9ut0NBQP1cHAAD8LeAnAL/44osqKyvT6NGjlZSU5Hu89dZb/i4NAAAEgIDfM2OM8XcJAAAggAX8nhkAAIDTIcwAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLI8wAAABLs0SYmT9/vrp06aKQkBCNGDFCGzZs8HdJAAAgQAR8mHnrrbc0Y8YMPfLII8rIyNCAAQM0btw4FRYW+rs0AAAQAAI+zDz33HO68847dfvtt6tv375asGCBwsLC9Oc//9nfpQEAgADg9HcBp1NXV6dNmzZp9uzZvmV2u11jx47V2rVrT/oaj8cjj8fje15WViZJKi8vb5Ua8/PzlZ+f3yrbPh273S6v10u/7bDfXbt2SZIO7tkuT011m/Vb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GaKvvvpKaWlpp23r9XoVHR2tN954Q1deeaWkYxOAlyxZomuvvfakr3n22We1aNEibdy4UdKxPTNPPvmk8vLy1LFjR1+7e+65R1999ZU++OADSdJzzz2n+fPna+/evbLZbC0wUgBthT0zANrUgAEDdOmll6p///664YYb9PLLL6ukpESSVFBQoDvvvFM9evSQ2+1WVFSUKisrlZOTc8rtvfXWWxo1apQSExMVERGhhx566IT2aWlpTYKMJN1555365z//qby8PEnSwoULddtttxFkAAsizABoUw6HQ8uXL9eHH36ovn376oUXXlCvXr2UnZ2tKVOmKDMzU88//7w+//xzZWZmKjY29pSTdteuXatJkyZpwoQJeu+997R582Y9+OCDJ7QPDw8/4bWDBg3SgAED9Nprr2nTpk3avn27brvtttYYMoBW5vR3AQDOPzabTaNGjdKoUaP08MMPKy0tTUuWLNG//vUv/fGPf9SECRMkSbm5uSoqKjrldj7//HOlpaXpwQcf9C07cODAWdfx05/+VPPmzVNeXp7Gjh2rlJSU5g8KgN8QZgC0qfXr12vFihW6/PLLFR8fr/Xr1+vIkSPq06ePevToof/7v//T0KFDVV5erpkzZyo0NPSU2+rRo4dycnK0aNEiDRs2TO+//76WLFly1rX8x3/8h/7zP/9TL7/8sl577bWWGB4AP+AwE4A2FRUVpdWrV2vChAnq2bOnHnroIf32t7/V+PHj9b//+78qKSnR4MGDNXnyZE2bNk3x8fGn3NbVV1+tBx54QPfee68GDhyozz//XHPmzDnrWtxut66//npFREScckIxgMDH2UwAzmuXXnqp0tPT9fvf/97fpQBoJsIMgPNSSUmJVq1apR//+MfasWOHevXq5e+SADQTc2YAnJcGDRqkkpISPf300wQZwOLYMwMAACyNCcAAAMDSCDMAAMDSCDMAAMDSCDMAAMDSCDMAAMDSCDMAAMDSCDMAAMDSCDMAAMDS/j9DaSi4hWz9FAAAAABJRU5ErkJggg==\n",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAjMAAAHHCAYAAABKudlQAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/NK7nSAAAACXBIWXMAAA9hAAAPYQGoP6dpAAA55klEQVR4nO3deXQUVd7G8adJSGcPEEggQAiyiBD27UVRVg3IJjouyBLQURFQEARlHGQchQBqBhcGZhxZPIIgIzAIAiIEEETZQdBhkSUIJFGWrJKE5L5/+NKvbRJImpDugu/nnDrHunWr6lfXhjxU30rZjDFGAAAAFlXO3QUAAABcC8IMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMcBPo2LGjOnbs6O4yrsnx48dls9k0d+7c636uuXPnymaz6fjx4462qKgo9ezZ87qfW5I2bNggm82mDRs2lMn5AKsjzAAe6Ntvv9Uf/vAH1apVS76+vqpevbruvvtuvfPOO+4urdTYbDbH4u3trUqVKqlly5YaOXKkvvvuu1I7z9///vcyCUCu8OTaACux8W4mwLN89dVX6tSpkyIjIxUbG6uqVavq5MmT+vrrr/XDDz/oyJEjJT7m5bsynvQvfZvNprvvvluDBg2SMUapqanau3evFi9erMzMTE2dOlWjR4929DfGKDs7W+XLl5eXl1exzxMdHa3KlSuX6Nrz8vKUm5sru90um80m6dc7M9HR0VqxYkWxj+Nqbfn5+crJyZGPj4/KlePfnMDVeLu7AADOJk2apJCQEG3fvl0VKlRw2paSkuKeon7j0qVLys/Pl4+PzzUfq379+howYIBT25QpU9SrVy+NGTNGDRo00L333ivp1/Dj6+t7zee8kszMTAUEBMjLy6tEgam0lStX7rpfK3AjIfIDHuaHH35Qo0aNCgQZSQoLC3NanzNnjjp37qywsDDZ7XY1bNhQM2fOvOo5cnJy9PLLL6tly5YKCQlRQECA7rzzTiUkJDj1uzxP5Y033tD06dNVp04d2e12bdu2TQEBARo5cmSBY//444/y8vJSXFxcyS78/4SGhmrhwoXy9vbWpEmTCtTy269lkpKSNGTIENWoUUN2u13VqlVTnz59HHNdoqKidODAAW3cuNHxldblu1SX58Vs3LhRw4YNU1hYmGrUqOG07bdzZi77/PPP1axZM/n6+qphw4ZasmSJ0/a//OUvjrs5v/X7Y16ptqLmzCxevFgtW7aUn5+fKleurAEDBujUqVNOfQYPHqzAwECdOnVK9913nwIDA1WlShU9//zzysvLu8roA9bEnRnAw9SqVUtbt27V/v37FR0dfcW+M2fOVKNGjdS7d295e3vr008/1bBhw5Sfn6/hw4cXuV9aWpr+9a9/qV+/fnriiSeUnp6u999/XzExMdq2bZuaNWvm1H/OnDm6ePGinnzySdntdkVGRqpv375atGiR4uPjne5ifPTRRzLGqH///i6PQWRkpDp06KCEhASlpaUpODi40H4PPPCADhw4oGeeeUZRUVFKSUnR2rVrlZiYqKioKE2fPl3PPPOMAgMD9dJLL0mSwsPDnY4xbNgwValSRS+//LIyMzOvWNfhw4f18MMPa+jQoYqNjdWcOXP04IMPavXq1br77rtLdI3Fqe235s6dqyFDhqh169aKi4tTcnKy3nrrLW3ZskW7d+92Cr95eXmKiYlR27Zt9cYbb+iLL77Qm2++qTp16ujpp58uUZ2AJRgAHuXzzz83Xl5exsvLy7Rr186MGzfOrFmzxuTk5BTom5WVVaAtJibG3HLLLU5tHTp0MB06dHCsX7p0yWRnZzv1OX/+vAkPDzePPfaYo+3YsWNGkgkODjYpKSlO/desWWMkmVWrVjm1N2nSxOlcRZFkhg8fXuT2kSNHGklm7969TrXMmTPHUa8k8/rrr1/xPI0aNSq0njlz5hhJpn379ubSpUuFbjt27JijrVatWkaS+eSTTxxtqampplq1aqZ58+aOtokTJ5rC/mot7JhF1ZaQkGAkmYSEBGOMMTk5OSYsLMxER0ebX375xdFvxYoVRpJ5+eWXHW2xsbFGkvnrX//qdMzmzZubli1bFjgXcCPgaybAw9x9993aunWrevfurb1792ratGmKiYlR9erVtXz5cqe+fn5+jv9OTU3Vzz//rA4dOujo0aNKTU0t8hxeXl6OOS/5+fk6d+6cLl26pFatWmnXrl0F+j/wwAOqUqWKU1vXrl0VERGh+fPnO9r279+vffv2FZgH44rAwEBJUnp6eqHb/fz85OPjow0bNuj8+fMun+eJJ54o9vyYiIgI9e3b17EeHBysQYMGaffu3UpKSnK5hqvZsWOHUlJSNGzYMKe5ND169FCDBg20cuXKAvsMHTrUaf3OO+/U0aNHr1uNgDsRZgAP1Lp1ay1ZskTnz5/Xtm3bNH78eKWnp+sPf/iD02PLW7ZsUdeuXRUQEKAKFSqoSpUq+tOf/iRJVwwzkjRv3jw1adJEvr6+Cg0NVZUqVbRy5cpC96tdu3aBtnLlyql///5atmyZsrKyJEnz58+Xr6+vHnzwwWu5fElSRkaGJCkoKKjQ7Xa7XVOnTtWqVasUHh6uu+66S9OmTStxqCjs2opSt27dAvNh6tevL0mFzq8pLSdOnJAk3XrrrQW2NWjQwLH9Ml9f3wLhs2LFitcU+gBPRpgBPJiPj49at26tyZMna+bMmcrNzdXixYsl/TpRuEuXLvr5558VHx+vlStXau3atXruueck/XrHpSgffvihBg8erDp16uj999/X6tWrtXbtWnXu3LnQ/X57B+i3Bg0apIyMDC1btkzGGC1YsEA9e/ZUSEjINV/7/v375eXldcWwMWrUKB06dEhxcXHy9fXVhAkTdNttt2n37t3FPk9R1+aqwib/SirTybfufBILcAcmAAMW0apVK0nSmTNnJEmffvqpsrOztXz5ckVGRjr6/f6JpML8+9//1i233KIlS5Y4/fCdOHFiiWqKjo5W8+bNNX/+fNWoUUOJiYml8ov9EhMTtXHjRrVr167IOzOX1alTR2PGjNGYMWN0+PBhNWvWTG+++aY+/PBDSUWHC1ccOXJExhinYx46dEjSr08nSb/eAZGkCxcuOE3K/f3dk5LUVqtWLUnSwYMH1blzZ6dtBw8edGwHblbcmQE8TEJCgkwhv8vys88+k/T/XzVc/tf3b/umpqZqzpw5Vz1HYft+88032rp1a4nrHThwoD7//HNNnz5doaGh6t69e4mP8Vvnzp1Tv379lJeX53jKpzBZWVm6ePGiU1udOnUUFBSk7OxsR1tAQIAuXLhwTTVddvr0aS1dutSxnpaWpg8++EDNmjVT1apVHTVI0qZNmxz9MjMzNW/evALHK25trVq1UlhYmGbNmuV0batWrdL333+vHj16uHpJwA2BOzOAh3nmmWeUlZWlvn37qkGDBsrJydFXX32lRYsWKSoqSkOGDJEk3XPPPfLx8VGvXr301FNPKSMjQ++9957CwsIcd2+K0rNnTy1ZskR9+/ZVjx49dOzYMc2aNUsNGzZ0zFUprkcffVTjxo3T0qVL9fTTT6t8+fLF3vfQoUP68MMPZYxRWlqa4zcAZ2RkKD4+Xt26dbvivl26dNFDDz2khg0bytvbW0uXLlVycrIeeeQRR7+WLVtq5syZeu2111S3bl2FhYUVuLtRXPXr19fjjz+u7du3Kzw8XLNnz1ZycrJTgLznnnsUGRmpxx9/XGPHjpWXl5dmz56tKlWqKDEx0el4xa2tfPnymjp1qoYMGaIOHTqoX79+jkezo6KiHF8tAjctdz5KBaCgVatWmccee8w0aNDABAYGGh8fH1O3bl3zzDPPmOTkZKe+y5cvN02aNDG+vr4mKirKTJ061cyePbvAI8C/fzQ7Pz/fTJ482dSqVcvY7XbTvHlzs2LFChMbG2tq1arl6Hf5ceirPf587733Gknmq6++KvZ1SnIs5cqVMxUqVDDNmzc3I0eONAcOHCjQ//ePZv/8889m+PDhpkGDBiYgIMCEhISYtm3bmo8//thpv6SkJNOjRw8TFBRkJDnG4fKj0tu3by9wrqIeze7Ro4dZs2aNadKkibHb7aZBgwZm8eLFBfbfuXOnadu2rfHx8TGRkZEmPj6+0GMWVdvvH82+bNGiRaZ58+bGbrebSpUqmf79+5sff/zRqU9sbKwJCAgoUFNRj4wDNwLezQTgmvXt21fffvutS++NAoBrxZwZANfkzJkzWrlypQYOHOjuUgDcpJgzA8Alx44d05YtW/Svf/1L5cuX11NPPeXukgDcpLgzA8AlGzdu1MCBA3Xs2DHNmzfP8TQPAJQ15swAAABL484MAACwNMIMAACwtBt+AnB+fr5Onz6toKCgUv215gAA4Poxxig9PV0REREqV+7K915u+DBz+vRp1axZ091lAAAAF5w8eVI1atS4Yp8bPsxcfkndyZMnFRwc7OZqAABAcaSlpalmzZpXfdmsdBOEmctfLQUHBxNmAACwmOJMEWECMAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDRvdxcA4OaVmpqqrKwsd5chf39/hYSEuLsMAC4izABwi9TUVE2a9jedTXd/mAkN8tdL454j0AAWRZgB4BZZWVk6m56lSo3aKzCkktvqyEg9p7MHNisrK4swA1gUYQaAWwWGVFJwaJhbazjn1rMDuFZMAAYAAJZGmAEAAJZGmAEAAJZGmAEAAJZGmAEAAJZGmAEAAJZGmAEAAJZGmAEAAJZGmAEAAJZGmAEAAJZGmAEAAJZGmAEAAJZGmAEAAJbm1jCzadMm9erVSxEREbLZbFq2bFmBPt9//7169+6tkJAQBQQEqHXr1kpMTCz7YgEAgEdya5jJzMxU06ZNNWPGjEK3//DDD2rfvr0aNGigDRs2aN++fZowYYJ8fX3LuFIAAOCpvN158u7du6t79+5Fbn/ppZd07733atq0aY62OnXqlEVpAADAIjx2zkx+fr5Wrlyp+vXrKyYmRmFhYWrbtm2hX0X9VnZ2ttLS0pwWAABw4/LYMJOSkqKMjAxNmTJF3bp10+eff66+ffvq/vvv18aNG4vcLy4uTiEhIY6lZs2aZVg1AAAoax4bZvLz8yVJffr00XPPPadmzZrpxRdfVM+ePTVr1qwi9xs/frxSU1Mdy8mTJ8uqZAAA4AZunTNzJZUrV5a3t7caNmzo1H7bbbdp8+bNRe5nt9tlt9uvd3kAAMBDeOydGR8fH7Vu3VoHDx50aj906JBq1arlpqoAAICnceudmYyMDB05csSxfuzYMe3Zs0eVKlVSZGSkxo4dq4cfflh33XWXOnXqpNWrV+vTTz/Vhg0b3Fc0AADwKG4NMzt27FCnTp0c66NHj5YkxcbGau7cuerbt69mzZqluLg4Pfvss7r11lv1ySefqH379u4qGQAAeBi3hpmOHTvKGHPFPo899pgee+yxMqoIAABYjcfOmQEAACgOwgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0wgwAALA0t4aZTZs2qVevXoqIiJDNZtOyZcuK7Dt06FDZbDZNnz69zOoDAACez61hJjMzU02bNtWMGTOu2G/p0qX6+uuvFRERUUaVAQAAq/B258m7d++u7t27X7HPqVOn9Mwzz2jNmjXq0aNHGVUGAACswq1h5mry8/M1cOBAjR07Vo0aNSrWPtnZ2crOznasp6WlXa/yAOCGlpqaqqysLHeXIX9/f4WEhLi7DEmeMyaSZ42Lu3l0mJk6daq8vb317LPPFnufuLg4vfLKK9exKgC48aWmpmrStL/pbLr7f3CHBvnrpXHPuf0HtyeNieQ54+IJPDbM7Ny5U2+99ZZ27dolm81W7P3Gjx+v0aNHO9bT0tJUs2bN61EiANywsrKydDY9S5UatVdgSCW31ZGRek5nD2xWVlaW239oe8qYSJ41Lp7AY8PMl19+qZSUFEVGRjra8vLyNGbMGE2fPl3Hjx8vdD+73S673V5GVQLAjS0wpJKCQ8PcWsM5t569IE8YE8nzxsWdPDbMDBw4UF27dnVqi4mJ0cCBAzVkyBA3VQUAADyNW8NMRkaGjhw54lg/duyY9uzZo0qVKikyMlKhoaFO/cuXL6+qVavq1ltvLetSAQCAh3JrmNmxY4c6derkWL881yU2NlZz5851U1UAAMBK3BpmOnbsKGNMsfsXNU8GAADcvHg3EwAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDTCDAAAsDS3hplNmzapV69eioiIkM1m07JlyxzbcnNz9cILL6hx48YKCAhQRESEBg0apNOnT7uvYAAA4HHcGmYyMzPVtGlTzZgxo8C2rKws7dq1SxMmTNCuXbu0ZMkSHTx4UL1793ZDpQAAwFN5u/Pk3bt3V/fu3QvdFhISorVr1zq1vfvuu2rTpo0SExMVGRlZFiUCAAAP59YwU1Kpqamy2WyqUKFCkX2ys7OVnZ3tWE9LSyuDygAAgLtYZgLwxYsX9cILL6hfv34KDg4usl9cXJxCQkIcS82aNcuwSgAAUNYsEWZyc3P10EMPyRijmTNnXrHv+PHjlZqa6lhOnjxZRlUCAAB38PivmS4HmRMnTmj9+vVXvCsjSXa7XXa7vYyqAwAA7ubRYeZykDl8+LASEhIUGhrq7pIAAICHcWuYycjI0JEjRxzrx44d0549e1SpUiVVq1ZNf/jDH7Rr1y6tWLFCeXl5SkpKkiRVqlRJPj4+7iobAAB4ELeGmR07dqhTp06O9dGjR0uSYmNj9Ze//EXLly+XJDVr1sxpv4SEBHXs2LGsygQAAB7MrWGmY8eOMsYUuf1K2wAAACSLPM0EAABQFMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNMIMAACwNJfCzNGjR0u7DgAAAJe4FGbq1q2rTp066cMPP9TFixdLuyYAAIBicynM7Nq1S02aNNHo0aNVtWpVPfXUU9q2bVtp1wYAAHBVLoWZZs2a6a233tLp06c1e/ZsnTlzRu3bt1d0dLTi4+P1008/lXadAAAAhbqmCcDe3t66//77tXjxYk2dOlVHjhzR888/r5o1a2rQoEE6c+ZMadUJAABQqGsKMzt27NCwYcNUrVo1xcfH6/nnn9cPP/ygtWvX6vTp0+rTp09p1QkAAFAol8JMfHy8GjdurNtvv12nT5/WBx98oBMnTui1115T7dq1deedd2ru3LnatWvXFY+zadMm9erVSxEREbLZbFq2bJnTdmOMXn75ZVWrVk1+fn7q2rWrDh8+7ErJAADgBuVSmJk5c6YeffRRnThxQsuWLVPPnj1VrpzzocLCwvT+++9f8TiZmZlq2rSpZsyYUej2adOm6e2339asWbP0zTffKCAgQDExMTxBBQAAHLxd2ak4d0d8fHwUGxt7xT7du3dX9+7dC91mjNH06dP15z//2fF11QcffKDw8HAtW7ZMjzzySMkLBwAANxyX7szMmTNHixcvLtC+ePFizZs375qLkqRjx44pKSlJXbt2dbSFhISobdu22rp1a6mcAwAAWJ9LYSYuLk6VK1cu0B4WFqbJkydfc1GSlJSUJEkKDw93ag8PD3dsK0x2drbS0tKcFgAAcONyKcwkJiaqdu3aBdpr1aqlxMTEay7qWsTFxSkkJMSx1KxZ0631AACA68ulMBMWFqZ9+/YVaN+7d69CQ0OvuShJqlq1qiQpOTnZqT05OdmxrTDjx49XamqqYzl58mSp1AMAADyTS2GmX79+evbZZ5WQkKC8vDzl5eVp/fr1GjlyZKlNzK1du7aqVq2qdevWOdrS0tL0zTffqF27dkXuZ7fbFRwc7LQAAIAbl0tPM7366qs6fvy4unTpIm/vXw+Rn5+vQYMGlWjOTEZGho4cOeJYP3bsmPbs2aNKlSopMjJSo0aN0muvvaZ69eqpdu3amjBhgiIiInTfffe5UjYAALgBuRRmfHx8tGjRIr366qvau3ev/Pz81LhxY9WqVatEx9mxY4c6derkWB89erQkKTY2VnPnztW4ceOUmZmpJ598UhcuXFD79u21evVq+fr6ulI2AAC4AbkUZi6rX7++6tev7/L+HTt2lDGmyO02m01//etf9de//tXlcwAAgBubS2EmLy9Pc+fO1bp165SSkqL8/Hyn7evXry+V4gAAAK7GpTAzcuRIzZ07Vz169FB0dLRsNltp1wUAAFAsLoWZhQsX6uOPP9a9995b2vUAAACUiEuPZvv4+Khu3bqlXQsAAECJuRRmxowZo7feeuuKk3cBAADKgktfM23evFkJCQlatWqVGjVqpPLlyzttX7JkSakUBwAAcDUuhZkKFSqob9++pV0LAABAibkUZubMmVPadQAAALjEpTkzknTp0iV98cUX+sc//qH09HRJ0unTp5WRkVFqxQEAAFyNS3dmTpw4oW7duikxMVHZ2dm6++67FRQUpKlTpyo7O1uzZs0q7ToBAAAK5dKdmZEjR6pVq1Y6f/68/Pz8HO19+/Z1ess1AADA9ebSnZkvv/xSX331lXx8fJzao6KidOrUqVIpDAAAoDhcujOTn5+vvLy8Au0//vijgoKCrrkoAACA4nLpzsw999yj6dOn65///KekX99unZGRoYkTJ/KKA6AQqampysrKcncZkiR/f3+FhIS4uwwUwVM+K8nJycrNzXF3GZKknOxsJScnu7sMjxoTOHMpzLz55puKiYlRw4YNdfHiRT366KM6fPiwKleurI8++qi0awQsLTU1VZOm/U1n093/A0qSQoP89dK45wg0HsiTPitZmRn6/tAR1WiX7dY6LmZlaN+3+zRtxvtOczTdwVPGBAW5FGZq1KihvXv3auHChdq3b58yMjL0+OOPq3///m7/sAGeJisrS2fTs1SpUXsFhlRyay0Zqed09sBmZWVlEWY8kCd9VpISjyj7wH91KfeSW+vIzb6onHybKja8Q2HVari1Fk8ZExTkUpiRJG9vbw0YMKA0awFuaIEhlRQcGubuMnTO3QXgqjzhs5J+/me3nv/3AoIrMiYokkth5oMPPrji9kGDBrlUDAAAQEm5FGZGjhzptJ6bm6usrCz5+PjI39+fMAMAAMqMS49mnz9/3mnJyMjQwYMH1b59eyYAAwCAMuXyu5l+r169epoyZUqBuzYAAADXU6mFGenXScGnT58uzUMCAABckUtzZpYvX+60bozRmTNn9O677+qOO+4olcIAAACKw6Uwc9999zmt22w2ValSRZ07d9abb75ZGnUBAAAUi0thJj8/v7TrAAAAcEmpzpkBAAAoay7dmRk9enSx+8bHx7tyCgAAgGJxKczs3r1bu3fvVm5urm699VZJ0qFDh+Tl5aUWLVo4+tlsttKpEgAAoAguhZlevXopKChI8+bNU8WKFSX9+ov0hgwZojvvvFNjxowp1SIBAACK4tKcmTfffFNxcXGOICNJFStW1GuvvcbTTAAAoEy5FGbS0tL0008/FWj/6aeflJ6efs1FAQAAFJdLYaZv374aMmSIlixZoh9//FE//vijPvnkEz3++OO6//77S624vLw8TZgwQbVr15afn5/q1KmjV199VcaYUjsHAACwNpfmzMyaNUvPP/+8Hn30UeXm5v56IG9vPf7443r99ddLrbipU6dq5syZmjdvnho1aqQdO3ZoyJAhCgkJ0bPPPltq5wEAANblUpjx9/fX3//+d73++uv64YcfJEl16tRRQEBAqRb31VdfqU+fPurRo4ckKSoqSh999JG2bdtWqucBAADWdU2/NO/MmTM6c+aM6tWrp4CAgFL/+uf222/XunXrdOjQIUnS3r17tXnzZnXv3r3IfbKzs5WWlua0AACAG5dLd2bOnj2rhx56SAkJCbLZbDp8+LBuueUWPf7446pYsWKpPdH04osvKi0tTQ0aNJCXl5fy8vI0adIk9e/fv8h94uLi9Morr5TK+QEAgOdz6c7Mc889p/LlyysxMVH+/v6O9ocfflirV68uteI+/vhjzZ8/XwsWLNCuXbs0b948vfHGG5o3b16R+4wfP16pqamO5eTJk6VWDwAA8Dwu3Zn5/PPPtWbNGtWoUcOpvV69ejpx4kSpFCZJY8eO1YsvvqhHHnlEktS4cWOdOHFCcXFxio2NLXQfu90uu91eajUAAADP5tKdmczMTKc7MpedO3euVINEVlaWypVzLtHLy4u3dgMAAAeXwsydd96pDz74wLFus9mUn5+vadOmqVOnTqVWXK9evTRp0iStXLlSx48f19KlSxUfH6++ffuW2jkAAIC1ufQ107Rp09SlSxft2LFDOTk5GjdunA4cOKBz585py5YtpVbcO++8owkTJmjYsGFKSUlRRESEnnrqKb388suldg4AAGBtLoWZ6OhoHTp0SO+++66CgoKUkZGh+++/X8OHD1e1atVKrbigoCBNnz5d06dPL7VjAgCAG0uJw0xubq66deumWbNm6aWXXroeNQEAABRbiefMlC9fXvv27bsetQAAAJSYSxOABwwYoPfff7+0awEAACgxl+bMXLp0SbNnz9YXX3yhli1bFngnU3x8fKkUBwAAcDUlCjNHjx5VVFSU9u/frxYtWkiS471Jl9lsttKrDgAA4CpKFGbq1aunM2fOKCEhQdKvry94++23FR4efl2KAwAAuJoSzZn5/VuxV61apczMzFItCAAAoCRcmgB82e/DDQAAQFkrUZix2WwF5sQwRwYAALhTiebMGGM0ePBgx8skL168qKFDhxZ4mmnJkiWlVyEAAMAVlCjMxMbGOq0PGDCgVIsBAAAoqRKFmTlz5lyvOgAAAFxyTROAAQAA3I0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALI0wAwAALM3jw8ypU6c0YMAAhYaGys/PT40bN9aOHTvcXRYAAPAQ3u4u4ErOnz+vO+64Q506ddKqVatUpUoVHT58WBUrVnR3aQAAwEN4dJiZOnWqatasqTlz5jjaateu7caKAACAp/HoMLN8+XLFxMTowQcf1MaNG1W9enUNGzZMTzzxRJH7ZGdnKzs727GelpZWFqUClpGTna3k5GR3l6Hk5GTl5ua4uwxJjAmsyVM+t/7+/goJCXFrDR4dZo4ePaqZM2dq9OjR+tOf/qTt27fr2WeflY+Pj2JjYwvdJy4uTq+88koZVwpYw8WsDO37dp+mzXhffn5+bq0lKzND3x86ohrtsq/e+TpiTGBFnvS5DQ3y10vjnnNroPHoMJOfn69WrVpp8uTJkqTmzZtr//79mjVrVpFh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R2rt2rXy9fV1dzkeIz8/X61atdLkyZMlSc2bN9f+/fs1a9YsxcbGurk69/j44481f/58LViwQI0aNdKePXs0atQoRURE3LRjgpLJzc3VQw89JGOMZs6c6e5yLIs7MyVUuXJleXl5FXhyJTk5WVWrVnVTVdduxIgRWrFihRISElSjRg1He9WqVZWTk6MLFy449f/t9VatWrXQ8bi87Up9goOD5efn51HjunPnTqWkpKhFixby9vaWt7e3Nm7cqLffflve3t4KDw+/6cZEkqpVq6aGDRs6td12221KTEyU9P/XdaV6q1atqpSUFKftly5d0rlz50pl7Mp6XMaOHeu4O9O4cWMNHDhQzz33nOOO3s04Jr/nSWNQnFrK0uUgc+LECa1du9ZxV0a6ecfEVYSZEvLx8VHLli21bt06R1t+fr7WrVundu3aubEy1xhjNGLECC1dulTr169X7dq1nba3bNlS5cuXd7regwcPKjEx0XG97dq107fffuv0B+/yH8zLP/zatWvndIzLfS4fw5PGtUuXLvr222+1Z88ex9KqVSv179/f8d8325hI0h133FHgsf1Dhw6pVq1akqTatWuratWqTvWmpaXpm2++cRqXCxcuaOfOnY4+69evV35+vtq2bevos2nTJuXm5jr6rF27VrfeeqsqVqzo6HOlsSsrWVlZKlfO+a9RLy8v5efnS7o5x+T3PGkMilNLWbkcZA4fPqwvvvhCoaGhTttvxjG5Ju6egWxFCxcuNHa73cydO9d899135sknnzQVKlRwenLFKp5++mkTEhJiNmzYYM6cOeNYsrKyHH2GDh1qIiMjzfr1682OHTtMu3btTLt27RzbLz+GfM8995g9e/aY1atXmypVqhT6GPLYsWPN999/b2bMmFHoY8ieOq6/fZrJmJtzTLZt22a8vb3NpEmTzOHDh838+fONv7+/+fDDDx19pkyZYipUqGD+85//mH379pk+ffoU+ghu8+bNzTfffGM2b95s6tWr5/S46YULF0x4eLgZOHCg2b9/v1m4cKHx9/cv8Lipt7e3eeONN8z3339vJk6c6JZHs2NjY0316tUdj2YvWbLEVK5c2YwbN87R52YYk/T0dLN7926ze/duI8nEx8eb3bt3O57M8aQxKE4t13tMcnJyTO/evU2NGjXMnj17nP7u/e2TSTfamFxPhBkXvfPOOyYyMtL4+PiYNm3amK+//trdJblEUqHLnDlzHH1++eUXM2zYMFOxYkXj7+9v+vbta86cOeN0nOPHj5vu3bsbPz8/U7lyZTNmzBiTm5vr1CchIcE0a9bM+Pj4mFtuucXpHJd56rj+PszcrGPy6aefmujoaGO3202DBg3MP//5T6ft+fn5ZsKECSY8PNzY7XbTpUsXc/DgQac+Z8+eNf369TOBgYEmODjYDBkyxKSnpzv12bt3r2nfvr2x2+2mevXqZsqUKQVq+fjjj039+vWNj4+PadSokVm5cmXpX/BVpKWlmZEjR5rIyEjj6+trbrnlFvPSSy85/UC6GcYkISGh0L9HYmNjjTGeNQbFqaU0XGlMjh07VuTfvQkJCTfsmFxPNmN+86sqAQAALIY5MwAAwNIIMwAAwNIIMwAAwNIIMwAAwNIIMwAAwNIIMwAAwNIIMwAAwNIIMwAsZe7cuQXeWA7g5kaYAVCmfvrpJz399NOKjIyU3W5X1apVFRMToy1btri7NAAW5e3uAgDcXB544AHl5ORo3rx5uuWWW5ScnKx169bp7NmzZVZDTk6OfHx8yux8AK4v7swAKDMXLlzQl19+qalTp6pTp06qVauW2rRpo/Hjx6t3796SpPj4eDVu3FgBAQGqWbOmhg0bpoyMjCKP+cMPP6hPnz4KDw9XYGCgWrdurS+++MKpT1RUlF599VUNGjRIwcHBevLJJ9W5c2eNGDHCqd9PP/0kHx+fAm8ZBuDZCDMAykxgYKACAwO1bNkyZWdnF9qnXLlyevvtt3XgwAHNmzdP69ev17hx44o8ZkZGhu69916tW7dOu3fvVrdu3dSrVy8lJiY69XvjjTfUtGlT7d69WxMmTNAf//hHLViwwKmODz/8UNWrV1fnzp1L54IBlAleNAmgTH3yySd64okn9Msvv6hFixbq0KGDHnnkETVp0qTQ/v/+9781dOhQ/fzzz5J+nQA8atQoXbhwochzREdHa+jQoY47L1FRUWrevLmWLl3q6HPx4kVFRERo1qxZeuihhyRJTZs21f3336+JEyeW0tUCKAvcmQFQph544AGdPn1ay5cvV7du3bRhwwa1aNFCc+fOlSR98cUX6tKli6pXr66goCANHDhQZ8+eVVZWVqHHy8jI0PPPP6/bbrtNFSpUUGBgoL7//vsCd2ZatWrltO7r66uBAwdq9uzZkqRdu3Zp//79Gjx4cKlfM4DrizADoMz5+vrq7rvv1oQJE/TVV19p8ODBmjhxoo4fP66ePXuqSZMm+uSTT7Rz507NmDFD0q+Tdgvz/PPPa+nSpZo8ebK+/PJL7dmzR40bNy7QPyAgoMC+f/zjH7V27Vr9+OOPmjNnjjp37qxatWqV/gUDuK54mgmA2zVs2FDLli3Tzp07lZ+frzfffFPlyv36b62PP/74ivtu2bJFgwcPVt++fSX9eqfm+PHjxTpv48aN1apVK7333ntasGCB3n333Wu6DgDuQZgBUGbOnj2rBx98UI899piaNGmioKAg7dixQ9OmTVOfPn1Ut25d5ebm6p133lGvXr20ZcsWzZo164rHrFevnpYsWaJevXrJZrNpwoQJys/PL3ZNf/zjHzVixAgFBAQ4AhEAa+FrJgBlJjAwUG3bttXf/vY33XXXXYqOjtaECRP0xBNP6N1331XTpk0VHx+vqVOnKjo6WvPnz1dcXNwVjxkfH6+KFSvq9ttvV69evRQTE6MWLVoUu6Z+/frJ29tb/fr1k6+v77VeIgA34GkmADe148ePq06dOtq+fXuJQhAAz0GYAXBTys3N1dmzZ/X888/r2LFjvE4BsDC+ZgJwU9qyZYuqVaum7du3X3VeDgDPxp0ZAABgadyZAQAAlkaYAQAAlkaYAQAAlkaYAQAAlkaYAQAAlkaYAQAAlkaYAQAAlkaYAQAAlkaYAQAAlva/d3gjHluJyI0AAAAASUVORK5CYII=\n",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "dist_salary(df_missing)"
+                "genie.plz(\"plot distribution of salary, create bins of 10K each, ignore missing values\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 12,
             "id": "45559024-5905-43df-a021-19a2d0b77dff",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Executor saved to cache file boxplots_of_salary_by_department_12125.py\n"
+                        "Genie cached with id: plot_salary_by_department_20090\n"
                     ]
-                }
-            ],
-            "source": [
-                "dept_salary = PandasGenie(\"make boxplots of salary grouped by department\", columns=df_missing.columns)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 23,
-            "id": "637d39d9-c0bf-4a20-89bc-37af671c77cd",
-            "metadata": {},
-            "outputs": [
+                },
                 {
                     "data": {
-                        "image/png": "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48dr4MCBGjx4sKKjo1W/fn3FxcXd1j4CVd3gwYN16dIlde7cWSNGjNCoUaOsWydcT4cOHfTRRx/pww8/VOvWrTVp0iRNmTJFQ4cOtWoWL16s0NBQxcTE6KmnntLw4cPVuHFjl/W8++67KikpUceOHTV69Ohr/khq1KiRNm7cqIKCAsXExKhjx47685//bAWnYcOGKSIiQp06ddK99957zdEzVG0Ow8UXgIuf/OQnCg4O1vvvv+/uVu6IsrIyRUZG6rnnntPUqVPd3Q5gu0cffVTt2rXj62Nw13H6D7XaxYsXtXDhQsXFxcnT01MffPCB1q9fr9TUVHe3ZpujR49q3bp1iomJUVFRkd5++21lZ2dr0KBB7m4NAGoUQhVqtfJTdW+88YYKCwsVERGhv/3tb4qNjXV3a7bx8PDQkiVLNHbsWBlj1Lp1a61fv16RkZHubg0AahRO/wEAANiAC9UBAABsQKgCAACwAaEKAADABoQqAAAAGxCqAAAAbECoAlCtPfrooxo9erS72wAAQhUA2OGbb76Rw+G45gt03alZs2bcVRy4iwhVAHCbLl++7O4WAFQBhCoA1caFCxc0ePBg1a9fXyEhIZo9e7bLeFFRkcaOHav77rtP9erVU1RUlDZt2mSNL1myRAEBAVq1apWaN28up9OpuLg4HT9+3Ko5cuSI+vXrp6CgINWvX18PP/yw1q9f77KdZs2aaerUqRo8eLD8/Pw0fPhw60u827dvL4fDoUcffVSSNHToUMXHx+vNN99UUFCQAgICNGXKFJWUlGjcuHEKDAzU/fffr8WLF7ts4/jx43ruuecUEBCgwMBA9evXT9988401Xr7eWbNmKSQkRI0aNdKIESNUXFws6cpp0aNHj+qll16Sw+GQw+G43acfwE0QqgBUG+PGjdM//vEP/f3vf9e6deu0adMm7dy50xpPSkrS1q1b9eGHH2rv3r169tln1bt3bx06dMiquXjxot544w2999572rx5s3JzczVgwABrvKCgQI8//rg2bNigXbt2qXfv3urbt6+OHTvm0susWbPUtm1b7dq1SxMnTtT27dslSevXr9epU6f0ySefWLUbN27UyZMnlZaWprfeeku//e1v9eSTT6phw4ZKT0/Xr371K73wwgv69ttvJUnFxcWKi4tTgwYN9OWXX2rz5s2qX7++evfu7XJU7IsvvtCRI0f0xRdfaOnSpVqyZImWLFkiSfrkk090//33a8qUKTp16pROnTpl3y8CwPUZAKgGzp8/b7y9vc1HH31kzfv++++Nr6+vGTVqlDl69Kjx9PQ0J06ccFmuZ8+eZsKECcYYYxYvXmwkmW3btlnjBw4cMJJMenr6DbfdqlUrM3/+fGu6adOmJj4+3qUmOzvbSDK7du1ymT9kyBDTtGlTU1paas2LiIgw3bt3t6ZLSkpMvXr1zAcffGCMMeb99983ERERpqyszKopKioyvr6+5vPPP3dZb0lJiVXz7LPPmueff96lzzlz5txwvwDYiy9UBlAtHDlyRJcvX1ZUVJQ1LzAwUBEREZKkr776SqWlpXrooYdclisqKlKjRo2saS8vLz388MPWdIsWLRQQEKADBw6oc+fOKigoUHJystasWaNTp06ppKREly5duuZIVadOnSrce6tWreTh8X8nBoKCgtS6dWtr2tPTU40aNdKZM2ckSXv27NHhw4fVoEEDl/UUFhbqyJEjLuv19PS0pkNCQvTVV19VuC8A9iJUAagRCgoK5OnpqczMTJegIUn169ev8HrGjh2r1NRUzZo1Sw8++KB8fX31zDPPXHMxer169Sq8zjp16rhMOxyO684rKyuz9qVjx45atmzZNeu69957f3C95esAcPcRqgBUCw888IDq1Kmj9PR0NWnSRJJ07tw5ff3114qJiVH79u1VWlqqM2fOqHv37jdcT0lJiXbs2KHOnTtLkrKyspSbm6vIyEhJ0ubNmzV06FD1799f0pWAc/UF4jfi7e0tSSotLb2d3ZQkdejQQStWrFDjxo3l5+dX6fV4e3vb0g+AiuFCdQDVQv369ZWYmKhx48Zp48aN2rdvn4YOHWqdVnvooYeUkJCgwYMH65NPPlF2dra2b9+u6dOna82aNdZ66tSpoxdffFHp6enKzMzU0KFD1aVLFytkNW/eXJ988ol2796tPXv2aNCgQRU6+tO4cWP5+vpq7dq1On36tPLy8iq9rwkJCbrnnnvUr18/ffnll8rOztamTZs0cuRI62L2imjWrJnS0tJ04sQJfffdd5XuB0DFEKoAVBszZ85U9+7d1bdvX8XGxqpbt27q2LGjNb548WINHjxYL7/8siIiIhQfH6+MjAzryJYk1a1bV+PHj9egQYP0yCOPqH79+lqxYoU1/tZbb6lhw4bq2rWr+vbtq7i4OHXo0OGmvXl5eWnevHn605/+pNDQUPXr16/S+1m3bl2lpaWpSZMmeuqppxQZGanExEQVFhbe0pGrKVOm6JtvvtEDDzzgctoQwJ3hMMYYdzcBAHfDkiVLNHr0aOXm5rq7FQA1EEeqAAAAbECoAgAAsAGn/wAAAGzAkSoAAAAbEKoAAABsQKgCAACwAaEKAADABoQqAAAAGxCqAAAAbECoAgAAsAGhCgAAwAb/H0d+J2TIZjqsAAAAAElFTkSuQmCC\n",
+                        "image/png": "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IiKSAYYyIiIiIhlgKCMiIiKSAYYyIiIiIhlgKCMiIiKSAYYyIiIiIhlgKCMiIiKSAYYyIiIiIhlgKCMiIiKSAYYyIiIiIhlgKCMiIiKSAYYyIiIiIhlgKCMiIiKSAYYyIiIiIhlgKCMiIiKSAYYyIiIiIhlgKCMiIiKSAYYyIiIiIhlgKCMiIiKSAYYyIiIiIhlgKCMiIiKSAb2yLoBI7uIePsGTrNwSj3PjwRPpu55eyV96Jko9OFUxKfE4REQkDwxlRK8Q9/AJ2n1/pFTH/OK3mFIb6/D4tgxmRETlBEMZ0StozpAt+NANta1NSzbW0yzsOhKBbm09YWKkLNFY15MyMGbTuVI5g0dERPLAUEZUCLWtTeFa1axEY+Tk5CDBCmjqaAF9ff1SqoyIiMoL3uhPREREJAMMZUREREQywFBGREREJAMMZUREREQywFBGREREJAMMZUREREQywFBGREREJAMMZUREREQywFBGREREJAMMZUREREQywFBGREREJAMMZUREREQywFBGREREJAMMZUREREQywFBGREREJAMMZUREREQywFBGREREJAMMZUREREQywFBGREREJAMMZUREREQywFBGREREJAMMZUREREQywFBGREREJAMMZUREREQywFBGREREJAMMZUREREQywFBGREREJAMMZUREREQywFBGREREJAMMZUREREQywFBGREREJAMMZUREREQywFBGREREJAMMZUREREQyUKah7OjRo+jevTvs7e2hUCiwfft2rfVCCEydOhV2dnYwMjKCj48Prl27ptUnOTkZAwcOhEqlgrm5OYKCgpCRkaHV58KFC2jdujUMDQ3h4OCA0NDQfLVs2bIFLi4uMDQ0RMOGDbFnz54i10JERERUXGUayp48eYLGjRvjxx9/LHB9aGgoFi1ahOXLlyMyMhImJibw8/PDs2fPpD4DBw7EpUuXEB4ejl27duHo0aMYNmyYtD49PR2+vr5wdHREdHQ05s6di5CQEKxYsULqc+LECfTv3x9BQUE4e/Ys/P394e/vj4sXLxapFiIiIqJiEzIBQPz+++/SslqtFra2tmLu3LlSW2pqqlAqlWLjxo1CCCEuX74sAIioqCipz969e4VCoRD37t0TQgixdOlSYWFhIbKysqQ+EydOFM7OztJy3759RdeuXbXq8fDwEMOHDy90LYWRlpYm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EREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREckAQxkRERGRDDCUEREREcmAXlkXQPSuy8zMxNWrV1/bLzY+FVkJ13HlohHUj8xf29/FxQXGxsalUCEREb0TxDtk9uzZAoAYPXq01Pb06VPx+eefC0tLS2FiYiLef/99kZCQoLXdrVu3RJcuXYSRkZGwsrIS48ePFzk5OVp9Dh8+LJo0aSIMDAxErVq1xKpVq/Ltf8mSJcLR0VEolUrx3nvvicjIyCLVn5aWJgCItLS0Im1H8hYdHS0AlPpXdHR0WT80IiolZ28+FI4Td4mzNx+WdSlUBgr79/+dOVMWFRWFn376CY0aNdJqHzt2LHbv3o0tW7bAzMwMwcHBeP/993H8+HEAQF5eHrp27QpbW1ucOHEC8fHxCAgIgL6+PmbNmgUAiIuLQ9euXfHpp59i/fr1OHjwID755BPY2dnBz88PALBp0yaMGzcOy5cvh4eHBxYsWAA/Pz/ExsbC2tr67T4ZJCsuLi6Ijo5+bb+Mp1nYfTgCXdt5wtRIWahxiYio4lAIIURZF/E6GRkZaNq0KZYuXYqZM2fCzc0NCxYsQFpaGqysrLBhwwb07t0bAHD1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\n",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "dept_salary(df_missing)"
+                "genie.plz(\"make boxplots of salary grouped by department\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 13,
             "id": "538ddd26-4b79-4251-9f40-d8a8fc57673f",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Loading executor from cache file count_high_earners_61505.py, set override = True to rerun\n"
+                        "Genie cached with id: high_earners_26869\n"
                     ]
-                }
-            ],
-            "source": [
-                "dept_100k = PandasGenie(\"how many people in each department make more than 100K?\", columns=df_missing.columns)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 29,
-            "id": "4e2e88e7-ac81-4710-8b45-cd94d3c44912",
-            "metadata": {},
-            "outputs": [
+                },
                 {
                     "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>count</th>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>department</th>\n",
-                            "      <th></th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>engineering</th>\n",
-                            "      <td>20</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>product</th>\n",
-                            "      <td>24</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "</div>"
-                        ],
                         "text/plain": [
-                            "             count\n",
-                            "department        \n",
-                            "engineering     20\n",
-                            "product         24"
+                            "department\n",
+                            "engineering    18\n",
+                            "product        11\n",
+                            "dtype: int64"
                         ]
                     },
-                    "execution_count": 29,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "dept_100k(df_missing)"
+                "genie.plz(\"how many people in each department make more than 100K?\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c28b9343-8f96-4d99-a664-f7035a237ace",
             "metadata": {},
             "source": [
                 "# Inspecting Code\n",
                 "\n",
                 "All the genies export the generated code to the cache_dir path under individual py files. The exact name of the file used can be found in the log generated on execution. These could be of 2 types:\n",
                 "\n",
-                "1. `Executor saved to cache file make_boxplots_25996.py`: this will be shown the first time we run this\n",
-                "2. `Loading executor from cache file count_high_earners_86151.py, set override = True to rerun`: this will be shown when we run the genie after its cached without setting `override=True`\n",
+                "1. `Genie cached with id: high_earners_19109.py`: this will be shown the first time we run this\n",
+                "2. `Loading cached genie id: generate_employee_df_56623.py, set override = True to rerun`: this will be shown when we run the genie after its cached without setting `override=True`\n",
                 "\n",
                 "all cached py files for the starter notebook can be found [here](https://github.com/thismlguy/code-genie/tree/main/docs/notebooks/_cache_starter)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 26,
-            "id": "b09e7679-9cc2-4b21-9d00-726a6035f570",
+            "execution_count": 14,
+            "id": "4c5898dd-a521-4ea2-893f-955540979c81",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "import pandas as pd\n",
-                        "import random\n",
-                        "\n",
-                        "def generate_employee_data():\n",
-                        "    employee_ids = []\n",
-                        "    employee_names = []\n",
-                        "    salaries = []\n",
-                        "    departments = []\n",
-                        "\n",
-                        "    departments_list = ['engineering', 'product']\n",
-                        "    \n",
-                        "    for i in range(100):\n",
-                        "        employee_ids.append(random.randint(100, 999))\n",
-                        "        employee_names.append('Employee_' + str(i))\n",
-                        "        salaries.append(random.randint(50000, 150000))\n",
-                        "        departments.append(random.choice(departments_list))\n",
-                        "\n",
-                        "    df = pd.DataFrame({\n",
-                        "        'id': employee_ids,\n",
-                        "        'name': employee_names,\n",
-                        "        'salary': salaries,\n",
-                        "        'department': departments\n",
-                        "    })\n",
-                        "    \n",
-                        "    return df\n",
-                        "\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "# the code can be inspected using `code` property:\n",
-                "print(data_gen.code)"
+                "# you can read all cached code using the command:\n",
+                "cache = genie.read_cache()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 27,
-            "id": "410d75a1-c890-47e2-b09e-0a9c7654c231",
+            "execution_count": 15,
+            "id": "a2adb6e0-6448-45aa-9b29-e5e7e5a7a021",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "'generate_employee_data_58297.py'"
+                            "dict_keys(['generate_employee_dataframe_16305', 'count_missing_values_57234', 'plot_salary_distribution_88606', 'plot_salary_by_department_20090', 'high_earners_26869'])"
                         ]
                     },
-                    "execution_count": 27,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "# the filename in which a genie is stored can be found using the `filename` property:\n",
-                "data_gen.filename"
+                "# these are all the cached genies available\n",
+                "cache.keys()"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 16,
+            "id": "b09e7679-9cc2-4b21-9d00-726a6035f570",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "def high_earners(df):\n",
+                        "    high_earners_df = df[df['salary'] > 100000]\n",
+                        "    return high_earners_df.groupby('department').size()\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# lets read one of them\n",
+                "print(cache[\"high_earners_26869\"])"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "d6509530-b02e-434a-bb7c-dca49025d0b3",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "code-genie",
             "language": "python",
             "name": "code-genie"
```

### Comparing `code_genie-0.2.1.dev0/docs/requirements.txt` & `code_genie-0.3.0/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.1.dev0/pyproject.toml` & `code_genie-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -47,12 +47,12 @@
 ]
 notebook = [
     "jupyterlab>=3.1,<4",
     "ipykernel>=6.0,<7",
 ]
 
 [project.urls]
-Documentation = "https://TBD"
+Documentation = "https://code-genie.readthedocs.io/en/latest/"
 Source = "https://github.com/thismlguy/code-genie"
 
 [tool.flit.sdist]
 include = ["LICENSE"]
```

### Comparing `code_genie-0.2.1.dev0/tox.ini` & `code_genie-0.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `code_genie-0.2.1.dev0/PKG-INFO` & `code_genie-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code_genie
-Version: 0.2.1.dev0
+Version: 0.3.0
 Summary: Copilot to supercharge your notebooks
 Keywords: copilot,jupyter
 Author-email: Aarshay Jain <aarshay.jain@columbia.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -26,24 +26,24 @@
 Requires-Dist: sphinx==5.3.0 ; extra == "docs"
 Requires-Dist: autodocsumm ; extra == "docs"
 Requires-Dist: sphinx_rtd_theme ; extra == "docs"
 Requires-Dist: nbsphinx ; extra == "docs"
 Requires-Dist: sphinx_gallery ; extra == "docs"
 Requires-Dist: jupyterlab>=3.1,<4 ; extra == "notebook"
 Requires-Dist: ipykernel>=6.0,<7 ; extra == "notebook"
-Project-URL: Documentation, https://TBD
+Project-URL: Documentation, https://code-genie.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/thismlguy/code-genie
 Provides-Extra: build
 Provides-Extra: docs
 Provides-Extra: notebook
 
 # code-genie
 This library is your copilot for jupyter notebooks
 
-Latest version: 0.2.1-dev0
+Latest version: 0.3.0
 
 ## Documentation
 
 - [Starter Notebook](https://code-genie.readthedocs.io/en/main/notebooks/Starter.html)
 - [All Examples](https://code-genie.readthedocs.io/en/main/examples.html)
 - [API Documentation](https://code-genie.readthedocs.io/en/main/api.html)
```

