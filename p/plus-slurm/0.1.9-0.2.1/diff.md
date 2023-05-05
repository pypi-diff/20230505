# Comparing `tmp/plus_slurm-0.1.9.tar.gz` & `tmp/plus_slurm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plus_slurm-0.1.9.tar", last modified: Mon Jan  9 12:11:17 2023, max compression
+gzip compressed data, was "plus_slurm-0.2.1.tar", last modified: Fri May  5 12:41:19 2023, max compression
```

## Comparing `plus_slurm-0.1.9.tar` & `plus_slurm-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-01-09 12:11:17.762205 plus_slurm-0.1.9/
--rw-r--r--   0 th        (1011) th        (1011)    35078 2022-08-08 13:55:25.000000 plus_slurm-0.1.9/LICENSE
--rw-r--r--   0 th        (1011) th        (1011)       97 2022-08-08 13:47:18.000000 plus_slurm-0.1.9/MANIFEST.in
--rw-r--r--   0 th        (1011) th        (1011)     1035 2023-01-09 12:11:17.761205 plus_slurm-0.1.9/PKG-INFO
--rw-r--r--   0 th        (1011) th        (1011)      407 2022-08-24 09:22:58.000000 plus_slurm-0.1.9/README.md
--rw-r--r--   0 th        (1011) th        (1011)        5 2023-01-09 12:10:53.000000 plus_slurm-0.1.9/VERSION
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-01-09 12:11:17.760205 plus_slurm-0.1.9/plus_slurm/
--rw-r--r--   0 th        (1011) th        (1011)      951 2022-08-24 12:16:21.000000 plus_slurm-0.1.9/plus_slurm/__init__.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-01-09 12:11:17.761205 plus_slurm-0.1.9/plus_slurm/jinja2_templates/
--rw-r--r--   0 th        (1011) th        (1011)     2929 2022-08-25 14:01:46.000000 plus_slurm-0.1.9/plus_slurm/jinja2_templates/runner.py
--rw-r--r--   0 th        (1011) th        (1011)      395 2023-01-09 12:10:38.000000 plus_slurm-0.1.9/plus_slurm/jinja2_templates/submit.sh
--rw-r--r--   0 th        (1011) th        (1011)     8429 2022-08-24 12:16:21.000000 plus_slurm-0.1.9/plus_slurm/job.py
--rw-r--r--   0 th        (1011) th        (1011)    16297 2022-09-08 11:52:42.000000 plus_slurm-0.1.9/plus_slurm/jobcluster.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-01-09 12:11:17.761205 plus_slurm-0.1.9/plus_slurm.egg-info/
--rw-r--r--   0 th        (1011) th        (1011)     1035 2023-01-09 12:11:17.000000 plus_slurm-0.1.9/plus_slurm.egg-info/PKG-INFO
--rw-r--r--   0 th        (1011) th        (1011)      357 2023-01-09 12:11:17.000000 plus_slurm-0.1.9/plus_slurm.egg-info/SOURCES.txt
--rw-r--r--   0 th        (1011) th        (1011)        1 2023-01-09 12:11:17.000000 plus_slurm-0.1.9/plus_slurm.egg-info/dependency_links.txt
--rw-r--r--   0 th        (1011) th        (1011)       45 2023-01-09 12:11:17.000000 plus_slurm-0.1.9/plus_slurm.egg-info/requires.txt
--rw-r--r--   0 th        (1011) th        (1011)       11 2023-01-09 12:11:17.000000 plus_slurm-0.1.9/plus_slurm.egg-info/top_level.txt
--rw-r--r--   0 th        (1011) th        (1011)       38 2023-01-09 12:11:17.762205 plus_slurm-0.1.9/setup.cfg
--rw-r--r--   0 th        (1011) th        (1011)     1426 2022-08-25 14:01:46.000000 plus_slurm-0.1.9/setup.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-05 12:41:19.877760 plus_slurm-0.2.1/
+-rw-r--r--   0 th        (1011) th        (1011)    35078 2022-08-08 13:55:25.000000 plus_slurm-0.2.1/LICENSE
+-rw-r--r--   0 th        (1011) th        (1011)       97 2022-08-08 13:47:18.000000 plus_slurm-0.2.1/MANIFEST.in
+-rw-r--r--   0 th        (1011) th        (1011)     1035 2023-05-05 12:41:19.877760 plus_slurm-0.2.1/PKG-INFO
+-rw-r--r--   0 th        (1011) th        (1011)      407 2022-08-24 09:22:58.000000 plus_slurm-0.2.1/README.md
+-rw-r--r--   0 th        (1011) th        (1011)        5 2023-05-05 12:38:10.000000 plus_slurm-0.2.1/VERSION
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-05 12:41:19.872760 plus_slurm-0.2.1/plus_slurm/
+-rw-r--r--   0 th        (1011) th        (1011)      949 2023-05-05 12:37:55.000000 plus_slurm-0.2.1/plus_slurm/__init__.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-05 12:41:19.877760 plus_slurm-0.2.1/plus_slurm/jinja2_templates/
+-rw-r--r--   0 th        (1011) th        (1011)     3040 2023-04-27 11:56:08.000000 plus_slurm-0.2.1/plus_slurm/jinja2_templates/runner.py
+-rw-r--r--   0 th        (1011) th        (1011)      395 2023-01-09 12:10:38.000000 plus_slurm-0.2.1/plus_slurm/jinja2_templates/submit.sh
+-rw-r--r--   0 th        (1011) th        (1011)     8429 2022-08-24 12:16:21.000000 plus_slurm-0.2.1/plus_slurm/job.py
+-rw-r--r--   0 th        (1011) th        (1011)    16755 2023-05-05 12:37:55.000000 plus_slurm-0.2.1/plus_slurm/jobcluster.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-05 12:41:19.876760 plus_slurm-0.2.1/plus_slurm.egg-info/
+-rw-r--r--   0 th        (1011) th        (1011)     1035 2023-05-05 12:41:19.000000 plus_slurm-0.2.1/plus_slurm.egg-info/PKG-INFO
+-rw-r--r--   0 th        (1011) th        (1011)      357 2023-05-05 12:41:19.000000 plus_slurm-0.2.1/plus_slurm.egg-info/SOURCES.txt
+-rw-r--r--   0 th        (1011) th        (1011)        1 2023-05-05 12:41:19.000000 plus_slurm-0.2.1/plus_slurm.egg-info/dependency_links.txt
+-rw-r--r--   0 th        (1011) th        (1011)       45 2023-05-05 12:41:19.000000 plus_slurm-0.2.1/plus_slurm.egg-info/requires.txt
+-rw-r--r--   0 th        (1011) th        (1011)       11 2023-05-05 12:41:19.000000 plus_slurm-0.2.1/plus_slurm.egg-info/top_level.txt
+-rw-r--r--   0 th        (1011) th        (1011)       38 2023-05-05 12:41:19.877760 plus_slurm-0.2.1/setup.cfg
+-rw-r--r--   0 th        (1011) th        (1011)     1426 2022-08-25 14:01:46.000000 plus_slurm-0.2.1/setup.py
```

### Comparing `plus_slurm-0.1.9/LICENSE` & `plus_slurm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plus_slurm-0.1.9/PKG-INFO` & `plus_slurm-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plus_slurm
-Version: 0.1.9
+Version: 0.2.1
 Summary: Convenient Python Abstraction for the Slurm based cluster at the PLUS
 Home-page: https://gitlab.com/thht/plus-slurm
 Author: Thomas Hartmann
 Author-email: thomas.hartmann@th-ht.de
 License: GPL3
 Keywords: Slurm
 Classifier: Development Status :: 4 - Beta
