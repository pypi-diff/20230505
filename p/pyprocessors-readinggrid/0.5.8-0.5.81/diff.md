# Comparing `tmp/pyprocessors-readinggrid-0.5.8.tar.gz` & `tmp/pyprocessors-readinggrid-0.5.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors-readinggrid-0.5.8.tar", last modified: Tue Nov 30 11:25:54 2021, max compression
+gzip compressed data, was "pyprocessors-readinggrid-0.5.81.tar", last modified: Fri May  5 13:28:58 2023, max compression
```

## Comparing `pyprocessors-readinggrid-0.5.8.tar` & `pyprocessors-readinggrid-0.5.81.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0      500 2021-11-26 09:11:13.456292 pyprocessors-readinggrid-0.5.8/.bumpversion.cfg
--rw-r--r--   0        0        0     1750 2021-11-26 09:11:13.456292 pyprocessors-readinggrid-0.5.8/.gitignore
--rw-r--r--   0        0        0      419 2021-11-26 09:11:13.456292 pyprocessors-readinggrid-0.5.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      202 2021-11-26 09:11:13.456292 pyprocessors-readinggrid-0.5.8/.readthedocs.yml
--rw-r--r--   0        0        0      120 2021-11-26 09:11:13.456292 pyprocessors-readinggrid-0.5.8/AUTHORS.md
--rw-r--r--   0        0        0      268 2021-11-26 09:11:13.456292 pyprocessors-readinggrid-0.5.8/CHANGELOG.md
--rw-r--r--   0        0        0      476 2021-11-26 09:11:13.456292 pyprocessors-readinggrid-0.5.8/Dockerfile
--rw-r--r--   0        0        0     8074 2021-11-26 09:11:13.457292 pyprocessors-readinggrid-0.5.8/Jenkinsfile
--rw-r--r--   0        0        0     1082 2021-11-26 09:11:13.457292 pyprocessors-readinggrid-0.5.8/LICENSE
--rw-r--r--   0        0        0     1651 2021-11-26 09:11:13.457292 pyprocessors-readinggrid-0.5.8/README.md
--rw-r--r--   0        0        0      947 2021-11-26 09:11:13.457292 pyprocessors-readinggrid-0.5.8/RELEASE.md
--rw-r--r--   0        0        0     1563 2021-11-26 09:11:13.457292 pyprocessors-readinggrid-0.5.8/bumpversion.py
--rw-r--r--   0        0        0       62 2021-11-26 09:11:13.457292 pyprocessors-readinggrid-0.5.8/docs/.gitignore
--rw-r--r--   0        0        0      268 2021-11-26 09:11:13.457292 pyprocessors-readinggrid-0.5.8/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2021-11-26 09:11:13.457292 pyprocessors-readinggrid-0.5.8/docs/LICENSE
--rw-r--r--   0        0        0        0 2021-11-26 09:11:13.458292 pyprocessors-readinggrid-0.5.8/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2021-11-26 09:11:13.458292 pyprocessors-readinggrid-0.5.8/docs/_templates/.gitkeep
--rw-r--r--   0        0        0     2894 2021-11-26 09:11:13.462292 pyprocessors-readinggrid-0.5.8/docs/conf.py
--rw-r--r--   0        0        0      145 2021-11-26 09:11:13.468292 pyprocessors-readinggrid-0.5.8/docs/index.rst
--rw-r--r--   0        0        0       98 2021-11-26 09:11:13.468292 pyprocessors-readinggrid-0.5.8/mypy.ini
--rw-r--r--   0        0        0     2228 2021-11-26 09:11:13.468292 pyprocessors-readinggrid-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      124 2021-11-30 11:25:52.780788 pyprocessors-readinggrid-0.5.8/src/pyprocessors_readinggrid/__init__.py
--rw-r--r--   0        0        0     2558 2021-11-30 11:23:31.804117 pyprocessors-readinggrid-0.5.8/src/pyprocessors_readinggrid/readinggrid.py
--rw-r--r--   0        0        0     1695 2021-11-26 09:11:13.471292 pyprocessors-readinggrid-0.5.8/tests/data/french.json
--rw-r--r--   0        0        0     1432 2021-11-30 11:25:45.819607 pyprocessors-readinggrid-0.5.8/tests/data/french_grid.json
--rw-r--r--   0        0        0     1031 2021-11-30 11:23:31.806117 pyprocessors-readinggrid-0.5.8/tests/test_readinggrid.py
--rw-r--r--   0        0        0     1170 2021-11-26 09:11:13.471292 pyprocessors-readinggrid-0.5.8/tox.ini
--rw-r--r--   0        0        0     1423 1970-01-01 00:00:00.000000 pyprocessors-readinggrid-0.5.8/setup.py
--rw-r--r--   0        0        0     3489 1970-01-01 00:00:00.000000 pyprocessors-readinggrid-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0      500 2022-10-04 08:09:14.192886 pyprocessors-readinggrid-0.5.81/.bumpversion.cfg
+-rw-r--r--   0        0        0     1750 2022-10-04 08:09:14.196886 pyprocessors-readinggrid-0.5.81/.gitignore
+-rw-r--r--   0        0        0      419 2022-10-04 08:09:14.198886 pyprocessors-readinggrid-0.5.81/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      202 2022-10-04 08:09:14.201886 pyprocessors-readinggrid-0.5.81/.readthedocs.yml
+-rw-r--r--   0        0        0      120 2022-10-04 08:09:14.201886 pyprocessors-readinggrid-0.5.81/AUTHORS.md
+-rw-r--r--   0        0        0      268 2022-10-04 08:09:14.203886 pyprocessors-readinggrid-0.5.81/CHANGELOG.md
+-rw-r--r--   0        0        0      476 2022-10-04 08:09:14.205886 pyprocessors-readinggrid-0.5.81/Dockerfile
+-rw-r--r--   0        0        0    10394 2022-12-15 21:54:21.752273 pyprocessors-readinggrid-0.5.81/Jenkinsfile
+-rw-r--r--   0        0        0     1082 2022-10-04 08:09:14.208886 pyprocessors-readinggrid-0.5.81/LICENSE
+-rw-r--r--   0        0        0     1651 2022-10-04 08:09:14.211887 pyprocessors-readinggrid-0.5.81/README.md
+-rw-r--r--   0        0        0      947 2022-10-04 08:09:14.213887 pyprocessors-readinggrid-0.5.81/RELEASE.md
+-rw-r--r--   0        0        0     1559 2022-10-04 08:09:14.215887 pyprocessors-readinggrid-0.5.81/bumpversion.py
+-rw-r--r--   0        0        0       62 2022-10-04 08:09:14.215887 pyprocessors-readinggrid-0.5.81/docs/.gitignore
+-rw-r--r--   0        0        0      268 2022-10-04 08:09:14.216887 pyprocessors-readinggrid-0.5.81/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2022-10-04 08:09:14.216887 pyprocessors-readinggrid-0.5.81/docs/LICENSE
+-rw-r--r--   0        0        0        0 2022-10-04 08:09:14.216887 pyprocessors-readinggrid-0.5.81/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2022-10-04 08:09:14.217887 pyprocessors-readinggrid-0.5.81/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0     2894 2022-10-04 08:09:14.219887 pyprocessors-readinggrid-0.5.81/docs/conf.py
+-rw-r--r--   0        0        0      145 2022-10-04 08:09:14.220887 pyprocessors-readinggrid-0.5.81/docs/index.rst
+-rw-r--r--   0        0        0       98 2022-10-04 08:09:14.222887 pyprocessors-readinggrid-0.5.81/mypy.ini
+-rw-r--r--   0        0        0     2285 2023-03-16 16:18:07.383609 pyprocessors-readinggrid-0.5.81/pyproject.toml
+-rw-r--r--   0        0        0      125 2023-05-05 13:28:56.928398 pyprocessors-readinggrid-0.5.81/src/pyprocessors_readinggrid/__init__.py
+-rw-r--r--   0        0        0     4712 2023-05-05 13:23:44.969015 pyprocessors-readinggrid-0.5.81/src/pyprocessors_readinggrid/readinggrid.py
+-rw-r--r--   0        0        0     1962 2023-05-05 13:23:44.970016 pyprocessors-readinggrid-0.5.81/tests/data/french.json
+-rw-r--r--   0        0        0     1721 2023-05-05 13:28:54.096322 pyprocessors-readinggrid-0.5.81/tests/data/french_grid.json
+-rw-r--r--   0        0        0     2226 2023-05-05 13:28:54.097323 pyprocessors-readinggrid-0.5.81/tests/data/french_grid_alt.json
+-rw-r--r--   0        0        0     3546 2023-05-05 13:23:44.973016 pyprocessors-readinggrid-0.5.81/tests/test_readinggrid.py
+-rw-r--r--   0        0        0      943 2023-05-05 13:23:44.978016 pyprocessors-readinggrid-0.5.81/tox.ini
+-rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 pyprocessors-readinggrid-0.5.81/setup.py
+-rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 pyprocessors-readinggrid-0.5.81/PKG-INFO
```

### Comparing `pyprocessors-readinggrid-0.5.8/.gitignore` & `pyprocessors-readinggrid-0.5.81/.gitignore`

 * *Files identical despite different names*

### Comparing `pyprocessors-readinggrid-0.5.8/Jenkinsfile` & `pyprocessors-readinggrid-0.5.81/Jenkinsfile`

 * *Files 17% similar despite different names*

```diff
@@ -19,26 +19,36 @@
 
   parameters {
       booleanParam(defaultValue: false, description: 'if set to true (ticked), it will not skip on CI commit', name: 'forcePublishing')
   }
 
   stages {
 
-    stage('Abort when upstream') {
-      steps {
-        script {
-          abortBuild()
+    stage('Catch build termination') {
+      agent {
+        node {
+          label 'built-in'
+          customWorkspace "/home/jenkins/${env.JOB_NAME}"
+        }
+      }
+      stages {
+        stage('Abort if upstream or CI_commit') {
+          steps {
+            script {
+              abortBuild()
+            }
+          }
         }
       }
     }
 
     stage('Generate new version') {
       agent {
         node {
-          label 'master'
+          label 'built-in'
           customWorkspace "/home/jenkins/${env.JOB_NAME}"
         }
       }
 
       stages {
 
         stage('Add credentials') {
@@ -101,27 +111,28 @@
 
       agent {
         // dockerfile agent
         // Mounted volume for Junit reports
         //   - docker: /root/test-reports
         //   - host  : /tmp/_${env.JOB_NAME}/test-reports
         dockerfile {
-          label 'master'
+          label 'built-in'
           customWorkspace "/home/jenkins/${env.JOB_NAME}"
           filename 'Dockerfile'
           args "-u root --privileged -v /tmp/_${env.JOB_NAME}/test-reports:${TEST_REPORT_DIR}"
         }
       }
 
       stages {
 
         stage('Install flit & flake8') {
           steps {
             // remove any previous tox env
             sh 'rm -rf .tox'
+            sh 'python -m pip install pip==22.0.3'
             sh 'pip install --no-cache-dir flit==3.2.0 flake8==3.9.2 flakehell tox'
             sh 'flit install'
           }
         }
 
         stage('Test & lint python code') {
           steps {
@@ -140,14 +151,15 @@
             // remove any previous folder dist
             sh 'rm -rf dist'
             // create (as root) folder dist
             sh 'mkdir dist'
             // pull recent updates of file __init__.py
             withCredentials([gitUsernamePassword(credentialsId: 'bitbucket-user', gitToolName: 'git-tool')]) {
               sh 'git config --global pull.rebase false'
+              sh "git config --global --add safe.directory ${PATH_HOME}/${env.JOB_NAME}"
               sh 'git pull'
             }
             // put back owner of pulled file
             sh 'chown 1000:1000 src/pyprocessors_readinggrid/__init__.py'
             // get git status
             sh 'git status'
             // publish on PyPI
@@ -165,23 +177,43 @@
 
     }
 
   }
 
   post {
     // only triggered when blue or green sign
-    //success {
-    //}
+    success {
+      // node is specified here to get an agent
+      node('built-in') {
+        // keep using customWorkspace to store Junit report
+        ws("/home/jenkins/${env.JOB_NAME}") {
+          script {
+            try {
+              sh "rm -f results.xml"
+              sh "cp /tmp/_${env.JOB_NAME}/test-reports/results.xml results.xml"
+            } catch (Exception e) {
+              echo 'Exception occurred: ' + e.toString()
+            }
+            try {
+              junit 'results.xml'
+            } catch (Exception e) {
+              echo 'Exception occurred: ' + e.toString()
+            }
+            println "sending Systematic Build notification"
+            emailext(body: '${DEFAULT_CONTENT}', mimeType: 'text/html',
+                    replyTo: '${DEFAULT_REPLYTO}', subject: '${DEFAULT_SUBJECT}',
+                    to: '${DEFAULT_RECIPIENTS}')
+          }
+        }
+      }
+    }
     // triggered when red sign
-    //failure {
-    //}
-    // trigger every-works
-    always {
+    failure {
       // node is specified here to get an agent
-      node('master') {
+      node('built-in') {
         // keep using customWorkspace to store Junit report
         ws("/home/jenkins/${env.JOB_NAME}") {
           script {
             try {
               sh "rm -f results.xml"
               sh "cp /tmp/_${env.JOB_NAME}/test-reports/results.xml results.xml"
             } catch (Exception e) {
@@ -196,14 +228,17 @@
             emailext(body: '${DEFAULT_CONTENT}', mimeType: 'text/html',
                     replyTo: '${DEFAULT_REPLYTO}', subject: '${DEFAULT_SUBJECT}',
                     to: '${DEFAULT_RECIPIENTS}')
           }
         }
       }
     }
+    // trigger every-works
+    //always {
+    //}
   }
 
 }
 
 // return FLIT_USERNAME from given file
 def getUserName(path) {
   USERNAME = sh(
@@ -246,16 +281,42 @@
           if ( isRunning ) {
             upstream_running = true
           }
         }
       }
     }
   }
+  // Abort build when upstream detected
   if (upstream_running != null) {
     println 'Aborting build because upstream job detected (' + jobName + ')'
     currentBuild.result = 'ABORTED'
     currentBuild.getRawBuild().getExecutor().interrupt(Result.ABORTED)
     sleep(1)   // Interrupt is not blocking and does not take effect immediately.
-
-    //error('Aborting build because upstream job detected (' + jobName + ')')
+  }
+  // Abort build when last commit is CI commit
+  // returnStatus = 1 when string not found -> Team commit
+  // returnStatus = 0 when string is found  -> CI commit
+  def last_commit_is_team = sh(
+    script: 'git log -1 | grep "\\[Jenkins CI\\]"',
+    returnStatus: true
+  )
+  if (params.forcePublishing) {
+    println "Try to publish, proceeding"
+    last_commit_is_team = 1
+  }
+  def isStartedByUser = currentBuild.rawBuild.getCause(hudson.model.Cause$UserIdCause) != null
+  if (isStartedByUser) {
+    println "Job started by User, proceeding"
+    last_commit_is_team = 1
+  }
+  def isStartedByUpstream = currentBuild.rawBuild.getCause(hudson.model.Cause$UpstreamCause) != null
+  if (isStartedByUpstream) {
+    println "Job started by Upstream, proceeding"
+    last_commit_is_team = 1
+  }
+  if (last_commit_is_team == 0) {
+    println 'Aborting build because last commit has been done by CI'
+    currentBuild.result = 'ABORTED'
+    currentBuild.getRawBuild().getExecutor().interrupt(Result.ABORTED)
+    sleep(1)   // Interrupt is not blocking and does not take effect immediately.
   }
 }
```

### Comparing `pyprocessors-readinggrid-0.5.8/LICENSE` & `pyprocessors-readinggrid-0.5.81/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors-readinggrid-0.5.8/README.md` & `pyprocessors-readinggrid-0.5.81/README.md`

 * *Files identical despite different names*

### Comparing `pyprocessors-readinggrid-0.5.8/RELEASE.md` & `pyprocessors-readinggrid-0.5.81/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pyprocessors-readinggrid-0.5.8/bumpversion.py` & `pyprocessors-readinggrid-0.5.81/bumpversion.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,22 +12,22 @@
         for line in data.split(fin.newlines):
             if "MAJOR_VERSION" in line:
                 result = re.search(r'MAJOR_VERSION\s*=\s*"([0-9]+)"', line)
                 if result:
                     major = int(result.group(1))
                     if part == "major":
                         to_replace = result.group(0)
-                        by_replace = f"MAJOR_VERSION = \"{major + 1}\""
+                        by_replace = f'MAJOR_VERSION = "{major + 1}"'
             if "MINOR_VERSION" in line:
                 result = re.search(r'MINOR_VERSION\s*=\s*"([0-9]+)"', line)
                 if result:
                     minor = int(result.group(1))
                     if part == "minor":
                         to_replace = result.group(0)
-                        by_replace = f"MINOR_VERSION = \"{minor + 1}\""
+                        by_replace = f'MINOR_VERSION = "{minor + 1}"'
     data = data.replace(to_replace, by_replace)
     with Jenkinsfile.open("wt") as fout:
         fout.write(data)
 
     depend_string = f"{major}.{minor}.0,<{major}.{minor + 1}.0"
     new_depend_string = f"{major}.{minor + 1}.0,<{major}.{minor + 2}.0"
     with pyprojectfile.open("r", encoding="utf-8") as fin:
```

### Comparing `pyprocessors-readinggrid-0.5.8/docs/LICENSE` & `pyprocessors-readinggrid-0.5.81/docs/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprocessors-readinggrid-0.5.8/docs/conf.py` & `pyprocessors-readinggrid-0.5.81/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-readinggrid-0.5.8/pyproject.toml` & `pyprocessors-readinggrid-0.5.81/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     "pytest-flake8",
     "pytest-black",
 #    "hypothesis",
     "flake8==3.9.2",
     "tox",
     "pandas==1.2.3",
     "openpyxl==3.0.7",
+    "tox",
+    "dirty-equals"
 ]
 docs = [
     "sphinx",
     "sphinx-rtd-theme",
     "m2r2",  # markdown support
     "sphinxcontrib.apidoc",  # run sphinx-apidoc when building docs
     "jupyter_sphinx",   # for execution of code snippets in the documentation
@@ -60,14 +62,15 @@
 [tool.flakehell]
 exclude = ["README.md"]
 format = "colored"
 #format = "junit-xml"
 max_line_length = 120
 show_source = true
 #whitelist = "../../allowlist.txt"
+extended_default_ignore=[]
 
 [tool.flakehell.plugins]
 flake8-bandit = ["+*", "-S322"]
 flake8-bugbear = ["+*"]
 flake8-builtins = ["+*"]
 flake8-comprehensions = ["+*"]
 #flake8-darglint = ["+*"]
```

### Comparing `pyprocessors-readinggrid-0.5.8/tests/data/french.json` & `pyprocessors-readinggrid-0.5.81/tests/data/french.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9833333333333334%*

 * *Differences: {"'annotations'": "{0: {'labelName': 'wiki1', 'label': 'Wikidata1'}, 2: {'labelName': 'wiki2', "*

 * *                  "'label': 'Wikidata2'}, 3: {'labelName': 'wiki3', 'label': 'Wikidata3'}, insert: "*

 * *                  "[(1, OrderedDict([('end', 8), ('start', 7), ('createdBy', 'oterrier'), "*

 * *                  "('createdDate', '2021-11-26T08:07:57.438Z'), ('labelName', 'wiki3'), "*

 * *                  "('modifiedDate', '2021-11-26T08:07:57.438Z'), ('status', 'OK'), ('text', '1'), "*

 * *                  "('label', 'Wi […]*

```diff
@@ -1,37 +1,48 @@
 {
     "annotations": [
         {
             "createdBy": "oterrier",
             "createdDate": "2021-11-26T08:07:57.438Z",
             "end": 6,
-            "label": "Wikidata",
-            "labelName": "wikidata",
+            "label": "Wikidata1",
+            "labelName": "wiki1",
             "modifiedDate": "2021-11-26T08:07:57.438Z",
             "start": 0,
             "status": "OK",
             "text": "Phrase"
         },
         {
             "createdBy": "oterrier",
+            "createdDate": "2021-11-26T08:07:57.438Z",
+            "end": 8,
+            "label": "Wikidata3",
+            "labelName": "wiki3",
+            "modifiedDate": "2021-11-26T08:07:57.438Z",
+            "start": 7,
+            "status": "OK",
+            "text": "1"
+        },
+        {
+            "createdBy": "oterrier",
             "createdDate": "2021-11-26T08:08:04.385Z",
             "end": 83,
-            "label": "Wikidata",
-            "labelName": "wikidata",
+            "label": "Wikidata2",
+            "labelName": "wiki2",
             "modifiedDate": "2021-11-26T08:08:04.385Z",
             "start": 82,
             "status": "OK",
             "text": "3"
         },
         {
             "createdBy": "oterrier",
             "createdDate": "2021-11-26T08:08:09.44Z",
             "end": 183,
-            "label": "Wikidata",
-            "labelName": "wikidata",
+            "label": "Wikidata3",
+            "labelName": "wiki3",
             "modifiedDate": "2021-11-26T08:08:09.44Z",
             "start": 173,
             "status": "OK",
             "text": "annotation"
         }
     ],
     "categories": [],
```

### Comparing `pyprocessors-readinggrid-0.5.8/tests/data/french_grid.json` & `pyprocessors-readinggrid-0.5.81/tests/data/french_grid.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {'0': "{'annotations': {0: {'labelName': 'wiki1', 'label': 'Wikidata1'}, 2: {'labelName': 'wiki2', "*

 * *      "'label': 'Wikidata2'}, 3: {'labelName': 'wiki3', 'label': 'Wikidata3'}, insert: [(1, "*

 * *      "OrderedDict([('start', 7), ('end', 8), ('labelName', 'wiki3'), ('label', 'Wikidata3'), "*

 * *      "('text', '1'), ('createdBy', 'oterrier'), ('createdDate', '2021-11-26T08:07:57.438Z'), "*

 * *      "('modifiedDate', '2021-11-26T08:07:57.438Z'), ('status', 'OK')]))]}}"}*

```diff
@@ -1,38 +1,49 @@
 [
     {
         "annotations": [
             {
                 "createdBy": "oterrier",
                 "createdDate": "2021-11-26T08:07:57.438Z",
                 "end": 6,
-                "label": "Wikidata",
-                "labelName": "wikidata",
+                "label": "Wikidata1",
+                "labelName": "wiki1",
                 "modifiedDate": "2021-11-26T08:07:57.438Z",
                 "start": 0,
                 "status": "OK",
                 "text": "Phrase"
             },
             {
                 "createdBy": "oterrier",
+                "createdDate": "2021-11-26T08:07:57.438Z",
+                "end": 8,
+                "label": "Wikidata3",
+                "labelName": "wiki3",
+                "modifiedDate": "2021-11-26T08:07:57.438Z",
+                "start": 7,
+                "status": "OK",
+                "text": "1"
+            },
+            {
+                "createdBy": "oterrier",
                 "createdDate": "2021-11-26T08:08:04.385Z",
                 "end": 45,
-                "label": "Wikidata",
-                "labelName": "wikidata",
+                "label": "Wikidata2",
+                "labelName": "wiki2",
                 "modifiedDate": "2021-11-26T08:08:04.385Z",
                 "start": 44,
                 "status": "OK",
                 "text": "3"
             },
             {
                 "createdBy": "oterrier",
                 "createdDate": "2021-11-26T08:08:09.44Z",
                 "end": 107,
-                "label": "Wikidata",
-                "labelName": "wikidata",
+                "label": "Wikidata3",
+                "labelName": "wiki3",
                 "modifiedDate": "2021-11-26T08:08:09.44Z",
                 "start": 97,
                 "status": "OK",
                 "text": "annotation"
             }
         ],
         "categories": [],
```

### Comparing `pyprocessors-readinggrid-0.5.8/setup.py` & `pyprocessors-readinggrid-0.5.81/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,22 +25,24 @@
  'test': ['pytest',
           'pytest-cov',
           'pytest-flake8',
           'pytest-black',
           'flake8==3.9.2',
           'tox',
           'pandas==1.2.3',
-          'openpyxl==3.0.7']}
+          'openpyxl==3.0.7',
+          'tox',
+          'dirty-equals']}
 
 entry_points = \
 {'pyprocessors.plugins': ['readinggrid = '
                           'pyprocessors_readinggrid.readinggrid:ReadingGridProcessor']}
 
 setup(name='pyprocessors-readinggrid',
-      version='0.5.8',
+      version='0.5.81',
       description='Processor that generate a focussed reading-grid (keep only the sentences containing annotation)',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://github.com/oterrier/pyprocessors_readinggrid/',
       packages=packages,
       package_data=package_data,
       package_dir=package_dir,
```

### Comparing `pyprocessors-readinggrid-0.5.8/PKG-INFO` & `pyprocessors-readinggrid-0.5.81/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-readinggrid
-Version: 0.5.8
+Version: 0.5.81
 Summary: Processor that generate a focussed reading-grid (keep only the sentences containing annotation)
 Home-page: https://github.com/oterrier/pyprocessors_readinggrid/
 Keywords: 
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -33,14 +33,16 @@
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-flake8 ; extra == "test"
 Requires-Dist: pytest-black ; extra == "test"
 Requires-Dist: flake8==3.9.2 ; extra == "test"
 Requires-Dist: tox ; extra == "test"
 Requires-Dist: pandas==1.2.3 ; extra == "test"
 Requires-Dist: openpyxl==3.0.7 ; extra == "test"
+Requires-Dist: tox ; extra == "test"
+Requires-Dist: dirty-equals ; extra == "test"
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
 
 # pyprocessors_readinggrid
 
 [![license](https://img.shields.io/github/license/oterrier/pyprocessors_readinggrid)](https://github.com/oterrier/pyprocessors_readinggrid/blob/master/LICENSE)
```

