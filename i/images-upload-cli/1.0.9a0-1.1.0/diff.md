# Comparing `tmp/images_upload_cli-1.0.9a0.tar.gz` & `tmp/images_upload_cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "images_upload_cli-1.0.9a0.tar", max compression
+gzip compressed data, was "images_upload_cli-1.1.0.tar", max compression
```

## Comparing `images_upload_cli-1.0.9a0.tar` & `images_upload_cli-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2023-02-19 11:29:11.646036 images_upload_cli-1.0.9a0/LICENSE
--rw-r--r--   0        0        0     5338 2023-02-19 11:29:11.650036 images_upload_cli-1.0.9a0/README.md
--rw-r--r--   0        0        0     2741 2023-02-19 11:29:11.650036 images_upload_cli-1.0.9a0/pyproject.toml
--rwxr-xr-x   0        0        0      160 2023-02-19 11:29:11.650036 images_upload_cli-1.0.9a0/src/images_upload_cli/__init__.py
--rwxr-xr-x   0        0        0      180 2023-02-19 11:29:11.650036 images_upload_cli-1.0.9a0/src/images_upload_cli/__main__.py
--rwxr-xr-x   0        0        0     1733 2023-02-19 11:29:11.650036 images_upload_cli-1.0.9a0/src/images_upload_cli/cli.py
--rwxr-xr-x   0        0        0     9699 2023-02-19 11:29:11.650036 images_upload_cli-1.0.9a0/src/images_upload_cli/upload.py
--rwxr-xr-x   0        0        0     3072 2023-02-19 11:29:11.650036 images_upload_cli-1.0.9a0/src/images_upload_cli/util.py
--rw-r--r--   0        0        0     6407 1970-01-01 00:00:00.000000 images_upload_cli-1.0.9a0/setup.py
--rw-r--r--   0        0        0     6299 1970-01-01 00:00:00.000000 images_upload_cli-1.0.9a0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4984 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/README.md
+-rw-r--r--   0        0        0     2740 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0      160 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/src/images_upload_cli/__init__.py
+-rwxr-xr-x   0        0        0      180 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/src/images_upload_cli/__main__.py
+-rwxr-xr-x   0        0        0     1733 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/src/images_upload_cli/cli.py
+-rwxr-xr-x   0        0        0     9324 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/src/images_upload_cli/upload.py
+-rwxr-xr-x   0        0        0     3072 2023-02-24 11:07:46.979031 images_upload_cli-1.1.0/src/images_upload_cli/util.py
+-rw-r--r--   0        0        0     6050 1970-01-01 00:00:00.000000 images_upload_cli-1.1.0/setup.py
+-rw-r--r--   0        0        0     5943 1970-01-01 00:00:00.000000 images_upload_cli-1.1.0/PKG-INFO
```

### Comparing `images_upload_cli-1.0.9a0/LICENSE` & `images_upload_cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `images_upload_cli-1.0.9a0/README.md` & `images_upload_cli-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,50 +22,49 @@
 
 ```sh
 yay -S python-images-upload-cli
 ```
 
 ## Hostings
 
-| host                                           | key required | return example                                       |
-| :--------------------------------------------- | :----------: | :--------------------------------------------------- |
-| [beeimg](https://beeimg.com/)                  |      -       | `https://beeimg.com/images/{id}.png`                 |
-| [catbox](https://catbox.moe/)                  |      -       | `https://files.catbox.moe/{id}`                      |
-| [fastpic](https://fastpic.org/)                |      -       | `https://i120.fastpic.org/big/2022/0730/d9/{id}.png` |
-| [filecoffee](https://file.coffee/)             |      -       | `https://file.coffee/u/{id}.png`                     |
-| [freeimage](https://freeimage.host/)           |      -       | `https://iili.io/{id}.png`                           |
-| [gyazo](https://gyazo.com/)                    |      +       | `https://i.gyazo.com/{id}.png`                       |
-| [imageban](https://imageban.ru/)               |      +       | `https://i2.imageban.ru/out/2022/07/30/{id}.png`     |
-| [imagebin](https://imagebin.ca/)               |      -       | `https://ibin.co/{id}.png`                           |
-| [imgbb](https://imgbb.com/)                    |      +       | `https://i.ibb.co/{id}/image.png`                    |
-| [imgchest](https://imgchest.com/)              |      +       | `https://cdn.imgchest.com/files/{id}.png`            |
-| [imgur](https://imgur.com/)                    |      -       | `https://i.imgur.com/{id}.png`                       |
-| [pictshare](https://pictshare.net/)            |      -       | `https://pictshare.net/{id}.png`                     |
-| [pixeldrain](https://pixeldrain.com/)          |      -       | `https://pixeldrain.com/api/file/{id}`               |
-| [pixhost](https://pixhost.to/)                 |      -       | `https://img75.pixhost.to/images/69/{id}_img.png`    |
-| [ptpimg](https://ptpimg.me/)                   |      +       | `https://ptpimg.me/{id}.png`                         |
-| [screenshotting](https://screenshotting.site/) |      -       | `https://screenshotting.site/i/{id}.png`             |
-| [smms](https://sm.ms/)                         |      +       | `https://s2.loli.net/2022/07/30/{id}.png`            |
-| [sxcu](https://sxcu.net/)                      |      -       | `https://sxcu.net/{id}.png`                          |
-| [telegraph](https://telegra.ph/)               |      -       | `https://telegra.ph/file/{id}.png`                   |
-| [thumbsnap](https://thumbsnap.com/)            |      +       | `https://thumbsnap.com/i/{id}.png`                   |
-| [up2sha](https://up2sha.re/)                   |      +       | `https://up2sha.re/media/raw/{id}.png`               |
-| [uplio](https://upl.io/)                       |      +       | `https://upl.io/i/{id}.png`                          |
-| [uploadcare](https://uploadcare.com/)          |      +       | `https://ucarecdn.com/{id}/img.png`                  |
-| [vgy](https://vgy.me/)                         |      +       | `https://i.vgy.me/{id}.png`                          |
+| host                                  | key required | return example                                       |
+| :------------------------------------ | :----------: | :--------------------------------------------------- |
+| [beeimg](https://beeimg.com/)         |      -       | `https://beeimg.com/images/{id}.png`                 |
+| [catbox](https://catbox.moe/)         |      -       | `https://files.catbox.moe/{id}`                      |
+| [fastpic](https://fastpic.org/)       |      -       | `https://i120.fastpic.org/big/2022/0730/d9/{id}.png` |
+| [filecoffee](https://file.coffee/)    |      -       | `https://file.coffee/u/{id}.png`                     |
+| [freeimage](https://freeimage.host/)  |      -       | `https://iili.io/{id}.png`                           |
+| [gyazo](https://gyazo.com/)           |      +       | `https://i.gyazo.com/{id}.png`                       |
+| [imageban](https://imageban.ru/)      |      +       | `https://i2.imageban.ru/out/2022/07/30/{id}.png`     |
+| [imagebin](https://imagebin.ca/)      |      -       | `https://ibin.co/{id}.png`                           |
+| [imgbb](https://imgbb.com/)           |      +       | `https://i.ibb.co/{id}/image.png`                    |
+| [imgchest](https://imgchest.com/)     |      +       | `https://cdn.imgchest.com/files/{id}.png`            |
+| [imgur](https://imgur.com/)           |      -       | `https://i.imgur.com/{id}.png`                       |
+| [pictshare](https://pictshare.net/)   |      -       | `https://pictshare.net/{id}.png`                     |
+| [pixeldrain](https://pixeldrain.com/) |      -       | `https://pixeldrain.com/api/file/{id}`               |
+| [pixhost](https://pixhost.to/)        |      -       | `https://img75.pixhost.to/images/69/{id}_img.png`    |
+| [ptpimg](https://ptpimg.me/)          |      +       | `https://ptpimg.me/{id}.png`                         |
+| [smms](https://sm.ms/)                |      +       | `https://s2.loli.net/2022/07/30/{id}.png`            |
+| [sxcu](https://sxcu.net/)             |      -       | `https://sxcu.net/{id}.png`                          |
+| [telegraph](https://telegra.ph/)      |      -       | `https://telegra.ph/file/{id}.png`                   |
+| [thumbsnap](https://thumbsnap.com/)   |      +       | `https://thumbsnap.com/i/{id}.png`                   |
+| [up2sha](https://up2sha.re/)          |      +       | `https://up2sha.re/media/raw/{id}.png`               |
+| [uplio](https://upl.io/)              |      +       | `https://upl.io/i/{id}.png`                          |
+| [uploadcare](https://uploadcare.com/) |      +       | `https://ucarecdn.com/{id}/img.png`                  |
+| [vgy](https://vgy.me/)                |      +       | `https://i.vgy.me/{id}.png`                          |
 
 ## Usage
 
 ```sh
 Usage: images-upload-cli [OPTIONS] IMAGES...
 
   Upload images via APIs.
 
 Options:
-  -h, --hosting [catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|pictshare|pixeldrain|pixhost|ptpimg|screenshotting|smms|sxcu|telegraph|thumbsnap|up2sha|uplio|uploadcare|vgy]
+  -h, --hosting [beeimg|catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|pictshare|pixeldrain|pixhost|ptpimg|smms|sxcu|telegraph|thumbsnap|up2sha|uplio|uploadcare|vgy]
                                   [default: imgur]
   -b, --bbcode                    Add bbcode tags.
   -t, --thumbnail                 Add caption thumbnail and bbcode tags.
   -c, --clipboard / -C, --no-clipboard
                                   Copy result to clipboard.  [default: c]
   --version                       Show the version and exit.
   --help                          Show this message and exit.
```

### Comparing `images_upload_cli-1.0.9a0/pyproject.toml` & `images_upload_cli-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "images-upload-cli"
-version = "1.0.9a0"
+version = "1.1.0"
 description = "Upload images via APIs"
 authors = ["DeadNews <uhjnnn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/images-upload-cli"
 repository = "https://github.com/DeadNews/images-upload-cli"
 keywords = ["cli", "imgur", "image-upload", "upload-images", "upload-pictures"]
@@ -14,41 +14,41 @@
 images-upload-cli = "images_upload_cli.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 click = "^8.1.3"
 pillow = "^9.4.0"
 pyperclip = "^1.8.2"
-python-dotenv = ">=0.21,<1.0.0"
-requests = "^2.28.1"
+python-dotenv = ">=0.21,<2.0.0"
+requests = "^2.28.2"
 
 [tool.poetry.group.ci.dependencies]
 bandit = "^1.7.4"
 black = "^22.12.0"
 flake8 = "^6.0.0"
-flake8-bugbear = "^22.12.6"
+flake8-bugbear = "^23.2.13"
 flake8-builtins = "^2.1.0"
 flake8-comprehensions = "^3.10.1"
-flake8-implicit-str-concat = "^0.3.0"
+flake8-implicit-str-concat = "^0.4.0"
 flake8-pie = "^0.16.0"
 flake8-pyproject = "^1.2.2"
-flake8-pytest-style = "^1.6.0"
-flake8-requirements = "^1.7.5"
+flake8-pytest-style = "^1.7.2"
+flake8-requirements = "^1.7.7"
 flake8-simplify = "^0.19.3"
-flake8-unused-arguments = "^0.0.12"
+flake8-unused-arguments = "^0.0.13"
 flake8-use-pathlib = "^0.3.0"
-isort = "^5.11.4"
-mypy = "^0.991"
+isort = "^5.12.0"
+mypy = "^1.0.1"
 pep8-naming = "^0.13.3"
-poethepoet = "^0.17.1"
+poethepoet = "^0.18.1"
 safety = "^2.3.5"
-types-requests = "^2.28.11.7"
+types-requests = "^2.28.11.14"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.2.0"
+pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `images_upload_cli-1.0.9a0/src/images_upload_cli/cli.py` & `images_upload_cli-1.1.0/src/images_upload_cli/cli.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-1.0.9a0/src/images_upload_cli/upload.py` & `images_upload_cli-1.1.0/src/images_upload_cli/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,27 +222,14 @@
     )
     if not response.ok:
         raise UploadError(response.json())
 
     return f"https://ptpimg.me/{response.json()[0]['code']}.{response.json()[0]['ext']}"
 
 
-def screenshotting_upload(img: bytes) -> str:
-    name = f"img.{get_img_ext(img)}"
-
-    response = post(
-        url="https://screenshotting.site/upload",
-        files={"img": (name, img)},
-    )
-    if not response.ok:
-        raise UploadError(response.text)
-
-    return response.json()["url"].replace("http://", "https://")
-
-
 def smms_upload(img: bytes) -> str:
     key = get_env_val("SMMS_KEY")
 
     response = post(
         url="https://sm.ms/api/v2/upload",
         headers={"Authorization": key},
         files={"smfile": img},
@@ -369,15 +356,14 @@
     "imgbb": imgbb_upload,
     "imgchest": imgchest_upload,
     "imgur": imgur_upload,
     "pictshare": pictshare_upload,
     "pixeldrain": pixeldrain_upload,
     "pixhost": pixhost_upload,
     "ptpimg": ptpimg_upload,
-    "screenshotting": screenshotting_upload,
     "smms": smms_upload,
     "sxcu": sxcu_upload,
     "telegraph": telegraph_upload,
     "thumbsnap": thumbsnap_upload,
     "up2sha": up2sha_upload,
     "uplio": uplio_upload,
     "uploadcare": uploadcare_upload,
```

### Comparing `images_upload_cli-1.0.9a0/src/images_upload_cli/util.py` & `images_upload_cli-1.1.0/src/images_upload_cli/util.py`

 * *Files identical despite different names*

### Comparing `images_upload_cli-1.0.9a0/setup.py` & `images_upload_cli-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0',
  'pillow>=9.4.0,<10.0.0',
  'pyperclip>=1.8.2,<2.0.0',
- 'python-dotenv>=0.21,<1.0.0',
- 'requests>=2.28.1,<3.0.0']
+ 'python-dotenv>=0.21,<2.0.0',
+ 'requests>=2.28.2,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['images-upload-cli = images_upload_cli.cli:cli']}
 
 setup_kwargs = {
     'name': 'images-upload-cli',
-    'version': '1.0.9a0',
+    'version': '1.1.0',
     'description': 'Upload images via APIs',
-    'long_description': '# images-upload-cli\n\n> Upload images via APIs\n\n[![PyPI version](https://img.shields.io/pypi/v/images-upload-cli)](https://pypi.org/project/images-upload-cli)\n[![AUR version](https://img.shields.io/aur/version/python-images-upload-cli)](https://aur.archlinux.org/packages/python-images-upload-cli)\n[![CI/CD](https://github.com/DeadNews/images-upload-cli/actions/workflows/python-app.yml/badge.svg)](https://github.com/DeadNews/images-upload-cli/actions/workflows/python-app.yml)\n[![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/images-upload-cli/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/images-upload-cli/main)\n[![codecov](https://codecov.io/gh/DeadNews/images-upload-cli/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/images-upload-cli)\n\n## Installation\n\nPyPI\n\n```sh\npip install images-upload-cli\n# or\npipx install images-upload-cli\n```\n\nAUR\n\n```sh\nyay -S python-images-upload-cli\n```\n\n## Hostings\n\n| host                                           | key required | return example                                       |\n| :--------------------------------------------- | :----------: | :--------------------------------------------------- |\n| [beeimg](https://beeimg.com/)                  |      -       | `https://beeimg.com/images/{id}.png`                 |\n| [catbox](https://catbox.moe/)                  |      -       | `https://files.catbox.moe/{id}`                      |\n| [fastpic](https://fastpic.org/)                |      -       | `https://i120.fastpic.org/big/2022/0730/d9/{id}.png` |\n| [filecoffee](https://file.coffee/)             |      -       | `https://file.coffee/u/{id}.png`                     |\n| [freeimage](https://freeimage.host/)           |      -       | `https://iili.io/{id}.png`                           |\n| [gyazo](https://gyazo.com/)                    |      +       | `https://i.gyazo.com/{id}.png`                       |\n| [imageban](https://imageban.ru/)               |      +       | `https://i2.imageban.ru/out/2022/07/30/{id}.png`     |\n| [imagebin](https://imagebin.ca/)               |      -       | `https://ibin.co/{id}.png`                           |\n| [imgbb](https://imgbb.com/)                    |      +       | `https://i.ibb.co/{id}/image.png`                    |\n| [imgchest](https://imgchest.com/)              |      +       | `https://cdn.imgchest.com/files/{id}.png`            |\n| [imgur](https://imgur.com/)                    |      -       | `https://i.imgur.com/{id}.png`                       |\n| [pictshare](https://pictshare.net/)            |      -       | `https://pictshare.net/{id}.png`                     |\n| [pixeldrain](https://pixeldrain.com/)          |      -       | `https://pixeldrain.com/api/file/{id}`               |\n| [pixhost](https://pixhost.to/)                 |      -       | `https://img75.pixhost.to/images/69/{id}_img.png`    |\n| [ptpimg](https://ptpimg.me/)                   |      +       | `https://ptpimg.me/{id}.png`                         |\n| [screenshotting](https://screenshotting.site/) |      -       | `https://screenshotting.site/i/{id}.png`             |\n| [smms](https://sm.ms/)                         |      +       | `https://s2.loli.net/2022/07/30/{id}.png`            |\n| [sxcu](https://sxcu.net/)                      |      -       | `https://sxcu.net/{id}.png`                          |\n| [telegraph](https://telegra.ph/)               |      -       | `https://telegra.ph/file/{id}.png`                   |\n| [thumbsnap](https://thumbsnap.com/)            |      +       | `https://thumbsnap.com/i/{id}.png`                   |\n| [up2sha](https://up2sha.re/)                   |      +       | `https://up2sha.re/media/raw/{id}.png`               |\n| [uplio](https://upl.io/)                       |      +       | `https://upl.io/i/{id}.png`                          |\n| [uploadcare](https://uploadcare.com/)          |      +       | `https://ucarecdn.com/{id}/img.png`                  |\n| [vgy](https://vgy.me/)                         |      +       | `https://i.vgy.me/{id}.png`                          |\n\n## Usage\n\n```sh\nUsage: images-upload-cli [OPTIONS] IMAGES...\n\n  Upload images via APIs.\n\nOptions:\n  -h, --hosting [catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|pictshare|pixeldrain|pixhost|ptpimg|screenshotting|smms|sxcu|telegraph|thumbsnap|up2sha|uplio|uploadcare|vgy]\n                                  [default: imgur]\n  -b, --bbcode                    Add bbcode tags.\n  -t, --thumbnail                 Add caption thumbnail and bbcode tags.\n  -c, --clipboard / -C, --no-clipboard\n                                  Copy result to clipboard.  [default: c]\n  --version                       Show the version and exit.\n  --help                          Show this message and exit.\n```\n\n## Env variables\n\n```ini\nCAPTION_FONT= # The default font is system dependent.\n\nFREEIMAGE_KEY=\nGYAZO_TOKEN=\nIMAGEBAN_TOKEN=\nIMGBB_KEY=\nIMGCHEST_KEY=\nIMGUR_CLIENT_ID=\nPTPIMG_KEY=\nSMMS_KEY=\nTHUMBSNAP_KEY=\nUP2SHA_KEY=\nUPLIO_KEY=\nUPLOADCARE_KEY=\nVGY_KEY=\n```\n\nYou can set these in environment variables, or in `.env` file:\n\n- Unix: `~/.config/images-upload-cli/.env`\n- MacOS: `~/Library/Application Support/images-upload-cli/.env`\n- Windows: `C:\\Users\\<user>\\AppData\\Roaming\\images-upload-cli\\.env`\n',
+    'long_description': '# images-upload-cli\n\n> Upload images via APIs\n\n[![PyPI version](https://img.shields.io/pypi/v/images-upload-cli)](https://pypi.org/project/images-upload-cli)\n[![AUR version](https://img.shields.io/aur/version/python-images-upload-cli)](https://aur.archlinux.org/packages/python-images-upload-cli)\n[![CI/CD](https://github.com/DeadNews/images-upload-cli/actions/workflows/python-app.yml/badge.svg)](https://github.com/DeadNews/images-upload-cli/actions/workflows/python-app.yml)\n[![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/images-upload-cli/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/images-upload-cli/main)\n[![codecov](https://codecov.io/gh/DeadNews/images-upload-cli/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/images-upload-cli)\n\n## Installation\n\nPyPI\n\n```sh\npip install images-upload-cli\n# or\npipx install images-upload-cli\n```\n\nAUR\n\n```sh\nyay -S python-images-upload-cli\n```\n\n## Hostings\n\n| host                                  | key required | return example                                       |\n| :------------------------------------ | :----------: | :--------------------------------------------------- |\n| [beeimg](https://beeimg.com/)         |      -       | `https://beeimg.com/images/{id}.png`                 |\n| [catbox](https://catbox.moe/)         |      -       | `https://files.catbox.moe/{id}`                      |\n| [fastpic](https://fastpic.org/)       |      -       | `https://i120.fastpic.org/big/2022/0730/d9/{id}.png` |\n| [filecoffee](https://file.coffee/)    |      -       | `https://file.coffee/u/{id}.png`                     |\n| [freeimage](https://freeimage.host/)  |      -       | `https://iili.io/{id}.png`                           |\n| [gyazo](https://gyazo.com/)           |      +       | `https://i.gyazo.com/{id}.png`                       |\n| [imageban](https://imageban.ru/)      |      +       | `https://i2.imageban.ru/out/2022/07/30/{id}.png`     |\n| [imagebin](https://imagebin.ca/)      |      -       | `https://ibin.co/{id}.png`                           |\n| [imgbb](https://imgbb.com/)           |      +       | `https://i.ibb.co/{id}/image.png`                    |\n| [imgchest](https://imgchest.com/)     |      +       | `https://cdn.imgchest.com/files/{id}.png`            |\n| [imgur](https://imgur.com/)           |      -       | `https://i.imgur.com/{id}.png`                       |\n| [pictshare](https://pictshare.net/)   |      -       | `https://pictshare.net/{id}.png`                     |\n| [pixeldrain](https://pixeldrain.com/) |      -       | `https://pixeldrain.com/api/file/{id}`               |\n| [pixhost](https://pixhost.to/)        |      -       | `https://img75.pixhost.to/images/69/{id}_img.png`    |\n| [ptpimg](https://ptpimg.me/)          |      +       | `https://ptpimg.me/{id}.png`                         |\n| [smms](https://sm.ms/)                |      +       | `https://s2.loli.net/2022/07/30/{id}.png`            |\n| [sxcu](https://sxcu.net/)             |      -       | `https://sxcu.net/{id}.png`                          |\n| [telegraph](https://telegra.ph/)      |      -       | `https://telegra.ph/file/{id}.png`                   |\n| [thumbsnap](https://thumbsnap.com/)   |      +       | `https://thumbsnap.com/i/{id}.png`                   |\n| [up2sha](https://up2sha.re/)          |      +       | `https://up2sha.re/media/raw/{id}.png`               |\n| [uplio](https://upl.io/)              |      +       | `https://upl.io/i/{id}.png`                          |\n| [uploadcare](https://uploadcare.com/) |      +       | `https://ucarecdn.com/{id}/img.png`                  |\n| [vgy](https://vgy.me/)                |      +       | `https://i.vgy.me/{id}.png`                          |\n\n## Usage\n\n```sh\nUsage: images-upload-cli [OPTIONS] IMAGES...\n\n  Upload images via APIs.\n\nOptions:\n  -h, --hosting [beeimg|catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|pictshare|pixeldrain|pixhost|ptpimg|smms|sxcu|telegraph|thumbsnap|up2sha|uplio|uploadcare|vgy]\n                                  [default: imgur]\n  -b, --bbcode                    Add bbcode tags.\n  -t, --thumbnail                 Add caption thumbnail and bbcode tags.\n  -c, --clipboard / -C, --no-clipboard\n                                  Copy result to clipboard.  [default: c]\n  --version                       Show the version and exit.\n  --help                          Show this message and exit.\n```\n\n## Env variables\n\n```ini\nCAPTION_FONT= # The default font is system dependent.\n\nFREEIMAGE_KEY=\nGYAZO_TOKEN=\nIMAGEBAN_TOKEN=\nIMGBB_KEY=\nIMGCHEST_KEY=\nIMGUR_CLIENT_ID=\nPTPIMG_KEY=\nSMMS_KEY=\nTHUMBSNAP_KEY=\nUP2SHA_KEY=\nUPLIO_KEY=\nUPLOADCARE_KEY=\nVGY_KEY=\n```\n\nYou can set these in environment variables, or in `.env` file:\n\n- Unix: `~/.config/images-upload-cli/.env`\n- MacOS: `~/Library/Application Support/images-upload-cli/.env`\n- Windows: `C:\\Users\\<user>\\AppData\\Roaming\\images-upload-cli\\.env`\n',
     'author': 'DeadNews',
     'author_email': 'uhjnnn@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DeadNews/images-upload-cli',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `images_upload_cli-1.0.9a0/PKG-INFO` & `images_upload_cli-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: images-upload-cli
-Version: 1.0.9a0
+Version: 1.1.0
 Summary: Upload images via APIs
 Home-page: https://github.com/DeadNews/images-upload-cli
 License: MIT
 Keywords: cli,imgur,image-upload,upload-images,upload-pictures
 Author: DeadNews
 Author-email: uhjnnn@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
-Requires-Dist: python-dotenv (>=0.21,<1.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: python-dotenv (>=0.21,<2.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/DeadNews/images-upload-cli
 Description-Content-Type: text/markdown
 
 # images-upload-cli
 
 > Upload images via APIs
 
@@ -47,50 +47,49 @@
 
 ```sh
 yay -S python-images-upload-cli
 ```
 
 ## Hostings
 
-| host                                           | key required | return example                                       |
-| :--------------------------------------------- | :----------: | :--------------------------------------------------- |
-| [beeimg](https://beeimg.com/)                  |      -       | `https://beeimg.com/images/{id}.png`                 |
-| [catbox](https://catbox.moe/)                  |      -       | `https://files.catbox.moe/{id}`                      |
-| [fastpic](https://fastpic.org/)                |      -       | `https://i120.fastpic.org/big/2022/0730/d9/{id}.png` |
-| [filecoffee](https://file.coffee/)             |      -       | `https://file.coffee/u/{id}.png`                     |
-| [freeimage](https://freeimage.host/)           |      -       | `https://iili.io/{id}.png`                           |
-| [gyazo](https://gyazo.com/)                    |      +       | `https://i.gyazo.com/{id}.png`                       |
-| [imageban](https://imageban.ru/)               |      +       | `https://i2.imageban.ru/out/2022/07/30/{id}.png`     |
-| [imagebin](https://imagebin.ca/)               |      -       | `https://ibin.co/{id}.png`                           |
-| [imgbb](https://imgbb.com/)                    |      +       | `https://i.ibb.co/{id}/image.png`                    |
-| [imgchest](https://imgchest.com/)              |      +       | `https://cdn.imgchest.com/files/{id}.png`            |
-| [imgur](https://imgur.com/)                    |      -       | `https://i.imgur.com/{id}.png`                       |
-| [pictshare](https://pictshare.net/)            |      -       | `https://pictshare.net/{id}.png`                     |
-| [pixeldrain](https://pixeldrain.com/)          |      -       | `https://pixeldrain.com/api/file/{id}`               |
-| [pixhost](https://pixhost.to/)                 |      -       | `https://img75.pixhost.to/images/69/{id}_img.png`    |
-| [ptpimg](https://ptpimg.me/)                   |      +       | `https://ptpimg.me/{id}.png`                         |
-| [screenshotting](https://screenshotting.site/) |      -       | `https://screenshotting.site/i/{id}.png`             |
-| [smms](https://sm.ms/)                         |      +       | `https://s2.loli.net/2022/07/30/{id}.png`            |
-| [sxcu](https://sxcu.net/)                      |      -       | `https://sxcu.net/{id}.png`                          |
-| [telegraph](https://telegra.ph/)               |      -       | `https://telegra.ph/file/{id}.png`                   |
-| [thumbsnap](https://thumbsnap.com/)            |      +       | `https://thumbsnap.com/i/{id}.png`                   |
-| [up2sha](https://up2sha.re/)                   |      +       | `https://up2sha.re/media/raw/{id}.png`               |
-| [uplio](https://upl.io/)                       |      +       | `https://upl.io/i/{id}.png`                          |
-| [uploadcare](https://uploadcare.com/)          |      +       | `https://ucarecdn.com/{id}/img.png`                  |
-| [vgy](https://vgy.me/)                         |      +       | `https://i.vgy.me/{id}.png`                          |
+| host                                  | key required | return example                                       |
+| :------------------------------------ | :----------: | :--------------------------------------------------- |
+| [beeimg](https://beeimg.com/)         |      -       | `https://beeimg.com/images/{id}.png`                 |
+| [catbox](https://catbox.moe/)         |      -       | `https://files.catbox.moe/{id}`                      |
+| [fastpic](https://fastpic.org/)       |      -       | `https://i120.fastpic.org/big/2022/0730/d9/{id}.png` |
+| [filecoffee](https://file.coffee/)    |      -       | `https://file.coffee/u/{id}.png`                     |
+| [freeimage](https://freeimage.host/)  |      -       | `https://iili.io/{id}.png`                           |
+| [gyazo](https://gyazo.com/)           |      +       | `https://i.gyazo.com/{id}.png`                       |
+| [imageban](https://imageban.ru/)      |      +       | `https://i2.imageban.ru/out/2022/07/30/{id}.png`     |
+| [imagebin](https://imagebin.ca/)      |      -       | `https://ibin.co/{id}.png`                           |
+| [imgbb](https://imgbb.com/)           |      +       | `https://i.ibb.co/{id}/image.png`                    |
+| [imgchest](https://imgchest.com/)     |      +       | `https://cdn.imgchest.com/files/{id}.png`            |
+| [imgur](https://imgur.com/)           |      -       | `https://i.imgur.com/{id}.png`                       |
+| [pictshare](https://pictshare.net/)   |      -       | `https://pictshare.net/{id}.png`                     |
+| [pixeldrain](https://pixeldrain.com/) |      -       | `https://pixeldrain.com/api/file/{id}`               |
+| [pixhost](https://pixhost.to/)        |      -       | `https://img75.pixhost.to/images/69/{id}_img.png`    |
+| [ptpimg](https://ptpimg.me/)          |      +       | `https://ptpimg.me/{id}.png`                         |
+| [smms](https://sm.ms/)                |      +       | `https://s2.loli.net/2022/07/30/{id}.png`            |
+| [sxcu](https://sxcu.net/)             |      -       | `https://sxcu.net/{id}.png`                          |
+| [telegraph](https://telegra.ph/)      |      -       | `https://telegra.ph/file/{id}.png`                   |
+| [thumbsnap](https://thumbsnap.com/)   |      +       | `https://thumbsnap.com/i/{id}.png`                   |
+| [up2sha](https://up2sha.re/)          |      +       | `https://up2sha.re/media/raw/{id}.png`               |
+| [uplio](https://upl.io/)              |      +       | `https://upl.io/i/{id}.png`                          |
+| [uploadcare](https://uploadcare.com/) |      +       | `https://ucarecdn.com/{id}/img.png`                  |
+| [vgy](https://vgy.me/)                |      +       | `https://i.vgy.me/{id}.png`                          |
 
 ## Usage
 
 ```sh
 Usage: images-upload-cli [OPTIONS] IMAGES...
 
   Upload images via APIs.
 
 Options:
-  -h, --hosting [catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|pictshare|pixeldrain|pixhost|ptpimg|screenshotting|smms|sxcu|telegraph|thumbsnap|up2sha|uplio|uploadcare|vgy]
+  -h, --hosting [beeimg|catbox|fastpic|filecoffee|freeimage|gyazo|imageban|imagebin|imgbb|imgchest|imgur|pictshare|pixeldrain|pixhost|ptpimg|smms|sxcu|telegraph|thumbsnap|up2sha|uplio|uploadcare|vgy]
                                   [default: imgur]
   -b, --bbcode                    Add bbcode tags.
   -t, --thumbnail                 Add caption thumbnail and bbcode tags.
   -c, --clipboard / -C, --no-clipboard
                                   Copy result to clipboard.  [default: c]
   --version                       Show the version and exit.
   --help                          Show this message and exit.
```