```

### Comparing `plus_slurm-0.1.9/plus_slurm/__init__.py` & `plus_slurm-0.2.1/plus_slurm/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with obob_subjectdb. If not, see <http://www.gnu.org/licenses/>.
 
-from .jobcluster import JobCluster, SingularityJobCluster, PermuteArgument  # noqa
+from .jobcluster import JobCluster, ApptainerJobCluster, PermuteArgument  # noqa
 from .job import Job, AutomaticFilenameJob  # noqa
```

### Comparing `plus_slurm-0.1.9/plus_slurm/jinja2_templates/runner.py` & `plus_slurm-0.2.1/plus_slurm/jinja2_templates/runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,18 @@
         'ProcId': 0,
         'requested_ram': requested_ram,
     }
 
     slurm_task_id = int(os.environ['SLURM_ARRAY_TASK_ID'])
     slurm_job_id = int(os.getenv('SLURM_ARRAY_JOB_ID'))
 
+    additional_path = '{{ append_to_path }}'
+    if additional_path:
+        sys.path.append(additional_path)
+
     job_fname = Path('{{ jobs_dir }}',
                      'slurm',
                      f'job{slurm_task_id:03d}.json.gzip')
 
     job_item = JobItem(job_fname)
 
     job_object = job_item.make_object()
