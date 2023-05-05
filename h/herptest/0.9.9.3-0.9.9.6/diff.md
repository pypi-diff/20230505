# Comparing `tmp/herptest-0.9.9.3.tar.gz` & `tmp/herptest-0.9.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/herptest-0.9.9.3.tar", last modified: Wed Jul 22 19:24:08 2020, max compression
+gzip compressed data, was "dist/herptest-0.9.9.6.tar", last modified: Tue Feb  9 23:00:50 2021, max compression
```

## Comparing `herptest-0.9.9.3.tar` & `herptest-0.9.9.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 jjb       (1000) jjb       (1000)        0 2020-07-22 19:24:08.277793 herptest-0.9.9.3/
--rwxrwxrwx   0 jjb       (1000) jjb       (1000)      259 2020-07-22 19:24:08.271798 herptest-0.9.9.3/PKG-INFO
--rwxrwxrwx   0 jjb       (1000) jjb       (1000)     8345 2020-01-03 03:00:20.000000 herptest-0.9.9.3/README
-drwxrwxrwx   0 jjb       (1000) jjb       (1000)        0 2020-07-22 19:24:08.125793 herptest-0.9.9.3/herptest/
--rwxrwxrwx   0 jjb       (1000) jjb       (1000)        0 2019-12-31 22:26:35.000000 herptest-0.9.9.3/herptest/__init__.py
--rwxrwxrwx   0 jjb       (1000) jjb       (1000)     2897 2020-07-22 19:18:59.000000 herptest-0.9.9.3/herptest/extract_lms_archive.py
--rwxrwxrwx   0 jjb       (1000) jjb       (1000)    15974 2020-07-22 19:23:49.000000 herptest-0.9.9.3/herptest/run_test_suite.py
--rwxrwxrwx   0 jjb       (1000) jjb       (1000)    14012 2020-07-22 17:44:51.000000 herptest-0.9.9.3/herptest/toolbox.py
-drwxrwxrwx   0 jjb       (1000) jjb       (1000)        0 2020-07-22 19:24:08.246795 herptest-0.9.9.3/herptest.egg-info/
--rwxrwxrwx   0 jjb       (1000) jjb       (1000)      259 2020-07-22 19:24:07.000000 herptest-0.9.9.3/herptest.egg-info/PKG-INFO
--rwxrwxrwx   0 jjb       (1000) jjb       (1000)      278 2020-07-22 19:24:07.000000 herptest-0.9.9.3/herptest.egg-info/SOURCES.txt
--rwxrwxrwx   0 jjb       (1000) jjb       (1000)        1 2020-07-22 19:24:07.000000 herptest-0.9.9.3/herptest.egg-info/dependency_links.txt
--rwxrwxrwx   0 jjb       (1000) jjb       (1000)       96 2020-07-22 19:24:07.000000 herptest-0.9.9.3/herptest.egg-info/entry_points.txt
--rwxrwxrwx   0 jjb       (1000) jjb       (1000)        9 2020-07-22 19:24:07.000000 herptest-0.9.9.3/herptest.egg-info/top_level.txt
--rwxrwxrwx   0 jjb       (1000) jjb       (1000)       38 2020-07-22 19:24:08.278795 herptest-0.9.9.3/setup.cfg
--rwxrwxrwx   0 jjb       (1000) jjb       (1000)      528 2020-07-22 18:45:57.000000 herptest-0.9.9.3/setup.py
+drwxrwxrwx   0 jjb       (1000) jjb       (1000)        0 2021-02-09 23:00:50.259588 herptest-0.9.9.6/
+-rwxrwxrwx   0 jjb       (1000) jjb       (1000)      259 2021-02-09 23:00:50.255587 herptest-0.9.9.6/PKG-INFO
+-rwxrwxrwx   0 jjb       (1000) jjb       (1000)     8345 2020-01-03 03:00:20.000000 herptest-0.9.9.6/README
+drwxrwxrwx   0 jjb       (1000) jjb       (1000)        0 2021-02-09 23:00:50.161831 herptest-0.9.9.6/herptest/
+-rwxrwxrwx   0 jjb       (1000) jjb       (1000)        0 2019-12-31 22:26:35.000000 herptest-0.9.9.6/herptest/__init__.py
+-rwxrwxrwx   0 jjb       (1000) jjb       (1000)     2974 2020-07-22 21:39:17.000000 herptest-0.9.9.6/herptest/extract_lms_archive.py
+-rwxrwxrwx   0 jjb       (1000) jjb       (1000)    19369 2021-02-09 23:00:34.000000 herptest-0.9.9.6/herptest/run_test_suite.py
+-rwxrwxrwx   0 jjb       (1000) jjb       (1000)    29066 2021-02-09 22:57:10.000000 herptest-0.9.9.6/herptest/toolbox.py
+drwxrwxrwx   0 jjb       (1000) jjb       (1000)        0 2021-02-09 23:00:50.240936 herptest-0.9.9.6/herptest.egg-info/
+-rwxrwxrwx   0 jjb       (1000) jjb       (1000)      259 2021-02-09 23:00:49.000000 herptest-0.9.9.6/herptest.egg-info/PKG-INFO
+-rwxrwxrwx   0 jjb       (1000) jjb       (1000)      278 2021-02-09 23:00:50.000000 herptest-0.9.9.6/herptest.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jjb       (1000) jjb       (1000)        1 2021-02-09 23:00:49.000000 herptest-0.9.9.6/herptest.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jjb       (1000) jjb       (1000)       96 2021-02-09 23:00:49.000000 herptest-0.9.9.6/herptest.egg-info/entry_points.txt
+-rwxrwxrwx   0 jjb       (1000) jjb       (1000)        9 2021-02-09 23:00:49.000000 herptest-0.9.9.6/herptest.egg-info/top_level.txt
+-rwxrwxrwx   0 jjb       (1000) jjb       (1000)       38 2021-02-09 23:00:50.259588 herptest-0.9.9.6/setup.cfg
+-rwxrwxrwx   0 jjb       (1000) jjb       (1000)      528 2021-02-09 23:00:22.000000 herptest-0.9.9.6/setup.py
```

### Comparing `herptest-0.9.9.3/README` & `herptest-0.9.9.6/README`

 * *Files identical despite different names*

### Comparing `herptest-0.9.9.3/herptest/extract_lms_archive.py` & `herptest-0.9.9.6/herptest/extract_lms_archive.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-#!/usr/bin/python
-
-import zipfile
-import tempfile
-import glob
-import os
-import os.path
-import shutil
-import argparse
-
-def main():
-    parser = argparse.ArgumentParser(description="Unzips submissions", formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_help = True
-    parser.add_argument('filename', help='submissions zip file')
-    parser.add_argument('destination', help='where to extract submissions to')
-    args = parser.parse_args()
-
-    tmp_path = tempfile.mkdtemp()
-    with zipfile.ZipFile(args.filename) as zf:
-        zf.extractall(path=tmp_path)
-
-    submissions = glob.glob(os.path.join(tmp_path, "*"))
-    success_count = 0
-    warning_count = 0
-    for submission in submissions:
-        success_count += 1
-        attributes = os.path.basename(submission).split("_", 3)
-
-        # Deal with Canvas appending "LATE" to student names with an underscore (add to name with a dash)
-        if len(attributes) > 1 and attributes[1] == "LATE":
-            attributes[0:2] = [attributes[0] + "-LATE"]
-            if len(attributes) == 3:
-                attributes[2:] = attributes[2].split("_", 1)
-
-        # Handle missing elements in filenames as best we can (limited to weird Canvas output configurations)
-        if len(attributes) == 1:
-            print("Warning: [%s] cannot be reformatted. Assuming generic filename." % submission)
-            attributes[1:1] = ["", "", "submission.file"]
-            warning_count += 1
-        elif len(attributes) == 2:
-            attributes[1:1] = ["", ""]
-        elif len(attributes) == 3:
-            attributes[2:2] = [""]
-
-        student, lms_id, submission_id, filename = attributes
-
-        # Extract submission information from the Canvas formatted filename.
-        header, ext = os.path.splitext(filename)
-
-        # Handle the special case of gzip files (which by default contain another extension)
-        if ext.lower() == ".gz":
-            header, ext = os.path.splitext(header)
-            ext = ext + ".gz"
-
-        # Account for Canvas's submission count suffix.
-        count_info = header.rsplit("-", 1)
-        if len(count_info) > 1:
-            try:
-                int(count_info[1])
-                filename = count_info[0] + ext
-            except ValueError:
-                pass # Right side of "-" was not a number, so this is not a Canvas submission count suffix.
-
-        student_path = os.path.join(args.destination, student + "_" + lms_id)
-        if not os.path.isdir(student_path):
-            os.mkdir(student_path)
-
-        if ext.lower() == ".zip":
-            with zipfile.ZipFile(submission) as zf:
-                zf.extractall(path=student_path)
-        else:
-            shutil.copyfile(submission, os.path.join(student_path, filename))
-    print("Successfuly extracted %d submissions with %d warnings." % (success_count, warning_count))
-
-if __name__ == "__main__":
-    main()
-
+#!/usr/bin/python
+
+import zipfile
+import tempfile
+import glob
+import os
+import os.path
+import shutil
+import argparse
+
+def main():
+    parser = argparse.ArgumentParser(description="Unzips submissions", formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser.add_help = True
+    parser.add_argument('filename', help='submissions zip file')
+    parser.add_argument('destination', help='where to extract submissions to')
+    args = parser.parse_args()
+
+    tmp_path = tempfile.mkdtemp()
+    with zipfile.ZipFile(args.filename) as zf:
+        zf.extractall(path=tmp_path)
+
+    submissions = glob.glob(os.path.join(tmp_path, "*"))
+    success_count = 0
+    warning_count = 0
+    for submission in submissions:
+        success_count += 1
+        attributes = os.path.basename(submission).split("_", 3)
+
+        # Deal with Canvas appending "LATE" to student names with an underscore (add to name with a dash)
+        if len(attributes) > 1 and attributes[1] == "LATE":
+            attributes[0:2] = [attributes[0] + "-LATE"]
+            if len(attributes) == 3:
+                attributes[2:] = attributes[2].split("_", 1)
+
+        # Handle missing elements in filenames as best we can (limited to weird Canvas output configurations)
+        if len(attributes) == 1:
+            print("Warning: [%s] cannot be reformatted. Assuming generic filename." % submission)
+            attributes[1:1] = ["", "", "submission.file"]
+            warning_count += 1
+        elif len(attributes) == 2:
+            attributes[1:1] = ["", ""]
+        elif len(attributes) == 3:
+            attributes[2:2] = [""]
+
+        student, lms_id, submission_id, filename = attributes
+
+        # Extract submission information from the Canvas formatted filename.
+        header, ext = os.path.splitext(filename)
+
+        # Handle the special case of gzip files (which by default contain another extension)
+        if ext.lower() == ".gz":
+            header, ext = os.path.splitext(header)
+            ext = ext + ".gz"
+
+        # Account for Canvas's submission count suffix.
+        count_info = header.rsplit("-", 1)
+        if len(count_info) > 1:
+            try:
+                int(count_info[1])
+                filename = count_info[0] + ext
+            except ValueError:
+                pass # Right side of "-" was not a number, so this is not a Canvas submission count suffix.
+
+        student_path = os.path.join(args.destination, student + "_" + lms_id)
+        if not os.path.isdir(student_path):
+            os.mkdir(student_path)
+
+        if ext.lower() == ".zip":
+            with zipfile.ZipFile(submission) as zf:
+                zf.extractall(path=student_path)
+        else:
+            shutil.copyfile(submission, os.path.join(student_path, filename))
+    print("Successfuly extracted %d submissions with %d warnings." % (success_count, warning_count))
+
+if __name__ == "__main__":
+    main()
+
```

### Comparing `herptest-0.9.9.3/herptest/run_test_suite.py` & `herptest-0.9.9.6/herptest/run_test_suite.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import numbers
 import string
 import logging
 
 from . import toolbox
 from concurrent import futures
 
-VERSION = '0.9.9.2'
+VERSION = '0.9.9.6'
 
 cfg = argparse.Namespace()
 cfg.runtime = argparse.Namespace()
 
 
 # handle command line args
 def parse_arguments():
@@ -31,14 +31,15 @@
 #    cfg.logformat = "%(message)s"
 #    cfg.logformat = "[%(levelname)s] %(message)s"
     parser = argparse.ArgumentParser(description='A program to run a set of tests for a programming assignment.')
     parser.add_help = True
     parser.add_argument('suite_path', nargs='?', default="./", help='path of test suite to load')
     parser.add_argument('target_path', nargs='?', default="Projects", help='path of target projects (by subdirectory)')
     parser.add_argument('-V', '--version', action='version', version='%(prog)s ' + VERSION)
+    parser.add_argument('-t', '--threads', dest='threads', action='store_true', help='use threads instead of processes')
     parser.add_argument('-q', '--quiet', dest='INFO', action='store_false', help='execute in quiet mode (console)')
     parser.add_argument('-w', '--warn', dest='WARN', action='store_true', help='display warning information (console)')
     parser.add_argument('-d', '--debug', dest='DEBUG', action='store_true', help='capture debug information (logfile)')
     parser.add_argument('-s', '--set', dest='set', default="*", help = 'test only projects designated (e.g., *_LATE*')
     config = parser.parse_args(sys.argv[1:])
     config.logformat = "%(message)s"
     return config
@@ -50,59 +51,75 @@
     result_error = None
     current_dir = os.getcwd()
 
     # If there is a not a specified build directory, fall back to the source directory instead.
     if not build_root:
         build_root = source_root
 
-    if build_root:
-        # If the build exists, remove old project folder, recreate it, and switch to it.
-        if os.path.isdir(build_root) and not build_root == source_root:
-            shutil.rmtree(build_root)
-        if not os.path.exists(build_root):
-            os.makedirs(build_root)
-        os.chdir(build_root)
+    # If the build exists, remove old project folder, recreate it, and switch to it.
+    if os.path.isdir(build_root) and not build_root == source_root:
+        shutil.rmtree(build_root)
+    if not os.path.exists(build_root):
+        os.makedirs(build_root)
+    os.chdir(build_root)
 
     try:
         # Prepare to make substitutions to the prep / build commands if applicable.
-        replacements = {key : value for key, value in build_cfg.__dict__.items() if not key in ['prep_cmd', 'compile_cmd']}
+        replacements = {key : value for key, value in build_cfg.__dict__.items() if not key in ['prep_cmd', 'compile_cmd', 'post_cmd']}
         replacements["source_dir"] = source_root
         replacements["build_dir"] = build_root
         template = string.Template("")
 
-        if build_cfg.prep_cmd:
-            # Apply substitutions from the build configuration to the prep command
-            prep_cmd = []
-            for entry in build_cfg.prep_cmd:
-                template.template = entry
-                prep_cmd.append(template.substitute(**replacements))
-            subprocess.check_output(prep_cmd, stderr=subprocess.STDOUT)
+        if hasattr(build_cfg, 'prep_cmd') and build_cfg.prep_cmd:
+            # Apply substitutions from the build configuration to the prep command(s)
+            source_cmds = build_cfg.prep_cmd if isinstance(build_cfg.prep_cmd, tuple) else (build_cfg.prep_cmd,)
+            for source_cmd in source_cmds:
+                prep_cmd = []
+                for entry in source_cmd:
+                    template.template = entry
+                    prep_cmd.append(template.substitute(**replacements))
+                subprocess.check_output(prep_cmd, stderr=subprocess.STDOUT)
 
-        if build_cfg.compile_cmd:
+        if hasattr(build_cfg, 'compile_cmd') and build_cfg.compile_cmd:
             # Apply substitutions from the build configuration to the compile command
-            compile_cmd = []
-            for entry in build_cfg.compile_cmd:
-                template.template = entry
-                compile_cmd.append(template.substitute(**replacements))
-            subprocess.check_output(compile_cmd, stderr=subprocess.STDOUT)
+            source_cmds = build_cfg.compile_cmd if isinstance(build_cfg.compile_cmd, tuple) else (build_cfg.compile_cmd,)
+            for source_cmd in source_cmds:
+                compile_cmd = []
+                for entry in build_cfg.compile_cmd:
+                    template.template = entry
+                    compile_cmd.append(template.substitute(**replacements))
+                subprocess.check_output(compile_cmd, stderr=subprocess.STDOUT)
+
+        if hasattr(build_cfg, 'post_cmd') and build_cfg.post_cmd:
+            # Apply substitutions from the build configuration to the prep command(s)
+            source_cmds = build_cfg.post_cmd if isinstance(build_cfg.post_cmd, tuple) else (build_cfg.post_cmd,)
+            for source_cmd in source_cmds:
+                post_cmd = []
+                for entry in source_cmd:
+                    template.template = entry
+                    post_cmd.append(template.substitute(**replacements))
+                subprocess.check_output(post_cmd, stderr=subprocess.STDOUT)
 
     except (subprocess.CalledProcessError, FileNotFoundError) as error:
         result_error = error
 
     os.chdir(current_dir)
     return result_error
 
 
 def run_suite_tests(framework, subject, proj_settings):
     results = []
+    exception_sets = {}
 
+    print("In suite for", subject)
     # Run each project's tests.
     for project in proj_settings.projects:
         display_name, identifier, points = project
-        data_set, score, penalty_totals = run_project_tests(identifier, framework, subject, proj_settings)
+        data_set, score, penalty_totals, exception_list = run_project_tests(identifier, framework, subject, proj_settings)
+        exception_sets[project] = exception_list
 
         # If the project didn't compile, just add a single line indicating that.
         if isinstance(data_set, str):
             logging.error("Error: %s" % data_set)
             data_set = [[], ["Grade: 0 (Does not compile / run)"]]
             score = 0
 
@@ -125,18 +142,19 @@
             # Apply the penalties and scale to the number of points
             score = (score - min(proj_settings.max_penalty, overall_penalty)) * points
 
         # Add to the results list.
         data_set = [ ["Project %s" % display_name] ] + data_set
         results.append((display_name, score, data_set))
 
-    return results
+    return results, exception_sets
 
 
 def run_project_tests(name, framework, subject, proj_settings):
+    exception_list = []
     context = proj_settings.initialize_project(name, framework, subject, proj_settings)
     penalty_totals = [0] * (len(proj_settings.test_case_penalties) + len(proj_settings.project_penalties))
     num_of_tests = proj_settings.get_number_of_tests(context)
 
     if not isinstance(num_of_tests, int) or num_of_tests == 0:
         proj_settings.shutdown_project(context)
         return "get_number_of_tests() returned [%s]" % num_of_tests, None, None
@@ -149,23 +167,29 @@
     header.extend(["%s-Pen" % name for name, pct in proj_settings.test_case_penalties])
     data_set.append(header)
 
     score = 0
     for test_num in range(0, num_of_tests):
         # Set up the row for this test and run it.
         row = [ '%d' % test_num ]
-        case_result = proj_settings.run_case_test(test_num, context)
+        try:
+            case_result = proj_settings.run_case_test(test_num, context)
+        except Exception as e:
+            stack_trace = traceback.format_exc()
+            exception_list.append("Test %d, %s: %s\n%s" % (test_num, type(e).__name__, e, stack_trace))
+            case_result = 0
+
 
         # If we successfuly completed the run, this should be a number; otherwise, a message.
         if isinstance(case_result, numbers.Number):
             case_score = case_result
             message = None
         else:
             case_score = 0
-            message = case_result
+            message = str(case_result)
 
         score += case_score
         # Add score, run message, and description as applicable
         row.append('%.2f%%' % (case_score * 100))
         row.append(message if message else '')
         row.append(proj_settings.get_test_description(test_num, context) if round(case_score, 10) < 1 else '')
 
@@ -180,30 +204,30 @@
             # If we successfuly completed the run, this should be a tuple; otherwise, a message.
             if isinstance(pen_result, tuple):
                 penalty_name, magnitude = pen_result
                 message = None
             else:
                 penalty_name = None
                 maginitude = 0
-                message = pen_result
+                message = str(pen_result)
 
             penalty_totals[penalty_num] += penalty * magnitude * case_score / num_of_tests
             row.append('%.2f%%' % (penalty * 100))
 
         # Add this test data to the data set.
         data_set.append(row)
 
     for penalty_num in range(0, len(proj_settings.project_penalties)):
         penalty_name, magnitude = proj_settings.project_penalties[penalty_num]
         penalty = proj_settings.run_project_penalty(penalty_num, context) * score * magnitude
         penalty_totals[penalty_num + len(proj_settings.test_case_penalties)] = penalty
 
     # Return the data set, score (proportion), and penalty totals
     proj_settings.shutdown_project(context)
-    return data_set, score / num_of_tests, penalty_totals
+    return data_set, score / num_of_tests, penalty_totals, exception_list
 
 
 def process_configuration(config):
     if not config:
         return None
 
     # Fill default values
@@ -223,14 +247,32 @@
     config.build.subject_bin = os.path.abspath(config.build.subject_bin) if config.build.subject_bin else None
     config.build.framework_src = os.path.abspath(config.build.framework_src) if config.build.framework_src else None
     config.build.framework_bin = os.path.abspath(config.build.framework_bin) if config.build.framework_bin else None
 
     return config
 
 # For each submission, copy the base files, then the submission, into the destination folder.
+def prepare_and_init_framework(build_cfg, proj_cfg):
+    # Build the environment components (only need to do this once.)
+    if build_cfg.framework_src and build_cfg.framework_bin:
+        if build_cfg.prep_cmd or build_cfg.compile_cmd:
+            logging.info("Prepping / building framework environment... ")
+            result_error = build_project(build_cfg.framework_src, build_cfg.framework_bin, build_cfg)
+            if result_error:
+                logging.info("%s: %s\n" % (type(result_error).__name__, result_error))
+                return
+
+        logging.info("initializing framework... ")
+        framework_data = proj_cfg.initialize_framework(cfg)
+        logging.info("done.\n")
+    else:
+        framework_data = None
+    return framework_data
+
+# For each submission, copy the base files, then the submission, into the destination folder.
 def prepare_and_test_submission(framework_context, submission):
     global cfg
     if not os.path.isdir(submission):
         return None
 
     # Create a new subject folder with base files in it - then copy oer the submission to be tested.
     if os.path.isdir(cfg.build.destination):
@@ -258,86 +300,99 @@
         logging.error("Error initializing subject %s - %s: %s" % (submission, type(error).__name__, error))
         logging.info("error initializing (see logs)... ")
 
     os.chdir(starting_dir)
     logging.info("done.\n")
 
     starting_dir = os.getcwd()
-    results = run_suite_tests(framework_context, subject_context, cfg.project)
+    results, exception_sets = run_suite_tests(framework_context, subject_context, cfg.project)
     cfg.project.shutdown_subject(subject_context)
     os.chdir(starting_dir)
-    return results
+    return results, exception_sets
 
 
 def main():
     global cfg # TODO: Eventually take this out of global scope for simplicity
     cfg.runtime = parse_arguments()
-    console_logger = toolbox.SelectiveStreamHandler(INFO=cfg.runtime.INFO, WARNING=cfg.runtime.WARN, CRITICAL=True)
-    logging.basicConfig(format=cfg.runtime.logformat, level=logging.DEBUG, handlers=[console_logger])
-    root_logger = logging.getLogger('')
-    console_logger.terminator = ""
 
     # Save the current folder and move to the test suite location.
     starting_dir = os.getcwd()
     os.chdir(cfg.runtime.suite_path)
 
-    # Load the config for this project.
-    if not (config := process_configuration(toolbox.load_module("config.py"))):
-        logging.info("Error: no configuration file. Exiting...\n")
+    # Load the config file for this project.
+    if not os.path.isfile("config.py") or not (config := process_configuration(toolbox.load_module("config.py"))):
+        sys.stderr.write("Error: no configuration file. Exiting...\n")
         return
 
     cfg.project = config.project
     cfg.build = config.build
     cfg.general = config.general
 
-    # Prepare paths
+    # Prepare result paths.
     if not os.path.isdir(cfg.general.result_path):
         os.mkdir(cfg.general.result_path)
-
     summary_path = os.path.join(cfg.general.result_path, cfg.general.summary_file)
 
+    # Set up logging.
+    console_logger = toolbox.SelectiveStreamHandler(INFO=cfg.runtime.INFO, WARNING=cfg.runtime.WARN, CRITICAL=True)
+    logging.basicConfig(format=cfg.runtime.logformat, level=logging.DEBUG, handlers=[console_logger])
+    root_logger = logging.getLogger('')
+    console_logger.terminator = ""
+
+    logfile = os.path.join(cfg.general.result_path, cfg.general.error_log)
+    file_logger = toolbox.SelectiveFileHandler(logfile, mode="w", DEBUG=cfg.runtime.DEBUG, ERROR=True)
+    root_logger.addHandler(file_logger)
+
+    # Write header for summary file.
     try:
         toolbox.save_csv(summary_path, [[ "Student", "LMS ID", "Score" ]])
     except Exception as e:
         logging.info("Warning: couldn't open summary file for writing: [%s]" % summary_path)
 
-    # Build the environment components (only need to do this once.)
-    if cfg.build.framework_src and cfg.build.framework_bin:
-        if cfg.build.prep_cmd or cfg.build.compile_cmd:
-            logging.info("Prepping / building framework environment... ")
-            result_error = build_project(cfg.build.framework_src, cfg.build.framework_bin, cfg.build)
-            if result_error:
-                logging.info("%s: %s\n" % (type(result_error).__name__, result_error))
-                return
-
-        logging.info("initializing framework... ")
-        framework_context = cfg.project.initialize_framework(cfg)
-        logging.info("done.\n")
-    else:
-        framework_context = None
+    # Initialize the framework / get any important info
+#    with futures.ProcessPoolExecutor() as executor:
+#        try:
+#            future = executor.submit(prepare_and_init_framework, cfg.build, cfg.project)
+#            framework_context = future.result()
+            # This is a fatal error; if we can't initalize the framework, we should stop here.
+#        except Exception as e:
+#            sys.stderr.write("Error initializing framework - %s: %s. Exiting.\n" % (type(e).__name__, e))
+#            exit()
+    framework_context = prepare_and_init_framework(cfg.build, cfg.project)
+
+    # Close general log file and move on to student-specific logs.
+    root_logger.removeHandler(file_logger)
+    file_logger.close()
 
     # Prepare and run each submission.
     for submission in glob.glob(os.path.join(cfg.runtime.target_path, cfg.runtime.set)):
         submission_info = os.path.basename(submission).split("_", 1)
         student_name, lms_id = submission_info + ["NONE"] * (2 - len(submission_info))
         output_dir = os.path.join(cfg.general.result_path, os.path.basename(submission))
 
         if not os.path.isdir(output_dir):
             os.mkdir(output_dir)
 
-        logfile = filename=os.path.join(output_dir, cfg.general.error_log)
+        logfile = os.path.join(output_dir, cfg.general.error_log)
         file_logger = toolbox.SelectiveFileHandler(logfile, mode="w", DEBUG=cfg.runtime.DEBUG, ERROR=True)
         root_logger.addHandler(file_logger)
 
-        with futures.ThreadPoolExecutor() as executor:
-            future = executor.submit(prepare_and_test_submission, framework_context, submission)
+        exec_class = futures.ThreadPoolExecutor if cfg.runtime.threads else futures.ProcessPoolExecutor
+        with exec_class() as executor:
             try:
-                suite_results = future.result()
+                future = executor.submit(prepare_and_test_submission, framework_context, submission)
+                suite_results, exception_sets = future.result()
+                # If there were exceptions in the tests, we should log them.
+                for project, exception_list in exception_sets.items():
+                   if len(exception_list) > 0:
+                       log_header = "Exceptions for %s\n%s\n" % (project, "-"*(15 + len(project)))
+                       logging.error(log_header + "\n".join(exception_list))
             except Exception as e:
-                logging.error("Error preparing / running %s - %s: %s" % (submission, type(e).__name__, e))
+                stack_trace = traceback.format_exc()
+                logging.error("Error preparing / running %s - %s: %s\n%s" % (submission, type(e).__name__, e, stack_trace))
                 root_logger.removeHandler(file_logger)
                 file_logger.close()
                 continue
 
         # Generate and save individual test score information to results file.
         grand_total = 0.0
 
@@ -359,13 +414,14 @@
             pass
 
         root_logger.removeHandler(file_logger)
         file_logger.close()
         time.sleep(2)
 
     cfg.project.shutdown_framework(framework_context)
+    print("Framework shutdown")
     # Return to where we started at.
     os.chdir(starting_dir)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `herptest-0.9.9.3/setup.py` & `herptest-0.9.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='herptest',
-    version='0.9.9.3',
+    version='0.9.9.6',
     packages=['herptest',],
     url='https://github.com/cacticouncil/herptest',
     license='GPL 3',
     author='Jeremiah Blanchard',
     author_email='jjb@eng.ufl.edu',
     description='Test suite tools for instructors',
     install_requires=[],
```