```

### Comparing `plus_slurm-0.1.9/plus_slurm/job.py` & `plus_slurm-0.2.1/plus_slurm/job.py`

 * *Files identical despite different names*

### Comparing `plus_slurm-0.1.9/plus_slurm/jobcluster.py` & `plus_slurm-0.2.1/plus_slurm/jobcluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,35 +78,39 @@
     exclude_nodes : :class:`str`, optional
         Comma separated list of nodes to exclude.
     max_jobs_per_jobcluster : :class:`int`, optional
         Slurm only allows a certain number of jobs per array job
         (1000 by default).
         If the number of jobs to be submitted is higher that this number, jobs
         will be split in more than one array job.
+    append_to_path : :class:`str`, optional
+        Path to append to the python module search path.
     """
 
     _slurm_submit = '/usr/bin/sbatch'
     _runner_template = 'runner.py'
     _submit_template = 'submit.sh'
 
     def __init__(self, required_ram='2G', request_cpus=1, jobs_dir='jobs',
                  request_time=10,
                  inc_jobsdir=True,
                  python_bin=None, working_directory=None,
-                 exclude_nodes=None, max_jobs_per_jobcluster=1000):
+                 exclude_nodes=None, max_jobs_per_jobcluster=1000,
+                 append_to_path=None):
         self.required_ram = required_ram
         self.request_time = request_time
         self.request_cpus = request_cpus
         self.jobs_dir = jobs_dir
         self.inc_jobsdir = inc_jobsdir
         self.python_bin = python_bin
         self.working_directory = working_directory
         self._output_folder = None
         self._exclude_nodes = exclude_nodes
         self._max_jobs_per_jobcluster = max_jobs_per_jobcluster
+        self._append_to_path = append_to_path
 
         self._jobs = list()
 
         self._jinja_env = jinja2.Environment(
             loader=jinja2.PackageLoader('plus_slurm', 'jinja2_templates'),
             trim_blocks=True,
             lstrip_blocks=True
@@ -246,15 +250,16 @@
             'required_mem': int(self.required_ram / 1024 / 1024),
             'request_cpus': self.request_cpus,
             'request_time': self.request_time,
             'uuid': str(uuid.uuid4()),
             'python_home': self.python_home,
             'n_jobs': len(self._current_jobs_submitting),
             'working_directory': self.working_directory,
-            'exclude_nodes': self._exclude_nodes
+            'exclude_nodes': self._exclude_nodes,
+            'append_to_path': self._append_to_path
         }
 
     @property
     def jobs_submitted(self):
         return tuple(self._jobs_submitted)
 
     @property
@@ -394,71 +399,79 @@
         return len(self._jobs)
 
     @property
     def runner_filename(self):
         return Path(self.output_folder, 'slurm', 'runner.py')
 
 
-class SingularityJobCluster(JobCluster):
+class ApptainerJobCluster(JobCluster):
     """
     If you use this class instead of :class:`JobCluster`, the jobs will
-    run in a Singularity Container.
+    run in a Apptainer Container.
 
     You need to supply the same parameters as when instantiating
     :class:`JobCluster`. Additionally, you need to at least set the
-    Singularity Image you want to use.
+    Apptainer Image you want to use.
 
     Parameters
     ----------
-    singularity_image ::class:`str`
-        Set this to a singularity image to have the jobs execute in it.
+    apptainer_image ::class:`str`
+        Set this to a apptainer image to have the jobs execute in it.
         Can be a link to a local file or to some online
         repository.
     mounts : :class:`tuple`, :class:`list`, optional
         What to mount in the container.
     mount_slurm_folders : :class:`bool`
         If `true`, mount `/etc/slurm` and `/var/run/munge` so you can
         issue slurm commands from within the job.
+    apptainer_args : :class:`str`, optional
+        Additional arguments to supply to apptainer
     """
 
     _slurm_folders = ('/etc/slurm', '/var/run/munge')
 
-    def __init__(self, *args, singularity_image=None,
+    def __init__(self, *args, apptainer_image=None,
                  mounts=('/mnt', ),
-                 mount_slurm_folders=True, **kwargs):
+                 mount_slurm_folders=True,
+                 apptainer_args='', **kwargs):
         super().__init__(*args, **kwargs)
-        if singularity_image is None:
-            raise RuntimeError('You must specify a Singularity Image')
+        if apptainer_image is None:
+            raise RuntimeError('You must specify a Apptainer Image')
 
-        self._singularity_image = singularity_image
+        self._apptainer_image = apptainer_image
         self._mounts = list(mounts)
+        self._apptainer_args = apptainer_args
+
         if mount_slurm_folders:
             for mnt in self._slurm_folders:
                 if mnt not in self._mounts:
                     self._mounts.append(mnt)
 
     @property
-    def singularity_command(self):
+    def apptainer_command(self):
         return '/usr/bin/singularity'
 
     @property
-    def singularity_arguments(self):
-        cmd_list = ['exec', '--writable-tmpfs']
+    def apptainer_arguments(self):
+        cmd_list = ['exec']
         for mnt in self._mounts:
             cmd_list.append(f'-B {mnt}')
 
+        if self._apptainer_args:
+            cmd_list.append(self._apptainer_args.strip())
+
         return ' '.join(cmd_list)
 
     @property
     def executable(self):
-        return self.singularity_command
+        return self.apptainer_command
 
     @property
     def arguments(self):
-        return f'{self.singularity_arguments} {self._singularity_image} {self.python_bin} {self.runner_filename}'  # noqa
+        return f'{self.apptainer_arguments} {self._apptainer_image} {self.python_bin} {self.runner_filename}'  # noqa
 
 
 class PermuteArgument(object):
     """
     This is a container for to-be-permuted arguments.
     See the example in the introductions for details.
     """
```

### Comparing `plus_slurm-0.1.9/plus_slurm.egg-info/PKG-INFO` & `plus_slurm-0.2.1/plus_slurm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plus-slurm
-Version: 0.1.9
+Version: 0.2.1
 Summary: Convenient Python Abstraction for the Slurm based cluster at the PLUS
 Home-page: https://gitlab.com/thht/plus-slurm
 Author: Thomas Hartmann
 Author-email: thomas.hartmann@th-ht.de
 License: GPL3
 Keywords: Slurm
 Classifier: Development Status :: 4 - Beta
```

### Comparing `plus_slurm-0.1.9/setup.py` & `plus_slurm-0.2.1/setup.py`

 * *Files identical despite different names*

