# Comparing `tmp/windmill_api-1.93.1.tar.gz` & `tmp/windmill_api-1.94.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windmill_api-1.93.1.tar", max compression
+gzip compressed data, was "windmill_api-1.94.0.tar", max compression
```

## Comparing `windmill_api-1.93.1.tar` & `windmill_api-1.94.0.tar`

### file list

```diff
@@ -1,1289 +1,1289 @@
--rw-r--r--   0        0        0    11348 2023-05-03 14:46:02.955253 windmill_api-1.93.1/LICENSE
--rw-r--r--   0        0        0     2952 2023-05-03 14:46:02.959253 windmill_api-1.93.1/README.md
--rw-r--r--   0        0        0      717 2023-05-03 14:46:02.959253 windmill_api-1.93.1/pyproject.toml
--rw-r--r--   0        0        0      100 2023-05-03 14:45:28.453196 windmill_api-1.93.1/windmill_api/__init__.py
--rw-r--r--   0        0        0       47 2023-05-03 14:45:28.977229 windmill_api-1.93.1/windmill_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.101237 windmill_api-1.93.1/windmill_api/api/app/__init__.py
--rw-r--r--   0        0        0     1999 2023-05-03 14:45:40.085921 windmill_api-1.93.1/windmill_api/api/app/create_app.py
--rw-r--r--   0        0        0     1769 2023-05-03 14:45:40.097922 windmill_api-1.93.1/windmill_api/api/app/delete_app.py
--rw-r--r--   0        0        0     2214 2023-05-03 14:45:40.129924 windmill_api-1.93.1/windmill_api/api/app/execute_component.py
--rw-r--r--   0        0        0     2782 2023-05-03 14:45:40.149925 windmill_api-1.93.1/windmill_api/api/app/exists_app.py
--rw-r--r--   0        0        0     3020 2023-05-03 14:45:40.185927 windmill_api-1.93.1/windmill_api/api/app/get_app_by_path.py
--rw-r--r--   0        0        0     3187 2023-05-03 14:45:40.189927 windmill_api-1.93.1/windmill_api/api/app/get_app_by_path_with_draft.py
--rw-r--r--   0        0        0     3031 2023-05-03 14:45:40.229929 windmill_api-1.93.1/windmill_api/api/app/get_app_by_version.py
--rw-r--r--   0        0        0     2649 2023-05-03 14:45:40.249930 windmill_api-1.93.1/windmill_api/api/app/get_hub_app_by_id.py
--rw-r--r--   0        0        0     3168 2023-05-03 14:45:40.281932 windmill_api-1.93.1/windmill_api/api/app/get_public_app_by_secret.py
--rw-r--r--   0        0        0     1797 2023-05-03 14:45:40.277932 windmill_api-1.93.1/windmill_api/api/app/get_public_secret_of_app.py
--rw-r--r--   0        0        0     7289 2023-05-03 14:45:40.377937 windmill_api-1.93.1/windmill_api/api/app/list_apps.py
--rw-r--r--   0        0        0     2405 2023-05-03 14:45:40.317934 windmill_api-1.93.1/windmill_api/api/app/list_hub_apps.py
--rw-r--r--   0        0        0     2140 2023-05-03 14:45:40.349935 windmill_api-1.93.1/windmill_api/api/app/update_app.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.021232 windmill_api-1.93.1/windmill_api/api/audit/__init__.py
--rw-r--r--   0        0        0     3065 2023-05-03 14:45:40.389937 windmill_api-1.93.1/windmill_api/api/audit/get_audit_log.py
--rw-r--r--   0        0        0     8723 2023-05-03 14:45:40.497943 windmill_api-1.93.1/windmill_api/api/audit/list_audit_logs.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.177242 windmill_api-1.93.1/windmill_api/api/capture/__init__.py
--rw-r--r--   0        0        0     1796 2023-05-03 14:45:40.417939 windmill_api-1.93.1/windmill_api/api/capture/create_capture.py
--rw-r--r--   0        0        0     1790 2023-05-03 14:45:40.445940 windmill_api-1.93.1/windmill_api/api/capture/get_capture.py
--rw-r--r--   0        0        0     1799 2023-05-03 14:45:40.477942 windmill_api-1.93.1/windmill_api/api/capture/update_capture.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.129239 windmill_api-1.93.1/windmill_api/api/draft/__init__.py
--rw-r--r--   0        0        0     2019 2023-05-03 14:45:40.509944 windmill_api-1.93.1/windmill_api/api/draft/create_draft.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.177242 windmill_api-1.93.1/windmill_api/api/favorite/__init__.py
--rw-r--r--   0        0        0     1964 2023-05-03 14:45:40.533945 windmill_api-1.93.1/windmill_api/api/favorite/star.py
--rw-r--r--   0        0        0     1984 2023-05-03 14:45:40.541945 windmill_api-1.93.1/windmill_api/api/favorite/unstar.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.089236 windmill_api-1.93.1/windmill_api/api/flow/__init__.py
--rw-r--r--   0        0        0     2220 2023-05-03 14:45:40.573947 windmill_api-1.93.1/windmill_api/api/flow/archive_flow_by_path.py
--rw-r--r--   0        0        0     2009 2023-05-03 14:45:40.569947 windmill_api-1.93.1/windmill_api/api/flow/create_flow.py
--rw-r--r--   0        0        0     1788 2023-05-03 14:45:40.613949 windmill_api-1.93.1/windmill_api/api/flow/delete_flow_by_path.py
--rw-r--r--   0        0        0     2755 2023-05-03 14:45:40.613949 windmill_api-1.93.1/windmill_api/api/flow/exists_flow_by_path.py
--rw-r--r--   0        0        0     3036 2023-05-03 14:45:40.681953 windmill_api-1.93.1/windmill_api/api/flow/get_flow_by_path.py
--rw-r--r--   0        0        0     3205 2023-05-03 14:45:40.653951 windmill_api-1.93.1/windmill_api/api/flow/get_flow_by_path_with_draft.py
--rw-r--r--   0        0        0     4827 2023-05-03 14:45:40.717954 windmill_api-1.93.1/windmill_api/api/flow/get_flow_input_history_by_path.py
--rw-r--r--   0        0        0     2667 2023-05-03 14:45:40.725955 windmill_api-1.93.1/windmill_api/api/flow/get_hub_flow_by_id.py
--rw-r--r--   0        0        0     1668 2023-05-03 14:45:40.745956 windmill_api-1.93.1/windmill_api/api/flow/list_flow_paths.py
--rw-r--r--   0        0        0     7969 2023-05-03 14:45:40.829960 windmill_api-1.93.1/windmill_api/api/flow/list_flows.py
--rw-r--r--   0        0        0     2423 2023-05-03 14:45:40.781958 windmill_api-1.93.1/windmill_api/api/flow/list_hub_flows.py
--rw-r--r--   0        0        0     2150 2023-05-03 14:45:40.813960 windmill_api-1.93.1/windmill_api/api/flow/update_flow.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.169241 windmill_api-1.93.1/windmill_api/api/folder/__init__.py
--rw-r--r--   0        0        0     2214 2023-05-03 14:45:40.849961 windmill_api-1.93.1/windmill_api/api/folder/add_owner_to_folder.py
--rw-r--r--   0        0        0     2029 2023-05-03 14:45:40.861962 windmill_api-1.93.1/windmill_api/api/folder/create_folder.py
--rw-r--r--   0        0        0     1778 2023-05-03 14:45:40.881963 windmill_api-1.93.1/windmill_api/api/folder/delete_folder.py
--rw-r--r--   0        0        0     2960 2023-05-03 14:45:40.901964 windmill_api-1.93.1/windmill_api/api/folder/get_folder.py
--rw-r--r--   0        0        0     3055 2023-05-03 14:45:40.925965 windmill_api-1.93.1/windmill_api/api/folder/get_folder_usage.py
--rw-r--r--   0        0        0     3405 2023-05-03 14:45:40.953967 windmill_api-1.93.1/windmill_api/api/folder/list_folder_names.py
--rw-r--r--   0        0        0     4251 2023-05-03 14:45:41.017970 windmill_api-1.93.1/windmill_api/api/folder/list_folders.py
--rw-r--r--   0        0        0     2244 2023-05-03 14:45:40.981968 windmill_api-1.93.1/windmill_api/api/folder/remove_owner_to_folder.py
--rw-r--r--   0        0        0     2170 2023-05-03 14:45:41.033971 windmill_api-1.93.1/windmill_api/api/folder/update_folder.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.173241 windmill_api-1.93.1/windmill_api/api/granular_acl/__init__.py
--rw-r--r--   0        0        0     2480 2023-05-03 14:45:41.053972 windmill_api-1.93.1/windmill_api/api/granular_acl/add_granular_acls.py
--rw-r--r--   0        0        0     3526 2023-05-03 14:45:41.077973 windmill_api-1.93.1/windmill_api/api/granular_acl/get_granular_acls.py
--rw-r--r--   0        0        0     2545 2023-05-03 14:45:41.093974 windmill_api-1.93.1/windmill_api/api/granular_acl/remove_granular_acls.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.165241 windmill_api-1.93.1/windmill_api/api/group/__init__.py
--rw-r--r--   0        0        0     2194 2023-05-03 14:45:41.109975 windmill_api-1.93.1/windmill_api/api/group/add_user_to_group.py
--rw-r--r--   0        0        0     2019 2023-05-03 14:45:41.125976 windmill_api-1.93.1/windmill_api/api/group/create_group.py
--rw-r--r--   0        0        0     1775 2023-05-03 14:45:41.141977 windmill_api-1.93.1/windmill_api/api/group/delete_group.py
--rw-r--r--   0        0        0     2942 2023-05-03 14:45:41.169978 windmill_api-1.93.1/windmill_api/api/group/get_group.py
--rw-r--r--   0        0        0     3400 2023-05-03 14:45:41.189979 windmill_api-1.93.1/windmill_api/api/group/list_group_names.py
--rw-r--r--   0        0        0     4233 2023-05-03 14:45:41.229981 windmill_api-1.93.1/windmill_api/api/group/list_groups.py
--rw-r--r--   0        0        0     2224 2023-05-03 14:45:41.217981 windmill_api-1.93.1/windmill_api/api/group/remove_user_to_group.py
--rw-r--r--   0        0        0     2160 2023-05-03 14:45:41.249982 windmill_api-1.93.1/windmill_api/api/group/update_group.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.181242 windmill_api-1.93.1/windmill_api/api/input_/__init__.py
--rw-r--r--   0        0        0     3338 2023-05-03 14:45:41.285984 windmill_api-1.93.1/windmill_api/api/input_/create_input.py
--rw-r--r--   0        0        0     1811 2023-05-03 14:45:41.281984 windmill_api-1.93.1/windmill_api/api/input_/delete_input.py
--rw-r--r--   0        0        0     6187 2023-05-03 14:45:41.377989 windmill_api-1.93.1/windmill_api/api/input_/get_input_history.py
--rw-r--r--   0        0        0     6010 2023-05-03 14:45:41.389990 windmill_api-1.93.1/windmill_api/api/input_/list_inputs.py
--rw-r--r--   0        0        0     2025 2023-05-03 14:45:41.409991 windmill_api-1.93.1/windmill_api/api/input_/update_input.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.129239 windmill_api-1.93.1/windmill_api/api/job/__init__.py
--rw-r--r--   0        0        0     2181 2023-05-03 14:45:41.425992 windmill_api-1.93.1/windmill_api/api/job/cancel_queued_job.py
--rw-r--r--   0        0        0     2687 2023-05-03 14:45:41.449993 windmill_api-1.93.1/windmill_api/api/job/cancel_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-05-03 14:45:41.485995 windmill_api-1.93.1/windmill_api/api/job/cancel_suspended_job_post.py
--rw-r--r--   0        0        0     2535 2023-05-03 14:45:41.489995 windmill_api-1.93.1/windmill_api/api/job/create_job_signature.py
--rw-r--r--   0        0        0     3217 2023-05-03 14:45:41.533997 windmill_api-1.93.1/windmill_api/api/job/delete_completed_job.py
--rw-r--r--   0        0        0     2235 2023-05-03 14:45:41.525997 windmill_api-1.93.1/windmill_api/api/job/force_cancel_queued_job.py
--rw-r--r--   0        0        0     3034 2023-05-03 14:45:41.574000 windmill_api-1.93.1/windmill_api/api/job/get_completed_job.py
--rw-r--r--   0        0        0     1784 2023-05-03 14:45:41.561999 windmill_api-1.93.1/windmill_api/api/job/get_completed_job_result.py
--rw-r--r--   0        0        0     2868 2023-05-03 14:45:41.606001 windmill_api-1.93.1/windmill_api/api/job/get_job.py
--rw-r--r--   0        0        0     4305 2023-05-03 14:45:41.638003 windmill_api-1.93.1/windmill_api/api/job/get_job_updates.py
--rw-r--r--   0        0        0     4306 2023-05-03 14:45:41.666004 windmill_api-1.93.1/windmill_api/api/job/get_resume_urls.py
--rw-r--r--   0        0        0     4601 2023-05-03 14:45:41.702006 windmill_api-1.93.1/windmill_api/api/job/get_suspended_job_flow.py
--rw-r--r--   0        0        0    13065 2023-05-03 14:45:41.850014 windmill_api-1.93.1/windmill_api/api/job/list_completed_jobs.py
--rw-r--r--   0        0        0    12292 2023-05-03 14:45:41.882016 windmill_api-1.93.1/windmill_api/api/job/list_jobs.py
--rw-r--r--   0        0        0    12830 2023-05-03 14:45:42.010022 windmill_api-1.93.1/windmill_api/api/job/list_queue.py
--rw-r--r--   0        0        0     2067 2023-05-03 14:45:41.914017 windmill_api-1.93.1/windmill_api/api/job/result_by_id.py
--rw-r--r--   0        0        0     2313 2023-05-03 14:45:41.950019 windmill_api-1.93.1/windmill_api/api/job/resume_suspended_flow_as_owner.py
--rw-r--r--   0        0        0     2994 2023-05-03 14:45:41.998022 windmill_api-1.93.1/windmill_api/api/job/resume_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-05-03 14:45:42.046024 windmill_api-1.93.1/windmill_api/api/job/resume_suspended_job_post.py
--rw-r--r--   0        0        0     4566 2023-05-03 14:45:42.074026 windmill_api-1.93.1/windmill_api/api/job/run_flow_by_path.py
--rw-r--r--   0        0        0     3037 2023-05-03 14:45:42.094027 windmill_api-1.93.1/windmill_api/api/job/run_flow_preview.py
--rw-r--r--   0        0        0     4594 2023-05-03 14:45:42.138029 windmill_api-1.93.1/windmill_api/api/job/run_script_by_hash.py
--rw-r--r--   0        0        0     4200 2023-05-03 14:45:42.154030 windmill_api-1.93.1/windmill_api/api/job/run_script_by_path.py
--rw-r--r--   0        0        0     3050 2023-05-03 14:45:42.218033 windmill_api-1.93.1/windmill_api/api/job/run_script_preview.py
--rw-r--r--   0        0        0     3215 2023-05-03 14:45:42.234034 windmill_api-1.93.1/windmill_api/api/job/run_wait_result_flow_by_path.py
--rw-r--r--   0        0        0     3521 2023-05-03 14:45:42.270036 windmill_api-1.93.1/windmill_api/api/job/run_wait_result_script_by_path.py
--rw-r--r--   0        0        0     3356 2023-05-03 14:45:42.286037 windmill_api-1.93.1/windmill_api/api/job/run_wait_result_script_by_path_get.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.057234 windmill_api-1.93.1/windmill_api/api/oauth/__init__.py
--rw-r--r--   0        0        0     3506 2023-05-03 14:45:42.318038 windmill_api-1.93.1/windmill_api/api/oauth/connect_callback.py
--rw-r--r--   0        0        0     2118 2023-05-03 14:45:42.322039 windmill_api-1.93.1/windmill_api/api/oauth/connect_slack_callback.py
--rw-r--r--   0        0        0     2056 2023-05-03 14:45:42.350040 windmill_api-1.93.1/windmill_api/api/oauth/create_account.py
--rw-r--r--   0        0        0     1764 2023-05-03 14:45:42.354040 windmill_api-1.93.1/windmill_api/api/oauth/disconnect_account.py
--rw-r--r--   0        0        0     1649 2023-05-03 14:45:42.378042 windmill_api-1.93.1/windmill_api/api/oauth/disconnect_slack.py
--rw-r--r--   0        0        0     1426 2023-05-03 14:45:42.382042 windmill_api-1.93.1/windmill_api/api/oauth/list_o_auth_connects.py
--rw-r--r--   0        0        0     2162 2023-05-03 14:45:42.414044 windmill_api-1.93.1/windmill_api/api/oauth/list_o_auth_logins.py
--rw-r--r--   0        0        0     2151 2023-05-03 14:45:42.426044 windmill_api-1.93.1/windmill_api/api/oauth/refresh_token.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.061234 windmill_api-1.93.1/windmill_api/api/resource/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-03 14:45:42.442045 windmill_api-1.93.1/windmill_api/api/resource/create_resource.py
--rw-r--r--   0        0        0     2093 2023-05-03 14:45:42.458046 windmill_api-1.93.1/windmill_api/api/resource/create_resource_type.py
--rw-r--r--   0        0        0     1784 2023-05-03 14:45:42.470046 windmill_api-1.93.1/windmill_api/api/resource/delete_resource.py
--rw-r--r--   0        0        0     1799 2023-05-03 14:45:42.486047 windmill_api-1.93.1/windmill_api/api/resource/delete_resource_type.py
--rw-r--r--   0        0        0     2763 2023-05-03 14:45:42.510048 windmill_api-1.93.1/windmill_api/api/resource/exists_resource.py
--rw-r--r--   0        0        0     2788 2023-05-03 14:45:42.530049 windmill_api-1.93.1/windmill_api/api/resource/exists_resource_type.py
--rw-r--r--   0        0        0     2996 2023-05-03 14:45:42.570052 windmill_api-1.93.1/windmill_api/api/resource/get_resource.py
--rw-r--r--   0        0        0     3074 2023-05-03 14:45:42.594053 windmill_api-1.93.1/windmill_api/api/resource/get_resource_type.py
--rw-r--r--   0        0        0     1790 2023-05-03 14:45:42.602053 windmill_api-1.93.1/windmill_api/api/resource/get_resource_value.py
--rw-r--r--   0        0        0     5732 2023-05-03 14:45:42.674057 windmill_api-1.93.1/windmill_api/api/resource/list_resource.py
--rw-r--r--   0        0        0     3149 2023-05-03 14:45:42.646056 windmill_api-1.93.1/windmill_api/api/resource/list_resource_type.py
--rw-r--r--   0        0        0     2600 2023-05-03 14:45:42.686058 windmill_api-1.93.1/windmill_api/api/resource/list_resource_type_names.py
--rw-r--r--   0        0        0     2190 2023-05-03 14:45:42.706059 windmill_api-1.93.1/windmill_api/api/resource/update_resource.py
--rw-r--r--   0        0        0     2234 2023-05-03 14:45:42.718059 windmill_api-1.93.1/windmill_api/api/resource/update_resource_type.py
--rw-r--r--   0        0        0     2244 2023-05-03 14:45:42.742061 windmill_api-1.93.1/windmill_api/api/resource/update_resource_value.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.157240 windmill_api-1.93.1/windmill_api/api/schedule/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-03 14:45:42.750061 windmill_api-1.93.1/windmill_api/api/schedule/create_schedule.py
--rw-r--r--   0        0        0     1784 2023-05-03 14:45:42.770062 windmill_api-1.93.1/windmill_api/api/schedule/delete_schedule.py
--rw-r--r--   0        0        0     2763 2023-05-03 14:45:42.798064 windmill_api-1.93.1/windmill_api/api/schedule/exists_schedule.py
--rw-r--r--   0        0        0     2996 2023-05-03 14:45:42.814064 windmill_api-1.93.1/windmill_api/api/schedule/get_schedule.py
--rw-r--r--   0        0        0     4287 2023-05-03 14:45:42.866067 windmill_api-1.93.1/windmill_api/api/schedule/list_schedules.py
--rw-r--r--   0        0        0     3217 2023-05-03 14:45:42.862067 windmill_api-1.93.1/windmill_api/api/schedule/preview_schedule.py
--rw-r--r--   0        0        0     2233 2023-05-03 14:45:42.894069 windmill_api-1.93.1/windmill_api/api/schedule/set_schedule_enabled.py
--rw-r--r--   0        0        0     2190 2023-05-03 14:45:42.902069 windmill_api-1.93.1/windmill_api/api/schedule/update_schedule.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.073235 windmill_api-1.93.1/windmill_api/api/script/__init__.py
--rw-r--r--   0        0        0     3165 2023-05-03 14:45:42.938071 windmill_api-1.93.1/windmill_api/api/script/archive_script_by_hash.py
--rw-r--r--   0        0        0     1797 2023-05-03 14:45:42.950071 windmill_api-1.93.1/windmill_api/api/script/archive_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-05-03 14:45:42.998074 windmill_api-1.93.1/windmill_api/api/script/bash_to_jsonschema.py
--rw-r--r--   0        0        0     2029 2023-05-03 14:45:42.982073 windmill_api-1.93.1/windmill_api/api/script/create_script.py
--rw-r--r--   0        0        0     3327 2023-05-03 14:45:43.026075 windmill_api-1.93.1/windmill_api/api/script/delete_script_by_hash.py
--rw-r--r--   0        0        0     2873 2023-05-03 14:45:43.038076 windmill_api-1.93.1/windmill_api/api/script/delete_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-05-03 14:45:43.066078 windmill_api-1.93.1/windmill_api/api/script/deno_to_jsonschema.py
--rw-r--r--   0        0        0     2767 2023-05-03 14:45:43.082078 windmill_api-1.93.1/windmill_api/api/script/exists_script_by_path.py
--rw-r--r--   0        0        0     2802 2023-05-03 14:45:43.114080 windmill_api-1.93.1/windmill_api/api/script/get_hub_script_by_path.py
--rw-r--r--   0        0        0     1607 2023-05-03 14:45:43.110080 windmill_api-1.93.1/windmill_api/api/script/get_hub_script_content_by_path.py
--rw-r--r--   0        0        0     3092 2023-05-03 14:45:43.154082 windmill_api-1.93.1/windmill_api/api/script/get_script_by_hash.py
--rw-r--r--   0        0        0     3074 2023-05-03 14:45:43.158082 windmill_api-1.93.1/windmill_api/api/script/get_script_by_path.py
--rw-r--r--   0        0        0     3241 2023-05-03 14:45:43.190084 windmill_api-1.93.1/windmill_api/api/script/get_script_by_path_with_draft.py
--rw-r--r--   0        0        0     3276 2023-05-03 14:45:43.202085 windmill_api-1.93.1/windmill_api/api/script/get_script_deployment_status.py
--rw-r--r--   0        0        0     2967 2023-05-03 14:45:43.234086 windmill_api-1.93.1/windmill_api/api/script/go_to_jsonschema.py
--rw-r--r--   0        0        0     2459 2023-05-03 14:45:43.238087 windmill_api-1.93.1/windmill_api/api/script/list_hub_scripts.py
--rw-r--r--   0        0        0     1676 2023-05-03 14:45:43.258088 windmill_api-1.93.1/windmill_api/api/script/list_script_paths.py
--rw-r--r--   0        0        0    11165 2023-05-03 14:45:43.406097 windmill_api-1.93.1/windmill_api/api/script/list_scripts.py
--rw-r--r--   0        0        0     3039 2023-05-03 14:45:43.318092 windmill_api-1.93.1/windmill_api/api/script/python_to_jsonschema.py
--rw-r--r--   0        0        0     1784 2023-05-03 14:45:43.346094 windmill_api-1.93.1/windmill_api/api/script/raw_script_by_hash.py
--rw-r--r--   0        0        0     1784 2023-05-03 14:45:43.374095 windmill_api-1.93.1/windmill_api/api/script/raw_script_by_path.py
--rw-r--r--   0        0        0     2119 2023-05-03 14:45:43.406097 windmill_api-1.93.1/windmill_api/api/script/raw_script_by_path_tokened.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:28.993230 windmill_api-1.93.1/windmill_api/api/settings/__init__.py
--rw-r--r--   0        0        0     1414 2023-05-03 14:45:43.434099 windmill_api-1.93.1/windmill_api/api/settings/backend_version.py
--rw-r--r--   0        0        0     1423 2023-05-03 14:45:43.438099 windmill_api-1.93.1/windmill_api/api/settings/get_open_api_yaml.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.025232 windmill_api-1.93.1/windmill_api/api/user/__init__.py
--rw-r--r--   0        0        0     1857 2023-05-03 14:45:43.462101 windmill_api-1.93.1/windmill_api/api/user/accept_invite.py
--rw-r--r--   0        0        0     1822 2023-05-03 14:45:43.470101 windmill_api-1.93.1/windmill_api/api/user/create_token.py
--rw-r--r--   0        0        0     1991 2023-05-03 14:45:43.490103 windmill_api-1.93.1/windmill_api/api/user/create_token_impersonate.py
--rw-r--r--   0        0        0     2058 2023-05-03 14:45:43.502103 windmill_api-1.93.1/windmill_api/api/user/create_user.py
--rw-r--r--   0        0        0     1863 2023-05-03 14:45:43.522105 windmill_api-1.93.1/windmill_api/api/user/create_user_globally.py
--rw-r--r--   0        0        0     1867 2023-05-03 14:45:43.534106 windmill_api-1.93.1/windmill_api/api/user/decline_invite.py
--rw-r--r--   0        0        0     1674 2023-05-03 14:45:43.550107 windmill_api-1.93.1/windmill_api/api/user/delete_token.py
--rw-r--r--   0        0        0     1872 2023-05-03 14:45:43.566108 windmill_api-1.93.1/windmill_api/api/user/delete_user.py
--rw-r--r--   0        0        0     1454 2023-05-03 14:45:43.574108 windmill_api-1.93.1/windmill_api/api/user/get_current_email.py
--rw-r--r--   0        0        0     1474 2023-05-03 14:45:43.594109 windmill_api-1.93.1/windmill_api/api/user/get_usage.py
--rw-r--r--   0        0        0     1639 2023-05-03 14:45:43.602110 windmill_api-1.93.1/windmill_api/api/user/global_user_delete.py
--rw-r--r--   0        0        0     2060 2023-05-03 14:45:43.626111 windmill_api-1.93.1/windmill_api/api/user/global_user_update.py
--rw-r--r--   0        0        0     2468 2023-05-03 14:45:43.634112 windmill_api-1.93.1/windmill_api/api/user/global_whoami.py
--rw-r--r--   0        0        0     2745 2023-05-03 14:45:43.682115 windmill_api-1.93.1/windmill_api/api/user/is_owner_of_path.py
--rw-r--r--   0        0        0     1646 2023-05-03 14:45:43.662114 windmill_api-1.93.1/windmill_api/api/user/leave_workspace.py
--rw-r--r--   0        0        0     2633 2023-05-03 14:45:43.722118 windmill_api-1.93.1/windmill_api/api/user/list_tokens.py
--rw-r--r--   0        0        0     2552 2023-05-03 14:45:43.746119 windmill_api-1.93.1/windmill_api/api/user/list_usernames.py
--rw-r--r--   0        0        0     3012 2023-05-03 14:45:43.766120 windmill_api-1.93.1/windmill_api/api/user/list_users.py
--rw-r--r--   0        0        0     4222 2023-05-03 14:45:43.810123 windmill_api-1.93.1/windmill_api/api/user/list_users_as_super_admin.py
--rw-r--r--   0        0        0     2829 2023-05-03 14:45:43.806123 windmill_api-1.93.1/windmill_api/api/user/list_workspace_invites.py
--rw-r--r--   0        0        0     1784 2023-05-03 14:45:43.834125 windmill_api-1.93.1/windmill_api/api/user/login.py
--rw-r--r--   0        0        0     2116 2023-05-03 14:45:43.842125 windmill_api-1.93.1/windmill_api/api/user/login_with_oauth.py
--rw-r--r--   0        0        0     1393 2023-05-03 14:45:43.858126 windmill_api-1.93.1/windmill_api/api/user/logout.py
--rw-r--r--   0        0        0     1820 2023-05-03 14:45:43.870127 windmill_api-1.93.1/windmill_api/api/user/set_password.py
--rw-r--r--   0        0        0     2250 2023-05-03 14:45:43.894129 windmill_api-1.93.1/windmill_api/api/user/update_user.py
--rw-r--r--   0        0        0     2652 2023-05-03 14:45:43.914130 windmill_api-1.93.1/windmill_api/api/user/whoami.py
--rw-r--r--   0        0        0     2967 2023-05-03 14:45:43.934131 windmill_api-1.93.1/windmill_api/api/user/whois.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.053234 windmill_api-1.93.1/windmill_api/api/variable/__init__.py
--rw-r--r--   0        0        0     2634 2023-05-03 14:45:43.954132 windmill_api-1.93.1/windmill_api/api/variable/create_variable.py
--rw-r--r--   0        0        0     1784 2023-05-03 14:45:43.966133 windmill_api-1.93.1/windmill_api/api/variable/delete_variable.py
--rw-r--r--   0        0        0     2795 2023-05-03 14:45:44.002135 windmill_api-1.93.1/windmill_api/api/variable/exists_variable.py
--rw-r--r--   0        0        0     3840 2023-05-03 14:45:44.018137 windmill_api-1.93.1/windmill_api/api/variable/get_variable.py
--rw-r--r--   0        0        0     3270 2023-05-03 14:45:44.046138 windmill_api-1.93.1/windmill_api/api/variable/list_contextual_variables.py
--rw-r--r--   0        0        0     3071 2023-05-03 14:45:44.082141 windmill_api-1.93.1/windmill_api/api/variable/list_variable.py
--rw-r--r--   0        0        0     2775 2023-05-03 14:45:44.114143 windmill_api-1.93.1/windmill_api/api/variable/update_variable.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.129239 windmill_api-1.93.1/windmill_api/api/worker/__init__.py
--rw-r--r--   0        0        0     2448 2023-05-03 14:45:44.118143 windmill_api-1.93.1/windmill_api/api/worker/get_custom_tags.py
--rw-r--r--   0        0        0     3896 2023-05-03 14:45:44.178147 windmill_api-1.93.1/windmill_api/api/worker/list_workers.py
--rw-r--r--   0        0        0        0 2023-05-03 14:45:29.041233 windmill_api-1.93.1/windmill_api/api/workspace/__init__.py
--rw-r--r--   0        0        0     2015 2023-05-03 14:45:44.150145 windmill_api-1.93.1/windmill_api/api/workspace/add_user.py
--rw-r--r--   0        0        0     1647 2023-05-03 14:45:44.182147 windmill_api-1.93.1/windmill_api/api/workspace/archive_workspace.py
--rw-r--r--   0        0        0     1856 2023-05-03 14:45:44.210149 windmill_api-1.93.1/windmill_api/api/workspace/create_workspace.py
--rw-r--r--   0        0        0     2049 2023-05-03 14:45:44.210149 windmill_api-1.93.1/windmill_api/api/workspace/delete_invite.py
--rw-r--r--   0        0        0     1688 2023-05-03 14:45:44.238150 windmill_api-1.93.1/windmill_api/api/workspace/delete_workspace.py
--rw-r--r--   0        0        0     2063 2023-05-03 14:45:44.242151 windmill_api-1.93.1/windmill_api/api/workspace/edit_auto_invite.py
--rw-r--r--   0        0        0     2083 2023-05-03 14:45:44.270153 windmill_api-1.93.1/windmill_api/api/workspace/edit_slack_command.py
--rw-r--r--   0        0        0     2029 2023-05-03 14:45:44.274153 windmill_api-1.93.1/windmill_api/api/workspace/edit_webhook.py
--rw-r--r--   0        0        0     1856 2023-05-03 14:45:44.298154 windmill_api-1.93.1/windmill_api/api/workspace/exists_username.py
--rw-r--r--   0        0        0     1856 2023-05-03 14:45:44.298154 windmill_api-1.93.1/windmill_api/api/workspace/exists_workspace.py
--rw-r--r--   0        0        0     2809 2023-05-03 14:45:44.342157 windmill_api-1.93.1/windmill_api/api/workspace/get_premium_info.py
--rw-r--r--   0        0        0     2753 2023-05-03 14:45:44.338157 windmill_api-1.93.1/windmill_api/api/workspace/get_settings.py
--rw-r--r--   0        0        0     2045 2023-05-03 14:45:44.370159 windmill_api-1.93.1/windmill_api/api/workspace/invite_user.py
--rw-r--r--   0        0        0     2176 2023-05-03 14:45:44.378160 windmill_api-1.93.1/windmill_api/api/workspace/is_domain_allowed.py
--rw-r--r--   0        0        0     3255 2023-05-03 14:45:44.434163 windmill_api-1.93.1/windmill_api/api/workspace/list_pending_invites.py
--rw-r--r--   0        0        0     2583 2023-05-03 14:45:44.418162 windmill_api-1.93.1/windmill_api/api/workspace/list_user_workspaces.py
--rw-r--r--   0        0        0     2775 2023-05-03 14:45:44.458165 windmill_api-1.93.1/windmill_api/api/workspace/list_workspaces.py
--rw-r--r--   0        0        0     4311 2023-05-03 14:45:44.490167 windmill_api-1.93.1/windmill_api/api/workspace/list_workspaces_as_super_admin.py
--rw-r--r--   0        0        0     1651 2023-05-03 14:45:44.506168 windmill_api-1.93.1/windmill_api/api/workspace/unarchive_workspace.py
--rw-r--r--   0        0        0     1821 2023-05-03 14:45:44.522169 windmill_api-1.93.1/windmill_api/client.py
--rw-r--r--   0        0        0        1 2023-05-03 14:46:02.951253 windmill_api-1.93.1/windmill_api/models/__init__.py
--rw-r--r--   0        0        0     1667 2023-05-03 14:45:44.550171 windmill_api-1.93.1/windmill_api/models/accept_invite_json_body.py
--rw-r--r--   0        0        0     1710 2023-05-03 14:45:44.578172 windmill_api-1.93.1/windmill_api/models/add_granular_acls_json_body.py
--rw-r--r--   0        0        0      301 2023-05-03 14:45:38.521836 windmill_api-1.93.1/windmill_api/models/add_granular_acls_kind.py
--rw-r--r--   0        0        0     1529 2023-05-03 14:45:44.606174 windmill_api-1.93.1/windmill_api/models/add_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1940 2023-05-03 14:45:44.638176 windmill_api-1.93.1/windmill_api/models/add_user_json_body.py
--rw-r--r--   0        0        0     1552 2023-05-03 14:45:44.666178 windmill_api-1.93.1/windmill_api/models/add_user_to_group_json_body.py
--rw-r--r--   0        0        0     3940 2023-05-03 14:45:44.702180 windmill_api-1.93.1/windmill_api/models/app_with_last_version.py
--rw-r--r--   0        0        0      214 2023-05-03 14:45:39.089869 windmill_api-1.93.1/windmill_api/models/app_with_last_version_execution_mode.py
--rw-r--r--   0        0        0     1248 2023-05-03 14:45:44.694180 windmill_api-1.93.1/windmill_api/models/app_with_last_version_extra_perms.py
--rw-r--r--   0        0        0     3716 2023-05-03 14:45:44.750183 windmill_api-1.93.1/windmill_api/models/app_with_last_version_policy.py
--rw-r--r--   0        0        0      220 2023-05-03 14:45:39.141872 windmill_api-1.93.1/windmill_api/models/app_with_last_version_policy_execution_mode.py
--rw-r--r--   0        0        0     1946 2023-05-03 14:45:44.730182 windmill_api-1.93.1/windmill_api/models/app_with_last_version_policy_triggerables.py
--rw-r--r--   0        0        0     1381 2023-05-03 14:45:44.754184 windmill_api-1.93.1/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4638 2023-05-03 14:45:44.814187 windmill_api-1.93.1/windmill_api/models/app_with_last_version_w_draft.py
--rw-r--r--   0        0        0      220 2023-05-03 14:45:39.161873 windmill_api-1.93.1/windmill_api/models/app_with_last_version_w_draft_execution_mode.py
--rw-r--r--   0        0        0     1284 2023-05-03 14:45:44.778185 windmill_api-1.93.1/windmill_api/models/app_with_last_version_w_draft_extra_perms.py
--rw-r--r--   0        0        0     3828 2023-05-03 14:45:44.862190 windmill_api-1.93.1/windmill_api/models/app_with_last_version_w_draft_policy.py
--rw-r--r--   0        0        0      226 2023-05-03 14:45:38.641843 windmill_api-1.93.1/windmill_api/models/app_with_last_version_w_draft_policy_execution_mode.py
--rw-r--r--   0        0        0     2020 2023-05-03 14:45:44.862190 windmill_api-1.93.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py
--rw-r--r--   0        0        0     1417 2023-05-03 14:45:44.894193 windmill_api-1.93.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     1569 2023-05-03 14:45:44.890192 windmill_api-1.93.1/windmill_api/models/archive_flow_by_path_json_body.py
--rw-r--r--   0        0        0     7662 2023-05-03 14:45:44.986198 windmill_api-1.93.1/windmill_api/models/archive_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1314 2023-05-03 14:45:44.914194 windmill_api-1.93.1/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      259 2023-05-03 14:45:39.409886 windmill_api-1.93.1/windmill_api/models/archive_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      217 2023-05-03 14:45:39.053867 windmill_api-1.93.1/windmill_api/models/archive_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1288 2023-05-03 14:45:44.946196 windmill_api-1.93.1/windmill_api/models/archive_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     3452 2023-05-03 14:45:44.998199 windmill_api-1.93.1/windmill_api/models/audit_log.py
--rw-r--r--   0        0        0      217 2023-05-03 14:45:39.129871 windmill_api-1.93.1/windmill_api/models/audit_log_action_kind.py
--rw-r--r--   0        0        0      620 2023-05-03 14:45:39.001865 windmill_api-1.93.1/windmill_api/models/audit_log_operation.py
--rw-r--r--   0        0        0     1186 2023-05-03 14:45:45.014200 windmill_api-1.93.1/windmill_api/models/audit_log_parameters.py
--rw-r--r--   0        0        0     2933 2023-05-03 14:45:45.038202 windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-05-03 14:45:45.078204 windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-05-03 14:45:39.021866 windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-05-03 14:45:45.070204 windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-05-03 14:45:45.098206 windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-05-03 14:45:45.106206 windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-05-03 14:45:45.142208 windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-05-03 14:45:39.213876 windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-05-03 14:45:45.130208 windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-05-03 14:45:45.174210 windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-05-03 14:45:39.141872 windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-05-03 14:45:45.170210 windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-05-03 14:45:38.345825 windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2377 2023-05-03 14:45:45.210213 windmill_api-1.93.1/windmill_api/models/branch_all.py
--rw-r--r--   0        0        0     2543 2023-05-03 14:45:45.238215 windmill_api-1.93.1/windmill_api/models/branch_all_branches_item.py
--rw-r--r--   0        0        0     6620 2023-05-03 14:45:45.314219 windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-05-03 14:45:45.278217 windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-05-03 14:45:45.310219 windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-03 14:45:45.346221 windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-03 14:45:45.342221 windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-03 14:45:39.109870 windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-03 14:45:45.374223 windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-03 14:45:38.657845 windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-03 14:45:45.382224 windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-03 14:45:45.402225 windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      146 2023-05-03 14:45:38.569839 windmill_api-1.93.1/windmill_api/models/branch_all_type.py
--rw-r--r--   0        0        0     2670 2023-05-03 14:45:45.426226 windmill_api-1.93.1/windmill_api/models/branch_one.py
--rw-r--r--   0        0        0     2372 2023-05-03 14:45:45.438227 windmill_api-1.93.1/windmill_api/models/branch_one_branches_item.py
--rw-r--r--   0        0        0     6620 2023-05-03 14:45:45.514232 windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-05-03 14:45:45.482230 windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-05-03 14:45:45.514232 windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-03 14:45:45.546234 windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-03 14:45:45.546234 windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-03 14:45:39.013865 windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-03 14:45:45.570236 windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-03 14:45:38.505835 windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-03 14:45:45.578236 windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-03 14:45:45.602238 windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6125 2023-05-03 14:45:45.682243 windmill_api-1.93.1/windmill_api/models/branch_one_default_item.py
--rw-r--r--   0        0        0     2906 2023-05-03 14:45:45.646241 windmill_api-1.93.1/windmill_api/models/branch_one_default_item_retry.py
--rw-r--r--   0        0        0     1863 2023-05-03 14:45:45.694244 windmill_api-1.93.1/windmill_api/models/branch_one_default_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-05-03 14:45:45.714245 windmill_api-1.93.1/windmill_api/models/branch_one_default_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-05-03 14:45:45.722246 windmill_api-1.93.1/windmill_api/models/branch_one_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-05-03 14:45:38.653844 windmill_api-1.93.1/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-05-03 14:45:45.750247 windmill_api-1.93.1/windmill_api/models/branch_one_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-05-03 14:45:39.309881 windmill_api-1.93.1/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-05-03 14:45:45.758248 windmill_api-1.93.1/windmill_api/models/branch_one_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-05-03 14:45:45.782249 windmill_api-1.93.1/windmill_api/models/branch_one_default_item_suspend.py
--rw-r--r--   0        0        0      146 2023-05-03 14:45:39.121871 windmill_api-1.93.1/windmill_api/models/branch_one_type.py
--rw-r--r--   0        0        0     1532 2023-05-03 14:45:45.782249 windmill_api-1.93.1/windmill_api/models/cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     1255 2023-05-03 14:45:45.806251 windmill_api-1.93.1/windmill_api/models/cancel_suspended_job_post_json_body.py
--rw-r--r--   0        0        0    10508 2023-05-03 14:45:45.926258 windmill_api-1.93.1/windmill_api/models/completed_job.py
--rw-r--r--   0        0        0     1176 2023-05-03 14:45:45.826252 windmill_api-1.93.1/windmill_api/models/completed_job_args.py
--rw-r--r--   0        0        0     3265 2023-05-03 14:45:45.874255 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status.py
--rw-r--r--   0        0        0     6800 2023-05-03 14:45:45.974262 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1789 2023-05-03 14:45:45.958261 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2136 2023-05-03 14:45:45.990263 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      202 2023-05-03 14:45:39.325882 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1694 2023-05-03 14:45:46.006264 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2230 2023-05-03 14:45:46.030265 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      360 2023-05-03 14:45:38.481833 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6402 2023-05-03 14:45:46.130272 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1779 2023-05-03 14:45:46.082269 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2116 2023-05-03 14:45:46.114271 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      200 2023-05-03 14:45:38.213816 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1684 2023-05-03 14:45:46.146273 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2220 2023-05-03 14:45:46.170274 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      358 2023-05-03 14:45:39.409886 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2040 2023-05-03 14:45:46.178274 windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_retry.py
--rw-r--r--   0        0        0      310 2023-05-03 14:45:38.749850 windmill_api-1.93.1/windmill_api/models/completed_job_job_kind.py
--rw-r--r--   0        0        0      199 2023-05-03 14:45:38.201815 windmill_api-1.93.1/windmill_api/models/completed_job_language.py
--rw-r--r--   0        0        0     3127 2023-05-03 14:45:46.222277 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow.py
--rw-r--r--   0        0        0     6620 2023-05-03 14:45:46.262280 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3129 2023-05-03 14:45:46.266280 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1929 2023-05-03 14:45:46.294282 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-03 14:45:46.302282 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-03 14:45:46.326284 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-03 14:45:38.853857 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-03 14:45:46.334285 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-03 14:45:38.849857 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-03 14:45:46.358286 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-03 14:45:46.370287 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6544 2023-05-03 14:45:46.462293 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3095 2023-05-03 14:45:46.418290 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1919 2023-05-03 14:45:46.450292 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2223 2023-05-03 14:45:46.510296 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2050 2023-05-03 14:45:46.494295 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      179 2023-05-03 14:45:38.621842 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1917 2023-05-03 14:45:46.522297 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      179 2023-05-03 14:45:38.665845 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1912 2023-05-03 14:45:46.542298 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1963 2023-05-03 14:45:46.554299 windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1572 2023-05-03 14:45:46.570300 windmill_api-1.93.1/windmill_api/models/connect_callback_json_body.py
--rw-r--r--   0        0        0     2533 2023-05-03 14:45:46.594301 windmill_api-1.93.1/windmill_api/models/connect_callback_response_200.py
--rw-r--r--   0        0        0     1600 2023-05-03 14:45:46.598302 windmill_api-1.93.1/windmill_api/models/connect_slack_callback_json_body.py
--rw-r--r--   0        0        0     1753 2023-05-03 14:45:46.622303 windmill_api-1.93.1/windmill_api/models/contextual_variable.py
--rw-r--r--   0        0        0     2147 2023-05-03 14:45:46.634304 windmill_api-1.93.1/windmill_api/models/create_account_json_body.py
--rw-r--r--   0        0        0     2367 2023-05-03 14:45:46.658305 windmill_api-1.93.1/windmill_api/models/create_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-05-03 14:45:46.686307 windmill_api-1.93.1/windmill_api/models/create_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-05-03 14:45:39.417886 windmill_api-1.93.1/windmill_api/models/create_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-05-03 14:45:46.686307 windmill_api-1.93.1/windmill_api/models/create_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-05-03 14:45:46.710309 windmill_api-1.93.1/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     1947 2023-05-03 14:45:46.718309 windmill_api-1.93.1/windmill_api/models/create_draft_json_body.py
--rw-r--r--   0        0        0      183 2023-05-03 14:45:38.797854 windmill_api-1.93.1/windmill_api/models/create_draft_json_body_typ.py
--rw-r--r--   0        0        0     1550 2023-05-03 14:45:46.738310 windmill_api-1.93.1/windmill_api/models/create_flow_json_body.py
--rw-r--r--   0        0        0     2126 2023-05-03 14:45:46.758312 windmill_api-1.93.1/windmill_api/models/create_folder_json_body.py
--rw-r--r--   0        0        0     1697 2023-05-03 14:45:46.770312 windmill_api-1.93.1/windmill_api/models/create_group_json_body.py
--rw-r--r--   0        0        0     1613 2023-05-03 14:45:46.782313 windmill_api-1.93.1/windmill_api/models/create_input.py
--rw-r--r--   0        0        0     1171 2023-05-03 14:45:46.790314 windmill_api-1.93.1/windmill_api/models/create_input_args.py
--rw-r--r--   0        0        0     1701 2023-05-03 14:45:46.814315 windmill_api-1.93.1/windmill_api/models/create_input_json_body.py
--rw-r--r--   0        0        0     1217 2023-05-03 14:45:46.814315 windmill_api-1.93.1/windmill_api/models/create_input_json_body_args.py
--rw-r--r--   0        0        0      214 2023-05-03 14:45:38.233817 windmill_api-1.93.1/windmill_api/models/create_input_runnable_type.py
--rw-r--r--   0        0        0     2094 2023-05-03 14:45:46.878319 windmill_api-1.93.1/windmill_api/models/create_resource.py
--rw-r--r--   0        0        0     2140 2023-05-03 14:45:46.854318 windmill_api-1.93.1/windmill_api/models/create_resource_json_body.py
--rw-r--r--   0        0        0     2335 2023-05-03 14:45:46.894319 windmill_api-1.93.1/windmill_api/models/create_resource_type_json_body.py
--rw-r--r--   0        0        0     2780 2023-05-03 14:45:46.918321 windmill_api-1.93.1/windmill_api/models/create_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-05-03 14:45:46.934321 windmill_api-1.93.1/windmill_api/models/create_schedule_json_body_args.py
--rw-r--r--   0        0        0     5120 2023-05-03 14:45:46.998324 windmill_api-1.93.1/windmill_api/models/create_script_json_body.py
--rw-r--r--   0        0        0      249 2023-05-03 14:45:39.417886 windmill_api-1.93.1/windmill_api/models/create_script_json_body_kind.py
--rw-r--r--   0        0        0      207 2023-05-03 14:45:38.201815 windmill_api-1.93.1/windmill_api/models/create_script_json_body_language.py
--rw-r--r--   0        0        0     1232 2023-05-03 14:45:46.966323 windmill_api-1.93.1/windmill_api/models/create_script_json_body_schema.py
--rw-r--r--   0        0        0     2534 2023-05-03 14:45:47.018325 windmill_api-1.93.1/windmill_api/models/create_token_impersonate_json_body.py
--rw-r--r--   0        0        0     2169 2023-05-03 14:45:47.034325 windmill_api-1.93.1/windmill_api/models/create_token_json_body.py
--rw-r--r--   0        0        0     2364 2023-05-03 14:45:47.058327 windmill_api-1.93.1/windmill_api/models/create_user_globally_json_body.py
--rw-r--r--   0        0        0     1771 2023-05-03 14:45:47.066327 windmill_api-1.93.1/windmill_api/models/create_user_json_body.py
--rw-r--r--   0        0        0     2493 2023-05-03 14:45:47.102328 windmill_api-1.93.1/windmill_api/models/create_variable.py
--rw-r--r--   0        0        0     2539 2023-05-03 14:45:47.106329 windmill_api-1.93.1/windmill_api/models/create_variable_json_body.py
--rw-r--r--   0        0        0     1678 2023-05-03 14:45:47.130330 windmill_api-1.93.1/windmill_api/models/create_workspace.py
--rw-r--r--   0        0        0     1724 2023-05-03 14:45:47.134330 windmill_api-1.93.1/windmill_api/models/create_workspace_json_body.py
--rw-r--r--   0        0        0     1490 2023-05-03 14:45:47.158331 windmill_api-1.93.1/windmill_api/models/decline_invite_json_body.py
--rw-r--r--   0        0        0    11110 2023-05-03 14:45:47.306337 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200.py
--rw-r--r--   0        0        0     1270 2023-05-03 14:45:47.178332 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3658 2023-05-03 14:45:47.226334 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7442 2023-05-03 14:45:47.342339 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1883 2023-05-03 14:45:47.330338 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2318 2023-05-03 14:45:47.366340 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      219 2023-05-03 14:45:38.885859 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1788 2023-05-03 14:45:47.374340 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2324 2023-05-03 14:45:47.402341 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      377 2023-05-03 14:45:39.117871 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7053 2023-05-03 14:45:47.470344 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1873 2023-05-03 14:45:47.430343 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2298 2023-05-03 14:45:47.462344 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      217 2023-05-03 14:45:38.393828 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1778 2023-05-03 14:45:47.486345 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2314 2023-05-03 14:45:47.506346 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      375 2023-05-03 14:45:38.413829 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2134 2023-05-03 14:45:47.522347 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      327 2023-05-03 14:45:38.209816 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      216 2023-05-03 14:45:38.817855 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3432 2023-05-03 14:45:47.558348 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7425 2023-05-03 14:45:47.610350 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3442 2023-05-03 14:45:47.602350 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2023 2023-05-03 14:45:47.634351 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2327 2023-05-03 14:45:47.642352 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2261 2023-05-03 14:45:47.666353 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      198 2023-05-03 14:45:38.425830 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-03 14:45:47.702354 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      198 2023-05-03 14:45:39.101870 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2016 2023-05-03 14:45:47.702354 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2067 2023-05-03 14:45:47.730356 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7349 2023-05-03 14:45:47.798359 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3408 2023-05-03 14:45:47.802359 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2013 2023-05-03 14:45:47.826360 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2317 2023-05-03 14:45:47.838360 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2241 2023-05-03 14:45:47.858361 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-05-03 14:45:39.081869 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2108 2023-05-03 14:45:47.874362 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-05-03 14:45:38.869858 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2006 2023-05-03 14:45:47.890362 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2057 2023-05-03 14:45:47.906363 windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1783 2023-05-03 14:45:47.918364 windmill_api-1.93.1/windmill_api/models/delete_invite_json_body.py
--rw-r--r--   0        0        0     7636 2023-05-03 14:45:48.010367 windmill_api-1.93.1/windmill_api/models/delete_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1309 2023-05-03 14:45:47.942365 windmill_api-1.93.1/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      258 2023-05-03 14:45:38.885859 windmill_api-1.93.1/windmill_api/models/delete_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      216 2023-05-03 14:45:38.301822 windmill_api-1.93.1/windmill_api/models/delete_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1283 2023-05-03 14:45:47.966366 windmill_api-1.93.1/windmill_api/models/delete_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     2933 2023-05-03 14:45:48.010367 windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-05-03 14:45:48.074370 windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-05-03 14:45:38.405829 windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-05-03 14:45:48.034369 windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-05-03 14:45:48.062370 windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-05-03 14:45:48.118372 windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-05-03 14:45:48.118372 windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-05-03 14:45:38.869858 windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-05-03 14:45:48.142373 windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-05-03 14:45:48.186375 windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-05-03 14:45:38.781852 windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-05-03 14:45:48.170374 windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-05-03 14:45:38.613842 windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     1551 2023-05-03 14:45:48.202376 windmill_api-1.93.1/windmill_api/models/edit_auto_invite_json_body.py
--rw-r--r--   0        0        0     1980 2023-05-03 14:45:48.218376 windmill_api-1.93.1/windmill_api/models/edit_resource.py
--rw-r--r--   0        0        0     1791 2023-05-03 14:45:48.234377 windmill_api-1.93.1/windmill_api/models/edit_resource_type.py
--rw-r--r--   0        0        0     1845 2023-05-03 14:45:48.250378 windmill_api-1.93.1/windmill_api/models/edit_schedule.py
--rw-r--r--   0        0        0     1176 2023-05-03 14:45:48.258378 windmill_api-1.93.1/windmill_api/models/edit_schedule_args.py
--rw-r--r--   0        0        0     1691 2023-05-03 14:45:48.274379 windmill_api-1.93.1/windmill_api/models/edit_slack_command_json_body.py
--rw-r--r--   0        0        0     2260 2023-05-03 14:45:48.298380 windmill_api-1.93.1/windmill_api/models/edit_variable.py
--rw-r--r--   0        0        0     1520 2023-05-03 14:45:48.302380 windmill_api-1.93.1/windmill_api/models/edit_webhook_json_body.py
--rw-r--r--   0        0        0     2058 2023-05-03 14:45:48.334382 windmill_api-1.93.1/windmill_api/models/edit_workspace_user.py
--rw-r--r--   0        0        0     3663 2023-05-03 14:45:48.366383 windmill_api-1.93.1/windmill_api/models/execute_component_json_body.py
--rw-r--r--   0        0        0     1346 2023-05-03 14:45:48.354382 windmill_api-1.93.1/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
--rw-r--r--   0        0        0     1942 2023-05-03 14:45:48.386384 windmill_api-1.93.1/windmill_api/models/execute_component_json_body_raw_code.py
--rw-r--r--   0        0        0     1577 2023-05-03 14:45:48.394384 windmill_api-1.93.1/windmill_api/models/exists_username_json_body.py
--rw-r--r--   0        0        0     1400 2023-05-03 14:45:48.410385 windmill_api-1.93.1/windmill_api/models/exists_workspace_json_body.py
--rw-r--r--   0        0        0     4924 2023-05-03 14:45:48.466387 windmill_api-1.93.1/windmill_api/models/flow.py
--rw-r--r--   0        0        0     1166 2023-05-03 14:45:48.430386 windmill_api-1.93.1/windmill_api/models/flow_extra_perms.py
--rw-r--r--   0        0        0     3707 2023-05-03 14:45:48.510389 windmill_api-1.93.1/windmill_api/models/flow_metadata.py
--rw-r--r--   0        0        0     1209 2023-05-03 14:45:48.490388 windmill_api-1.93.1/windmill_api/models/flow_metadata_extra_perms.py
--rw-r--r--   0        0        0     5729 2023-05-03 14:45:48.610393 windmill_api-1.93.1/windmill_api/models/flow_module.py
--rw-r--r--   0        0        0     2726 2023-05-03 14:45:48.554391 windmill_api-1.93.1/windmill_api/models/flow_module_retry.py
--rw-r--r--   0        0        0     1807 2023-05-03 14:45:48.586392 windmill_api-1.93.1/windmill_api/models/flow_module_retry_constant.py
--rw-r--r--   0        0        0     2111 2023-05-03 14:45:48.622394 windmill_api-1.93.1/windmill_api/models/flow_module_retry_exponential.py
--rw-r--r--   0        0        0     1834 2023-05-03 14:45:48.642395 windmill_api-1.93.1/windmill_api/models/flow_module_sleep_type_0.py
--rw-r--r--   0        0        0      159 2023-05-03 14:45:38.901859 windmill_api-1.93.1/windmill_api/models/flow_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1701 2023-05-03 14:45:48.650395 windmill_api-1.93.1/windmill_api/models/flow_module_sleep_type_1.py
--rw-r--r--   0        0        0      159 2023-05-03 14:45:38.549838 windmill_api-1.93.1/windmill_api/models/flow_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1800 2023-05-03 14:45:48.678396 windmill_api-1.93.1/windmill_api/models/flow_module_stop_after_if.py
--rw-r--r--   0        0        0     1851 2023-05-03 14:45:48.682397 windmill_api-1.93.1/windmill_api/models/flow_module_suspend.py
--rw-r--r--   0        0        0     3292 2023-05-03 14:45:48.726399 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_0.py
--rw-r--r--   0        0        0     3564 2023-05-03 14:45:48.722398 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-03 14:45:48.754400 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-03 14:45:38.877858 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-03 14:45:48.762400 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-03 14:45:38.889859 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      208 2023-05-03 14:45:38.653844 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_0_language.py
--rw-r--r--   0        0        0      158 2023-05-03 14:45:39.297880 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_0_type.py
--rw-r--r--   0        0        0     2477 2023-05-03 14:45:48.790401 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_1.py
--rw-r--r--   0        0        0     3564 2023-05-03 14:45:48.802402 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-03 14:45:48.822403 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-03 14:45:39.381885 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-03 14:45:48.834403 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-03 14:45:39.177874 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      152 2023-05-03 14:45:38.509835 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_1_type.py
--rw-r--r--   0        0        0     2204 2023-05-03 14:45:48.858404 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_2.py
--rw-r--r--   0        0        0     3564 2023-05-03 14:45:48.878405 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-03 14:45:48.910406 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-03 14:45:39.233877 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-03 14:45:48.910406 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-03 14:45:39.221876 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      148 2023-05-03 14:45:38.501834 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_2_type.py
--rw-r--r--   0        0        0     4138 2023-05-03 14:45:48.966409 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3.py
--rw-r--r--   0        0        0     1990 2023-05-03 14:45:48.946408 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
--rw-r--r--   0        0        0      173 2023-05-03 14:45:38.725849 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
--rw-r--r--   0        0        0     1857 2023-05-03 14:45:48.978409 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
--rw-r--r--   0        0        0      173 2023-05-03 14:45:39.297880 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
--rw-r--r--   0        0        0     6636 2023-05-03 14:45:49.054413 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item.py
--rw-r--r--   0        0        0     3148 2023-05-03 14:45:49.050413 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
--rw-r--r--   0        0        0     1935 2023-05-03 14:45:49.082414 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-05-03 14:45:49.090414 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-05-03 14:45:49.118415 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-03 14:45:39.393885 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-05-03 14:45:49.122416 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-03 14:45:38.197815 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-05-03 14:45:49.150417 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-05-03 14:45:49.154417 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
--rw-r--r--   0        0        0      162 2023-05-03 14:45:38.665845 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_type.py
--rw-r--r--   0        0        0     2934 2023-05-03 14:45:49.194419 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4.py
--rw-r--r--   0        0        0     2508 2023-05-03 14:45:49.190419 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item.py
--rw-r--r--   0        0        0     7243 2023-05-03 14:45:49.282422 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-05-03 14:45:49.234420 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-05-03 14:45:49.266422 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-05-03 14:45:49.330424 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-05-03 14:45:49.314424 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-03 14:45:38.685846 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-05-03 14:45:49.346425 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-03 14:45:38.537837 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-05-03 14:45:49.358426 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-05-03 14:45:49.378427 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6636 2023-05-03 14:45:49.442430 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item.py
--rw-r--r--   0        0        0     3148 2023-05-03 14:45:49.450430 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
--rw-r--r--   0        0        0     1935 2023-05-03 14:45:49.474432 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-05-03 14:45:49.486433 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-05-03 14:45:49.502434 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-03 14:45:38.281821 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-05-03 14:45:49.518435 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-03 14:45:38.401828 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-05-03 14:45:49.534436 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-05-03 14:45:49.546436 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
--rw-r--r--   0        0        0      158 2023-05-03 14:45:38.285821 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_type.py
--rw-r--r--   0        0        0     2577 2023-05-03 14:45:49.566438 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5.py
--rw-r--r--   0        0        0     2679 2023-05-03 14:45:49.586439 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item.py
--rw-r--r--   0        0        0     7243 2023-05-03 14:45:49.654443 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-05-03 14:45:49.630442 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-05-03 14:45:49.662444 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-05-03 14:45:49.734448 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-05-03 14:45:49.694446 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-03 14:45:38.469833 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-05-03 14:45:49.726448 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-03 14:45:38.813855 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-05-03 14:45:49.758450 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-05-03 14:45:49.766450 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      158 2023-05-03 14:45:39.037866 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_type.py
--rw-r--r--   0        0        0     1839 2023-05-03 14:45:49.794452 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_6.py
--rw-r--r--   0        0        0      156 2023-05-03 14:45:39.249878 windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_6_type.py
--rw-r--r--   0        0        0     2009 2023-05-03 14:45:49.798452 windmill_api-1.93.1/windmill_api/models/flow_preview.py
--rw-r--r--   0        0        0     1171 2023-05-03 14:45:49.818453 windmill_api-1.93.1/windmill_api/models/flow_preview_args.py
--rw-r--r--   0        0        0     3074 2023-05-03 14:45:49.842455 windmill_api-1.93.1/windmill_api/models/flow_preview_value.py
--rw-r--r--   0        0        0     6498 2023-05-03 14:45:49.934461 windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module.py
--rw-r--r--   0        0        0     3064 2023-05-03 14:45:49.886458 windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_retry.py
--rw-r--r--   0        0        0     1911 2023-05-03 14:45:49.914460 windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2215 2023-05-03 14:45:49.954462 windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2036 2023-05-03 14:45:49.962463 windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-03 14:45:38.897859 windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1903 2023-05-03 14:45:49.986464 windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-03 14:45:38.341824 windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1904 2023-05-03 14:45:49.994464 windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1955 2023-05-03 14:45:50.018466 windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6422 2023-05-03 14:45:50.078470 windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item.py
--rw-r--r--   0        0        0     3030 2023-05-03 14:45:50.058468 windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_retry.py
--rw-r--r--   0        0        0     1901 2023-05-03 14:45:50.094471 windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2205 2023-05-03 14:45:50.114472 windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2016 2023-05-03 14:45:50.162475 windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-05-03 14:45:38.449831 windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1883 2023-05-03 14:45:50.142474 windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-05-03 14:45:38.357825 windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1894 2023-05-03 14:45:50.178476 windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1945 2023-05-03 14:45:50.194477 windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1143 2023-05-03 14:45:50.198477 windmill_api-1.93.1/windmill_api/models/flow_schema.py
--rw-r--r--   0        0        0     3001 2023-05-03 14:45:50.242480 windmill_api-1.93.1/windmill_api/models/flow_status.py
--rw-r--r--   0        0        0     6370 2023-05-03 14:45:50.326485 windmill_api-1.93.1/windmill_api/models/flow_status_failure_module.py
--rw-r--r--   0        0        0     1723 2023-05-03 14:45:50.270482 windmill_api-1.93.1/windmill_api/models/flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     1999 2023-05-03 14:45:50.302484 windmill_api-1.93.1/windmill_api/models/flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      190 2023-05-03 14:45:38.413829 windmill_api-1.93.1/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1628 2023-05-03 14:45:50.334486 windmill_api-1.93.1/windmill_api/models/flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2164 2023-05-03 14:45:50.362488 windmill_api-1.93.1/windmill_api/models/flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      348 2023-05-03 14:45:39.113870 windmill_api-1.93.1/windmill_api/models/flow_status_failure_module_type.py
--rw-r--r--   0        0        0     5808 2023-05-03 14:45:50.422491 windmill_api-1.93.1/windmill_api/models/flow_status_module.py
--rw-r--r--   0        0        0     1685 2023-05-03 14:45:50.390489 windmill_api-1.93.1/windmill_api/models/flow_status_module_approvers_item.py
--rw-r--r--   0        0        0     1925 2023-05-03 14:45:50.418491 windmill_api-1.93.1/windmill_api/models/flow_status_module_branch_chosen.py
--rw-r--r--   0        0        0      183 2023-05-03 14:45:39.177874 windmill_api-1.93.1/windmill_api/models/flow_status_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1590 2023-05-03 14:45:50.450493 windmill_api-1.93.1/windmill_api/models/flow_status_module_branchall.py
--rw-r--r--   0        0        0     2126 2023-05-03 14:45:50.458494 windmill_api-1.93.1/windmill_api/models/flow_status_module_iterator.py
--rw-r--r--   0        0        0      341 2023-05-03 14:45:39.209875 windmill_api-1.93.1/windmill_api/models/flow_status_module_type.py
--rw-r--r--   0        0        0     5981 2023-05-03 14:45:50.546499 windmill_api-1.93.1/windmill_api/models/flow_status_modules_item.py
--rw-r--r--   0        0        0     1713 2023-05-03 14:45:50.486495 windmill_api-1.93.1/windmill_api/models/flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     1979 2023-05-03 14:45:50.518497 windmill_api-1.93.1/windmill_api/models/flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      188 2023-05-03 14:45:38.797854 windmill_api-1.93.1/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1618 2023-05-03 14:45:50.582502 windmill_api-1.93.1/windmill_api/models/flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2154 2023-05-03 14:45:50.582502 windmill_api-1.93.1/windmill_api/models/flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      346 2023-05-03 14:45:38.629843 windmill_api-1.93.1/windmill_api/models/flow_status_modules_item_type.py
--rw-r--r--   0        0        0     1974 2023-05-03 14:45:50.618504 windmill_api-1.93.1/windmill_api/models/flow_status_retry.py
--rw-r--r--   0        0        0     2957 2023-05-03 14:45:50.634505 windmill_api-1.93.1/windmill_api/models/flow_value.py
--rw-r--r--   0        0        0     6224 2023-05-03 14:45:50.742511 windmill_api-1.93.1/windmill_api/models/flow_value_failure_module.py
--rw-r--r--   0        0        0     2940 2023-05-03 14:45:50.678507 windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1873 2023-05-03 14:45:50.714510 windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-05-03 14:45:50.746512 windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-05-03 14:45:50.774513 windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-05-03 14:45:38.829856 windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-05-03 14:45:50.778514 windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-05-03 14:45:39.077869 windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-05-03 14:45:50.806516 windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-05-03 14:45:50.810516 windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6125 2023-05-03 14:45:50.890521 windmill_api-1.93.1/windmill_api/models/flow_value_modules_item.py
--rw-r--r--   0        0        0     2906 2023-05-03 14:45:50.854519 windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1863 2023-05-03 14:45:50.886520 windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-05-03 14:45:50.926523 windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-05-03 14:45:50.922523 windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-05-03 14:45:38.629843 windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-05-03 14:45:50.946524 windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-05-03 14:45:38.849857 windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-05-03 14:45:50.994527 windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-05-03 14:45:50.978526 windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1858 2023-05-03 14:45:51.010528 windmill_api-1.93.1/windmill_api/models/folder.py
--rw-r--r--   0        0        0     1179 2023-05-03 14:45:51.014528 windmill_api-1.93.1/windmill_api/models/folder_extra_perms.py
--rw-r--r--   0        0        0     1560 2023-05-03 14:45:51.034530 windmill_api-1.93.1/windmill_api/models/force_cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     3807 2023-05-03 14:45:51.070532 windmill_api-1.93.1/windmill_api/models/forloop_flow.py
--rw-r--r--   0        0        0     1874 2023-05-03 14:45:51.066532 windmill_api-1.93.1/windmill_api/models/forloop_flow_iterator_type_0.py
--rw-r--r--   0        0        0      163 2023-05-03 14:45:39.037866 windmill_api-1.93.1/windmill_api/models/forloop_flow_iterator_type_0_type.py
--rw-r--r--   0        0        0     1741 2023-05-03 14:45:51.134536 windmill_api-1.93.1/windmill_api/models/forloop_flow_iterator_type_1.py
--rw-r--r--   0        0        0      163 2023-05-03 14:45:38.901859 windmill_api-1.93.1/windmill_api/models/forloop_flow_iterator_type_1_type.py
--rw-r--r--   0        0        0     6224 2023-05-03 14:45:51.162538 windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item.py
--rw-r--r--   0        0        0     2940 2023-05-03 14:45:51.174538 windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1873 2023-05-03 14:45:51.194540 windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-05-03 14:45:51.210541 windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-05-03 14:45:51.230542 windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-05-03 14:45:38.241818 windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-05-03 14:45:51.242543 windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-05-03 14:45:39.325882 windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-05-03 14:45:51.262544 windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-05-03 14:45:51.270545 windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_suspend.py
--rw-r--r--   0        0        0      152 2023-05-03 14:45:38.453832 windmill_api-1.93.1/windmill_api/models/forloop_flow_type.py
--rw-r--r--   0        0        0     4052 2023-05-03 14:45:51.318548 windmill_api-1.93.1/windmill_api/models/get_app_by_path_response_200.py
--rw-r--r--   0        0        0      219 2023-05-03 14:45:39.349883 windmill_api-1.93.1/windmill_api/models/get_app_by_path_response_200_execution_mode.py
--rw-r--r--   0        0        0     1279 2023-05-03 14:45:51.294546 windmill_api-1.93.1/windmill_api/models/get_app_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     3811 2023-05-03 14:45:51.350550 windmill_api-1.93.1/windmill_api/models/get_app_by_path_response_200_policy.py
--rw-r--r--   0        0        0      225 2023-05-03 14:45:38.657845 windmill_api-1.93.1/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2009 2023-05-03 14:45:51.346549 windmill_api-1.93.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1412 2023-05-03 14:45:51.366551 windmill_api-1.93.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4819 2023-05-03 14:45:51.410553 windmill_api-1.93.1/windmill_api/models/get_app_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0      228 2023-05-03 14:45:39.165873 windmill_api-1.93.1/windmill_api/models/get_app_by_path_with_draft_response_200_execution_mode.py
--rw-r--r--   0        0        0     1330 2023-05-03 14:45:51.426554 windmill_api-1.93.1/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py
--rw-r--r--   0        0        0     3992 2023-05-03 14:45:51.462556 windmill_api-1.93.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py
--rw-r--r--   0        0        0      234 2023-05-03 14:45:38.689847 windmill_api-1.93.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2160 2023-05-03 14:45:51.458556 windmill_api-1.93.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1463 2023-05-03 14:45:51.478557 windmill_api-1.93.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4112 2023-05-03 14:45:51.546562 windmill_api-1.93.1/windmill_api/models/get_app_by_version_response_200.py
--rw-r--r--   0        0        0      222 2023-05-03 14:45:38.733849 windmill_api-1.93.1/windmill_api/models/get_app_by_version_response_200_execution_mode.py
--rw-r--r--   0        0        0     1294 2023-05-03 14:45:51.502559 windmill_api-1.93.1/windmill_api/models/get_app_by_version_response_200_extra_perms.py
--rw-r--r--   0        0        0     3862 2023-05-03 14:45:51.554562 windmill_api-1.93.1/windmill_api/models/get_app_by_version_response_200_policy.py
--rw-r--r--   0        0        0      228 2023-05-03 14:45:39.081869 windmill_api-1.93.1/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2042 2023-05-03 14:45:51.574564 windmill_api-1.93.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1427 2023-05-03 14:45:51.574564 windmill_api-1.93.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3764 2023-05-03 14:45:51.622567 windmill_api-1.93.1/windmill_api/models/get_audit_log_response_200.py
--rw-r--r--   0        0        0      231 2023-05-03 14:45:38.909860 windmill_api-1.93.1/windmill_api/models/get_audit_log_response_200_action_kind.py
--rw-r--r--   0        0        0      634 2023-05-03 14:45:39.233877 windmill_api-1.93.1/windmill_api/models/get_audit_log_response_200_operation.py
--rw-r--r--   0        0        0     1265 2023-05-03 14:45:51.602565 windmill_api-1.93.1/windmill_api/models/get_audit_log_response_200_parameters.py
--rw-r--r--   0        0        0    11008 2023-05-03 14:45:51.742574 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200.py
--rw-r--r--   0        0        0     1255 2023-05-03 14:45:51.646568 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3595 2023-05-03 14:45:51.690571 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7343 2023-05-03 14:45:51.774576 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1868 2023-05-03 14:45:51.770576 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2288 2023-05-03 14:45:51.802578 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      216 2023-05-03 14:45:38.513835 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1773 2023-05-03 14:45:51.846581 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2309 2023-05-03 14:45:51.838580 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      374 2023-05-03 14:45:38.205816 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6924 2023-05-03 14:45:51.974589 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1858 2023-05-03 14:45:51.878583 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-05-03 14:45:51.906584 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-05-03 14:45:38.777852 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-05-03 14:45:51.938586 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2299 2023-05-03 14:45:51.978589 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      372 2023-05-03 14:45:38.513835 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2119 2023-05-03 14:45:52.010591 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      324 2023-05-03 14:45:38.533837 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      213 2023-05-03 14:45:38.705848 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3375 2023-05-03 14:45:52.030592 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7311 2023-05-03 14:45:52.098596 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3391 2023-05-03 14:45:52.070595 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2008 2023-05-03 14:45:52.106597 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2312 2023-05-03 14:45:52.134599 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2231 2023-05-03 14:45:52.138599 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      195 2023-05-03 14:45:38.537837 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2098 2023-05-03 14:45:52.166601 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      195 2023-05-03 14:45:39.261878 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2001 2023-05-03 14:45:52.170601 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2052 2023-05-03 14:45:52.194602 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7235 2023-05-03 14:45:52.298609 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3357 2023-05-03 14:45:52.238605 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1998 2023-05-03 14:45:52.270607 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-05-03 14:45:52.350612 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-05-03 14:45:52.350612 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-03 14:45:38.881858 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-05-03 14:45:52.382614 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-03 14:45:38.737850 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-05-03 14:45:52.386614 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-05-03 14:45:52.418616 windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     5374 2023-05-03 14:45:52.462619 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200.py
--rw-r--r--   0        0        0     1281 2023-05-03 14:45:52.438618 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     1258 2023-05-03 14:45:52.462619 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_schema.py
--rw-r--r--   0        0        0     3302 2023-05-03 14:45:52.506622 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value.py
--rw-r--r--   0        0        0     7159 2023-05-03 14:45:52.550625 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
--rw-r--r--   0        0        0     3323 2023-05-03 14:45:52.550625 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
--rw-r--r--   0        0        0     1988 2023-05-03 14:45:52.578626 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-05-03 14:45:52.582627 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-05-03 14:45:52.610628 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-05-03 14:45:38.181814 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-05-03 14:45:52.610628 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-05-03 14:45:38.257819 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-05-03 14:45:52.638630 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-05-03 14:45:52.638630 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7066 2023-05-03 14:45:52.762638 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
--rw-r--r--   0        0        0     3289 2023-05-03 14:45:52.730636 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
--rw-r--r--   0        0        0     1978 2023-05-03 14:45:52.762638 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2282 2023-05-03 14:45:52.798640 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2171 2023-05-03 14:45:52.794640 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-05-03 14:45:38.193815 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2038 2023-05-03 14:45:52.826642 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-05-03 14:45:38.653844 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1971 2023-05-03 14:45:52.838643 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2022 2023-05-03 14:45:52.854644 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2093 2023-05-03 14:45:52.866644 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0     5695 2023-05-03 14:45:52.922648 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py
--rw-r--r--   0        0        0     1360 2023-05-03 14:45:52.886646 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py
--rw-r--r--   0        0        0     1337 2023-05-03 14:45:52.910647 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py
--rw-r--r--   0        0        0     3559 2023-05-03 14:45:52.954650 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py
--rw-r--r--   0        0        0     7829 2023-05-03 14:45:53.002653 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py
--rw-r--r--   0        0        0     3606 2023-05-03 14:45:52.990652 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py
--rw-r--r--   0        0        0     2067 2023-05-03 14:45:53.022654 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2371 2023-05-03 14:45:53.034655 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2343 2023-05-03 14:45:53.050656 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      205 2023-05-03 14:45:38.441831 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2210 2023-05-03 14:45:53.110660 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      205 2023-05-03 14:45:38.553838 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2060 2023-05-03 14:45:53.082658 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2111 2023-05-03 14:45:53.114660 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7685 2023-05-03 14:45:53.198665 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py
--rw-r--r--   0        0        0     3542 2023-05-03 14:45:53.158663 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py
--rw-r--r--   0        0        0     2057 2023-05-03 14:45:53.190665 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2361 2023-05-03 14:45:53.270670 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2323 2023-05-03 14:45:53.226667 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      203 2023-05-03 14:45:38.389827 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2190 2023-05-03 14:45:53.258669 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      203 2023-05-03 14:45:39.381885 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2050 2023-05-03 14:45:53.290671 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2101 2023-05-03 14:45:53.298672 windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2756 2023-05-03 14:45:53.334674 windmill_api-1.93.1/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
--rw-r--r--   0        0        0     1337 2023-05-03 14:45:53.318673 windmill_api-1.93.1/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
--rw-r--r--   0        0        0     2010 2023-05-03 14:45:53.350675 windmill_api-1.93.1/windmill_api/models/get_folder_response_200.py
--rw-r--r--   0        0        0     1258 2023-05-03 14:45:53.354675 windmill_api-1.93.1/windmill_api/models/get_folder_response_200_extra_perms.py
--rw-r--r--   0        0        0     2357 2023-05-03 14:45:53.386677 windmill_api-1.93.1/windmill_api/models/get_folder_usage_response_200.py
--rw-r--r--   0        0        0      301 2023-05-03 14:45:38.453832 windmill_api-1.93.1/windmill_api/models/get_granular_acls_kind.py
--rw-r--r--   0        0        0     1235 2023-05-03 14:45:53.378677 windmill_api-1.93.1/windmill_api/models/get_granular_acls_response_200.py
--rw-r--r--   0        0        0     2888 2023-05-03 14:45:53.426680 windmill_api-1.93.1/windmill_api/models/get_group_response_200.py
--rw-r--r--   0        0        0     1253 2023-05-03 14:45:53.410679 windmill_api-1.93.1/windmill_api/models/get_group_response_200_extra_perms.py
--rw-r--r--   0        0        0     1606 2023-05-03 14:45:53.434680 windmill_api-1.93.1/windmill_api/models/get_hub_app_by_id_response_200.py
--rw-r--r--   0        0        0     1634 2023-05-03 14:45:53.454681 windmill_api-1.93.1/windmill_api/models/get_hub_app_by_id_response_200_app.py
--rw-r--r--   0        0        0     1977 2023-05-03 14:45:53.466682 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200.py
--rw-r--r--   0        0        0     2950 2023-05-03 14:45:53.546687 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
--rw-r--r--   0        0        0     1289 2023-05-03 14:45:53.486683 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
--rw-r--r--   0        0        0     3410 2023-05-03 14:45:53.534686 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
--rw-r--r--   0        0        0     7365 2023-05-03 14:45:53.662695 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
--rw-r--r--   0        0        0     3418 2023-05-03 14:45:53.586690 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     2019 2023-05-03 14:45:53.618692 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2323 2023-05-03 14:45:53.654694 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2249 2023-05-03 14:45:53.686696 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-05-03 14:45:39.077869 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2116 2023-05-03 14:45:53.690696 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-05-03 14:45:38.509835 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2012 2023-05-03 14:45:53.718698 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2063 2023-05-03 14:45:53.722698 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7289 2023-05-03 14:45:53.806703 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
--rw-r--r--   0        0        0     3384 2023-05-03 14:45:53.766701 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     2009 2023-05-03 14:45:53.794703 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2313 2023-05-03 14:45:53.826705 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2229 2023-05-03 14:45:53.834705 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      194 2023-05-03 14:45:39.429887 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2096 2023-05-03 14:45:53.854706 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      194 2023-05-03 14:45:39.165873 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2002 2023-05-03 14:45:53.866707 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2053 2023-05-03 14:45:53.886709 windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2698 2023-05-03 14:45:53.966714 windmill_api-1.93.1/windmill_api/models/get_hub_script_by_path_response_200.py
--rw-r--r--   0        0        0      216 2023-05-03 14:45:39.357883 windmill_api-1.93.1/windmill_api/models/get_hub_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     2644 2023-05-03 14:45:53.930711 windmill_api-1.93.1/windmill_api/models/get_input_history_response_200_item.py
--rw-r--r--   0        0        0     1278 2023-05-03 14:45:53.950713 windmill_api-1.93.1/windmill_api/models/get_input_history_response_200_item_args.py
--rw-r--r--   0        0        0      218 2023-05-03 14:45:38.621842 windmill_api-1.93.1/windmill_api/models/get_input_history_runnable_type.py
--rw-r--r--   0        0        0     1852 2023-05-03 14:45:53.982715 windmill_api-1.93.1/windmill_api/models/get_job_response_200.py
--rw-r--r--   0        0        0      188 2023-05-03 14:45:38.829856 windmill_api-1.93.1/windmill_api/models/get_job_response_200_type.py
--rw-r--r--   0        0        0     2364 2023-05-03 14:45:54.006716 windmill_api-1.93.1/windmill_api/models/get_job_updates_response_200.py
--rw-r--r--   0        0        0     1744 2023-05-03 14:45:54.014716 windmill_api-1.93.1/windmill_api/models/get_premium_info_response_200.py
--rw-r--r--   0        0        0     4218 2023-05-03 14:45:54.062719 windmill_api-1.93.1/windmill_api/models/get_public_app_by_secret_response_200.py
--rw-r--r--   0        0        0      227 2023-05-03 14:45:38.205816 windmill_api-1.93.1/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
--rw-r--r--   0        0        0     1322 2023-05-03 14:45:54.038718 windmill_api-1.93.1/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
--rw-r--r--   0        0        0     3970 2023-05-03 14:45:54.134724 windmill_api-1.93.1/windmill_api/models/get_public_app_by_secret_response_200_policy.py
--rw-r--r--   0        0        0      233 2023-05-03 14:45:38.701847 windmill_api-1.93.1/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2131 2023-05-03 14:45:54.094721 windmill_api-1.93.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1455 2023-05-03 14:45:54.114723 windmill_api-1.93.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3533 2023-05-03 14:45:54.170726 windmill_api-1.93.1/windmill_api/models/get_resource_response_200.py
--rw-r--r--   0        0        0     1268 2023-05-03 14:45:54.154725 windmill_api-1.93.1/windmill_api/models/get_resource_response_200_extra_perms.py
--rw-r--r--   0        0        0     2335 2023-05-03 14:45:54.194728 windmill_api-1.93.1/windmill_api/models/get_resource_type_response_200.py
--rw-r--r--   0        0        0     1840 2023-05-03 14:45:54.198728 windmill_api-1.93.1/windmill_api/models/get_resume_urls_response_200.py
--rw-r--r--   0        0        0     4325 2023-05-03 14:45:54.258732 windmill_api-1.93.1/windmill_api/models/get_schedule_response_200.py
--rw-r--r--   0        0        0     1232 2023-05-03 14:45:54.222730 windmill_api-1.93.1/windmill_api/models/get_schedule_response_200_args.py
--rw-r--r--   0        0        0     1268 2023-05-03 14:45:54.246731 windmill_api-1.93.1/windmill_api/models/get_schedule_response_200_extra_perms.py
--rw-r--r--   0        0        0     7558 2023-05-03 14:45:54.402741 windmill_api-1.93.1/windmill_api/models/get_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1294 2023-05-03 14:45:54.282733 windmill_api-1.93.1/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-03 14:45:39.421887 windmill_api-1.93.1/windmill_api/models/get_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-05-03 14:45:38.809854 windmill_api-1.93.1/windmill_api/models/get_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-05-03 14:45:54.306735 windmill_api-1.93.1/windmill_api/models/get_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     7558 2023-05-03 14:45:54.410741 windmill_api-1.93.1/windmill_api/models/get_script_by_path_response_200.py
--rw-r--r--   0        0        0     1294 2023-05-03 14:45:54.426742 windmill_api-1.93.1/windmill_api/models/get_script_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-03 14:45:39.033866 windmill_api-1.93.1/windmill_api/models/get_script_by_path_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-05-03 14:45:38.825855 windmill_api-1.93.1/windmill_api/models/get_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-05-03 14:45:54.434743 windmill_api-1.93.1/windmill_api/models/get_script_by_path_response_200_schema.py
--rw-r--r--   0        0        0     6383 2023-05-03 14:45:54.514748 windmill_api-1.93.1/windmill_api/models/get_script_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0     5608 2023-05-03 14:45:54.562751 windmill_api-1.93.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py
--rw-r--r--   0        0        0      269 2023-05-03 14:45:38.573839 windmill_api-1.93.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_kind.py
--rw-r--r--   0        0        0      227 2023-05-03 14:45:39.393885 windmill_api-1.93.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_language.py
--rw-r--r--   0        0        0     1347 2023-05-03 14:45:54.542750 windmill_api-1.93.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py
--rw-r--r--   0        0        0      264 2023-05-03 14:45:38.345825 windmill_api-1.93.1/windmill_api/models/get_script_by_path_with_draft_response_200_kind.py
--rw-r--r--   0        0        0      222 2023-05-03 14:45:39.373884 windmill_api-1.93.1/windmill_api/models/get_script_by_path_with_draft_response_200_language.py
--rw-r--r--   0        0        0     1319 2023-05-03 14:45:54.570751 windmill_api-1.93.1/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py
--rw-r--r--   0        0        0     1922 2023-05-03 14:45:54.594753 windmill_api-1.93.1/windmill_api/models/get_script_deployment_status_response_200.py
--rw-r--r--   0        0        0     4157 2023-05-03 14:45:54.634755 windmill_api-1.93.1/windmill_api/models/get_settings_response_200.py
--rw-r--r--   0        0        0     2428 2023-05-03 14:45:54.630755 windmill_api-1.93.1/windmill_api/models/get_suspended_job_flow_response_200.py
--rw-r--r--   0        0        0     1764 2023-05-03 14:45:54.658757 windmill_api-1.93.1/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
--rw-r--r--   0        0        0     2040 2023-05-03 14:45:54.670758 windmill_api-1.93.1/windmill_api/models/get_suspended_job_flow_response_200_job.py
--rw-r--r--   0        0        0      204 2023-05-03 14:45:38.269820 windmill_api-1.93.1/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
--rw-r--r--   0        0        0     4554 2023-05-03 14:45:54.730761 windmill_api-1.93.1/windmill_api/models/get_variable_response_200.py
--rw-r--r--   0        0        0     1268 2023-05-03 14:45:54.690759 windmill_api-1.93.1/windmill_api/models/get_variable_response_200_extra_perms.py
--rw-r--r--   0        0        0     2647 2023-05-03 14:45:54.734762 windmill_api-1.93.1/windmill_api/models/global_user_info.py
--rw-r--r--   0        0        0      176 2023-05-03 14:45:38.709848 windmill_api-1.93.1/windmill_api/models/global_user_info_login_type.py
--rw-r--r--   0        0        0     1627 2023-05-03 14:45:54.762763 windmill_api-1.93.1/windmill_api/models/global_user_update_json_body.py
--rw-r--r--   0        0        0     2741 2023-05-03 14:45:54.778764 windmill_api-1.93.1/windmill_api/models/global_whoami_response_200.py
--rw-r--r--   0        0        0      185 2023-05-03 14:45:38.389827 windmill_api-1.93.1/windmill_api/models/global_whoami_response_200_login_type.py
--rw-r--r--   0        0        0     2903 2023-05-03 14:45:54.810766 windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5478 2023-05-03 14:45:54.906772 windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      324 2023-05-03 14:45:38.785853 windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1598 2023-05-03 14:45:54.842769 windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1663 2023-05-03 14:45:54.870770 windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2151 2023-05-03 14:45:54.902772 windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3257 2023-05-03 14:45:54.994778 windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      342 2023-05-03 14:45:38.213816 windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1631 2023-05-03 14:45:54.934774 windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3100 2023-05-03 14:45:54.974776 windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      333 2023-05-03 14:45:38.425830 windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1580 2023-05-03 14:45:55.002778 windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      178 2023-05-03 14:45:38.681846 windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2722 2023-05-03 14:45:55.042780 windmill_api-1.93.1/windmill_api/models/group.py
--rw-r--r--   0        0        0     1174 2023-05-03 14:45:55.026780 windmill_api-1.93.1/windmill_api/models/group_extra_perms.py
--rw-r--r--   0        0        0     1689 2023-05-03 14:45:55.058781 windmill_api-1.93.1/windmill_api/models/identity.py
--rw-r--r--   0        0        0      143 2023-05-03 14:45:38.545837 windmill_api-1.93.1/windmill_api/models/identity_type.py
--rw-r--r--   0        0        0     2377 2023-05-03 14:45:55.082783 windmill_api-1.93.1/windmill_api/models/input_.py
--rw-r--r--   0        0        0     1138 2023-05-03 14:45:55.082783 windmill_api-1.93.1/windmill_api/models/input_args.py
--rw-r--r--   0        0        0     1820 2023-05-03 14:45:55.114785 windmill_api-1.93.1/windmill_api/models/input_transform_type_0.py
--rw-r--r--   0        0        0      158 2023-05-03 14:45:38.709848 windmill_api-1.93.1/windmill_api/models/input_transform_type_0_type.py
--rw-r--r--   0        0        0     1687 2023-05-03 14:45:55.114785 windmill_api-1.93.1/windmill_api/models/input_transform_type_1.py
--rw-r--r--   0        0        0      158 2023-05-03 14:45:39.241877 windmill_api-1.93.1/windmill_api/models/input_transform_type_1_type.py
--rw-r--r--   0        0        0     1773 2023-05-03 14:45:55.146787 windmill_api-1.93.1/windmill_api/models/invite_user_json_body.py
--rw-r--r--   0        0        0     1679 2023-05-03 14:45:55.146787 windmill_api-1.93.1/windmill_api/models/javascript_transform.py
--rw-r--r--   0        0        0      158 2023-05-03 14:45:38.721849 windmill_api-1.93.1/windmill_api/models/javascript_transform_type.py
--rw-r--r--   0        0        0     1686 2023-05-03 14:45:55.182789 windmill_api-1.93.1/windmill_api/models/job.py
--rw-r--r--   0        0        0      174 2023-05-03 14:45:39.277879 windmill_api-1.93.1/windmill_api/models/job_type.py
--rw-r--r--   0        0        0     3583 2023-05-03 14:45:55.202790 windmill_api-1.93.1/windmill_api/models/list_apps_response_200_item.py
--rw-r--r--   0        0        0      219 2023-05-03 14:45:38.361826 windmill_api-1.93.1/windmill_api/models/list_apps_response_200_item_execution_mode.py
--rw-r--r--   0        0        0     1276 2023-05-03 14:45:55.206790 windmill_api-1.93.1/windmill_api/models/list_apps_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      218 2023-05-03 14:45:38.885859 windmill_api-1.93.1/windmill_api/models/list_audit_logs_action_kind.py
--rw-r--r--   0        0        0     3896 2023-05-03 14:45:55.258793 windmill_api-1.93.1/windmill_api/models/list_audit_logs_response_200_item.py
--rw-r--r--   0        0        0      237 2023-05-03 14:45:39.361883 windmill_api-1.93.1/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
--rw-r--r--   0        0        0      640 2023-05-03 14:45:38.853857 windmill_api-1.93.1/windmill_api/models/list_audit_logs_response_200_item_operation.py
--rw-r--r--   0        0        0     1298 2023-05-03 14:45:55.234792 windmill_api-1.93.1/windmill_api/models/list_audit_logs_response_200_item_parameters.py
--rw-r--r--   0        0        0    11220 2023-05-03 14:45:55.450805 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item.py
--rw-r--r--   0        0        0     1288 2023-05-03 14:45:55.278795 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_args.py
--rw-r--r--   0        0        0     3736 2023-05-03 14:45:55.330798 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7579 2023-05-03 14:45:55.474806 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1901 2023-05-03 14:45:55.482807 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2352 2023-05-03 14:45:55.510808 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      222 2023-05-03 14:45:38.497834 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1806 2023-05-03 14:45:55.514809 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2342 2023-05-03 14:45:55.546810 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      380 2023-05-03 14:45:38.705848 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7160 2023-05-03 14:45:55.602814 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1891 2023-05-03 14:45:55.574812 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2332 2023-05-03 14:45:55.602814 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      220 2023-05-03 14:45:38.597841 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1796 2023-05-03 14:45:55.630816 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2332 2023-05-03 14:45:55.646817 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      378 2023-05-03 14:45:38.793853 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2152 2023-05-03 14:45:55.670818 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      330 2023-05-03 14:45:39.237877 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
--rw-r--r--   0        0        0      219 2023-05-03 14:45:38.789853 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_language.py
--rw-r--r--   0        0        0     3485 2023-05-03 14:45:55.698820 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7593 2023-05-03 14:45:55.766824 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3498 2023-05-03 14:45:55.814827 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2041 2023-05-03 14:45:55.798826 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2345 2023-05-03 14:45:55.894831 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2295 2023-05-03 14:45:55.846829 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      201 2023-05-03 14:45:38.169813 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2162 2023-05-03 14:45:55.878830 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      201 2023-05-03 14:45:38.933861 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2034 2023-05-03 14:45:55.914832 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2085 2023-05-03 14:45:55.926833 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7471 2023-05-03 14:45:56.006838 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3464 2023-05-03 14:45:55.966836 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2031 2023-05-03 14:45:55.998838 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2335 2023-05-03 14:45:56.034840 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2275 2023-05-03 14:45:56.038840 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      199 2023-05-03 14:45:38.193815 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2142 2023-05-03 14:45:56.066842 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      199 2023-05-03 14:45:38.557838 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2024 2023-05-03 14:45:56.070842 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2075 2023-05-03 14:45:56.102844 windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1865 2023-05-03 14:45:56.102844 windmill_api-1.93.1/windmill_api/models/list_contextual_variables_response_200_item.py
--rw-r--r--   0        0        0     1863 2023-05-03 14:45:56.134846 windmill_api-1.93.1/windmill_api/models/list_flows_response_200_item.py
--rw-r--r--   0        0        0     2074 2023-05-03 14:45:56.138846 windmill_api-1.93.1/windmill_api/models/list_folders_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-05-03 14:45:56.154847 windmill_api-1.93.1/windmill_api/models/list_folders_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2958 2023-05-03 14:45:56.250853 windmill_api-1.93.1/windmill_api/models/list_groups_response_200_item.py
--rw-r--r--   0        0        0     1286 2023-05-03 14:45:56.178848 windmill_api-1.93.1/windmill_api/models/list_groups_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2076 2023-05-03 14:45:56.214851 windmill_api-1.93.1/windmill_api/models/list_hub_apps_response_200.py
--rw-r--r--   0        0        0     2304 2023-05-03 14:45:56.254853 windmill_api-1.93.1/windmill_api/models/list_hub_apps_response_200_apps_item.py
--rw-r--r--   0        0        0     2116 2023-05-03 14:45:56.286855 windmill_api-1.93.1/windmill_api/models/list_hub_flows_response_200.py
--rw-r--r--   0        0        0     2324 2023-05-03 14:45:56.294855 windmill_api-1.93.1/windmill_api/models/list_hub_flows_response_200_flows_item.py
--rw-r--r--   0        0        0     2106 2023-05-03 14:45:56.322857 windmill_api-1.93.1/windmill_api/models/list_hub_scripts_response_200.py
--rw-r--r--   0        0        0     2790 2023-05-03 14:45:56.338858 windmill_api-1.93.1/windmill_api/models/list_hub_scripts_response_200_asks_item.py
--rw-r--r--   0        0        0      262 2023-05-03 14:45:38.993864 windmill_api-1.93.1/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
--rw-r--r--   0        0        0     2590 2023-05-03 14:45:56.366860 windmill_api-1.93.1/windmill_api/models/list_inputs_response_200_item.py
--rw-r--r--   0        0        0     1250 2023-05-03 14:45:56.362859 windmill_api-1.93.1/windmill_api/models/list_inputs_response_200_item_args.py
--rw-r--r--   0        0        0      213 2023-05-03 14:45:38.825855 windmill_api-1.93.1/windmill_api/models/list_inputs_runnable_type.py
--rw-r--r--   0        0        0     1922 2023-05-03 14:45:56.394861 windmill_api-1.93.1/windmill_api/models/list_jobs_response_200_item.py
--rw-r--r--   0        0        0      194 2023-05-03 14:45:38.173814 windmill_api-1.93.1/windmill_api/models/list_jobs_response_200_item_type.py
--rw-r--r--   0        0        0     2076 2023-05-03 14:45:56.402862 windmill_api-1.93.1/windmill_api/models/list_pending_invites_response_200_item.py
--rw-r--r--   0        0        0    12114 2023-05-03 14:45:56.610874 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item.py
--rw-r--r--   0        0        0     1245 2023-05-03 14:45:56.422863 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_args.py
--rw-r--r--   0        0        0     3544 2023-05-03 14:45:56.474866 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7247 2023-05-03 14:45:56.566872 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1858 2023-05-03 14:45:56.594873 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-05-03 14:45:56.626875 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-05-03 14:45:39.433887 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-05-03 14:45:56.642876 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2299 2023-05-03 14:45:56.662877 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      372 2023-05-03 14:45:38.949862 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6858 2023-05-03 14:45:56.730881 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1848 2023-05-03 14:45:56.690879 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2248 2023-05-03 14:45:56.782884 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      212 2023-05-03 14:45:39.217876 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1753 2023-05-03 14:45:56.762883 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2289 2023-05-03 14:45:56.798885 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      370 2023-05-03 14:45:38.657845 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2109 2023-05-03 14:45:56.818887 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      322 2023-05-03 14:45:39.445888 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_job_kind.py
--rw-r--r--   0        0        0      211 2023-05-03 14:45:38.821855 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_language.py
--rw-r--r--   0        0        0     3334 2023-05-03 14:45:56.910892 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7235 2023-05-03 14:45:56.906892 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3357 2023-05-03 14:45:56.950894 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1998 2023-05-03 14:45:56.938894 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-05-03 14:45:56.974896 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-05-03 14:45:56.986897 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-03 14:45:39.057868 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-05-03 14:45:57.006898 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-03 14:45:38.645844 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-05-03 14:45:57.018899 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-05-03 14:45:57.034900 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7159 2023-05-03 14:45:57.106904 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3323 2023-05-03 14:45:57.078902 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1988 2023-05-03 14:45:57.110904 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-05-03 14:45:57.210910 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-05-03 14:45:57.142906 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-05-03 14:45:38.821855 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-05-03 14:45:57.174908 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-05-03 14:45:38.517836 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-05-03 14:45:57.206910 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-05-03 14:45:57.242912 windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     4884 2023-05-03 14:45:57.282914 windmill_api-1.93.1/windmill_api/models/list_resource_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-05-03 14:45:57.262913 windmill_api-1.93.1/windmill_api/models/list_resource_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2363 2023-05-03 14:45:57.302915 windmill_api-1.93.1/windmill_api/models/list_resource_type_response_200_item.py
--rw-r--r--   0        0        0     4426 2023-05-03 14:45:57.346918 windmill_api-1.93.1/windmill_api/models/list_schedules_response_200_item.py
--rw-r--r--   0        0        0     1265 2023-05-03 14:45:57.322917 windmill_api-1.93.1/windmill_api/models/list_schedules_response_200_item_args.py
--rw-r--r--   0        0        0     1301 2023-05-03 14:45:57.390921 windmill_api-1.93.1/windmill_api/models/list_schedules_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     7551 2023-05-03 14:45:57.446924 windmill_api-1.93.1/windmill_api/models/list_scripts_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-05-03 14:45:57.410922 windmill_api-1.93.1/windmill_api/models/list_scripts_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-03 14:45:39.153873 windmill_api-1.93.1/windmill_api/models/list_scripts_response_200_item_kind.py
--rw-r--r--   0        0        0      213 2023-05-03 14:45:39.149872 windmill_api-1.93.1/windmill_api/models/list_scripts_response_200_item_language.py
--rw-r--r--   0        0        0     1265 2023-05-03 14:45:57.450924 windmill_api-1.93.1/windmill_api/models/list_scripts_response_200_item_schema.py
--rw-r--r--   0        0        0     2985 2023-05-03 14:45:57.494927 windmill_api-1.93.1/windmill_api/models/list_tokens_response_200_item.py
--rw-r--r--   0        0        0     2250 2023-05-03 14:45:57.526929 windmill_api-1.93.1/windmill_api/models/list_user_workspaces_response_200.py
--rw-r--r--   0        0        0     1833 2023-05-03 14:45:57.526929 windmill_api-1.93.1/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
--rw-r--r--   0        0        0     2896 2023-05-03 14:45:57.566931 windmill_api-1.93.1/windmill_api/models/list_users_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0      198 2023-05-03 14:45:39.173874 windmill_api-1.93.1/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
--rw-r--r--   0        0        0     4307 2023-05-03 14:45:57.658937 windmill_api-1.93.1/windmill_api/models/list_users_response_200_item.py
--rw-r--r--   0        0        0     1613 2023-05-03 14:45:57.594933 windmill_api-1.93.1/windmill_api/models/list_users_response_200_item_usage.py
--rw-r--r--   0        0        0     4608 2023-05-03 14:45:57.658937 windmill_api-1.93.1/windmill_api/models/list_variable_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-05-03 14:45:57.678938 windmill_api-1.93.1/windmill_api/models/list_variable_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2693 2023-05-03 14:45:57.702939 windmill_api-1.93.1/windmill_api/models/list_workers_response_200_item.py
--rw-r--r--   0        0        0     2086 2023-05-03 14:45:57.710940 windmill_api-1.93.1/windmill_api/models/list_workspace_invites_response_200_item.py
--rw-r--r--   0        0        0     2082 2023-05-03 14:45:57.734941 windmill_api-1.93.1/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0     2013 2023-05-03 14:45:57.746942 windmill_api-1.93.1/windmill_api/models/list_workspaces_response_200_item.py
--rw-r--r--   0        0        0     3388 2023-05-03 14:45:57.790945 windmill_api-1.93.1/windmill_api/models/listable_app.py
--rw-r--r--   0        0        0      207 2023-05-03 14:45:38.929861 windmill_api-1.93.1/windmill_api/models/listable_app_execution_mode.py
--rw-r--r--   0        0        0     1207 2023-05-03 14:45:57.770943 windmill_api-1.93.1/windmill_api/models/listable_app_extra_perms.py
--rw-r--r--   0        0        0     4751 2023-05-03 14:45:57.886950 windmill_api-1.93.1/windmill_api/models/listable_resource.py
--rw-r--r--   0        0        0     1232 2023-05-03 14:45:57.810946 windmill_api-1.93.1/windmill_api/models/listable_resource_extra_perms.py
--rw-r--r--   0        0        0     4486 2023-05-03 14:45:57.874950 windmill_api-1.93.1/windmill_api/models/listable_variable.py
--rw-r--r--   0        0        0     1232 2023-05-03 14:45:57.894951 windmill_api-1.93.1/windmill_api/models/listable_variable_extra_perms.py
--rw-r--r--   0        0        0     1513 2023-05-03 14:45:57.910952 windmill_api-1.93.1/windmill_api/models/login.py
--rw-r--r--   0        0        0     1559 2023-05-03 14:45:57.922953 windmill_api-1.93.1/windmill_api/models/login_json_body.py
--rw-r--r--   0        0        0     1739 2023-05-03 14:45:57.942954 windmill_api-1.93.1/windmill_api/models/login_with_oauth_json_body.py
--rw-r--r--   0        0        0     2758 2023-05-03 14:45:57.962955 windmill_api-1.93.1/windmill_api/models/main_arg_signature.py
--rw-r--r--   0        0        0     5099 2023-05-03 14:45:58.002957 windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item.py
--rw-r--r--   0        0        0      315 2023-05-03 14:45:38.957862 windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1547 2023-05-03 14:45:57.986956 windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1612 2023-05-03 14:45:58.018958 windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2044 2023-05-03 14:45:58.034959 windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3049 2023-05-03 14:45:58.058961 windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      333 2023-05-03 14:45:38.321823 windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1580 2023-05-03 14:45:58.058961 windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     2862 2023-05-03 14:45:58.098963 windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
--rw-r--r--   0        0        0      324 2023-05-03 14:45:38.365826 windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1529 2023-05-03 14:45:58.086962 windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      169 2023-05-03 14:45:38.321823 windmill_api-1.93.1/windmill_api/models/main_arg_signature_type.py
--rw-r--r--   0        0        0     2662 2023-05-03 14:45:58.130965 windmill_api-1.93.1/windmill_api/models/new_schedule.py
--rw-r--r--   0        0        0     1171 2023-05-03 14:45:58.118964 windmill_api-1.93.1/windmill_api/models/new_schedule_args.py
--rw-r--r--   0        0        0     4866 2023-05-03 14:45:58.262973 windmill_api-1.93.1/windmill_api/models/new_script.py
--rw-r--r--   0        0        0      238 2023-05-03 14:45:38.997864 windmill_api-1.93.1/windmill_api/models/new_script_kind.py
--rw-r--r--   0        0        0      196 2023-05-03 14:45:39.181874 windmill_api-1.93.1/windmill_api/models/new_script_language.py
--rw-r--r--   0        0        0     1171 2023-05-03 14:45:58.158967 windmill_api-1.93.1/windmill_api/models/new_script_schema.py
--rw-r--r--   0        0        0     5879 2023-05-03 14:45:58.298975 windmill_api-1.93.1/windmill_api/models/new_script_with_draft.py
--rw-r--r--   0        0        0     5192 2023-05-03 14:45:58.338977 windmill_api-1.93.1/windmill_api/models/new_script_with_draft_draft.py
--rw-r--r--   0        0        0      252 2023-05-03 14:45:38.561838 windmill_api-1.93.1/windmill_api/models/new_script_with_draft_draft_kind.py
--rw-r--r--   0        0        0      210 2023-05-03 14:45:38.645844 windmill_api-1.93.1/windmill_api/models/new_script_with_draft_draft_language.py
--rw-r--r--   0        0        0     1250 2023-05-03 14:45:58.326977 windmill_api-1.93.1/windmill_api/models/new_script_with_draft_draft_schema.py
--rw-r--r--   0        0        0      247 2023-05-03 14:45:38.237818 windmill_api-1.93.1/windmill_api/models/new_script_with_draft_kind.py
--rw-r--r--   0        0        0      205 2023-05-03 14:45:38.641843 windmill_api-1.93.1/windmill_api/models/new_script_with_draft_language.py
--rw-r--r--   0        0        0     1222 2023-05-03 14:45:58.350978 windmill_api-1.93.1/windmill_api/models/new_script_with_draft_schema.py
--rw-r--r--   0        0        0     2108 2023-05-03 14:45:58.378980 windmill_api-1.93.1/windmill_api/models/new_token.py
--rw-r--r--   0        0        0     2473 2023-05-03 14:45:58.390981 windmill_api-1.93.1/windmill_api/models/new_token_impersonate.py
--rw-r--r--   0        0        0     1710 2023-05-03 14:45:58.406982 windmill_api-1.93.1/windmill_api/models/new_user.py
--rw-r--r--   0        0        0     2584 2023-05-03 14:45:58.434983 windmill_api-1.93.1/windmill_api/models/open_flow.py
--rw-r--r--   0        0        0     1166 2023-05-03 14:45:58.426983 windmill_api-1.93.1/windmill_api/models/open_flow_schema.py
--rw-r--r--   0        0        0     3026 2023-05-03 14:45:58.470985 windmill_api-1.93.1/windmill_api/models/open_flow_value.py
--rw-r--r--   0        0        0     6384 2023-05-03 14:45:58.522988 windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module.py
--rw-r--r--   0        0        0     3013 2023-05-03 14:45:58.514988 windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1896 2023-05-03 14:45:58.542990 windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2200 2023-05-03 14:45:58.554990 windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2006 2023-05-03 14:45:58.574992 windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      175 2023-05-03 14:45:38.533837 windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1873 2023-05-03 14:45:58.586992 windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      175 2023-05-03 14:45:39.257878 windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1889 2023-05-03 14:45:58.602993 windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1940 2023-05-03 14:45:58.614994 windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6308 2023-05-03 14:45:58.767003 windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item.py
--rw-r--r--   0        0        0     2979 2023-05-03 14:45:58.654996 windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1886 2023-05-03 14:45:58.747002 windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2190 2023-05-03 14:45:58.783004 windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1986 2023-05-03 14:45:58.799005 windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      173 2023-05-03 14:45:39.021866 windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1853 2023-05-03 14:45:58.815006 windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      173 2023-05-03 14:45:38.345825 windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1879 2023-05-03 14:45:58.831007 windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1930 2023-05-03 14:45:58.847008 windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2816 2023-05-03 14:45:58.875009 windmill_api-1.93.1/windmill_api/models/open_flow_w_path.py
--rw-r--r--   0        0        0     1197 2023-05-03 14:45:58.867009 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_schema.py
--rw-r--r--   0        0        0     3116 2023-05-03 14:45:58.915012 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value.py
--rw-r--r--   0        0        0     6590 2023-05-03 14:45:58.963015 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module.py
--rw-r--r--   0        0        0     3117 2023-05-03 14:45:58.959015 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
--rw-r--r--   0        0        0     1927 2023-05-03 14:45:58.991016 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2231 2023-05-03 14:45:59.003017 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2073 2023-05-03 14:45:59.027019 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      180 2023-05-03 14:45:38.449831 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1940 2023-05-03 14:45:59.039019 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      180 2023-05-03 14:45:38.405829 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1920 2023-05-03 14:45:59.063021 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1971 2023-05-03 14:45:59.075021 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6514 2023-05-03 14:45:59.219030 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item.py
--rw-r--r--   0        0        0     3074 2023-05-03 14:45:59.207029 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
--rw-r--r--   0        0        0     1917 2023-05-03 14:45:59.239031 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2221 2023-05-03 14:45:59.255032 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2044 2023-05-03 14:45:59.275033 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-03 14:45:38.889859 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1911 2023-05-03 14:45:59.287034 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-03 14:45:39.381885 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1910 2023-05-03 14:45:59.307035 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1961 2023-05-03 14:45:59.323036 windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1989 2023-05-03 14:45:59.343037 windmill_api-1.93.1/windmill_api/models/path_flow.py
--rw-r--r--   0        0        0     3089 2023-05-03 14:45:59.367039 windmill_api-1.93.1/windmill_api/models/path_flow_input_transforms.py
--rw-r--r--   0        0        0     2115 2023-05-03 14:45:59.379040 windmill_api-1.93.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      185 2023-05-03 14:45:38.489834 windmill_api-1.93.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1982 2023-05-03 14:45:59.403041 windmill_api-1.93.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      185 2023-05-03 14:45:38.317823 windmill_api-1.93.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      135 2023-05-03 14:45:38.545837 windmill_api-1.93.1/windmill_api/models/path_flow_type.py
--rw-r--r--   0        0        0     2292 2023-05-03 14:45:59.423042 windmill_api-1.93.1/windmill_api/models/path_script.py
--rw-r--r--   0        0        0     3181 2023-05-03 14:45:59.443043 windmill_api-1.93.1/windmill_api/models/path_script_input_transforms.py
--rw-r--r--   0        0        0     2135 2023-05-03 14:45:59.455044 windmill_api-1.93.1/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      187 2023-05-03 14:45:39.289880 windmill_api-1.93.1/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2002 2023-05-03 14:45:59.475045 windmill_api-1.93.1/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      187 2023-05-03 14:45:38.837856 windmill_api-1.93.1/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      141 2023-05-03 14:45:38.869858 windmill_api-1.93.1/windmill_api/models/path_script_type.py
--rw-r--r--   0        0        0     3390 2023-05-03 14:45:59.511047 windmill_api-1.93.1/windmill_api/models/policy.py
--rw-r--r--   0        0        0      202 2023-05-03 14:45:39.397885 windmill_api-1.93.1/windmill_api/models/policy_execution_mode.py
--rw-r--r--   0        0        0     1709 2023-05-03 14:45:59.503047 windmill_api-1.93.1/windmill_api/models/policy_triggerables.py
--rw-r--r--   0        0        0     1279 2023-05-03 14:45:59.527048 windmill_api-1.93.1/windmill_api/models/policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2359 2023-05-03 14:45:59.551050 windmill_api-1.93.1/windmill_api/models/preview.py
--rw-r--r--   0        0        0     1148 2023-05-03 14:45:59.547050 windmill_api-1.93.1/windmill_api/models/preview_args.py
--rw-r--r--   0        0        0      194 2023-05-03 14:45:39.205875 windmill_api-1.93.1/windmill_api/models/preview_language.py
--rw-r--r--   0        0        0     1642 2023-05-03 14:45:59.579052 windmill_api-1.93.1/windmill_api/models/preview_schedule_json_body.py
--rw-r--r--   0        0        0     2963 2023-05-03 14:45:59.595053 windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5679 2023-05-03 14:45:59.699059 windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      328 2023-05-03 14:45:38.325823 windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1618 2023-05-03 14:45:59.623054 windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1683 2023-05-03 14:45:59.651056 windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2191 2023-05-03 14:45:59.683058 windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3329 2023-05-03 14:45:59.727060 windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      346 2023-05-03 14:45:39.113870 windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1651 2023-05-03 14:45:59.731061 windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3214 2023-05-03 14:45:59.847067 windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      337 2023-05-03 14:45:38.189815 windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1600 2023-05-03 14:45:59.759062 windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      182 2023-05-03 14:45:39.313881 windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0    11580 2023-05-03 14:45:59.935073 windmill_api-1.93.1/windmill_api/models/queued_job.py
--rw-r--r--   0        0        0     1161 2023-05-03 14:45:59.867069 windmill_api-1.93.1/windmill_api/models/queued_job_args.py
--rw-r--r--   0        0        0     3202 2023-05-03 14:45:59.915072 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status.py
--rw-r--r--   0        0        0     6683 2023-05-03 14:46:00.011077 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1774 2023-05-03 14:45:59.963075 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2106 2023-05-03 14:45:59.995077 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      199 2023-05-03 14:45:38.869858 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1679 2023-05-03 14:46:00.027078 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2215 2023-05-03 14:46:00.051080 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      357 2023-05-03 14:45:38.889859 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6294 2023-05-03 14:46:00.179087 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1764 2023-05-03 14:46:00.079081 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2086 2023-05-03 14:46:00.111083 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      197 2023-05-03 14:45:38.421830 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1669 2023-05-03 14:46:00.139085 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2205 2023-05-03 14:46:00.175087 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      355 2023-05-03 14:45:38.177814 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2025 2023-05-03 14:46:00.211089 windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_retry.py
--rw-r--r--   0        0        0      307 2023-05-03 14:45:39.185874 windmill_api-1.93.1/windmill_api/models/queued_job_job_kind.py
--rw-r--r--   0        0        0      196 2023-05-03 14:45:38.573839 windmill_api-1.93.1/windmill_api/models/queued_job_language.py
--rw-r--r--   0        0        0     3079 2023-05-03 14:46:00.227090 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow.py
--rw-r--r--   0        0        0     6506 2023-05-03 14:46:00.299095 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3069 2023-05-03 14:46:00.271093 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1914 2023-05-03 14:46:00.387100 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2218 2023-05-03 14:46:00.335097 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2040 2023-05-03 14:46:00.367099 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-03 14:45:39.009865 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1907 2023-05-03 14:46:00.395100 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-03 14:45:38.937861 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1907 2023-05-03 14:46:00.419102 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1958 2023-05-03 14:46:00.427102 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6430 2023-05-03 14:46:00.507107 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3035 2023-05-03 14:46:00.471105 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1904 2023-05-03 14:46:00.567111 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2208 2023-05-03 14:46:00.547109 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2020 2023-05-03 14:46:00.579111 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-05-03 14:45:39.173874 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1887 2023-05-03 14:46:00.599113 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-05-03 14:45:38.809854 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1897 2023-05-03 14:46:00.611113 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1948 2023-05-03 14:46:00.635115 windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     3028 2023-05-03 14:46:00.659116 windmill_api-1.93.1/windmill_api/models/raw_script.py
--rw-r--r--   0        0        0     3139 2023-05-03 14:46:00.675117 windmill_api-1.93.1/windmill_api/models/raw_script_input_transforms.py
--rw-r--r--   0        0        0     2125 2023-05-03 14:46:00.691118 windmill_api-1.93.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      186 2023-05-03 14:45:38.829856 windmill_api-1.93.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1992 2023-05-03 14:46:00.707119 windmill_api-1.93.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      186 2023-05-03 14:45:38.761851 windmill_api-1.93.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      196 2023-05-03 14:45:39.309881 windmill_api-1.93.1/windmill_api/models/raw_script_language.py
--rw-r--r--   0        0        0      146 2023-05-03 14:45:38.205816 windmill_api-1.93.1/windmill_api/models/raw_script_type.py
--rw-r--r--   0        0        0     1405 2023-05-03 14:46:00.723120 windmill_api-1.93.1/windmill_api/models/refresh_token_json_body.py
--rw-r--r--   0        0        0     1448 2023-05-03 14:46:00.731120 windmill_api-1.93.1/windmill_api/models/remove_granular_acls_json_body.py
--rw-r--r--   0        0        0      304 2023-05-03 14:45:38.617842 windmill_api-1.93.1/windmill_api/models/remove_granular_acls_kind.py
--rw-r--r--   0        0        0     1544 2023-05-03 14:46:00.751122 windmill_api-1.93.1/windmill_api/models/remove_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1567 2023-05-03 14:46:00.763122 windmill_api-1.93.1/windmill_api/models/remove_user_to_group_json_body.py
--rw-r--r--   0        0        0     3367 2023-05-03 14:46:00.807125 windmill_api-1.93.1/windmill_api/models/resource.py
--rw-r--r--   0        0        0     1189 2023-05-03 14:46:00.783124 windmill_api-1.93.1/windmill_api/models/resource_extra_perms.py
--rw-r--r--   0        0        0     2256 2023-05-03 14:46:00.823126 windmill_api-1.93.1/windmill_api/models/resource_type.py
--rw-r--r--   0        0        0     1278 2023-05-03 14:46:00.831126 windmill_api-1.93.1/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
--rw-r--r--   0        0        0     1255 2023-05-03 14:46:00.847127 windmill_api-1.93.1/windmill_api/models/resume_suspended_job_post_json_body.py
--rw-r--r--   0        0        0     2546 2023-05-03 14:46:00.871129 windmill_api-1.93.1/windmill_api/models/retry.py
--rw-r--r--   0        0        0     1751 2023-05-03 14:46:00.875129 windmill_api-1.93.1/windmill_api/models/retry_constant.py
--rw-r--r--   0        0        0     2055 2023-05-03 14:46:00.907131 windmill_api-1.93.1/windmill_api/models/retry_exponential.py
--rw-r--r--   0        0        0     1210 2023-05-03 14:46:00.899130 windmill_api-1.93.1/windmill_api/models/run_flow_by_path_json_body.py
--rw-r--r--   0        0        0     2189 2023-05-03 14:46:00.935133 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body.py
--rw-r--r--   0        0        0     1235 2023-05-03 14:46:00.927132 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_args.py
--rw-r--r--   0        0        0     3265 2023-05-03 14:46:01.051139 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value.py
--rw-r--r--   0        0        0     7049 2023-05-03 14:46:01.087142 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3284 2023-05-03 14:46:01.095142 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1975 2023-05-03 14:46:01.119144 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-05-03 14:46:01.135145 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-05-03 14:46:01.151146 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-05-03 14:45:38.373826 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-05-03 14:46:01.167147 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-05-03 14:45:38.309822 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-05-03 14:46:01.183147 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-05-03 14:46:01.199148 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6939 2023-05-03 14:46:01.275153 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3250 2023-05-03 14:46:01.243151 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1965 2023-05-03 14:46:01.275153 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2269 2023-05-03 14:46:01.311155 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2147 2023-05-03 14:46:01.307155 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      187 2023-05-03 14:45:39.245877 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2014 2023-05-03 14:46:01.339157 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      187 2023-05-03 14:45:39.045867 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1958 2023-05-03 14:46:01.343157 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2009 2023-05-03 14:46:01.371159 windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1220 2023-05-03 14:46:01.363158 windmill_api-1.93.1/windmill_api/models/run_script_by_hash_json_body.py
--rw-r--r--   0        0        0     1220 2023-05-03 14:46:01.387160 windmill_api-1.93.1/windmill_api/models/run_script_by_path_json_body.py
--rw-r--r--   0        0        0     2634 2023-05-03 14:46:01.411161 windmill_api-1.93.1/windmill_api/models/run_script_preview_json_body.py
--rw-r--r--   0        0        0     1245 2023-05-03 14:46:01.407161 windmill_api-1.93.1/windmill_api/models/run_script_preview_json_body_args.py
--rw-r--r--   0        0        0      211 2023-05-03 14:45:39.149872 windmill_api-1.93.1/windmill_api/models/run_script_preview_json_body_language.py
--rw-r--r--   0        0        0     1266 2023-05-03 14:46:01.431162 windmill_api-1.93.1/windmill_api/models/run_wait_result_flow_by_path_json_body.py
--rw-r--r--   0        0        0     1276 2023-05-03 14:46:01.435162 windmill_api-1.93.1/windmill_api/models/run_wait_result_script_by_path_json_body.py
--rw-r--r--   0        0        0      203 2023-05-03 14:45:39.097870 windmill_api-1.93.1/windmill_api/models/runnable_type.py
--rw-r--r--   0        0        0     4086 2023-05-03 14:46:01.499166 windmill_api-1.93.1/windmill_api/models/schedule.py
--rw-r--r--   0        0        0     1153 2023-05-03 14:46:01.455164 windmill_api-1.93.1/windmill_api/models/schedule_args.py
--rw-r--r--   0        0        0     1189 2023-05-03 14:46:01.479165 windmill_api-1.93.1/windmill_api/models/schedule_extra_perms.py
--rw-r--r--   0        0        0     7003 2023-05-03 14:46:01.655176 windmill_api-1.93.1/windmill_api/models/script.py
--rw-r--r--   0        0        0     1143 2023-05-03 14:46:01.519168 windmill_api-1.93.1/windmill_api/models/script_args.py
--rw-r--r--   0        0        0     1179 2023-05-03 14:46:01.543169 windmill_api-1.93.1/windmill_api/models/script_extra_perms.py
--rw-r--r--   0        0        0      235 2023-05-03 14:45:39.009865 windmill_api-1.93.1/windmill_api/models/script_kind.py
--rw-r--r--   0        0        0      193 2023-05-03 14:45:39.253878 windmill_api-1.93.1/windmill_api/models/script_language.py
--rw-r--r--   0        0        0     1153 2023-05-03 14:46:01.567170 windmill_api-1.93.1/windmill_api/models/script_schema.py
--rw-r--r--   0        0        0     1440 2023-05-03 14:46:01.595172 windmill_api-1.93.1/windmill_api/models/set_password_json_body.py
--rw-r--r--   0        0        0     1470 2023-05-03 14:46:01.619173 windmill_api-1.93.1/windmill_api/models/set_schedule_enabled_json_body.py
--rw-r--r--   0        0        0     2032 2023-05-03 14:46:01.655176 windmill_api-1.93.1/windmill_api/models/slack_token.py
--rw-r--r--   0        0        0     1586 2023-05-03 14:46:01.683177 windmill_api-1.93.1/windmill_api/models/slack_token_bot.py
--rw-r--r--   0        0        0     2227 2023-05-03 14:46:01.695178 windmill_api-1.93.1/windmill_api/models/star_json_body.py
--rw-r--r--   0        0        0      185 2023-05-03 14:45:39.165873 windmill_api-1.93.1/windmill_api/models/star_json_body_favorite_kind.py
--rw-r--r--   0        0        0     1772 2023-05-03 14:46:01.715179 windmill_api-1.93.1/windmill_api/models/static_transform.py
--rw-r--r--   0        0        0      154 2023-05-03 14:45:38.909860 windmill_api-1.93.1/windmill_api/models/static_transform_type.py
--rw-r--r--   0        0        0     2462 2023-05-03 14:46:01.735180 windmill_api-1.93.1/windmill_api/models/token_response.py
--rw-r--r--   0        0        0     2921 2023-05-03 14:46:01.847187 windmill_api-1.93.1/windmill_api/models/truncated_token.py
--rw-r--r--   0        0        0     2249 2023-05-03 14:46:01.775183 windmill_api-1.93.1/windmill_api/models/unstar_json_body.py
--rw-r--r--   0        0        0      187 2023-05-03 14:45:39.117871 windmill_api-1.93.1/windmill_api/models/unstar_json_body_favorite_kind.py
--rw-r--r--   0        0        0     2638 2023-05-03 14:46:01.823186 windmill_api-1.93.1/windmill_api/models/update_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-05-03 14:46:01.875189 windmill_api-1.93.1/windmill_api/models/update_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-05-03 14:45:38.709848 windmill_api-1.93.1/windmill_api/models/update_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-05-03 14:46:01.879189 windmill_api-1.93.1/windmill_api/models/update_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-05-03 14:46:01.895190 windmill_api-1.93.1/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-05-03 14:46:01.923192 windmill_api-1.93.1/windmill_api/models/update_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-05-03 14:46:01.915191 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-05-03 14:46:01.959194 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-05-03 14:46:02.011197 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-05-03 14:46:02.067200 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-05-03 14:46:02.043199 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-05-03 14:46:02.079201 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-05-03 14:46:02.099202 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-05-03 14:45:39.129871 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-05-03 14:46:02.111203 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-05-03 14:45:39.297880 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-05-03 14:46:02.131204 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-05-03 14:46:02.143205 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-05-03 14:46:02.219209 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-05-03 14:46:02.187207 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-05-03 14:46:02.219209 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-05-03 14:46:02.339217 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-05-03 14:46:02.251211 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-05-03 14:45:38.805854 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-05-03 14:46:02.283213 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-05-03 14:45:39.013865 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-05-03 14:46:02.311215 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-05-03 14:46:02.343217 windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1949 2023-05-03 14:46:02.371218 windmill_api-1.93.1/windmill_api/models/update_folder_json_body.py
--rw-r--r--   0        0        0     1520 2023-05-03 14:46:02.371218 windmill_api-1.93.1/windmill_api/models/update_group_json_body.py
--rw-r--r--   0        0        0     1670 2023-05-03 14:46:02.399220 windmill_api-1.93.1/windmill_api/models/update_input.py
--rw-r--r--   0        0        0     1716 2023-05-03 14:46:02.403220 windmill_api-1.93.1/windmill_api/models/update_input_json_body.py
--rw-r--r--   0        0        0     2036 2023-05-03 14:46:02.435222 windmill_api-1.93.1/windmill_api/models/update_resource_json_body.py
--rw-r--r--   0        0        0     1847 2023-05-03 14:46:02.435222 windmill_api-1.93.1/windmill_api/models/update_resource_type_json_body.py
--rw-r--r--   0        0        0     1541 2023-05-03 14:46:02.463224 windmill_api-1.93.1/windmill_api/models/update_resource_value_json_body.py
--rw-r--r--   0        0        0     1953 2023-05-03 14:46:02.535228 windmill_api-1.93.1/windmill_api/models/update_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-05-03 14:46:02.483225 windmill_api-1.93.1/windmill_api/models/update_schedule_json_body_args.py
--rw-r--r--   0        0        0     2066 2023-05-03 14:46:02.519227 windmill_api-1.93.1/windmill_api/models/update_user_json_body.py
--rw-r--r--   0        0        0     2316 2023-05-03 14:46:02.559230 windmill_api-1.93.1/windmill_api/models/update_variable_json_body.py
--rw-r--r--   0        0        0     1478 2023-05-03 14:46:02.563230 windmill_api-1.93.1/windmill_api/models/usage.py
--rw-r--r--   0        0        0     4071 2023-05-03 14:46:02.627234 windmill_api-1.93.1/windmill_api/models/user.py
--rw-r--r--   0        0        0     1501 2023-05-03 14:46:02.591231 windmill_api-1.93.1/windmill_api/models/user_usage.py
--rw-r--r--   0        0        0     2122 2023-05-03 14:46:02.623233 windmill_api-1.93.1/windmill_api/models/user_workspace_list.py
--rw-r--r--   0        0        0     1767 2023-05-03 14:46:02.655235 windmill_api-1.93.1/windmill_api/models/user_workspace_list_workspaces_item.py
--rw-r--r--   0        0        0     4222 2023-05-03 14:46:02.695238 windmill_api-1.93.1/windmill_api/models/whoami_response_200.py
--rw-r--r--   0        0        0     1572 2023-05-03 14:46:02.683237 windmill_api-1.93.1/windmill_api/models/whoami_response_200_usage.py
--rw-r--r--   0        0        0     4211 2023-05-03 14:46:02.751241 windmill_api-1.93.1/windmill_api/models/whois_response_200.py
--rw-r--r--   0        0        0     1567 2023-05-03 14:46:02.723240 windmill_api-1.93.1/windmill_api/models/whois_response_200_usage.py
--rw-r--r--   0        0        0     2604 2023-05-03 14:46:02.763242 windmill_api-1.93.1/windmill_api/models/worker_ping.py
--rw-r--r--   0        0        0     1901 2023-05-03 14:46:02.787243 windmill_api-1.93.1/windmill_api/models/workspace.py
--rw-r--r--   0        0        0     1974 2023-05-03 14:46:02.795244 windmill_api-1.93.1/windmill_api/models/workspace_invite.py
--rw-r--r--   0        0        0       25 2023-05-03 14:45:28.453196 windmill_api-1.93.1/windmill_api/py.typed
--rw-r--r--   0        0        0      939 2023-05-03 14:46:02.803244 windmill_api-1.93.1/windmill_api/types.py
--rw-r--r--   0        0        0     4333 1970-01-01 00:00:00.000000 windmill_api-1.93.1/setup.py
--rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.93.1/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-05-05 00:52:50.482931 windmill_api-1.94.0/LICENSE
+-rw-r--r--   0        0        0     2952 2023-05-05 00:52:50.486931 windmill_api-1.94.0/README.md
+-rw-r--r--   0        0        0      717 2023-05-05 00:52:50.486931 windmill_api-1.94.0/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-05-05 00:52:19.394368 windmill_api-1.94.0/windmill_api/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-05 00:52:19.890377 windmill_api-1.94.0/windmill_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:19.998379 windmill_api-1.94.0/windmill_api/api/app/__init__.py
+-rw-r--r--   0        0        0     1999 2023-05-05 00:52:30.174564 windmill_api-1.94.0/windmill_api/api/app/create_app.py
+-rw-r--r--   0        0        0     1769 2023-05-05 00:52:30.166563 windmill_api-1.94.0/windmill_api/api/app/delete_app.py
+-rw-r--r--   0        0        0     2214 2023-05-05 00:52:30.198564 windmill_api-1.94.0/windmill_api/api/app/execute_component.py
+-rw-r--r--   0        0        0     2782 2023-05-05 00:52:30.230564 windmill_api-1.94.0/windmill_api/api/app/exists_app.py
+-rw-r--r--   0        0        0     3020 2023-05-05 00:52:30.238565 windmill_api-1.94.0/windmill_api/api/app/get_app_by_path.py
+-rw-r--r--   0        0        0     3187 2023-05-05 00:52:30.270565 windmill_api-1.94.0/windmill_api/api/app/get_app_by_path_with_draft.py
+-rw-r--r--   0        0        0     3031 2023-05-05 00:52:30.274565 windmill_api-1.94.0/windmill_api/api/app/get_app_by_version.py
+-rw-r--r--   0        0        0     2649 2023-05-05 00:52:30.318566 windmill_api-1.94.0/windmill_api/api/app/get_hub_app_by_id.py
+-rw-r--r--   0        0        0     3168 2023-05-05 00:52:30.326566 windmill_api-1.94.0/windmill_api/api/app/get_public_app_by_secret.py
+-rw-r--r--   0        0        0     1797 2023-05-05 00:52:30.350567 windmill_api-1.94.0/windmill_api/api/app/get_public_secret_of_app.py
+-rw-r--r--   0        0        0     7289 2023-05-05 00:52:30.414568 windmill_api-1.94.0/windmill_api/api/app/list_apps.py
+-rw-r--r--   0        0        0     2405 2023-05-05 00:52:30.382567 windmill_api-1.94.0/windmill_api/api/app/list_hub_apps.py
+-rw-r--r--   0        0        0     2140 2023-05-05 00:52:30.410568 windmill_api-1.94.0/windmill_api/api/app/update_app.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:19.930378 windmill_api-1.94.0/windmill_api/api/audit/__init__.py
+-rw-r--r--   0        0        0     3065 2023-05-05 00:52:30.454568 windmill_api-1.94.0/windmill_api/api/audit/get_audit_log.py
+-rw-r--r--   0        0        0     8723 2023-05-05 00:52:30.514570 windmill_api-1.94.0/windmill_api/api/audit/list_audit_logs.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:20.066380 windmill_api-1.94.0/windmill_api/api/capture/__init__.py
+-rw-r--r--   0        0        0     1796 2023-05-05 00:52:30.482569 windmill_api-1.94.0/windmill_api/api/capture/create_capture.py
+-rw-r--r--   0        0        0     1790 2023-05-05 00:52:30.506569 windmill_api-1.94.0/windmill_api/api/capture/get_capture.py
+-rw-r--r--   0        0        0     1799 2023-05-05 00:52:30.538570 windmill_api-1.94.0/windmill_api/api/capture/update_capture.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:20.022379 windmill_api-1.94.0/windmill_api/api/draft/__init__.py
+-rw-r--r--   0        0        0     2019 2023-05-05 00:52:30.542570 windmill_api-1.94.0/windmill_api/api/draft/create_draft.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:20.070380 windmill_api-1.94.0/windmill_api/api/favorite/__init__.py
+-rw-r--r--   0        0        0     1964 2023-05-05 00:52:30.570571 windmill_api-1.94.0/windmill_api/api/favorite/star.py
+-rw-r--r--   0        0        0     1984 2023-05-05 00:52:30.570571 windmill_api-1.94.0/windmill_api/api/favorite/unstar.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:19.990379 windmill_api-1.94.0/windmill_api/api/flow/__init__.py
+-rw-r--r--   0        0        0     2220 2023-05-05 00:52:30.602571 windmill_api-1.94.0/windmill_api/api/flow/archive_flow_by_path.py
+-rw-r--r--   0        0        0     2009 2023-05-05 00:52:30.602571 windmill_api-1.94.0/windmill_api/api/flow/create_flow.py
+-rw-r--r--   0        0        0     1788 2023-05-05 00:52:30.650572 windmill_api-1.94.0/windmill_api/api/flow/delete_flow_by_path.py
+-rw-r--r--   0        0        0     2755 2023-05-05 00:52:30.642572 windmill_api-1.94.0/windmill_api/api/flow/exists_flow_by_path.py
+-rw-r--r--   0        0        0     3036 2023-05-05 00:52:30.698573 windmill_api-1.94.0/windmill_api/api/flow/get_flow_by_path.py
+-rw-r--r--   0        0        0     3205 2023-05-05 00:52:30.690573 windmill_api-1.94.0/windmill_api/api/flow/get_flow_by_path_with_draft.py
+-rw-r--r--   0        0        0     4827 2023-05-05 00:52:30.746574 windmill_api-1.94.0/windmill_api/api/flow/get_flow_input_history_by_path.py
+-rw-r--r--   0        0        0     2667 2023-05-05 00:52:30.734574 windmill_api-1.94.0/windmill_api/api/flow/get_hub_flow_by_id.py
+-rw-r--r--   0        0        0     1668 2023-05-05 00:52:30.762574 windmill_api-1.94.0/windmill_api/api/flow/list_flow_paths.py
+-rw-r--r--   0        0        0     7969 2023-05-05 00:52:30.838575 windmill_api-1.94.0/windmill_api/api/flow/list_flows.py
+-rw-r--r--   0        0        0     2423 2023-05-05 00:52:30.794575 windmill_api-1.94.0/windmill_api/api/flow/list_hub_flows.py
+-rw-r--r--   0        0        0     2150 2023-05-05 00:52:30.822575 windmill_api-1.94.0/windmill_api/api/flow/update_flow.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:20.058380 windmill_api-1.94.0/windmill_api/api/folder/__init__.py
+-rw-r--r--   0        0        0     2214 2023-05-05 00:52:30.854576 windmill_api-1.94.0/windmill_api/api/folder/add_owner_to_folder.py
+-rw-r--r--   0        0        0     2029 2023-05-05 00:52:30.862576 windmill_api-1.94.0/windmill_api/api/folder/create_folder.py
+-rw-r--r--   0        0        0     1778 2023-05-05 00:52:30.882576 windmill_api-1.94.0/windmill_api/api/folder/delete_folder.py
+-rw-r--r--   0        0        0     2960 2023-05-05 00:52:30.902577 windmill_api-1.94.0/windmill_api/api/folder/get_folder.py
+-rw-r--r--   0        0        0     3055 2023-05-05 00:52:30.922577 windmill_api-1.94.0/windmill_api/api/folder/get_folder_usage.py
+-rw-r--r--   0        0        0     3405 2023-05-05 00:52:30.946577 windmill_api-1.94.0/windmill_api/api/folder/list_folder_names.py
+-rw-r--r--   0        0        0     4251 2023-05-05 00:52:30.982578 windmill_api-1.94.0/windmill_api/api/folder/list_folders.py
+-rw-r--r--   0        0        0     2244 2023-05-05 00:52:30.998578 windmill_api-1.94.0/windmill_api/api/folder/remove_owner_to_folder.py
+-rw-r--r--   0        0        0     2170 2023-05-05 00:52:31.042579 windmill_api-1.94.0/windmill_api/api/folder/update_folder.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:20.066380 windmill_api-1.94.0/windmill_api/api/granular_acl/__init__.py
+-rw-r--r--   0        0        0     2480 2023-05-05 00:52:31.034579 windmill_api-1.94.0/windmill_api/api/granular_acl/add_granular_acls.py
+-rw-r--r--   0        0        0     3526 2023-05-05 00:52:31.078580 windmill_api-1.94.0/windmill_api/api/granular_acl/get_granular_acls.py
+-rw-r--r--   0        0        0     2545 2023-05-05 00:52:31.074580 windmill_api-1.94.0/windmill_api/api/granular_acl/remove_granular_acls.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:20.054380 windmill_api-1.94.0/windmill_api/api/group/__init__.py
+-rw-r--r--   0        0        0     2194 2023-05-05 00:52:31.106580 windmill_api-1.94.0/windmill_api/api/group/add_user_to_group.py
+-rw-r--r--   0        0        0     2019 2023-05-05 00:52:31.106580 windmill_api-1.94.0/windmill_api/api/group/create_group.py
+-rw-r--r--   0        0        0     1775 2023-05-05 00:52:31.130581 windmill_api-1.94.0/windmill_api/api/group/delete_group.py
+-rw-r--r--   0        0        0     2942 2023-05-05 00:52:31.150581 windmill_api-1.94.0/windmill_api/api/group/get_group.py
+-rw-r--r--   0        0        0     3400 2023-05-05 00:52:31.178582 windmill_api-1.94.0/windmill_api/api/group/list_group_names.py
+-rw-r--r--   0        0        0     4233 2023-05-05 00:52:31.206582 windmill_api-1.94.0/windmill_api/api/group/list_groups.py
+-rw-r--r--   0        0        0     2224 2023-05-05 00:52:31.210582 windmill_api-1.94.0/windmill_api/api/group/remove_user_to_group.py
+-rw-r--r--   0        0        0     2160 2023-05-05 00:52:31.238583 windmill_api-1.94.0/windmill_api/api/group/update_group.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:20.070380 windmill_api-1.94.0/windmill_api/api/input_/__init__.py
+-rw-r--r--   0        0        0     3338 2023-05-05 00:52:31.250583 windmill_api-1.94.0/windmill_api/api/input_/create_input.py
+-rw-r--r--   0        0        0     1811 2023-05-05 00:52:31.266583 windmill_api-1.94.0/windmill_api/api/input_/delete_input.py
+-rw-r--r--   0        0        0     6187 2023-05-05 00:52:31.338585 windmill_api-1.94.0/windmill_api/api/input_/get_input_history.py
+-rw-r--r--   0        0        0     6010 2023-05-05 00:52:31.338585 windmill_api-1.94.0/windmill_api/api/input_/list_inputs.py
+-rw-r--r--   0        0        0     2025 2023-05-05 00:52:31.366585 windmill_api-1.94.0/windmill_api/api/input_/update_input.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:20.026379 windmill_api-1.94.0/windmill_api/api/job/__init__.py
+-rw-r--r--   0        0        0     2181 2023-05-05 00:52:31.390586 windmill_api-1.94.0/windmill_api/api/job/cancel_queued_job.py
+-rw-r--r--   0        0        0     2687 2023-05-05 00:52:31.402586 windmill_api-1.94.0/windmill_api/api/job/cancel_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-05-05 00:52:31.430586 windmill_api-1.94.0/windmill_api/api/job/cancel_suspended_job_post.py
+-rw-r--r--   0        0        0     2535 2023-05-05 00:52:31.438586 windmill_api-1.94.0/windmill_api/api/job/create_job_signature.py
+-rw-r--r--   0        0        0     3217 2023-05-05 00:52:31.474587 windmill_api-1.94.0/windmill_api/api/job/delete_completed_job.py
+-rw-r--r--   0        0        0     2235 2023-05-05 00:52:31.466587 windmill_api-1.94.0/windmill_api/api/job/force_cancel_queued_job.py
+-rw-r--r--   0        0        0     3034 2023-05-05 00:52:31.502587 windmill_api-1.94.0/windmill_api/api/job/get_completed_job.py
+-rw-r--r--   0        0        0     1784 2023-05-05 00:52:31.498587 windmill_api-1.94.0/windmill_api/api/job/get_completed_job_result.py
+-rw-r--r--   0        0        0     2868 2023-05-05 00:52:31.538588 windmill_api-1.94.0/windmill_api/api/job/get_job.py
+-rw-r--r--   0        0        0     4305 2023-05-05 00:52:31.558589 windmill_api-1.94.0/windmill_api/api/job/get_job_updates.py
+-rw-r--r--   0        0        0     4306 2023-05-05 00:52:31.594589 windmill_api-1.94.0/windmill_api/api/job/get_resume_urls.py
+-rw-r--r--   0        0        0     4601 2023-05-05 00:52:31.610589 windmill_api-1.94.0/windmill_api/api/job/get_suspended_job_flow.py
+-rw-r--r--   0        0        0    13065 2023-05-05 00:52:31.754592 windmill_api-1.94.0/windmill_api/api/job/list_completed_jobs.py
+-rw-r--r--   0        0        0    12292 2023-05-05 00:52:31.766592 windmill_api-1.94.0/windmill_api/api/job/list_jobs.py
+-rw-r--r--   0        0        0    12830 2023-05-05 00:52:31.898595 windmill_api-1.94.0/windmill_api/api/job/list_queue.py
+-rw-r--r--   0        0        0     2067 2023-05-05 00:52:31.794593 windmill_api-1.94.0/windmill_api/api/job/result_by_id.py
+-rw-r--r--   0        0        0     2313 2023-05-05 00:52:31.822593 windmill_api-1.94.0/windmill_api/api/job/resume_suspended_flow_as_owner.py
+-rw-r--r--   0        0        0     2994 2023-05-05 00:52:31.862594 windmill_api-1.94.0/windmill_api/api/job/resume_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-05-05 00:52:31.902595 windmill_api-1.94.0/windmill_api/api/job/resume_suspended_job_post.py
+-rw-r--r--   0        0        0     4566 2023-05-05 00:52:31.958596 windmill_api-1.94.0/windmill_api/api/job/run_flow_by_path.py
+-rw-r--r--   0        0        0     3037 2023-05-05 00:52:31.938595 windmill_api-1.94.0/windmill_api/api/job/run_flow_preview.py
+-rw-r--r--   0        0        0     4594 2023-05-05 00:52:32.014597 windmill_api-1.94.0/windmill_api/api/job/run_script_by_hash.py
+-rw-r--r--   0        0        0     4200 2023-05-05 00:52:32.010597 windmill_api-1.94.0/windmill_api/api/job/run_script_by_path.py
+-rw-r--r--   0        0        0     3050 2023-05-05 00:52:32.054597 windmill_api-1.94.0/windmill_api/api/job/run_script_preview.py
+-rw-r--r--   0        0        0     3215 2023-05-05 00:52:32.054597 windmill_api-1.94.0/windmill_api/api/job/run_wait_result_flow_by_path.py
+-rw-r--r--   0        0        0     3521 2023-05-05 00:52:32.126599 windmill_api-1.94.0/windmill_api/api/job/run_wait_result_script_by_path.py
+-rw-r--r--   0        0        0     3356 2023-05-05 00:52:32.098598 windmill_api-1.94.0/windmill_api/api/job/run_wait_result_script_by_path_get.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:19.962378 windmill_api-1.94.0/windmill_api/api/oauth/__init__.py
+-rw-r--r--   0        0        0     3506 2023-05-05 00:52:32.138599 windmill_api-1.94.0/windmill_api/api/oauth/connect_callback.py
+-rw-r--r--   0        0        0     2118 2023-05-05 00:52:32.158599 windmill_api-1.94.0/windmill_api/api/oauth/connect_slack_callback.py
+-rw-r--r--   0        0        0     2056 2023-05-05 00:52:32.166600 windmill_api-1.94.0/windmill_api/api/oauth/create_account.py
+-rw-r--r--   0        0        0     1764 2023-05-05 00:52:32.186600 windmill_api-1.94.0/windmill_api/api/oauth/disconnect_account.py
+-rw-r--r--   0        0        0     1649 2023-05-05 00:52:32.190600 windmill_api-1.94.0/windmill_api/api/oauth/disconnect_slack.py
+-rw-r--r--   0        0        0     1426 2023-05-05 00:52:32.210600 windmill_api-1.94.0/windmill_api/api/oauth/list_o_auth_connects.py
+-rw-r--r--   0        0        0     2162 2023-05-05 00:52:32.226601 windmill_api-1.94.0/windmill_api/api/oauth/list_o_auth_logins.py
+-rw-r--r--   0        0        0     2151 2023-05-05 00:52:32.250601 windmill_api-1.94.0/windmill_api/api/oauth/refresh_token.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:19.966378 windmill_api-1.94.0/windmill_api/api/resource/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-05 00:52:32.254601 windmill_api-1.94.0/windmill_api/api/resource/create_resource.py
+-rw-r--r--   0        0        0     2093 2023-05-05 00:52:32.282602 windmill_api-1.94.0/windmill_api/api/resource/create_resource_type.py
+-rw-r--r--   0        0        0     1784 2023-05-05 00:52:32.278602 windmill_api-1.94.0/windmill_api/api/resource/delete_resource.py
+-rw-r--r--   0        0        0     1799 2023-05-05 00:52:32.322602 windmill_api-1.94.0/windmill_api/api/resource/delete_resource_type.py
+-rw-r--r--   0        0        0     2763 2023-05-05 00:52:32.318602 windmill_api-1.94.0/windmill_api/api/resource/exists_resource.py
+-rw-r--r--   0        0        0     2788 2023-05-05 00:52:32.362603 windmill_api-1.94.0/windmill_api/api/resource/exists_resource_type.py
+-rw-r--r--   0        0        0     2996 2023-05-05 00:52:32.358603 windmill_api-1.94.0/windmill_api/api/resource/get_resource.py
+-rw-r--r--   0        0        0     3074 2023-05-05 00:52:32.398604 windmill_api-1.94.0/windmill_api/api/resource/get_resource_type.py
+-rw-r--r--   0        0        0     1790 2023-05-05 00:52:32.390604 windmill_api-1.94.0/windmill_api/api/resource/get_resource_value.py
+-rw-r--r--   0        0        0     5732 2023-05-05 00:52:32.474605 windmill_api-1.94.0/windmill_api/api/resource/list_resource.py
+-rw-r--r--   0        0        0     3149 2023-05-05 00:52:32.434604 windmill_api-1.94.0/windmill_api/api/resource/list_resource_type.py
+-rw-r--r--   0        0        0     2600 2023-05-05 00:52:32.470605 windmill_api-1.94.0/windmill_api/api/resource/list_resource_type_names.py
+-rw-r--r--   0        0        0     2190 2023-05-05 00:52:32.502606 windmill_api-1.94.0/windmill_api/api/resource/update_resource.py
+-rw-r--r--   0        0        0     2234 2023-05-05 00:52:32.506606 windmill_api-1.94.0/windmill_api/api/resource/update_resource_type.py
+-rw-r--r--   0        0        0     2244 2023-05-05 00:52:32.530606 windmill_api-1.94.0/windmill_api/api/resource/update_resource_value.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:20.050380 windmill_api-1.94.0/windmill_api/api/schedule/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-05 00:52:32.534606 windmill_api-1.94.0/windmill_api/api/schedule/create_schedule.py
+-rw-r--r--   0        0        0     1784 2023-05-05 00:52:32.558606 windmill_api-1.94.0/windmill_api/api/schedule/delete_schedule.py
+-rw-r--r--   0        0        0     2763 2023-05-05 00:52:32.574607 windmill_api-1.94.0/windmill_api/api/schedule/exists_schedule.py
+-rw-r--r--   0        0        0     2996 2023-05-05 00:52:32.598607 windmill_api-1.94.0/windmill_api/api/schedule/get_schedule.py
+-rw-r--r--   0        0        0     4287 2023-05-05 00:52:32.630608 windmill_api-1.94.0/windmill_api/api/schedule/list_schedules.py
+-rw-r--r--   0        0        0     3217 2023-05-05 00:52:32.654608 windmill_api-1.94.0/windmill_api/api/schedule/preview_schedule.py
+-rw-r--r--   0        0        0     2233 2023-05-05 00:52:32.662608 windmill_api-1.94.0/windmill_api/api/schedule/set_schedule_enabled.py
+-rw-r--r--   0        0        0     2190 2023-05-05 00:52:32.682609 windmill_api-1.94.0/windmill_api/api/schedule/update_schedule.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:19.974378 windmill_api-1.94.0/windmill_api/api/script/__init__.py
+-rw-r--r--   0        0        0     3165 2023-05-05 00:52:32.702609 windmill_api-1.94.0/windmill_api/api/script/archive_script_by_hash.py
+-rw-r--r--   0        0        0     1797 2023-05-05 00:52:32.710609 windmill_api-1.94.0/windmill_api/api/script/archive_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-05-05 00:52:32.742610 windmill_api-1.94.0/windmill_api/api/script/bash_to_jsonschema.py
+-rw-r--r--   0        0        0     2029 2023-05-05 00:52:32.738610 windmill_api-1.94.0/windmill_api/api/script/create_script.py
+-rw-r--r--   0        0        0     3327 2023-05-05 00:52:32.774610 windmill_api-1.94.0/windmill_api/api/script/delete_script_by_hash.py
+-rw-r--r--   0        0        0     2873 2023-05-05 00:52:32.782611 windmill_api-1.94.0/windmill_api/api/script/delete_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-05-05 00:52:32.810611 windmill_api-1.94.0/windmill_api/api/script/deno_to_jsonschema.py
+-rw-r--r--   0        0        0     2767 2023-05-05 00:52:32.838612 windmill_api-1.94.0/windmill_api/api/script/exists_script_by_path.py
+-rw-r--r--   0        0        0     2802 2023-05-05 00:52:32.846612 windmill_api-1.94.0/windmill_api/api/script/get_hub_script_by_path.py
+-rw-r--r--   0        0        0     1607 2023-05-05 00:52:32.866612 windmill_api-1.94.0/windmill_api/api/script/get_hub_script_content_by_path.py
+-rw-r--r--   0        0        0     3092 2023-05-05 00:52:32.882612 windmill_api-1.94.0/windmill_api/api/script/get_script_by_hash.py
+-rw-r--r--   0        0        0     3074 2023-05-05 00:52:32.906613 windmill_api-1.94.0/windmill_api/api/script/get_script_by_path.py
+-rw-r--r--   0        0        0     3241 2023-05-05 00:52:32.926613 windmill_api-1.94.0/windmill_api/api/script/get_script_by_path_with_draft.py
+-rw-r--r--   0        0        0     3276 2023-05-05 00:52:32.946614 windmill_api-1.94.0/windmill_api/api/script/get_script_deployment_status.py
+-rw-r--r--   0        0        0     2967 2023-05-05 00:52:32.974614 windmill_api-1.94.0/windmill_api/api/script/go_to_jsonschema.py
+-rw-r--r--   0        0        0     2459 2023-05-05 00:52:32.978614 windmill_api-1.94.0/windmill_api/api/script/list_hub_scripts.py
+-rw-r--r--   0        0        0     1676 2023-05-05 00:52:33.002615 windmill_api-1.94.0/windmill_api/api/script/list_script_paths.py
+-rw-r--r--   0        0        0    11165 2023-05-05 00:52:33.106617 windmill_api-1.94.0/windmill_api/api/script/list_scripts.py
+-rw-r--r--   0        0        0     3039 2023-05-05 00:52:33.038615 windmill_api-1.94.0/windmill_api/api/script/python_to_jsonschema.py
+-rw-r--r--   0        0        0     1784 2023-05-05 00:52:33.066616 windmill_api-1.94.0/windmill_api/api/script/raw_script_by_hash.py
+-rw-r--r--   0        0        0     1784 2023-05-05 00:52:33.090616 windmill_api-1.94.0/windmill_api/api/script/raw_script_by_path.py
+-rw-r--r--   0        0        0     2119 2023-05-05 00:52:33.118617 windmill_api-1.94.0/windmill_api/api/script/raw_script_by_path_tokened.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:19.906377 windmill_api-1.94.0/windmill_api/api/settings/__init__.py
+-rw-r--r--   0        0        0     1414 2023-05-05 00:52:33.134617 windmill_api-1.94.0/windmill_api/api/settings/backend_version.py
+-rw-r--r--   0        0        0     1423 2023-05-05 00:52:33.142617 windmill_api-1.94.0/windmill_api/api/settings/get_open_api_yaml.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:19.934378 windmill_api-1.94.0/windmill_api/api/user/__init__.py
+-rw-r--r--   0        0        0     1857 2023-05-05 00:52:33.186618 windmill_api-1.94.0/windmill_api/api/user/accept_invite.py
+-rw-r--r--   0        0        0     1822 2023-05-05 00:52:33.170618 windmill_api-1.94.0/windmill_api/api/user/create_token.py
+-rw-r--r--   0        0        0     1991 2023-05-05 00:52:33.194618 windmill_api-1.94.0/windmill_api/api/user/create_token_impersonate.py
+-rw-r--r--   0        0        0     2058 2023-05-05 00:52:33.214619 windmill_api-1.94.0/windmill_api/api/user/create_user.py
+-rw-r--r--   0        0        0     1863 2023-05-05 00:52:33.222619 windmill_api-1.94.0/windmill_api/api/user/create_user_globally.py
+-rw-r--r--   0        0        0     1867 2023-05-05 00:52:33.242619 windmill_api-1.94.0/windmill_api/api/user/decline_invite.py
+-rw-r--r--   0        0        0     1674 2023-05-05 00:52:33.246619 windmill_api-1.94.0/windmill_api/api/user/delete_token.py
+-rw-r--r--   0        0        0     1872 2023-05-05 00:52:33.270619 windmill_api-1.94.0/windmill_api/api/user/delete_user.py
+-rw-r--r--   0        0        0     1454 2023-05-05 00:52:33.282620 windmill_api-1.94.0/windmill_api/api/user/get_current_email.py
+-rw-r--r--   0        0        0     1474 2023-05-05 00:52:33.294620 windmill_api-1.94.0/windmill_api/api/user/get_usage.py
+-rw-r--r--   0        0        0     1639 2023-05-05 00:52:33.306620 windmill_api-1.94.0/windmill_api/api/user/global_user_delete.py
+-rw-r--r--   0        0        0     2060 2023-05-05 00:52:33.322620 windmill_api-1.94.0/windmill_api/api/user/global_user_update.py
+-rw-r--r--   0        0        0     2468 2023-05-05 00:52:33.338621 windmill_api-1.94.0/windmill_api/api/user/global_whoami.py
+-rw-r--r--   0        0        0     2745 2023-05-05 00:52:33.374621 windmill_api-1.94.0/windmill_api/api/user/is_owner_of_path.py
+-rw-r--r--   0        0        0     1646 2023-05-05 00:52:33.362621 windmill_api-1.94.0/windmill_api/api/user/leave_workspace.py
+-rw-r--r--   0        0        0     2633 2023-05-05 00:52:33.398622 windmill_api-1.94.0/windmill_api/api/user/list_tokens.py
+-rw-r--r--   0        0        0     2552 2023-05-05 00:52:33.414622 windmill_api-1.94.0/windmill_api/api/user/list_usernames.py
+-rw-r--r--   0        0        0     3012 2023-05-05 00:52:33.438623 windmill_api-1.94.0/windmill_api/api/user/list_users.py
+-rw-r--r--   0        0        0     4222 2023-05-05 00:52:33.466623 windmill_api-1.94.0/windmill_api/api/user/list_users_as_super_admin.py
+-rw-r--r--   0        0        0     2829 2023-05-05 00:52:33.478623 windmill_api-1.94.0/windmill_api/api/user/list_workspace_invites.py
+-rw-r--r--   0        0        0     1784 2023-05-05 00:52:33.494624 windmill_api-1.94.0/windmill_api/api/user/login.py
+-rw-r--r--   0        0        0     2116 2023-05-05 00:52:33.506624 windmill_api-1.94.0/windmill_api/api/user/login_with_oauth.py
+-rw-r--r--   0        0        0     1393 2023-05-05 00:52:33.530624 windmill_api-1.94.0/windmill_api/api/user/logout.py
+-rw-r--r--   0        0        0     1820 2023-05-05 00:52:33.534624 windmill_api-1.94.0/windmill_api/api/user/set_password.py
+-rw-r--r--   0        0        0     2250 2023-05-05 00:52:33.558625 windmill_api-1.94.0/windmill_api/api/user/update_user.py
+-rw-r--r--   0        0        0     2652 2023-05-05 00:52:33.570625 windmill_api-1.94.0/windmill_api/api/user/whoami.py
+-rw-r--r--   0        0        0     2967 2023-05-05 00:52:33.598625 windmill_api-1.94.0/windmill_api/api/user/whois.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:19.958378 windmill_api-1.94.0/windmill_api/api/variable/__init__.py
+-rw-r--r--   0        0        0     2634 2023-05-05 00:52:33.626626 windmill_api-1.94.0/windmill_api/api/variable/create_variable.py
+-rw-r--r--   0        0        0     1784 2023-05-05 00:52:33.622626 windmill_api-1.94.0/windmill_api/api/variable/delete_variable.py
+-rw-r--r--   0        0        0     2795 2023-05-05 00:52:33.658626 windmill_api-1.94.0/windmill_api/api/variable/exists_variable.py
+-rw-r--r--   0        0        0     3840 2023-05-05 00:52:33.674627 windmill_api-1.94.0/windmill_api/api/variable/get_variable.py
+-rw-r--r--   0        0        0     3270 2023-05-05 00:52:33.698627 windmill_api-1.94.0/windmill_api/api/variable/list_contextual_variables.py
+-rw-r--r--   0        0        0     3071 2023-05-05 00:52:33.714627 windmill_api-1.94.0/windmill_api/api/variable/list_variable.py
+-rw-r--r--   0        0        0     2775 2023-05-05 00:52:33.734628 windmill_api-1.94.0/windmill_api/api/variable/update_variable.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:20.026379 windmill_api-1.94.0/windmill_api/api/worker/__init__.py
+-rw-r--r--   0        0        0     2448 2023-05-05 00:52:33.750628 windmill_api-1.94.0/windmill_api/api/worker/get_custom_tags.py
+-rw-r--r--   0        0        0     3896 2023-05-05 00:52:33.786629 windmill_api-1.94.0/windmill_api/api/worker/list_workers.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:52:19.946378 windmill_api-1.94.0/windmill_api/api/workspace/__init__.py
+-rw-r--r--   0        0        0     2015 2023-05-05 00:52:33.782629 windmill_api-1.94.0/windmill_api/api/workspace/add_user.py
+-rw-r--r--   0        0        0     1647 2023-05-05 00:52:33.806629 windmill_api-1.94.0/windmill_api/api/workspace/archive_workspace.py
+-rw-r--r--   0        0        0     1856 2023-05-05 00:52:33.810629 windmill_api-1.94.0/windmill_api/api/workspace/create_workspace.py
+-rw-r--r--   0        0        0     2049 2023-05-05 00:52:33.838630 windmill_api-1.94.0/windmill_api/api/workspace/delete_invite.py
+-rw-r--r--   0        0        0     1688 2023-05-05 00:52:33.854630 windmill_api-1.94.0/windmill_api/api/workspace/delete_workspace.py
+-rw-r--r--   0        0        0     2063 2023-05-05 00:52:33.862630 windmill_api-1.94.0/windmill_api/api/workspace/edit_auto_invite.py
+-rw-r--r--   0        0        0     2083 2023-05-05 00:52:33.882630 windmill_api-1.94.0/windmill_api/api/workspace/edit_slack_command.py
+-rw-r--r--   0        0        0     2029 2023-05-05 00:52:33.890631 windmill_api-1.94.0/windmill_api/api/workspace/edit_webhook.py
+-rw-r--r--   0        0        0     1856 2023-05-05 00:52:33.910631 windmill_api-1.94.0/windmill_api/api/workspace/exists_username.py
+-rw-r--r--   0        0        0     1856 2023-05-05 00:52:33.918631 windmill_api-1.94.0/windmill_api/api/workspace/exists_workspace.py
+-rw-r--r--   0        0        0     2809 2023-05-05 00:52:33.950632 windmill_api-1.94.0/windmill_api/api/workspace/get_premium_info.py
+-rw-r--r--   0        0        0     2753 2023-05-05 00:52:33.966632 windmill_api-1.94.0/windmill_api/api/workspace/get_settings.py
+-rw-r--r--   0        0        0     2045 2023-05-05 00:52:33.978632 windmill_api-1.94.0/windmill_api/api/workspace/invite_user.py
+-rw-r--r--   0        0        0     2176 2023-05-05 00:52:33.998633 windmill_api-1.94.0/windmill_api/api/workspace/is_domain_allowed.py
+-rw-r--r--   0        0        0     3255 2023-05-05 00:52:34.018633 windmill_api-1.94.0/windmill_api/api/workspace/list_pending_invites.py
+-rw-r--r--   0        0        0     2583 2023-05-05 00:52:34.030633 windmill_api-1.94.0/windmill_api/api/workspace/list_user_workspaces.py
+-rw-r--r--   0        0        0     2775 2023-05-05 00:52:34.054634 windmill_api-1.94.0/windmill_api/api/workspace/list_workspaces.py
+-rw-r--r--   0        0        0     4311 2023-05-05 00:52:34.086634 windmill_api-1.94.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py
+-rw-r--r--   0        0        0     1651 2023-05-05 00:52:34.082634 windmill_api-1.94.0/windmill_api/api/workspace/unarchive_workspace.py
+-rw-r--r--   0        0        0     1821 2023-05-05 00:52:34.110635 windmill_api-1.94.0/windmill_api/client.py
+-rw-r--r--   0        0        0        1 2023-05-05 00:52:50.478931 windmill_api-1.94.0/windmill_api/models/__init__.py
+-rw-r--r--   0        0        0     1667 2023-05-05 00:52:34.134635 windmill_api-1.94.0/windmill_api/models/accept_invite_json_body.py
+-rw-r--r--   0        0        0     1710 2023-05-05 00:52:34.162636 windmill_api-1.94.0/windmill_api/models/add_granular_acls_json_body.py
+-rw-r--r--   0        0        0      301 2023-05-05 00:52:28.758538 windmill_api-1.94.0/windmill_api/models/add_granular_acls_kind.py
+-rw-r--r--   0        0        0     1529 2023-05-05 00:52:34.206636 windmill_api-1.94.0/windmill_api/models/add_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1940 2023-05-05 00:52:34.254637 windmill_api-1.94.0/windmill_api/models/add_user_json_body.py
+-rw-r--r--   0        0        0     1552 2023-05-05 00:52:34.230637 windmill_api-1.94.0/windmill_api/models/add_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3940 2023-05-05 00:52:34.282638 windmill_api-1.94.0/windmill_api/models/app_with_last_version.py
+-rw-r--r--   0        0        0      214 2023-05-05 00:52:29.258547 windmill_api-1.94.0/windmill_api/models/app_with_last_version_execution_mode.py
+-rw-r--r--   0        0        0     1248 2023-05-05 00:52:34.274638 windmill_api-1.94.0/windmill_api/models/app_with_last_version_extra_perms.py
+-rw-r--r--   0        0        0     3716 2023-05-05 00:52:34.326639 windmill_api-1.94.0/windmill_api/models/app_with_last_version_policy.py
+-rw-r--r--   0        0        0      220 2023-05-05 00:52:29.306548 windmill_api-1.94.0/windmill_api/models/app_with_last_version_policy_execution_mode.py
+-rw-r--r--   0        0        0     1946 2023-05-05 00:52:34.306638 windmill_api-1.94.0/windmill_api/models/app_with_last_version_policy_triggerables.py
+-rw-r--r--   0        0        0     1381 2023-05-05 00:52:34.326639 windmill_api-1.94.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4638 2023-05-05 00:52:34.378640 windmill_api-1.94.0/windmill_api/models/app_with_last_version_w_draft.py
+-rw-r--r--   0        0        0      220 2023-05-05 00:52:29.326548 windmill_api-1.94.0/windmill_api/models/app_with_last_version_w_draft_execution_mode.py
+-rw-r--r--   0        0        0     1284 2023-05-05 00:52:34.350639 windmill_api-1.94.0/windmill_api/models/app_with_last_version_w_draft_extra_perms.py
+-rw-r--r--   0        0        0     3828 2023-05-05 00:52:34.394640 windmill_api-1.94.0/windmill_api/models/app_with_last_version_w_draft_policy.py
+-rw-r--r--   0        0        0      226 2023-05-05 00:52:28.866540 windmill_api-1.94.0/windmill_api/models/app_with_last_version_w_draft_policy_execution_mode.py
+-rw-r--r--   0        0        0     2020 2023-05-05 00:52:34.406640 windmill_api-1.94.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py
+-rw-r--r--   0        0        0     1417 2023-05-05 00:52:34.414640 windmill_api-1.94.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1569 2023-05-05 00:52:34.434641 windmill_api-1.94.0/windmill_api/models/archive_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     7662 2023-05-05 00:52:34.530642 windmill_api-1.94.0/windmill_api/models/archive_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1314 2023-05-05 00:52:34.454641 windmill_api-1.94.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      259 2023-05-05 00:52:29.542552 windmill_api-1.94.0/windmill_api/models/archive_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      217 2023-05-05 00:52:29.226546 windmill_api-1.94.0/windmill_api/models/archive_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1288 2023-05-05 00:52:34.478641 windmill_api-1.94.0/windmill_api/models/archive_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     3452 2023-05-05 00:52:34.526642 windmill_api-1.94.0/windmill_api/models/audit_log.py
+-rw-r--r--   0        0        0      217 2023-05-05 00:52:29.298548 windmill_api-1.94.0/windmill_api/models/audit_log_action_kind.py
+-rw-r--r--   0        0        0      620 2023-05-05 00:52:29.186546 windmill_api-1.94.0/windmill_api/models/audit_log_operation.py
+-rw-r--r--   0        0        0     1186 2023-05-05 00:52:34.550643 windmill_api-1.94.0/windmill_api/models/audit_log_parameters.py
+-rw-r--r--   0        0        0     2933 2023-05-05 00:52:34.574643 windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-05-05 00:52:34.626644 windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-05-05 00:52:29.202546 windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-05-05 00:52:34.598643 windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-05-05 00:52:34.642644 windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-05-05 00:52:34.654644 windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-05-05 00:52:34.682645 windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-05-05 00:52:29.366549 windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-05-05 00:52:34.678645 windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-05-05 00:52:34.718646 windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-05-05 00:52:29.306548 windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-05-05 00:52:34.706645 windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-05 00:52:28.602535 windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2377 2023-05-05 00:52:34.746646 windmill_api-1.94.0/windmill_api/models/branch_all.py
+-rw-r--r--   0        0        0     2543 2023-05-05 00:52:34.750646 windmill_api-1.94.0/windmill_api/models/branch_all_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-05-05 00:52:34.826648 windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-05-05 00:52:34.790647 windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-05 00:52:34.818647 windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-05 00:52:34.846648 windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-05 00:52:34.858648 windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-05 00:52:29.278547 windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-05 00:52:34.874648 windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-05 00:52:28.878540 windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-05 00:52:34.886649 windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-05 00:52:34.902649 windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-05-05 00:52:28.802539 windmill_api-1.94.0/windmill_api/models/branch_all_type.py
+-rw-r--r--   0        0        0     2670 2023-05-05 00:52:34.926649 windmill_api-1.94.0/windmill_api/models/branch_one.py
+-rw-r--r--   0        0        0     2372 2023-05-05 00:52:34.954650 windmill_api-1.94.0/windmill_api/models/branch_one_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-05-05 00:52:35.030651 windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-05-05 00:52:34.990651 windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-05 00:52:35.018651 windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-05 00:52:35.050652 windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-05 00:52:35.058652 windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-05 00:52:29.194546 windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-05 00:52:35.078652 windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-05 00:52:28.742538 windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-05 00:52:35.090652 windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-05 00:52:35.106653 windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6125 2023-05-05 00:52:35.170654 windmill_api-1.94.0/windmill_api/models/branch_one_default_item.py
+-rw-r--r--   0        0        0     2906 2023-05-05 00:52:35.146653 windmill_api-1.94.0/windmill_api/models/branch_one_default_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-05-05 00:52:35.174654 windmill_api-1.94.0/windmill_api/models/branch_one_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-05-05 00:52:35.202654 windmill_api-1.94.0/windmill_api/models/branch_one_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-05-05 00:52:35.202654 windmill_api-1.94.0/windmill_api/models/branch_one_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-05-05 00:52:28.874540 windmill_api-1.94.0/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-05-05 00:52:35.230655 windmill_api-1.94.0/windmill_api/models/branch_one_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-05 00:52:29.454551 windmill_api-1.94.0/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-05-05 00:52:35.242655 windmill_api-1.94.0/windmill_api/models/branch_one_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-05-05 00:52:35.254655 windmill_api-1.94.0/windmill_api/models/branch_one_default_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-05-05 00:52:29.286548 windmill_api-1.94.0/windmill_api/models/branch_one_type.py
+-rw-r--r--   0        0        0     1532 2023-05-05 00:52:35.266656 windmill_api-1.94.0/windmill_api/models/cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     1255 2023-05-05 00:52:35.274656 windmill_api-1.94.0/windmill_api/models/cancel_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0    10508 2023-05-05 00:52:35.434659 windmill_api-1.94.0/windmill_api/models/completed_job.py
+-rw-r--r--   0        0        0     1176 2023-05-05 00:52:35.310656 windmill_api-1.94.0/windmill_api/models/completed_job_args.py
+-rw-r--r--   0        0        0     3265 2023-05-05 00:52:35.350657 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status.py
+-rw-r--r--   0        0        0     6800 2023-05-05 00:52:35.430658 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1789 2023-05-05 00:52:35.458659 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2136 2023-05-05 00:52:35.470659 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      202 2023-05-05 00:52:29.466551 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1694 2023-05-05 00:52:35.486659 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2230 2023-05-05 00:52:35.502660 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      360 2023-05-05 00:52:28.726537 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6402 2023-05-05 00:52:35.566661 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1779 2023-05-05 00:52:35.526660 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2116 2023-05-05 00:52:35.554661 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      200 2023-05-05 00:52:28.486533 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1684 2023-05-05 00:52:35.582661 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2220 2023-05-05 00:52:35.602661 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      358 2023-05-05 00:52:29.542552 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2040 2023-05-05 00:52:35.618662 windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_retry.py
+-rw-r--r--   0        0        0      310 2023-05-05 00:52:28.958541 windmill_api-1.94.0/windmill_api/models/completed_job_job_kind.py
+-rw-r--r--   0        0        0      199 2023-05-05 00:52:28.474533 windmill_api-1.94.0/windmill_api/models/completed_job_language.py
+-rw-r--r--   0        0        0     3127 2023-05-05 00:52:35.674663 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow.py
+-rw-r--r--   0        0        0     6620 2023-05-05 00:52:35.694663 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3129 2023-05-05 00:52:35.714664 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-05 00:52:35.722664 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-05 00:52:35.746664 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-05 00:52:35.774665 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-05 00:52:29.050543 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-05 00:52:35.778665 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-05 00:52:29.046543 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-05 00:52:35.802665 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-05 00:52:35.806665 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6544 2023-05-05 00:52:35.878666 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3095 2023-05-05 00:52:35.846666 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1919 2023-05-05 00:52:35.874667 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2223 2023-05-05 00:52:35.910667 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2050 2023-05-05 00:52:35.906667 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      179 2023-05-05 00:52:28.846540 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1917 2023-05-05 00:52:35.930667 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      179 2023-05-05 00:52:28.886540 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1912 2023-05-05 00:52:35.938668 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1963 2023-05-05 00:52:35.958668 windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1572 2023-05-05 00:52:35.966668 windmill_api-1.94.0/windmill_api/models/connect_callback_json_body.py
+-rw-r--r--   0        0        0     2533 2023-05-05 00:52:35.998669 windmill_api-1.94.0/windmill_api/models/connect_callback_response_200.py
+-rw-r--r--   0        0        0     1600 2023-05-05 00:52:35.990669 windmill_api-1.94.0/windmill_api/models/connect_slack_callback_json_body.py
+-rw-r--r--   0        0        0     1753 2023-05-05 00:52:36.018669 windmill_api-1.94.0/windmill_api/models/contextual_variable.py
+-rw-r--r--   0        0        0     2147 2023-05-05 00:52:36.026669 windmill_api-1.94.0/windmill_api/models/create_account_json_body.py
+-rw-r--r--   0        0        0     2367 2023-05-05 00:52:36.066670 windmill_api-1.94.0/windmill_api/models/create_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-05-05 00:52:36.070670 windmill_api-1.94.0/windmill_api/models/create_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-05-05 00:52:29.550552 windmill_api-1.94.0/windmill_api/models/create_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-05-05 00:52:36.094670 windmill_api-1.94.0/windmill_api/models/create_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-05-05 00:52:36.090670 windmill_api-1.94.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1947 2023-05-05 00:52:36.146671 windmill_api-1.94.0/windmill_api/models/create_draft_json_body.py
+-rw-r--r--   0        0        0      183 2023-05-05 00:52:29.002542 windmill_api-1.94.0/windmill_api/models/create_draft_json_body_typ.py
+-rw-r--r--   0        0        0     1550 2023-05-05 00:52:36.122671 windmill_api-1.94.0/windmill_api/models/create_flow_json_body.py
+-rw-r--r--   0        0        0     2126 2023-05-05 00:52:36.154672 windmill_api-1.94.0/windmill_api/models/create_folder_json_body.py
+-rw-r--r--   0        0        0     1697 2023-05-05 00:52:36.174672 windmill_api-1.94.0/windmill_api/models/create_group_json_body.py
+-rw-r--r--   0        0        0     1613 2023-05-05 00:52:36.182672 windmill_api-1.94.0/windmill_api/models/create_input.py
+-rw-r--r--   0        0        0     1171 2023-05-05 00:52:36.190672 windmill_api-1.94.0/windmill_api/models/create_input_args.py
+-rw-r--r--   0        0        0     1701 2023-05-05 00:52:36.210672 windmill_api-1.94.0/windmill_api/models/create_input_json_body.py
+-rw-r--r--   0        0        0     1217 2023-05-05 00:52:36.210672 windmill_api-1.94.0/windmill_api/models/create_input_json_body_args.py
+-rw-r--r--   0        0        0      214 2023-05-05 00:52:28.502533 windmill_api-1.94.0/windmill_api/models/create_input_runnable_type.py
+-rw-r--r--   0        0        0     2094 2023-05-05 00:52:36.242673 windmill_api-1.94.0/windmill_api/models/create_resource.py
+-rw-r--r--   0        0        0     2140 2023-05-05 00:52:36.246673 windmill_api-1.94.0/windmill_api/models/create_resource_json_body.py
+-rw-r--r--   0        0        0     2335 2023-05-05 00:52:36.278674 windmill_api-1.94.0/windmill_api/models/create_resource_type_json_body.py
+-rw-r--r--   0        0        0     2780 2023-05-05 00:52:36.286674 windmill_api-1.94.0/windmill_api/models/create_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-05 00:52:36.294674 windmill_api-1.94.0/windmill_api/models/create_schedule_json_body_args.py
+-rw-r--r--   0        0        0     5120 2023-05-05 00:52:36.366675 windmill_api-1.94.0/windmill_api/models/create_script_json_body.py
+-rw-r--r--   0        0        0      249 2023-05-05 00:52:29.546552 windmill_api-1.94.0/windmill_api/models/create_script_json_body_kind.py
+-rw-r--r--   0        0        0      207 2023-05-05 00:52:28.478533 windmill_api-1.94.0/windmill_api/models/create_script_json_body_language.py
+-rw-r--r--   0        0        0     1232 2023-05-05 00:52:36.318674 windmill_api-1.94.0/windmill_api/models/create_script_json_body_schema.py
+-rw-r--r--   0        0        0     2534 2023-05-05 00:52:36.354675 windmill_api-1.94.0/windmill_api/models/create_token_impersonate_json_body.py
+-rw-r--r--   0        0        0     2169 2023-05-05 00:52:36.386676 windmill_api-1.94.0/windmill_api/models/create_token_json_body.py
+-rw-r--r--   0        0        0     2364 2023-05-05 00:52:36.406676 windmill_api-1.94.0/windmill_api/models/create_user_globally_json_body.py
+-rw-r--r--   0        0        0     1771 2023-05-05 00:52:36.414676 windmill_api-1.94.0/windmill_api/models/create_user_json_body.py
+-rw-r--r--   0        0        0     2493 2023-05-05 00:52:36.462677 windmill_api-1.94.0/windmill_api/models/create_variable.py
+-rw-r--r--   0        0        0     2539 2023-05-05 00:52:36.450677 windmill_api-1.94.0/windmill_api/models/create_variable_json_body.py
+-rw-r--r--   0        0        0     1678 2023-05-05 00:52:36.478677 windmill_api-1.94.0/windmill_api/models/create_workspace.py
+-rw-r--r--   0        0        0     1724 2023-05-05 00:52:36.490678 windmill_api-1.94.0/windmill_api/models/create_workspace_json_body.py
+-rw-r--r--   0        0        0     1490 2023-05-05 00:52:36.522678 windmill_api-1.94.0/windmill_api/models/decline_invite_json_body.py
+-rw-r--r--   0        0        0    11110 2023-05-05 00:52:36.622680 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200.py
+-rw-r--r--   0        0        0     1270 2023-05-05 00:52:36.542678 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3658 2023-05-05 00:52:36.582679 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7442 2023-05-05 00:52:36.666681 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1883 2023-05-05 00:52:36.646680 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2318 2023-05-05 00:52:36.678681 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      219 2023-05-05 00:52:29.082544 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1788 2023-05-05 00:52:36.690681 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2324 2023-05-05 00:52:36.714682 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      377 2023-05-05 00:52:29.282547 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7053 2023-05-05 00:52:36.770683 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1873 2023-05-05 00:52:36.738682 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2298 2023-05-05 00:52:36.766682 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      217 2023-05-05 00:52:28.646536 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1778 2023-05-05 00:52:36.822684 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2314 2023-05-05 00:52:36.806683 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      375 2023-05-05 00:52:28.662536 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2134 2023-05-05 00:52:36.870684 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      327 2023-05-05 00:52:28.482533 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      216 2023-05-05 00:52:29.018543 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3432 2023-05-05 00:52:36.866684 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7425 2023-05-05 00:52:36.946686 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3442 2023-05-05 00:52:36.906685 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2023 2023-05-05 00:52:36.934686 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2327 2023-05-05 00:52:36.970686 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2261 2023-05-05 00:52:36.974686 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-05 00:52:28.674536 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-05 00:52:36.998687 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-05 00:52:29.270547 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2016 2023-05-05 00:52:37.002687 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2067 2023-05-05 00:52:37.026687 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7349 2023-05-05 00:52:37.086688 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3408 2023-05-05 00:52:37.070688 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2013 2023-05-05 00:52:37.098689 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2317 2023-05-05 00:52:37.118689 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2241 2023-05-05 00:52:37.130689 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-05-05 00:52:29.254547 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2108 2023-05-05 00:52:37.170690 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-05-05 00:52:29.066543 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2006 2023-05-05 00:52:37.158690 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2057 2023-05-05 00:52:37.186690 windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1783 2023-05-05 00:52:37.194690 windmill_api-1.94.0/windmill_api/models/delete_invite_json_body.py
+-rw-r--r--   0        0        0     7636 2023-05-05 00:52:37.298692 windmill_api-1.94.0/windmill_api/models/delete_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1309 2023-05-05 00:52:37.214691 windmill_api-1.94.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      258 2023-05-05 00:52:29.078544 windmill_api-1.94.0/windmill_api/models/delete_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      216 2023-05-05 00:52:28.562534 windmill_api-1.94.0/windmill_api/models/delete_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1283 2023-05-05 00:52:37.238691 windmill_api-1.94.0/windmill_api/models/delete_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     2933 2023-05-05 00:52:37.278692 windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-05-05 00:52:37.334693 windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-05-05 00:52:28.658536 windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-05-05 00:52:37.322693 windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-05-05 00:52:37.350693 windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-05-05 00:52:37.362693 windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-05-05 00:52:37.386694 windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-05-05 00:52:29.066543 windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-05-05 00:52:37.386694 windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-05-05 00:52:37.422695 windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-05-05 00:52:28.986542 windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-05-05 00:52:37.414694 windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-05 00:52:28.838539 windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     1551 2023-05-05 00:52:37.442695 windmill_api-1.94.0/windmill_api/models/edit_auto_invite_json_body.py
+-rw-r--r--   0        0        0     1980 2023-05-05 00:52:37.450695 windmill_api-1.94.0/windmill_api/models/edit_resource.py
+-rw-r--r--   0        0        0     1791 2023-05-05 00:52:37.470695 windmill_api-1.94.0/windmill_api/models/edit_resource_type.py
+-rw-r--r--   0        0        0     1845 2023-05-05 00:52:37.478695 windmill_api-1.94.0/windmill_api/models/edit_schedule.py
+-rw-r--r--   0        0        0     1176 2023-05-05 00:52:37.490696 windmill_api-1.94.0/windmill_api/models/edit_schedule_args.py
+-rw-r--r--   0        0        0     1691 2023-05-05 00:52:37.502696 windmill_api-1.94.0/windmill_api/models/edit_slack_command_json_body.py
+-rw-r--r--   0        0        0     2260 2023-05-05 00:52:37.526696 windmill_api-1.94.0/windmill_api/models/edit_variable.py
+-rw-r--r--   0        0        0     1520 2023-05-05 00:52:37.546697 windmill_api-1.94.0/windmill_api/models/edit_webhook_json_body.py
+-rw-r--r--   0        0        0     2058 2023-05-05 00:52:37.558697 windmill_api-1.94.0/windmill_api/models/edit_workspace_user.py
+-rw-r--r--   0        0        0     3663 2023-05-05 00:52:37.590697 windmill_api-1.94.0/windmill_api/models/execute_component_json_body.py
+-rw-r--r--   0        0        0     1346 2023-05-05 00:52:37.578697 windmill_api-1.94.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
+-rw-r--r--   0        0        0     1942 2023-05-05 00:52:37.646699 windmill_api-1.94.0/windmill_api/models/execute_component_json_body_raw_code.py
+-rw-r--r--   0        0        0     1577 2023-05-05 00:52:37.618698 windmill_api-1.94.0/windmill_api/models/exists_username_json_body.py
+-rw-r--r--   0        0        0     1400 2023-05-05 00:52:37.638698 windmill_api-1.94.0/windmill_api/models/exists_workspace_json_body.py
+-rw-r--r--   0        0        0     4924 2023-05-05 00:52:37.702700 windmill_api-1.94.0/windmill_api/models/flow.py
+-rw-r--r--   0        0        0     1166 2023-05-05 00:52:37.666699 windmill_api-1.94.0/windmill_api/models/flow_extra_perms.py
+-rw-r--r--   0        0        0     3707 2023-05-05 00:52:37.714700 windmill_api-1.94.0/windmill_api/models/flow_metadata.py
+-rw-r--r--   0        0        0     1209 2023-05-05 00:52:37.722700 windmill_api-1.94.0/windmill_api/models/flow_metadata_extra_perms.py
+-rw-r--r--   0        0        0     5729 2023-05-05 00:52:37.798701 windmill_api-1.94.0/windmill_api/models/flow_module.py
+-rw-r--r--   0        0        0     2726 2023-05-05 00:52:37.758700 windmill_api-1.94.0/windmill_api/models/flow_module_retry.py
+-rw-r--r--   0        0        0     1807 2023-05-05 00:52:37.786701 windmill_api-1.94.0/windmill_api/models/flow_module_retry_constant.py
+-rw-r--r--   0        0        0     2111 2023-05-05 00:52:37.818702 windmill_api-1.94.0/windmill_api/models/flow_module_retry_exponential.py
+-rw-r--r--   0        0        0     1834 2023-05-05 00:52:37.826702 windmill_api-1.94.0/windmill_api/models/flow_module_sleep_type_0.py
+-rw-r--r--   0        0        0      159 2023-05-05 00:52:29.094544 windmill_api-1.94.0/windmill_api/models/flow_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1701 2023-05-05 00:52:37.842702 windmill_api-1.94.0/windmill_api/models/flow_module_sleep_type_1.py
+-rw-r--r--   0        0        0      159 2023-05-05 00:52:28.782538 windmill_api-1.94.0/windmill_api/models/flow_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1800 2023-05-05 00:52:37.854702 windmill_api-1.94.0/windmill_api/models/flow_module_stop_after_if.py
+-rw-r--r--   0        0        0     1851 2023-05-05 00:52:37.898703 windmill_api-1.94.0/windmill_api/models/flow_module_suspend.py
+-rw-r--r--   0        0        0     3292 2023-05-05 00:52:37.902703 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_0.py
+-rw-r--r--   0        0        0     3564 2023-05-05 00:52:37.930704 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-05 00:52:37.938704 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-05 00:52:29.070544 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-05 00:52:37.958704 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-05 00:52:29.082544 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      208 2023-05-05 00:52:28.874540 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_0_language.py
+-rw-r--r--   0        0        0      158 2023-05-05 00:52:29.442550 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_0_type.py
+-rw-r--r--   0        0        0     2477 2023-05-05 00:52:37.978705 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_1.py
+-rw-r--r--   0        0        0     3564 2023-05-05 00:52:37.994705 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-05 00:52:38.030705 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-05 00:52:29.518552 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-05 00:52:38.022705 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-05 00:52:29.334548 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      152 2023-05-05 00:52:28.750538 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_1_type.py
+-rw-r--r--   0        0        0     2204 2023-05-05 00:52:38.058706 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_2.py
+-rw-r--r--   0        0        0     3564 2023-05-05 00:52:38.070706 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-05 00:52:38.086706 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-05 00:52:29.386549 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-05 00:52:38.098707 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-05 00:52:29.374549 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      148 2023-05-05 00:52:28.742538 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_2_type.py
+-rw-r--r--   0        0        0     4138 2023-05-05 00:52:38.134707 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3.py
+-rw-r--r--   0        0        0     1990 2023-05-05 00:52:38.126707 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
+-rw-r--r--   0        0        0      173 2023-05-05 00:52:28.938541 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1857 2023-05-05 00:52:38.158708 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
+-rw-r--r--   0        0        0      173 2023-05-05 00:52:29.442550 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6636 2023-05-05 00:52:38.214709 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py
+-rw-r--r--   0        0        0     3148 2023-05-05 00:52:38.194708 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-05-05 00:52:38.226709 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-05-05 00:52:38.274710 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-05-05 00:52:38.254710 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-05 00:52:29.530552 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-05-05 00:52:38.282710 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-05 00:52:28.474533 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-05-05 00:52:38.302710 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-05-05 00:52:38.310711 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
+-rw-r--r--   0        0        0      162 2023-05-05 00:52:28.886540 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_type.py
+-rw-r--r--   0        0        0     2934 2023-05-05 00:52:38.342711 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4.py
+-rw-r--r--   0        0        0     2508 2023-05-05 00:52:38.346711 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-05-05 00:52:38.422712 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-05-05 00:52:38.406712 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-05-05 00:52:38.438713 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-05-05 00:52:38.450713 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-05-05 00:52:38.466713 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-05 00:52:28.902541 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-05-05 00:52:38.478714 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-05 00:52:28.774538 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-05-05 00:52:38.494714 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-05-05 00:52:38.506714 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6636 2023-05-05 00:52:38.574715 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item.py
+-rw-r--r--   0        0        0     3148 2023-05-05 00:52:38.546715 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-05-05 00:52:38.570715 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-05-05 00:52:38.634716 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-05-05 00:52:38.602716 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-05 00:52:28.546534 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-05-05 00:52:38.634716 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-05 00:52:28.654536 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-05-05 00:52:38.662717 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-05-05 00:52:38.666717 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-05-05 00:52:28.550534 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_type.py
+-rw-r--r--   0        0        0     2577 2023-05-05 00:52:38.698717 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5.py
+-rw-r--r--   0        0        0     2679 2023-05-05 00:52:38.702718 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-05-05 00:52:38.774719 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-05-05 00:52:38.738718 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-05-05 00:52:38.794719 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-05-05 00:52:38.806719 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-05-05 00:52:38.826720 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-05 00:52:28.714537 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-05-05 00:52:38.834720 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-05 00:52:29.018543 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-05-05 00:52:38.854720 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-05-05 00:52:38.862720 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-05-05 00:52:29.214546 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_type.py
+-rw-r--r--   0        0        0     1839 2023-05-05 00:52:38.886721 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_6.py
+-rw-r--r--   0        0        0      156 2023-05-05 00:52:29.398549 windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_6_type.py
+-rw-r--r--   0        0        0     2009 2023-05-05 00:52:38.894721 windmill_api-1.94.0/windmill_api/models/flow_preview.py
+-rw-r--r--   0        0        0     1171 2023-05-05 00:52:38.906721 windmill_api-1.94.0/windmill_api/models/flow_preview_args.py
+-rw-r--r--   0        0        0     3074 2023-05-05 00:52:38.934722 windmill_api-1.94.0/windmill_api/models/flow_preview_value.py
+-rw-r--r--   0        0        0     6498 2023-05-05 00:52:38.986723 windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module.py
+-rw-r--r--   0        0        0     3064 2023-05-05 00:52:38.998723 windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1911 2023-05-05 00:52:39.018723 windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2215 2023-05-05 00:52:39.030723 windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2036 2023-05-05 00:52:39.046724 windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-05 00:52:29.090544 windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1903 2023-05-05 00:52:39.062724 windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-05 00:52:28.598535 windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1904 2023-05-05 00:52:39.074724 windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1955 2023-05-05 00:52:39.090725 windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6422 2023-05-05 00:52:39.182726 windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item.py
+-rw-r--r--   0        0        0     3030 2023-05-05 00:52:39.130725 windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1901 2023-05-05 00:52:39.158726 windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2205 2023-05-05 00:52:39.190726 windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2016 2023-05-05 00:52:39.210727 windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-05-05 00:52:28.694537 windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1883 2023-05-05 00:52:39.218727 windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-05-05 00:52:28.614535 windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1894 2023-05-05 00:52:39.238727 windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1945 2023-05-05 00:52:39.250728 windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1143 2023-05-05 00:52:39.254727 windmill_api-1.94.0/windmill_api/models/flow_schema.py
+-rw-r--r--   0        0        0     3001 2023-05-05 00:52:39.290728 windmill_api-1.94.0/windmill_api/models/flow_status.py
+-rw-r--r--   0        0        0     6370 2023-05-05 00:52:39.334729 windmill_api-1.94.0/windmill_api/models/flow_status_failure_module.py
+-rw-r--r--   0        0        0     1723 2023-05-05 00:52:39.318729 windmill_api-1.94.0/windmill_api/models/flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     1999 2023-05-05 00:52:39.374730 windmill_api-1.94.0/windmill_api/models/flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      190 2023-05-05 00:52:28.662536 windmill_api-1.94.0/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1628 2023-05-05 00:52:39.362729 windmill_api-1.94.0/windmill_api/models/flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2164 2023-05-05 00:52:39.398730 windmill_api-1.94.0/windmill_api/models/flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      348 2023-05-05 00:52:29.282547 windmill_api-1.94.0/windmill_api/models/flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     5808 2023-05-05 00:52:39.458731 windmill_api-1.94.0/windmill_api/models/flow_status_module.py
+-rw-r--r--   0        0        0     1685 2023-05-05 00:52:39.422731 windmill_api-1.94.0/windmill_api/models/flow_status_module_approvers_item.py
+-rw-r--r--   0        0        0     1925 2023-05-05 00:52:39.450731 windmill_api-1.94.0/windmill_api/models/flow_status_module_branch_chosen.py
+-rw-r--r--   0        0        0      183 2023-05-05 00:52:29.338549 windmill_api-1.94.0/windmill_api/models/flow_status_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1590 2023-05-05 00:52:39.474732 windmill_api-1.94.0/windmill_api/models/flow_status_module_branchall.py
+-rw-r--r--   0        0        0     2126 2023-05-05 00:52:39.494732 windmill_api-1.94.0/windmill_api/models/flow_status_module_iterator.py
+-rw-r--r--   0        0        0      341 2023-05-05 00:52:29.366549 windmill_api-1.94.0/windmill_api/models/flow_status_module_type.py
+-rw-r--r--   0        0        0     5981 2023-05-05 00:52:39.594734 windmill_api-1.94.0/windmill_api/models/flow_status_modules_item.py
+-rw-r--r--   0        0        0     1713 2023-05-05 00:52:39.518732 windmill_api-1.94.0/windmill_api/models/flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     1979 2023-05-05 00:52:39.546733 windmill_api-1.94.0/windmill_api/models/flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      188 2023-05-05 00:52:29.002542 windmill_api-1.94.0/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1618 2023-05-05 00:52:39.570733 windmill_api-1.94.0/windmill_api/models/flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2154 2023-05-05 00:52:39.610734 windmill_api-1.94.0/windmill_api/models/flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      346 2023-05-05 00:52:28.854540 windmill_api-1.94.0/windmill_api/models/flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     1974 2023-05-05 00:52:39.630734 windmill_api-1.94.0/windmill_api/models/flow_status_retry.py
+-rw-r--r--   0        0        0     2957 2023-05-05 00:52:39.650735 windmill_api-1.94.0/windmill_api/models/flow_value.py
+-rw-r--r--   0        0        0     6224 2023-05-05 00:52:39.710736 windmill_api-1.94.0/windmill_api/models/flow_value_failure_module.py
+-rw-r--r--   0        0        0     2940 2023-05-05 00:52:39.686735 windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1873 2023-05-05 00:52:39.746736 windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-05-05 00:52:39.746736 windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-05-05 00:52:39.774737 windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-05-05 00:52:29.030543 windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-05-05 00:52:39.770737 windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-05-05 00:52:29.250547 windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-05-05 00:52:39.798737 windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-05-05 00:52:39.806738 windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6125 2023-05-05 00:52:39.878739 windmill_api-1.94.0/windmill_api/models/flow_value_modules_item.py
+-rw-r--r--   0        0        0     2906 2023-05-05 00:52:39.842738 windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-05-05 00:52:39.870739 windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-05-05 00:52:39.958740 windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-05-05 00:52:39.902739 windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-05-05 00:52:28.854540 windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-05-05 00:52:39.930740 windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-05 00:52:29.046543 windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-05-05 00:52:39.962740 windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-05-05 00:52:39.986741 windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1858 2023-05-05 00:52:39.990741 windmill_api-1.94.0/windmill_api/models/folder.py
+-rw-r--r--   0        0        0     1179 2023-05-05 00:52:40.002741 windmill_api-1.94.0/windmill_api/models/folder_extra_perms.py
+-rw-r--r--   0        0        0     1560 2023-05-05 00:52:40.018741 windmill_api-1.94.0/windmill_api/models/force_cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     3807 2023-05-05 00:52:40.050742 windmill_api-1.94.0/windmill_api/models/forloop_flow.py
+-rw-r--r--   0        0        0     1874 2023-05-05 00:52:40.042742 windmill_api-1.94.0/windmill_api/models/forloop_flow_iterator_type_0.py
+-rw-r--r--   0        0        0      163 2023-05-05 00:52:29.214546 windmill_api-1.94.0/windmill_api/models/forloop_flow_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1741 2023-05-05 00:52:40.074742 windmill_api-1.94.0/windmill_api/models/forloop_flow_iterator_type_1.py
+-rw-r--r--   0        0        0      163 2023-05-05 00:52:29.094544 windmill_api-1.94.0/windmill_api/models/forloop_flow_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6224 2023-05-05 00:52:40.130743 windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item.py
+-rw-r--r--   0        0        0     2940 2023-05-05 00:52:40.150744 windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1873 2023-05-05 00:52:40.158744 windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-05-05 00:52:40.182744 windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-05-05 00:52:40.182744 windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-05-05 00:52:28.510533 windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-05-05 00:52:40.210745 windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-05-05 00:52:29.466551 windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-05-05 00:52:40.214745 windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-05-05 00:52:40.238745 windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0      152 2023-05-05 00:52:28.698537 windmill_api-1.94.0/windmill_api/models/forloop_flow_type.py
+-rw-r--r--   0        0        0     4052 2023-05-05 00:52:40.270746 windmill_api-1.94.0/windmill_api/models/get_app_by_path_response_200.py
+-rw-r--r--   0        0        0      219 2023-05-05 00:52:29.490551 windmill_api-1.94.0/windmill_api/models/get_app_by_path_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1279 2023-05-05 00:52:40.258746 windmill_api-1.94.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3811 2023-05-05 00:52:40.338747 windmill_api-1.94.0/windmill_api/models/get_app_by_path_response_200_policy.py
+-rw-r--r--   0        0        0      225 2023-05-05 00:52:28.878540 windmill_api-1.94.0/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2009 2023-05-05 00:52:40.298746 windmill_api-1.94.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1412 2023-05-05 00:52:40.318747 windmill_api-1.94.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4819 2023-05-05 00:52:40.374748 windmill_api-1.94.0/windmill_api/models/get_app_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0      228 2023-05-05 00:52:29.326548 windmill_api-1.94.0/windmill_api/models/get_app_by_path_with_draft_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1330 2023-05-05 00:52:40.358748 windmill_api-1.94.0/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3992 2023-05-05 00:52:40.406748 windmill_api-1.94.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py
+-rw-r--r--   0        0        0      234 2023-05-05 00:52:28.910541 windmill_api-1.94.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2160 2023-05-05 00:52:40.402748 windmill_api-1.94.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1463 2023-05-05 00:52:40.418748 windmill_api-1.94.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4112 2023-05-05 00:52:40.450749 windmill_api-1.94.0/windmill_api/models/get_app_by_version_response_200.py
+-rw-r--r--   0        0        0      222 2023-05-05 00:52:28.946541 windmill_api-1.94.0/windmill_api/models/get_app_by_version_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1294 2023-05-05 00:52:40.442749 windmill_api-1.94.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3862 2023-05-05 00:52:40.490750 windmill_api-1.94.0/windmill_api/models/get_app_by_version_response_200_policy.py
+-rw-r--r--   0        0        0      228 2023-05-05 00:52:29.254547 windmill_api-1.94.0/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2042 2023-05-05 00:52:40.478750 windmill_api-1.94.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1427 2023-05-05 00:52:40.498750 windmill_api-1.94.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3764 2023-05-05 00:52:40.570751 windmill_api-1.94.0/windmill_api/models/get_audit_log_response_200.py
+-rw-r--r--   0        0        0      231 2023-05-05 00:52:29.102544 windmill_api-1.94.0/windmill_api/models/get_audit_log_response_200_action_kind.py
+-rw-r--r--   0        0        0      634 2023-05-05 00:52:29.386549 windmill_api-1.94.0/windmill_api/models/get_audit_log_response_200_operation.py
+-rw-r--r--   0        0        0     1265 2023-05-05 00:52:40.518750 windmill_api-1.94.0/windmill_api/models/get_audit_log_response_200_parameters.py
+-rw-r--r--   0        0        0    11008 2023-05-05 00:52:40.694754 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200.py
+-rw-r--r--   0        0        0     1255 2023-05-05 00:52:40.586752 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3595 2023-05-05 00:52:40.630752 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7343 2023-05-05 00:52:40.710754 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1868 2023-05-05 00:52:40.718754 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2288 2023-05-05 00:52:40.738754 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      216 2023-05-05 00:52:28.750538 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1773 2023-05-05 00:52:40.746755 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2309 2023-05-05 00:52:40.774755 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      374 2023-05-05 00:52:28.482533 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6924 2023-05-05 00:52:40.830756 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1858 2023-05-05 00:52:40.798756 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-05-05 00:52:40.822756 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-05-05 00:52:28.982542 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-05-05 00:52:40.850756 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2299 2023-05-05 00:52:40.866757 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      372 2023-05-05 00:52:28.750538 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2119 2023-05-05 00:52:40.926758 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      324 2023-05-05 00:52:28.766538 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      213 2023-05-05 00:52:28.922541 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3375 2023-05-05 00:52:40.910757 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7311 2023-05-05 00:52:40.990759 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3391 2023-05-05 00:52:40.962758 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2008 2023-05-05 00:52:40.990759 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2312 2023-05-05 00:52:41.022760 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2231 2023-05-05 00:52:41.018759 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      195 2023-05-05 00:52:28.774538 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2098 2023-05-05 00:52:41.098761 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      195 2023-05-05 00:52:29.410550 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2001 2023-05-05 00:52:41.054760 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2052 2023-05-05 00:52:41.082760 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7235 2023-05-05 00:52:41.162762 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3357 2023-05-05 00:52:41.134761 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1998 2023-05-05 00:52:41.162762 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-05-05 00:52:41.194763 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-05-05 00:52:41.190763 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-05 00:52:29.074544 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-05-05 00:52:41.222763 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-05 00:52:28.946541 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-05-05 00:52:41.226763 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-05-05 00:52:41.250764 windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     5374 2023-05-05 00:52:41.326765 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200.py
+-rw-r--r--   0        0        0     1281 2023-05-05 00:52:41.266764 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1258 2023-05-05 00:52:41.286764 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     3302 2023-05-05 00:52:41.326765 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value.py
+-rw-r--r--   0        0        0     7159 2023-05-05 00:52:41.406767 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
+-rw-r--r--   0        0        0     3323 2023-05-05 00:52:41.366766 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1988 2023-05-05 00:52:41.394766 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-05-05 00:52:41.426767 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-05-05 00:52:41.470768 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-05-05 00:52:28.458532 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-05-05 00:52:41.454767 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-05-05 00:52:28.526534 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-05-05 00:52:41.486768 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-05-05 00:52:41.498768 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7066 2023-05-05 00:52:41.566769 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
+-rw-r--r--   0        0        0     3289 2023-05-05 00:52:41.534769 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1978 2023-05-05 00:52:41.562769 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2282 2023-05-05 00:52:41.594770 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2171 2023-05-05 00:52:41.594770 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-05-05 00:52:28.470533 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2038 2023-05-05 00:52:41.622770 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-05-05 00:52:28.878540 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1971 2023-05-05 00:52:41.634770 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2022 2023-05-05 00:52:41.650771 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2093 2023-05-05 00:52:41.702772 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0     5695 2023-05-05 00:52:41.714772 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py
+-rw-r--r--   0        0        0     1360 2023-05-05 00:52:41.726772 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py
+-rw-r--r--   0        0        0     1337 2023-05-05 00:52:41.734772 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py
+-rw-r--r--   0        0        0     3559 2023-05-05 00:52:41.766773 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py
+-rw-r--r--   0        0        0     7829 2023-05-05 00:52:41.850774 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py
+-rw-r--r--   0        0        0     3606 2023-05-05 00:52:41.806774 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2067 2023-05-05 00:52:41.834774 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2371 2023-05-05 00:52:41.866775 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2343 2023-05-05 00:52:41.878775 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      205 2023-05-05 00:52:28.690537 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2210 2023-05-05 00:52:41.894775 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      205 2023-05-05 00:52:28.786538 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2060 2023-05-05 00:52:41.906775 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2111 2023-05-05 00:52:41.922776 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7685 2023-05-05 00:52:41.986777 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py
+-rw-r--r--   0        0        0     3542 2023-05-05 00:52:41.962777 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2057 2023-05-05 00:52:41.990777 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2361 2023-05-05 00:52:42.018777 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2323 2023-05-05 00:52:42.018777 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      203 2023-05-05 00:52:28.642536 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2190 2023-05-05 00:52:42.042778 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      203 2023-05-05 00:52:29.514551 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2050 2023-05-05 00:52:42.090779 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2101 2023-05-05 00:52:42.074778 windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2756 2023-05-05 00:52:42.110779 windmill_api-1.94.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
+-rw-r--r--   0        0        0     1337 2023-05-05 00:52:42.110779 windmill_api-1.94.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
+-rw-r--r--   0        0        0     2010 2023-05-05 00:52:42.138780 windmill_api-1.94.0/windmill_api/models/get_folder_response_200.py
+-rw-r--r--   0        0        0     1258 2023-05-05 00:52:42.130780 windmill_api-1.94.0/windmill_api/models/get_folder_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2357 2023-05-05 00:52:42.166780 windmill_api-1.94.0/windmill_api/models/get_folder_usage_response_200.py
+-rw-r--r--   0        0        0      301 2023-05-05 00:52:28.698537 windmill_api-1.94.0/windmill_api/models/get_granular_acls_kind.py
+-rw-r--r--   0        0        0     1235 2023-05-05 00:52:42.158780 windmill_api-1.94.0/windmill_api/models/get_granular_acls_response_200.py
+-rw-r--r--   0        0        0     2888 2023-05-05 00:52:42.198781 windmill_api-1.94.0/windmill_api/models/get_group_response_200.py
+-rw-r--r--   0        0        0     1253 2023-05-05 00:52:42.226781 windmill_api-1.94.0/windmill_api/models/get_group_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1606 2023-05-05 00:52:42.222781 windmill_api-1.94.0/windmill_api/models/get_hub_app_by_id_response_200.py
+-rw-r--r--   0        0        0     1634 2023-05-05 00:52:42.246782 windmill_api-1.94.0/windmill_api/models/get_hub_app_by_id_response_200_app.py
+-rw-r--r--   0        0        0     1977 2023-05-05 00:52:42.258782 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200.py
+-rw-r--r--   0        0        0     2950 2023-05-05 00:52:42.286782 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
+-rw-r--r--   0        0        0     1289 2023-05-05 00:52:42.278782 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
+-rw-r--r--   0        0        0     3410 2023-05-05 00:52:42.318783 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
+-rw-r--r--   0        0        0     7365 2023-05-05 00:52:42.366784 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3418 2023-05-05 00:52:42.358784 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2019 2023-05-05 00:52:42.386784 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2323 2023-05-05 00:52:42.398784 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2249 2023-05-05 00:52:42.414785 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-05-05 00:52:29.246547 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2116 2023-05-05 00:52:42.462786 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-05-05 00:52:28.750538 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2012 2023-05-05 00:52:42.442785 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2063 2023-05-05 00:52:42.474786 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7289 2023-05-05 00:52:42.542787 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
+-rw-r--r--   0        0        0     3384 2023-05-05 00:52:42.514787 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2009 2023-05-05 00:52:42.538787 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2313 2023-05-05 00:52:42.574787 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2229 2023-05-05 00:52:42.570788 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      194 2023-05-05 00:52:29.558552 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2096 2023-05-05 00:52:42.598788 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      194 2023-05-05 00:52:29.326548 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2002 2023-05-05 00:52:42.646789 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2053 2023-05-05 00:52:42.626788 windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2698 2023-05-05 00:52:42.662789 windmill_api-1.94.0/windmill_api/models/get_hub_script_by_path_response_200.py
+-rw-r--r--   0        0        0      216 2023-05-05 00:52:29.498551 windmill_api-1.94.0/windmill_api/models/get_hub_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     2644 2023-05-05 00:52:42.686790 windmill_api-1.94.0/windmill_api/models/get_input_history_response_200_item.py
+-rw-r--r--   0        0        0     1278 2023-05-05 00:52:42.682789 windmill_api-1.94.0/windmill_api/models/get_input_history_response_200_item_args.py
+-rw-r--r--   0        0        0      218 2023-05-05 00:52:28.846540 windmill_api-1.94.0/windmill_api/models/get_input_history_runnable_type.py
+-rw-r--r--   0        0        0     1852 2023-05-05 00:52:42.710790 windmill_api-1.94.0/windmill_api/models/get_job_response_200.py
+-rw-r--r--   0        0        0      188 2023-05-05 00:52:29.030543 windmill_api-1.94.0/windmill_api/models/get_job_response_200_type.py
+-rw-r--r--   0        0        0     2364 2023-05-05 00:52:42.722790 windmill_api-1.94.0/windmill_api/models/get_job_updates_response_200.py
+-rw-r--r--   0        0        0     1744 2023-05-05 00:52:42.738791 windmill_api-1.94.0/windmill_api/models/get_premium_info_response_200.py
+-rw-r--r--   0        0        0     4218 2023-05-05 00:52:42.774791 windmill_api-1.94.0/windmill_api/models/get_public_app_by_secret_response_200.py
+-rw-r--r--   0        0        0      227 2023-05-05 00:52:28.478533 windmill_api-1.94.0/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1322 2023-05-05 00:52:42.758791 windmill_api-1.94.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3970 2023-05-05 00:52:42.842792 windmill_api-1.94.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py
+-rw-r--r--   0        0        0      233 2023-05-05 00:52:28.918541 windmill_api-1.94.0/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2131 2023-05-05 00:52:42.802792 windmill_api-1.94.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1455 2023-05-05 00:52:42.818792 windmill_api-1.94.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3533 2023-05-05 00:52:42.870793 windmill_api-1.94.0/windmill_api/models/get_resource_response_200.py
+-rw-r--r--   0        0        0     1268 2023-05-05 00:52:42.862793 windmill_api-1.94.0/windmill_api/models/get_resource_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2335 2023-05-05 00:52:42.894793 windmill_api-1.94.0/windmill_api/models/get_resource_type_response_200.py
+-rw-r--r--   0        0        0     1840 2023-05-05 00:52:42.898794 windmill_api-1.94.0/windmill_api/models/get_resume_urls_response_200.py
+-rw-r--r--   0        0        0     4325 2023-05-05 00:52:42.954795 windmill_api-1.94.0/windmill_api/models/get_schedule_response_200.py
+-rw-r--r--   0        0        0     1232 2023-05-05 00:52:42.918794 windmill_api-1.94.0/windmill_api/models/get_schedule_response_200_args.py
+-rw-r--r--   0        0        0     1268 2023-05-05 00:52:42.934794 windmill_api-1.94.0/windmill_api/models/get_schedule_response_200_extra_perms.py
+-rw-r--r--   0        0        0     7558 2023-05-05 00:52:43.074797 windmill_api-1.94.0/windmill_api/models/get_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-05 00:52:42.970795 windmill_api-1.94.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-05 00:52:29.550552 windmill_api-1.94.0/windmill_api/models/get_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-05-05 00:52:29.010542 windmill_api-1.94.0/windmill_api/models/get_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-05-05 00:52:42.994795 windmill_api-1.94.0/windmill_api/models/get_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     7558 2023-05-05 00:52:43.086797 windmill_api-1.94.0/windmill_api/models/get_script_by_path_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-05 00:52:43.094797 windmill_api-1.94.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-05 00:52:29.210546 windmill_api-1.94.0/windmill_api/models/get_script_by_path_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-05-05 00:52:29.026543 windmill_api-1.94.0/windmill_api/models/get_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-05-05 00:52:43.110797 windmill_api-1.94.0/windmill_api/models/get_script_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     6383 2023-05-05 00:52:43.174798 windmill_api-1.94.0/windmill_api/models/get_script_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0     5608 2023-05-05 00:52:43.230800 windmill_api-1.94.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py
+-rw-r--r--   0        0        0      269 2023-05-05 00:52:28.806539 windmill_api-1.94.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_kind.py
+-rw-r--r--   0        0        0      227 2023-05-05 00:52:29.526552 windmill_api-1.94.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_language.py
+-rw-r--r--   0        0        0     1347 2023-05-05 00:52:43.202799 windmill_api-1.94.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py
+-rw-r--r--   0        0        0      264 2023-05-05 00:52:28.602535 windmill_api-1.94.0/windmill_api/models/get_script_by_path_with_draft_response_200_kind.py
+-rw-r--r--   0        0        0      222 2023-05-05 00:52:29.510552 windmill_api-1.94.0/windmill_api/models/get_script_by_path_with_draft_response_200_language.py
+-rw-r--r--   0        0        0     1319 2023-05-05 00:52:43.226799 windmill_api-1.94.0/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py
+-rw-r--r--   0        0        0     1922 2023-05-05 00:52:43.254800 windmill_api-1.94.0/windmill_api/models/get_script_deployment_status_response_200.py
+-rw-r--r--   0        0        0     4157 2023-05-05 00:52:43.282801 windmill_api-1.94.0/windmill_api/models/get_settings_response_200.py
+-rw-r--r--   0        0        0     2428 2023-05-05 00:52:43.282801 windmill_api-1.94.0/windmill_api/models/get_suspended_job_flow_response_200.py
+-rw-r--r--   0        0        0     1764 2023-05-05 00:52:43.306801 windmill_api-1.94.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
+-rw-r--r--   0        0        0     2040 2023-05-05 00:52:43.314801 windmill_api-1.94.0/windmill_api/models/get_suspended_job_flow_response_200_job.py
+-rw-r--r--   0        0        0      204 2023-05-05 00:52:28.534534 windmill_api-1.94.0/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
+-rw-r--r--   0        0        0     4554 2023-05-05 00:52:43.370802 windmill_api-1.94.0/windmill_api/models/get_variable_response_200.py
+-rw-r--r--   0        0        0     1268 2023-05-05 00:52:43.334801 windmill_api-1.94.0/windmill_api/models/get_variable_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2647 2023-05-05 00:52:43.370802 windmill_api-1.94.0/windmill_api/models/global_user_info.py
+-rw-r--r--   0        0        0      176 2023-05-05 00:52:28.922541 windmill_api-1.94.0/windmill_api/models/global_user_info_login_type.py
+-rw-r--r--   0        0        0     1627 2023-05-05 00:52:43.442803 windmill_api-1.94.0/windmill_api/models/global_user_update_json_body.py
+-rw-r--r--   0        0        0     2741 2023-05-05 00:52:43.410803 windmill_api-1.94.0/windmill_api/models/global_whoami_response_200.py
+-rw-r--r--   0        0        0      185 2023-05-05 00:52:28.642536 windmill_api-1.94.0/windmill_api/models/global_whoami_response_200_login_type.py
+-rw-r--r--   0        0        0     2903 2023-05-05 00:52:43.450803 windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5478 2023-05-05 00:52:43.502804 windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      324 2023-05-05 00:52:28.990542 windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1598 2023-05-05 00:52:43.474804 windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1663 2023-05-05 00:52:43.498804 windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2151 2023-05-05 00:52:43.530805 windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3257 2023-05-05 00:52:43.538805 windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      342 2023-05-05 00:52:28.486533 windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1631 2023-05-05 00:52:43.554805 windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3100 2023-05-05 00:52:43.570806 windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      333 2023-05-05 00:52:28.674536 windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1580 2023-05-05 00:52:43.622807 windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-05 00:52:28.898540 windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2722 2023-05-05 00:52:43.618806 windmill_api-1.94.0/windmill_api/models/group.py
+-rw-r--r--   0        0        0     1174 2023-05-05 00:52:43.638807 windmill_api-1.94.0/windmill_api/models/group_extra_perms.py
+-rw-r--r--   0        0        0     1689 2023-05-05 00:52:43.650807 windmill_api-1.94.0/windmill_api/models/identity.py
+-rw-r--r--   0        0        0      143 2023-05-05 00:52:28.782538 windmill_api-1.94.0/windmill_api/models/identity_type.py
+-rw-r--r--   0        0        0     2377 2023-05-05 00:52:43.678808 windmill_api-1.94.0/windmill_api/models/input_.py
+-rw-r--r--   0        0        0     1138 2023-05-05 00:52:43.670807 windmill_api-1.94.0/windmill_api/models/input_args.py
+-rw-r--r--   0        0        0     1820 2023-05-05 00:52:43.698808 windmill_api-1.94.0/windmill_api/models/input_transform_type_0.py
+-rw-r--r--   0        0        0      158 2023-05-05 00:52:28.922541 windmill_api-1.94.0/windmill_api/models/input_transform_type_0_type.py
+-rw-r--r--   0        0        0     1687 2023-05-05 00:52:43.706808 windmill_api-1.94.0/windmill_api/models/input_transform_type_1.py
+-rw-r--r--   0        0        0      158 2023-05-05 00:52:29.390549 windmill_api-1.94.0/windmill_api/models/input_transform_type_1_type.py
+-rw-r--r--   0        0        0     1773 2023-05-05 00:52:43.730809 windmill_api-1.94.0/windmill_api/models/invite_user_json_body.py
+-rw-r--r--   0        0        0     1679 2023-05-05 00:52:43.730809 windmill_api-1.94.0/windmill_api/models/javascript_transform.py
+-rw-r--r--   0        0        0      158 2023-05-05 00:52:28.934541 windmill_api-1.94.0/windmill_api/models/javascript_transform_type.py
+-rw-r--r--   0        0        0     1686 2023-05-05 00:52:43.758809 windmill_api-1.94.0/windmill_api/models/job.py
+-rw-r--r--   0        0        0      174 2023-05-05 00:52:29.426550 windmill_api-1.94.0/windmill_api/models/job_type.py
+-rw-r--r--   0        0        0     3583 2023-05-05 00:52:43.778809 windmill_api-1.94.0/windmill_api/models/list_apps_response_200_item.py
+-rw-r--r--   0        0        0      219 2023-05-05 00:52:28.618535 windmill_api-1.94.0/windmill_api/models/list_apps_response_200_item_execution_mode.py
+-rw-r--r--   0        0        0     1276 2023-05-05 00:52:43.782810 windmill_api-1.94.0/windmill_api/models/list_apps_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      218 2023-05-05 00:52:29.078544 windmill_api-1.94.0/windmill_api/models/list_audit_logs_action_kind.py
+-rw-r--r--   0        0        0     3896 2023-05-05 00:52:43.874811 windmill_api-1.94.0/windmill_api/models/list_audit_logs_response_200_item.py
+-rw-r--r--   0        0        0      237 2023-05-05 00:52:29.498551 windmill_api-1.94.0/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
+-rw-r--r--   0        0        0      640 2023-05-05 00:52:29.050543 windmill_api-1.94.0/windmill_api/models/list_audit_logs_response_200_item_operation.py
+-rw-r--r--   0        0        0     1298 2023-05-05 00:52:43.806810 windmill_api-1.94.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py
+-rw-r--r--   0        0        0    11220 2023-05-05 00:52:43.934812 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item.py
+-rw-r--r--   0        0        0     1288 2023-05-05 00:52:43.894811 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_args.py
+-rw-r--r--   0        0        0     3736 2023-05-05 00:52:43.938812 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7579 2023-05-05 00:52:44.062815 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1901 2023-05-05 00:52:43.962813 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2352 2023-05-05 00:52:43.990813 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      222 2023-05-05 00:52:28.738538 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1806 2023-05-05 00:52:44.018814 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2342 2023-05-05 00:52:44.050814 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      380 2023-05-05 00:52:28.922541 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7160 2023-05-05 00:52:44.134816 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1891 2023-05-05 00:52:44.090815 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2332 2023-05-05 00:52:44.114816 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      220 2023-05-05 00:52:28.826539 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1796 2023-05-05 00:52:44.142816 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2332 2023-05-05 00:52:44.170817 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      378 2023-05-05 00:52:28.998542 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2152 2023-05-05 00:52:44.174817 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      330 2023-05-05 00:52:29.390549 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      219 2023-05-05 00:52:28.994542 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_language.py
+-rw-r--r--   0        0        0     3485 2023-05-05 00:52:44.214817 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7593 2023-05-05 00:52:44.302819 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3498 2023-05-05 00:52:44.254818 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2041 2023-05-05 00:52:44.282819 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2345 2023-05-05 00:52:44.310819 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2295 2023-05-05 00:52:44.330819 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      201 2023-05-05 00:52:28.446532 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2162 2023-05-05 00:52:44.338820 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      201 2023-05-05 00:52:29.122545 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2034 2023-05-05 00:52:44.362820 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2085 2023-05-05 00:52:44.406821 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7471 2023-05-05 00:52:44.438821 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3464 2023-05-05 00:52:44.442821 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2031 2023-05-05 00:52:44.470822 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2335 2023-05-05 00:52:44.478822 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2275 2023-05-05 00:52:44.498823 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      199 2023-05-05 00:52:28.470533 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2142 2023-05-05 00:52:44.506823 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      199 2023-05-05 00:52:28.790538 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2024 2023-05-05 00:52:44.526823 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2075 2023-05-05 00:52:44.534823 windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1865 2023-05-05 00:52:44.550824 windmill_api-1.94.0/windmill_api/models/list_contextual_variables_response_200_item.py
+-rw-r--r--   0        0        0     1863 2023-05-05 00:52:44.562824 windmill_api-1.94.0/windmill_api/models/list_flows_response_200_item.py
+-rw-r--r--   0        0        0     2074 2023-05-05 00:52:44.578824 windmill_api-1.94.0/windmill_api/models/list_folders_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-05-05 00:52:44.582824 windmill_api-1.94.0/windmill_api/models/list_folders_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2958 2023-05-05 00:52:44.678826 windmill_api-1.94.0/windmill_api/models/list_groups_response_200_item.py
+-rw-r--r--   0        0        0     1286 2023-05-05 00:52:44.598824 windmill_api-1.94.0/windmill_api/models/list_groups_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2076 2023-05-05 00:52:44.630825 windmill_api-1.94.0/windmill_api/models/list_hub_apps_response_200.py
+-rw-r--r--   0        0        0     2304 2023-05-05 00:52:44.666826 windmill_api-1.94.0/windmill_api/models/list_hub_apps_response_200_apps_item.py
+-rw-r--r--   0        0        0     2116 2023-05-05 00:52:44.698826 windmill_api-1.94.0/windmill_api/models/list_hub_flows_response_200.py
+-rw-r--r--   0        0        0     2324 2023-05-05 00:52:44.710826 windmill_api-1.94.0/windmill_api/models/list_hub_flows_response_200_flows_item.py
+-rw-r--r--   0        0        0     2106 2023-05-05 00:52:44.730827 windmill_api-1.94.0/windmill_api/models/list_hub_scripts_response_200.py
+-rw-r--r--   0        0        0     2790 2023-05-05 00:52:44.750827 windmill_api-1.94.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py
+-rw-r--r--   0        0        0      262 2023-05-05 00:52:29.178546 windmill_api-1.94.0/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
+-rw-r--r--   0        0        0     2590 2023-05-05 00:52:44.806828 windmill_api-1.94.0/windmill_api/models/list_inputs_response_200_item.py
+-rw-r--r--   0        0        0     1250 2023-05-05 00:52:44.766827 windmill_api-1.94.0/windmill_api/models/list_inputs_response_200_item_args.py
+-rw-r--r--   0        0        0      213 2023-05-05 00:52:29.026543 windmill_api-1.94.0/windmill_api/models/list_inputs_runnable_type.py
+-rw-r--r--   0        0        0     1922 2023-05-05 00:52:44.798828 windmill_api-1.94.0/windmill_api/models/list_jobs_response_200_item.py
+-rw-r--r--   0        0        0      194 2023-05-05 00:52:28.450532 windmill_api-1.94.0/windmill_api/models/list_jobs_response_200_item_type.py
+-rw-r--r--   0        0        0     2076 2023-05-05 00:52:44.830829 windmill_api-1.94.0/windmill_api/models/list_pending_invites_response_200_item.py
+-rw-r--r--   0        0        0    12114 2023-05-05 00:52:44.954831 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item.py
+-rw-r--r--   0        0        0     1245 2023-05-05 00:52:44.850829 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_args.py
+-rw-r--r--   0        0        0     3544 2023-05-05 00:52:44.890830 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7247 2023-05-05 00:52:44.974831 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1858 2023-05-05 00:52:44.978831 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-05-05 00:52:45.058833 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-05-05 00:52:29.562553 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-05-05 00:52:45.002832 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2299 2023-05-05 00:52:45.034832 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      372 2023-05-05 00:52:29.134545 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6858 2023-05-05 00:52:45.118834 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1848 2023-05-05 00:52:45.086833 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2248 2023-05-05 00:52:45.114834 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      212 2023-05-05 00:52:29.374549 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1753 2023-05-05 00:52:45.142834 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2289 2023-05-05 00:52:45.206835 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      370 2023-05-05 00:52:28.878540 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2109 2023-05-05 00:52:45.174835 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      322 2023-05-05 00:52:29.570553 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      211 2023-05-05 00:52:29.022543 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_language.py
+-rw-r--r--   0        0        0     3334 2023-05-05 00:52:45.218835 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7235 2023-05-05 00:52:45.290837 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3357 2023-05-05 00:52:45.258836 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1998 2023-05-05 00:52:45.286837 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-05-05 00:52:45.318837 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-05-05 00:52:45.318837 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-05 00:52:29.230547 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-05-05 00:52:45.342838 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-05 00:52:28.870540 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-05-05 00:52:45.346838 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-05-05 00:52:45.370838 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7159 2023-05-05 00:52:45.426839 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3323 2023-05-05 00:52:45.410839 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1988 2023-05-05 00:52:45.438840 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-05-05 00:52:45.458840 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-05-05 00:52:45.466840 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-05-05 00:52:29.022543 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-05-05 00:52:45.486840 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-05-05 00:52:28.754538 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-05-05 00:52:45.494840 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-05-05 00:52:45.514841 windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     4884 2023-05-05 00:52:45.610843 windmill_api-1.94.0/windmill_api/models/list_resource_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-05-05 00:52:45.578842 windmill_api-1.94.0/windmill_api/models/list_resource_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2363 2023-05-05 00:52:45.614843 windmill_api-1.94.0/windmill_api/models/list_resource_type_response_200_item.py
+-rw-r--r--   0        0        0     4426 2023-05-05 00:52:45.666844 windmill_api-1.94.0/windmill_api/models/list_schedules_response_200_item.py
+-rw-r--r--   0        0        0     1265 2023-05-05 00:52:45.634843 windmill_api-1.94.0/windmill_api/models/list_schedules_response_200_item_args.py
+-rw-r--r--   0        0        0     1301 2023-05-05 00:52:45.650843 windmill_api-1.94.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     7551 2023-05-05 00:52:45.742845 windmill_api-1.94.0/windmill_api/models/list_scripts_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-05-05 00:52:45.686844 windmill_api-1.94.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-05 00:52:29.314548 windmill_api-1.94.0/windmill_api/models/list_scripts_response_200_item_kind.py
+-rw-r--r--   0        0        0      213 2023-05-05 00:52:29.310548 windmill_api-1.94.0/windmill_api/models/list_scripts_response_200_item_language.py
+-rw-r--r--   0        0        0     1265 2023-05-05 00:52:45.710844 windmill_api-1.94.0/windmill_api/models/list_scripts_response_200_item_schema.py
+-rw-r--r--   0        0        0     2985 2023-05-05 00:52:45.750845 windmill_api-1.94.0/windmill_api/models/list_tokens_response_200_item.py
+-rw-r--r--   0        0        0     2250 2023-05-05 00:52:45.770846 windmill_api-1.94.0/windmill_api/models/list_user_workspaces_response_200.py
+-rw-r--r--   0        0        0     1833 2023-05-05 00:52:45.774846 windmill_api-1.94.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
+-rw-r--r--   0        0        0     2896 2023-05-05 00:52:45.810846 windmill_api-1.94.0/windmill_api/models/list_users_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0      198 2023-05-05 00:52:29.334548 windmill_api-1.94.0/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
+-rw-r--r--   0        0        0     4307 2023-05-05 00:52:45.834847 windmill_api-1.94.0/windmill_api/models/list_users_response_200_item.py
+-rw-r--r--   0        0        0     1613 2023-05-05 00:52:45.834847 windmill_api-1.94.0/windmill_api/models/list_users_response_200_item_usage.py
+-rw-r--r--   0        0        0     4608 2023-05-05 00:52:45.894848 windmill_api-1.94.0/windmill_api/models/list_variable_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-05-05 00:52:45.854847 windmill_api-1.94.0/windmill_api/models/list_variable_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2693 2023-05-05 00:52:45.890848 windmill_api-1.94.0/windmill_api/models/list_workers_response_200_item.py
+-rw-r--r--   0        0        0     2086 2023-05-05 00:52:45.918848 windmill_api-1.94.0/windmill_api/models/list_workspace_invites_response_200_item.py
+-rw-r--r--   0        0        0     2082 2023-05-05 00:52:45.974849 windmill_api-1.94.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0     2013 2023-05-05 00:52:45.950849 windmill_api-1.94.0/windmill_api/models/list_workspaces_response_200_item.py
+-rw-r--r--   0        0        0     3388 2023-05-05 00:52:45.994850 windmill_api-1.94.0/windmill_api/models/listable_app.py
+-rw-r--r--   0        0        0      207 2023-05-05 00:52:29.118544 windmill_api-1.94.0/windmill_api/models/listable_app_execution_mode.py
+-rw-r--r--   0        0        0     1207 2023-05-05 00:52:45.998850 windmill_api-1.94.0/windmill_api/models/listable_app_extra_perms.py
+-rw-r--r--   0        0        0     4751 2023-05-05 00:52:46.058851 windmill_api-1.94.0/windmill_api/models/listable_resource.py
+-rw-r--r--   0        0        0     1232 2023-05-05 00:52:46.014850 windmill_api-1.94.0/windmill_api/models/listable_resource_extra_perms.py
+-rw-r--r--   0        0        0     4486 2023-05-05 00:52:46.074851 windmill_api-1.94.0/windmill_api/models/listable_variable.py
+-rw-r--r--   0        0        0     1232 2023-05-05 00:52:46.130852 windmill_api-1.94.0/windmill_api/models/listable_variable_extra_perms.py
+-rw-r--r--   0        0        0     1513 2023-05-05 00:52:46.098852 windmill_api-1.94.0/windmill_api/models/login.py
+-rw-r--r--   0        0        0     1559 2023-05-05 00:52:46.126852 windmill_api-1.94.0/windmill_api/models/login_json_body.py
+-rw-r--r--   0        0        0     1739 2023-05-05 00:52:46.154852 windmill_api-1.94.0/windmill_api/models/login_with_oauth_json_body.py
+-rw-r--r--   0        0        0     2758 2023-05-05 00:52:46.166853 windmill_api-1.94.0/windmill_api/models/main_arg_signature.py
+-rw-r--r--   0        0        0     5099 2023-05-05 00:52:46.210854 windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item.py
+-rw-r--r--   0        0        0      315 2023-05-05 00:52:29.138545 windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1547 2023-05-05 00:52:46.194853 windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1612 2023-05-05 00:52:46.218854 windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2044 2023-05-05 00:52:46.238854 windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3049 2023-05-05 00:52:46.254854 windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      333 2023-05-05 00:52:28.582535 windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1580 2023-05-05 00:52:46.262854 windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     2862 2023-05-05 00:52:46.290855 windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      324 2023-05-05 00:52:28.622536 windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1529 2023-05-05 00:52:46.286855 windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-05 00:52:28.582535 windmill_api-1.94.0/windmill_api/models/main_arg_signature_type.py
+-rw-r--r--   0        0        0     2662 2023-05-05 00:52:46.370856 windmill_api-1.94.0/windmill_api/models/new_schedule.py
+-rw-r--r--   0        0        0     1171 2023-05-05 00:52:46.310855 windmill_api-1.94.0/windmill_api/models/new_schedule_args.py
+-rw-r--r--   0        0        0     4866 2023-05-05 00:52:46.378857 windmill_api-1.94.0/windmill_api/models/new_script.py
+-rw-r--r--   0        0        0      238 2023-05-05 00:52:29.182546 windmill_api-1.94.0/windmill_api/models/new_script_kind.py
+-rw-r--r--   0        0        0      196 2023-05-05 00:52:29.342548 windmill_api-1.94.0/windmill_api/models/new_script_language.py
+-rw-r--r--   0        0        0     1171 2023-05-05 00:52:46.394857 windmill_api-1.94.0/windmill_api/models/new_script_schema.py
+-rw-r--r--   0        0        0     5879 2023-05-05 00:52:46.458858 windmill_api-1.94.0/windmill_api/models/new_script_with_draft.py
+-rw-r--r--   0        0        0     5192 2023-05-05 00:52:46.462858 windmill_api-1.94.0/windmill_api/models/new_script_with_draft_draft.py
+-rw-r--r--   0        0        0      252 2023-05-05 00:52:28.794539 windmill_api-1.94.0/windmill_api/models/new_script_with_draft_draft_kind.py
+-rw-r--r--   0        0        0      210 2023-05-05 00:52:28.870540 windmill_api-1.94.0/windmill_api/models/new_script_with_draft_draft_language.py
+-rw-r--r--   0        0        0     1250 2023-05-05 00:52:46.486858 windmill_api-1.94.0/windmill_api/models/new_script_with_draft_draft_schema.py
+-rw-r--r--   0        0        0      247 2023-05-05 00:52:28.506533 windmill_api-1.94.0/windmill_api/models/new_script_with_draft_kind.py
+-rw-r--r--   0        0        0      205 2023-05-05 00:52:28.866540 windmill_api-1.94.0/windmill_api/models/new_script_with_draft_language.py
+-rw-r--r--   0        0        0     1222 2023-05-05 00:52:46.510859 windmill_api-1.94.0/windmill_api/models/new_script_with_draft_schema.py
+-rw-r--r--   0        0        0     2108 2023-05-05 00:52:46.542860 windmill_api-1.94.0/windmill_api/models/new_token.py
+-rw-r--r--   0        0        0     2473 2023-05-05 00:52:46.554860 windmill_api-1.94.0/windmill_api/models/new_token_impersonate.py
+-rw-r--r--   0        0        0     1710 2023-05-05 00:52:46.566860 windmill_api-1.94.0/windmill_api/models/new_user.py
+-rw-r--r--   0        0        0     2584 2023-05-05 00:52:46.590860 windmill_api-1.94.0/windmill_api/models/open_flow.py
+-rw-r--r--   0        0        0     1166 2023-05-05 00:52:46.586861 windmill_api-1.94.0/windmill_api/models/open_flow_schema.py
+-rw-r--r--   0        0        0     3026 2023-05-05 00:52:46.626861 windmill_api-1.94.0/windmill_api/models/open_flow_value.py
+-rw-r--r--   0        0        0     6384 2023-05-05 00:52:46.670862 windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3013 2023-05-05 00:52:46.666862 windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1896 2023-05-05 00:52:46.694862 windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2200 2023-05-05 00:52:46.698862 windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2006 2023-05-05 00:52:46.722863 windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      175 2023-05-05 00:52:28.770538 windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1873 2023-05-05 00:52:46.726863 windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      175 2023-05-05 00:52:29.410550 windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1889 2023-05-05 00:52:46.798864 windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1940 2023-05-05 00:52:46.754863 windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6308 2023-05-05 00:52:46.834865 windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item.py
+-rw-r--r--   0        0        0     2979 2023-05-05 00:52:46.834865 windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1886 2023-05-05 00:52:46.922866 windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2190 2023-05-05 00:52:46.866865 windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1986 2023-05-05 00:52:46.894866 windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      173 2023-05-05 00:52:29.202546 windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1853 2023-05-05 00:52:46.918866 windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      173 2023-05-05 00:52:28.602535 windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1879 2023-05-05 00:52:46.946867 windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1930 2023-05-05 00:52:46.950867 windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2816 2023-05-05 00:52:46.986868 windmill_api-1.94.0/windmill_api/models/open_flow_w_path.py
+-rw-r--r--   0        0        0     1197 2023-05-05 00:52:46.970867 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_schema.py
+-rw-r--r--   0        0        0     3116 2023-05-05 00:52:47.010868 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value.py
+-rw-r--r--   0        0        0     6590 2023-05-05 00:52:47.062869 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module.py
+-rw-r--r--   0        0        0     3117 2023-05-05 00:52:47.050869 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1927 2023-05-05 00:52:47.082869 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2231 2023-05-05 00:52:47.094870 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2073 2023-05-05 00:52:47.110870 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      180 2023-05-05 00:52:28.694537 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1940 2023-05-05 00:52:47.126870 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-05 00:52:28.658536 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1920 2023-05-05 00:52:47.134870 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1971 2023-05-05 00:52:47.154871 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6514 2023-05-05 00:52:47.254872 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item.py
+-rw-r--r--   0        0        0     3074 2023-05-05 00:52:47.190871 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1917 2023-05-05 00:52:47.218872 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2221 2023-05-05 00:52:47.250872 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2044 2023-05-05 00:52:47.278873 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-05 00:52:29.082544 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1911 2023-05-05 00:52:47.282873 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-05 00:52:29.518552 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1910 2023-05-05 00:52:47.306873 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1961 2023-05-05 00:52:47.310874 windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1989 2023-05-05 00:52:47.334874 windmill_api-1.94.0/windmill_api/models/path_flow.py
+-rw-r--r--   0        0        0     3089 2023-05-05 00:52:47.342874 windmill_api-1.94.0/windmill_api/models/path_flow_input_transforms.py
+-rw-r--r--   0        0        0     2115 2023-05-05 00:52:47.418876 windmill_api-1.94.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      185 2023-05-05 00:52:28.730538 windmill_api-1.94.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1982 2023-05-05 00:52:47.370875 windmill_api-1.94.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      185 2023-05-05 00:52:28.578535 windmill_api-1.94.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      135 2023-05-05 00:52:28.782538 windmill_api-1.94.0/windmill_api/models/path_flow_type.py
+-rw-r--r--   0        0        0     2292 2023-05-05 00:52:47.406875 windmill_api-1.94.0/windmill_api/models/path_script.py
+-rw-r--r--   0        0        0     3181 2023-05-05 00:52:47.442876 windmill_api-1.94.0/windmill_api/models/path_script_input_transforms.py
+-rw-r--r--   0        0        0     2135 2023-05-05 00:52:47.446876 windmill_api-1.94.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      187 2023-05-05 00:52:29.438550 windmill_api-1.94.0/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2002 2023-05-05 00:52:47.470877 windmill_api-1.94.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      187 2023-05-05 00:52:29.034543 windmill_api-1.94.0/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      141 2023-05-05 00:52:29.062543 windmill_api-1.94.0/windmill_api/models/path_script_type.py
+-rw-r--r--   0        0        0     3390 2023-05-05 00:52:47.494877 windmill_api-1.94.0/windmill_api/models/policy.py
+-rw-r--r--   0        0        0      202 2023-05-05 00:52:29.530552 windmill_api-1.94.0/windmill_api/models/policy_execution_mode.py
+-rw-r--r--   0        0        0     1709 2023-05-05 00:52:47.494877 windmill_api-1.94.0/windmill_api/models/policy_triggerables.py
+-rw-r--r--   0        0        0     1279 2023-05-05 00:52:47.510877 windmill_api-1.94.0/windmill_api/models/policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2359 2023-05-05 00:52:47.530877 windmill_api-1.94.0/windmill_api/models/preview.py
+-rw-r--r--   0        0        0     1148 2023-05-05 00:52:47.530877 windmill_api-1.94.0/windmill_api/models/preview_args.py
+-rw-r--r--   0        0        0      194 2023-05-05 00:52:29.362549 windmill_api-1.94.0/windmill_api/models/preview_language.py
+-rw-r--r--   0        0        0     1642 2023-05-05 00:52:47.558878 windmill_api-1.94.0/windmill_api/models/preview_schedule_json_body.py
+-rw-r--r--   0        0        0     2963 2023-05-05 00:52:47.574878 windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5679 2023-05-05 00:52:47.614879 windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      328 2023-05-05 00:52:28.586535 windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1618 2023-05-05 00:52:47.598879 windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1683 2023-05-05 00:52:47.674880 windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2191 2023-05-05 00:52:47.642880 windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3329 2023-05-05 00:52:47.678880 windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      346 2023-05-05 00:52:29.282547 windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1651 2023-05-05 00:52:47.698881 windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3214 2023-05-05 00:52:47.710881 windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      337 2023-05-05 00:52:28.466533 windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1600 2023-05-05 00:52:47.722881 windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      182 2023-05-05 00:52:29.458551 windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0    11580 2023-05-05 00:52:47.922885 windmill_api-1.94.0/windmill_api/models/queued_job.py
+-rw-r--r--   0        0        0     1161 2023-05-05 00:52:47.742881 windmill_api-1.94.0/windmill_api/models/queued_job_args.py
+-rw-r--r--   0        0        0     3202 2023-05-05 00:52:47.786882 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status.py
+-rw-r--r--   0        0        0     6683 2023-05-05 00:52:47.866884 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1774 2023-05-05 00:52:47.890884 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2106 2023-05-05 00:52:47.918885 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      199 2023-05-05 00:52:29.062543 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1679 2023-05-05 00:52:47.942885 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2215 2023-05-05 00:52:47.958885 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      357 2023-05-05 00:52:29.082544 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6294 2023-05-05 00:52:48.074887 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1764 2023-05-05 00:52:47.982886 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2086 2023-05-05 00:52:48.010886 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      197 2023-05-05 00:52:28.670536 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1669 2023-05-05 00:52:48.034887 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2205 2023-05-05 00:52:48.070887 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      355 2023-05-05 00:52:28.458532 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2025 2023-05-05 00:52:48.102888 windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_retry.py
+-rw-r--r--   0        0        0      307 2023-05-05 00:52:29.342548 windmill_api-1.94.0/windmill_api/models/queued_job_job_kind.py
+-rw-r--r--   0        0        0      196 2023-05-05 00:52:28.806539 windmill_api-1.94.0/windmill_api/models/queued_job_language.py
+-rw-r--r--   0        0        0     3079 2023-05-05 00:52:48.118888 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow.py
+-rw-r--r--   0        0        0     6506 2023-05-05 00:52:48.250891 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3069 2023-05-05 00:52:48.154889 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1914 2023-05-05 00:52:48.182889 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2218 2023-05-05 00:52:48.214890 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2040 2023-05-05 00:52:48.242890 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-05 00:52:29.190546 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1907 2023-05-05 00:52:48.270891 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-05 00:52:29.122545 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1907 2023-05-05 00:52:48.278891 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1958 2023-05-05 00:52:48.298891 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6430 2023-05-05 00:52:48.354893 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3035 2023-05-05 00:52:48.334892 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1904 2023-05-05 00:52:48.362893 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2208 2023-05-05 00:52:48.386893 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2020 2023-05-05 00:52:48.390893 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-05-05 00:52:29.334548 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1887 2023-05-05 00:52:48.418894 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-05-05 00:52:29.010542 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1897 2023-05-05 00:52:48.418894 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1948 2023-05-05 00:52:48.446894 windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     3028 2023-05-05 00:52:48.462895 windmill_api-1.94.0/windmill_api/models/raw_script.py
+-rw-r--r--   0        0        0     3139 2023-05-05 00:52:48.478895 windmill_api-1.94.0/windmill_api/models/raw_script_input_transforms.py
+-rw-r--r--   0        0        0     2125 2023-05-05 00:52:48.490895 windmill_api-1.94.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      186 2023-05-05 00:52:29.030543 windmill_api-1.94.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1992 2023-05-05 00:52:48.510895 windmill_api-1.94.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      186 2023-05-05 00:52:28.970542 windmill_api-1.94.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      196 2023-05-05 00:52:29.454551 windmill_api-1.94.0/windmill_api/models/raw_script_language.py
+-rw-r--r--   0        0        0      146 2023-05-05 00:52:28.478533 windmill_api-1.94.0/windmill_api/models/raw_script_type.py
+-rw-r--r--   0        0        0     1405 2023-05-05 00:52:48.514895 windmill_api-1.94.0/windmill_api/models/refresh_token_json_body.py
+-rw-r--r--   0        0        0     1448 2023-05-05 00:52:48.530896 windmill_api-1.94.0/windmill_api/models/remove_granular_acls_json_body.py
+-rw-r--r--   0        0        0      304 2023-05-05 00:52:28.846540 windmill_api-1.94.0/windmill_api/models/remove_granular_acls_kind.py
+-rw-r--r--   0        0        0     1544 2023-05-05 00:52:48.538896 windmill_api-1.94.0/windmill_api/models/remove_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1567 2023-05-05 00:52:48.554896 windmill_api-1.94.0/windmill_api/models/remove_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3367 2023-05-05 00:52:48.586897 windmill_api-1.94.0/windmill_api/models/resource.py
+-rw-r--r--   0        0        0     1189 2023-05-05 00:52:48.574896 windmill_api-1.94.0/windmill_api/models/resource_extra_perms.py
+-rw-r--r--   0        0        0     2256 2023-05-05 00:52:48.606897 windmill_api-1.94.0/windmill_api/models/resource_type.py
+-rw-r--r--   0        0        0     1278 2023-05-05 00:52:48.606897 windmill_api-1.94.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
+-rw-r--r--   0        0        0     1255 2023-05-05 00:52:48.626897 windmill_api-1.94.0/windmill_api/models/resume_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0     2546 2023-05-05 00:52:48.646898 windmill_api-1.94.0/windmill_api/models/retry.py
+-rw-r--r--   0        0        0     1751 2023-05-05 00:52:48.702899 windmill_api-1.94.0/windmill_api/models/retry_constant.py
+-rw-r--r--   0        0        0     2055 2023-05-05 00:52:48.678898 windmill_api-1.94.0/windmill_api/models/retry_exponential.py
+-rw-r--r--   0        0        0     1210 2023-05-05 00:52:48.770900 windmill_api-1.94.0/windmill_api/models/run_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     2189 2023-05-05 00:52:48.730899 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body.py
+-rw-r--r--   0        0        0     1235 2023-05-05 00:52:48.750900 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_args.py
+-rw-r--r--   0        0        0     3265 2023-05-05 00:52:48.794901 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value.py
+-rw-r--r--   0        0        0     7049 2023-05-05 00:52:48.854902 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3284 2023-05-05 00:52:48.830901 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1975 2023-05-05 00:52:48.858902 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2279 2023-05-05 00:52:48.886902 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2167 2023-05-05 00:52:48.886902 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-05-05 00:52:28.626536 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2034 2023-05-05 00:52:48.910903 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-05-05 00:52:28.570535 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1968 2023-05-05 00:52:48.914903 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2019 2023-05-05 00:52:48.938903 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6939 2023-05-05 00:52:48.994904 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3250 2023-05-05 00:52:48.978904 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1965 2023-05-05 00:52:49.006904 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2269 2023-05-05 00:52:49.078906 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2147 2023-05-05 00:52:49.030905 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      187 2023-05-05 00:52:29.394549 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2014 2023-05-05 00:52:49.058905 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      187 2023-05-05 00:52:29.222546 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1958 2023-05-05 00:52:49.086906 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2009 2023-05-05 00:52:49.110906 windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1220 2023-05-05 00:52:49.110906 windmill_api-1.94.0/windmill_api/models/run_script_by_hash_json_body.py
+-rw-r--r--   0        0        0     1220 2023-05-05 00:52:49.126906 windmill_api-1.94.0/windmill_api/models/run_script_by_path_json_body.py
+-rw-r--r--   0        0        0     2634 2023-05-05 00:52:49.146907 windmill_api-1.94.0/windmill_api/models/run_script_preview_json_body.py
+-rw-r--r--   0        0        0     1245 2023-05-05 00:52:49.146907 windmill_api-1.94.0/windmill_api/models/run_script_preview_json_body_args.py
+-rw-r--r--   0        0        0      211 2023-05-05 00:52:29.310548 windmill_api-1.94.0/windmill_api/models/run_script_preview_json_body_language.py
+-rw-r--r--   0        0        0     1266 2023-05-05 00:52:49.166907 windmill_api-1.94.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     1276 2023-05-05 00:52:49.166907 windmill_api-1.94.0/windmill_api/models/run_wait_result_script_by_path_json_body.py
+-rw-r--r--   0        0        0      203 2023-05-05 00:52:29.266547 windmill_api-1.94.0/windmill_api/models/runnable_type.py
+-rw-r--r--   0        0        0     4086 2023-05-05 00:52:49.222908 windmill_api-1.94.0/windmill_api/models/schedule.py
+-rw-r--r--   0        0        0     1153 2023-05-05 00:52:49.186908 windmill_api-1.94.0/windmill_api/models/schedule_args.py
+-rw-r--r--   0        0        0     1189 2023-05-05 00:52:49.206908 windmill_api-1.94.0/windmill_api/models/schedule_extra_perms.py
+-rw-r--r--   0        0        0     7003 2023-05-05 00:52:49.370911 windmill_api-1.94.0/windmill_api/models/script.py
+-rw-r--r--   0        0        0     1143 2023-05-05 00:52:49.242909 windmill_api-1.94.0/windmill_api/models/script_args.py
+-rw-r--r--   0        0        0     1179 2023-05-05 00:52:49.262909 windmill_api-1.94.0/windmill_api/models/script_extra_perms.py
+-rw-r--r--   0        0        0      235 2023-05-05 00:52:29.190546 windmill_api-1.94.0/windmill_api/models/script_kind.py
+-rw-r--r--   0        0        0      193 2023-05-05 00:52:29.402550 windmill_api-1.94.0/windmill_api/models/script_language.py
+-rw-r--r--   0        0        0     1153 2023-05-05 00:52:49.282909 windmill_api-1.94.0/windmill_api/models/script_schema.py
+-rw-r--r--   0        0        0     1440 2023-05-05 00:52:49.306910 windmill_api-1.94.0/windmill_api/models/set_password_json_body.py
+-rw-r--r--   0        0        0     1470 2023-05-05 00:52:49.326910 windmill_api-1.94.0/windmill_api/models/set_schedule_enabled_json_body.py
+-rw-r--r--   0        0        0     2032 2023-05-05 00:52:49.358911 windmill_api-1.94.0/windmill_api/models/slack_token.py
+-rw-r--r--   0        0        0     1586 2023-05-05 00:52:49.382911 windmill_api-1.94.0/windmill_api/models/slack_token_bot.py
+-rw-r--r--   0        0        0     2227 2023-05-05 00:52:49.402912 windmill_api-1.94.0/windmill_api/models/star_json_body.py
+-rw-r--r--   0        0        0      185 2023-05-05 00:52:29.326548 windmill_api-1.94.0/windmill_api/models/star_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     1772 2023-05-05 00:52:49.410912 windmill_api-1.94.0/windmill_api/models/static_transform.py
+-rw-r--r--   0        0        0      154 2023-05-05 00:52:29.098544 windmill_api-1.94.0/windmill_api/models/static_transform_type.py
+-rw-r--r--   0        0        0     2462 2023-05-05 00:52:49.442912 windmill_api-1.94.0/windmill_api/models/token_response.py
+-rw-r--r--   0        0        0     2921 2023-05-05 00:52:49.450912 windmill_api-1.94.0/windmill_api/models/truncated_token.py
+-rw-r--r--   0        0        0     2249 2023-05-05 00:52:49.474913 windmill_api-1.94.0/windmill_api/models/unstar_json_body.py
+-rw-r--r--   0        0        0      187 2023-05-05 00:52:29.282547 windmill_api-1.94.0/windmill_api/models/unstar_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     2638 2023-05-05 00:52:49.490913 windmill_api-1.94.0/windmill_api/models/update_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-05-05 00:52:49.518914 windmill_api-1.94.0/windmill_api/models/update_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-05-05 00:52:28.926541 windmill_api-1.94.0/windmill_api/models/update_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-05-05 00:52:49.518914 windmill_api-1.94.0/windmill_api/models/update_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-05-05 00:52:49.534914 windmill_api-1.94.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2896 2023-05-05 00:52:49.562914 windmill_api-1.94.0/windmill_api/models/update_flow_json_body.py
+-rw-r--r--   0        0        0     1222 2023-05-05 00:52:49.554914 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_schema.py
+-rw-r--r--   0        0        0     3196 2023-05-05 00:52:49.646916 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value.py
+-rw-r--r--   0        0        0     6855 2023-05-05 00:52:49.638916 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3211 2023-05-05 00:52:49.678917 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1952 2023-05-05 00:52:49.674916 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2256 2023-05-05 00:52:49.702917 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2123 2023-05-05 00:52:49.706917 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      185 2023-05-05 00:52:29.294548 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1990 2023-05-05 00:52:49.730918 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      185 2023-05-05 00:52:29.442550 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1945 2023-05-05 00:52:49.734917 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1996 2023-05-05 00:52:49.758918 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6739 2023-05-05 00:52:49.814919 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3177 2023-05-05 00:52:49.794919 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1942 2023-05-05 00:52:49.822919 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2246 2023-05-05 00:52:49.922921 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2103 2023-05-05 00:52:49.850920 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      183 2023-05-05 00:52:29.006542 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1970 2023-05-05 00:52:49.878920 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      183 2023-05-05 00:52:29.194546 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1935 2023-05-05 00:52:49.906921 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1986 2023-05-05 00:52:49.934921 windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1949 2023-05-05 00:52:49.954922 windmill_api-1.94.0/windmill_api/models/update_folder_json_body.py
+-rw-r--r--   0        0        0     1520 2023-05-05 00:52:49.958922 windmill_api-1.94.0/windmill_api/models/update_group_json_body.py
+-rw-r--r--   0        0        0     1670 2023-05-05 00:52:49.982922 windmill_api-1.94.0/windmill_api/models/update_input.py
+-rw-r--r--   0        0        0     1716 2023-05-05 00:52:49.982922 windmill_api-1.94.0/windmill_api/models/update_input_json_body.py
+-rw-r--r--   0        0        0     2036 2023-05-05 00:52:50.014923 windmill_api-1.94.0/windmill_api/models/update_resource_json_body.py
+-rw-r--r--   0        0        0     1847 2023-05-05 00:52:50.010923 windmill_api-1.94.0/windmill_api/models/update_resource_type_json_body.py
+-rw-r--r--   0        0        0     1541 2023-05-05 00:52:50.034923 windmill_api-1.94.0/windmill_api/models/update_resource_value_json_body.py
+-rw-r--r--   0        0        0     1953 2023-05-05 00:52:50.042923 windmill_api-1.94.0/windmill_api/models/update_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-05 00:52:50.054923 windmill_api-1.94.0/windmill_api/models/update_schedule_json_body_args.py
+-rw-r--r--   0        0        0     2066 2023-05-05 00:52:50.074924 windmill_api-1.94.0/windmill_api/models/update_user_json_body.py
+-rw-r--r--   0        0        0     2316 2023-05-05 00:52:50.130925 windmill_api-1.94.0/windmill_api/models/update_variable_json_body.py
+-rw-r--r--   0        0        0     1478 2023-05-05 00:52:50.098924 windmill_api-1.94.0/windmill_api/models/usage.py
+-rw-r--r--   0        0        0     4071 2023-05-05 00:52:50.154925 windmill_api-1.94.0/windmill_api/models/user.py
+-rw-r--r--   0        0        0     1501 2023-05-05 00:52:50.150925 windmill_api-1.94.0/windmill_api/models/user_usage.py
+-rw-r--r--   0        0        0     2122 2023-05-05 00:52:50.234927 windmill_api-1.94.0/windmill_api/models/user_workspace_list.py
+-rw-r--r--   0        0        0     1767 2023-05-05 00:52:50.182926 windmill_api-1.94.0/windmill_api/models/user_workspace_list_workspaces_item.py
+-rw-r--r--   0        0        0     4222 2023-05-05 00:52:50.238927 windmill_api-1.94.0/windmill_api/models/whoami_response_200.py
+-rw-r--r--   0        0        0     1572 2023-05-05 00:52:50.258927 windmill_api-1.94.0/windmill_api/models/whoami_response_200_usage.py
+-rw-r--r--   0        0        0     4211 2023-05-05 00:52:50.294928 windmill_api-1.94.0/windmill_api/models/whois_response_200.py
+-rw-r--r--   0        0        0     1567 2023-05-05 00:52:50.282928 windmill_api-1.94.0/windmill_api/models/whois_response_200_usage.py
+-rw-r--r--   0        0        0     2604 2023-05-05 00:52:50.318928 windmill_api-1.94.0/windmill_api/models/worker_ping.py
+-rw-r--r--   0        0        0     1901 2023-05-05 00:52:50.326928 windmill_api-1.94.0/windmill_api/models/workspace.py
+-rw-r--r--   0        0        0     1974 2023-05-05 00:52:50.346929 windmill_api-1.94.0/windmill_api/models/workspace_invite.py
+-rw-r--r--   0        0        0       25 2023-05-05 00:52:19.394368 windmill_api-1.94.0/windmill_api/py.typed
+-rw-r--r--   0        0        0      939 2023-05-05 00:52:50.342929 windmill_api-1.94.0/windmill_api/types.py
+-rw-r--r--   0        0        0     4333 1970-01-01 00:00:00.000000 windmill_api-1.94.0/setup.py
+-rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.94.0/PKG-INFO
```

### Comparing `windmill_api-1.93.1/LICENSE` & `windmill_api-1.94.0/LICENSE`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/README.md` & `windmill_api-1.94.0/README.md`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/pyproject.toml` & `windmill_api-1.94.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "windmill-api"
-version = "1.93.1"
+version = "1.94.0"
 description = "A client library for accessing Windmill API"
 license = "Apache-2.0"
 
 authors = ["Ruben Fiszel <ruben@windmill.dev>"]
 
 readme = "README.md"
 packages = [
```

### Comparing `windmill_api-1.93.1/windmill_api/api/app/create_app.py` & `windmill_api-1.94.0/windmill_api/api/app/create_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/app/delete_app.py` & `windmill_api-1.94.0/windmill_api/api/app/delete_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/app/execute_component.py` & `windmill_api-1.94.0/windmill_api/api/app/execute_component.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/app/exists_app.py` & `windmill_api-1.94.0/windmill_api/api/app/exists_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/app/get_app_by_path.py` & `windmill_api-1.94.0/windmill_api/api/app/get_app_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/app/get_app_by_path_with_draft.py` & `windmill_api-1.94.0/windmill_api/api/app/get_app_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/app/get_app_by_version.py` & `windmill_api-1.94.0/windmill_api/api/app/get_app_by_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/app/get_hub_app_by_id.py` & `windmill_api-1.94.0/windmill_api/api/app/get_hub_app_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/app/get_public_app_by_secret.py` & `windmill_api-1.94.0/windmill_api/api/app/get_public_app_by_secret.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/app/get_public_secret_of_app.py` & `windmill_api-1.94.0/windmill_api/api/app/get_public_secret_of_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/app/list_apps.py` & `windmill_api-1.94.0/windmill_api/api/app/list_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/app/list_hub_apps.py` & `windmill_api-1.94.0/windmill_api/api/app/list_hub_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/app/update_app.py` & `windmill_api-1.94.0/windmill_api/api/app/update_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/audit/get_audit_log.py` & `windmill_api-1.94.0/windmill_api/api/audit/get_audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/audit/list_audit_logs.py` & `windmill_api-1.94.0/windmill_api/api/audit/list_audit_logs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/capture/create_capture.py` & `windmill_api-1.94.0/windmill_api/api/capture/create_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/capture/get_capture.py` & `windmill_api-1.94.0/windmill_api/api/capture/get_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/capture/update_capture.py` & `windmill_api-1.94.0/windmill_api/api/capture/update_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/draft/create_draft.py` & `windmill_api-1.94.0/windmill_api/api/draft/create_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/favorite/star.py` & `windmill_api-1.94.0/windmill_api/api/favorite/star.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/favorite/unstar.py` & `windmill_api-1.94.0/windmill_api/api/favorite/unstar.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/flow/archive_flow_by_path.py` & `windmill_api-1.94.0/windmill_api/api/flow/archive_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/flow/create_flow.py` & `windmill_api-1.94.0/windmill_api/api/flow/create_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/flow/delete_flow_by_path.py` & `windmill_api-1.94.0/windmill_api/api/flow/delete_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/flow/exists_flow_by_path.py` & `windmill_api-1.94.0/windmill_api/api/flow/exists_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/flow/get_flow_by_path.py` & `windmill_api-1.94.0/windmill_api/api/flow/get_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/flow/get_flow_by_path_with_draft.py` & `windmill_api-1.94.0/windmill_api/api/flow/get_flow_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/flow/get_flow_input_history_by_path.py` & `windmill_api-1.94.0/windmill_api/api/flow/get_flow_input_history_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/flow/get_hub_flow_by_id.py` & `windmill_api-1.94.0/windmill_api/api/flow/get_hub_flow_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/flow/list_flow_paths.py` & `windmill_api-1.94.0/windmill_api/api/flow/list_flow_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/flow/list_flows.py` & `windmill_api-1.94.0/windmill_api/api/flow/list_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/flow/list_hub_flows.py` & `windmill_api-1.94.0/windmill_api/api/flow/list_hub_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/flow/update_flow.py` & `windmill_api-1.94.0/windmill_api/api/flow/update_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/folder/add_owner_to_folder.py` & `windmill_api-1.94.0/windmill_api/api/folder/add_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/folder/create_folder.py` & `windmill_api-1.94.0/windmill_api/api/folder/create_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/folder/delete_folder.py` & `windmill_api-1.94.0/windmill_api/api/folder/delete_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/folder/get_folder.py` & `windmill_api-1.94.0/windmill_api/api/folder/get_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/folder/get_folder_usage.py` & `windmill_api-1.94.0/windmill_api/api/folder/get_folder_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/folder/list_folder_names.py` & `windmill_api-1.94.0/windmill_api/api/folder/list_folder_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/folder/list_folders.py` & `windmill_api-1.94.0/windmill_api/api/folder/list_folders.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/folder/remove_owner_to_folder.py` & `windmill_api-1.94.0/windmill_api/api/folder/remove_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/folder/update_folder.py` & `windmill_api-1.94.0/windmill_api/api/folder/update_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/granular_acl/add_granular_acls.py` & `windmill_api-1.94.0/windmill_api/api/granular_acl/add_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/granular_acl/get_granular_acls.py` & `windmill_api-1.94.0/windmill_api/api/granular_acl/get_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/granular_acl/remove_granular_acls.py` & `windmill_api-1.94.0/windmill_api/api/granular_acl/remove_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/group/add_user_to_group.py` & `windmill_api-1.94.0/windmill_api/api/group/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/group/create_group.py` & `windmill_api-1.94.0/windmill_api/api/group/create_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/group/delete_group.py` & `windmill_api-1.94.0/windmill_api/api/group/delete_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/group/get_group.py` & `windmill_api-1.94.0/windmill_api/api/group/get_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/group/list_group_names.py` & `windmill_api-1.94.0/windmill_api/api/group/list_group_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/group/list_groups.py` & `windmill_api-1.94.0/windmill_api/api/group/list_groups.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/group/remove_user_to_group.py` & `windmill_api-1.94.0/windmill_api/api/group/remove_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/group/update_group.py` & `windmill_api-1.94.0/windmill_api/api/group/update_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/input_/create_input.py` & `windmill_api-1.94.0/windmill_api/api/input_/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/input_/delete_input.py` & `windmill_api-1.94.0/windmill_api/api/input_/delete_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/input_/get_input_history.py` & `windmill_api-1.94.0/windmill_api/api/input_/get_input_history.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/input_/list_inputs.py` & `windmill_api-1.94.0/windmill_api/api/input_/list_inputs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/input_/update_input.py` & `windmill_api-1.94.0/windmill_api/api/input_/update_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/cancel_queued_job.py` & `windmill_api-1.94.0/windmill_api/api/job/cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/cancel_suspended_job_get.py` & `windmill_api-1.94.0/windmill_api/api/job/cancel_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/cancel_suspended_job_post.py` & `windmill_api-1.94.0/windmill_api/api/job/cancel_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/create_job_signature.py` & `windmill_api-1.94.0/windmill_api/api/job/create_job_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/delete_completed_job.py` & `windmill_api-1.94.0/windmill_api/api/job/delete_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/force_cancel_queued_job.py` & `windmill_api-1.94.0/windmill_api/api/job/force_cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/get_completed_job.py` & `windmill_api-1.94.0/windmill_api/api/job/get_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/get_completed_job_result.py` & `windmill_api-1.94.0/windmill_api/api/job/get_completed_job_result.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/get_job.py` & `windmill_api-1.94.0/windmill_api/api/job/get_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/get_job_updates.py` & `windmill_api-1.94.0/windmill_api/api/job/get_job_updates.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/get_resume_urls.py` & `windmill_api-1.94.0/windmill_api/api/job/get_resume_urls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/get_suspended_job_flow.py` & `windmill_api-1.94.0/windmill_api/api/job/get_suspended_job_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/list_completed_jobs.py` & `windmill_api-1.94.0/windmill_api/api/job/list_completed_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/list_jobs.py` & `windmill_api-1.94.0/windmill_api/api/job/list_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/list_queue.py` & `windmill_api-1.94.0/windmill_api/api/job/list_queue.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/result_by_id.py` & `windmill_api-1.94.0/windmill_api/api/job/result_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/resume_suspended_flow_as_owner.py` & `windmill_api-1.94.0/windmill_api/api/job/resume_suspended_flow_as_owner.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/resume_suspended_job_get.py` & `windmill_api-1.94.0/windmill_api/api/job/resume_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/resume_suspended_job_post.py` & `windmill_api-1.94.0/windmill_api/api/job/resume_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/run_flow_by_path.py` & `windmill_api-1.94.0/windmill_api/api/job/run_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/run_flow_preview.py` & `windmill_api-1.94.0/windmill_api/api/job/run_flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/run_script_by_hash.py` & `windmill_api-1.94.0/windmill_api/api/job/run_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/run_script_by_path.py` & `windmill_api-1.94.0/windmill_api/api/job/run_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/run_script_preview.py` & `windmill_api-1.94.0/windmill_api/api/job/run_script_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/run_wait_result_flow_by_path.py` & `windmill_api-1.94.0/windmill_api/api/job/run_wait_result_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/run_wait_result_script_by_path.py` & `windmill_api-1.94.0/windmill_api/api/job/run_wait_result_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/job/run_wait_result_script_by_path_get.py` & `windmill_api-1.94.0/windmill_api/api/job/run_wait_result_script_by_path_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/oauth/connect_callback.py` & `windmill_api-1.94.0/windmill_api/api/oauth/connect_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/oauth/connect_slack_callback.py` & `windmill_api-1.94.0/windmill_api/api/oauth/connect_slack_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/oauth/create_account.py` & `windmill_api-1.94.0/windmill_api/api/oauth/create_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/oauth/disconnect_account.py` & `windmill_api-1.94.0/windmill_api/api/oauth/disconnect_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/oauth/disconnect_slack.py` & `windmill_api-1.94.0/windmill_api/api/oauth/disconnect_slack.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/oauth/list_o_auth_connects.py` & `windmill_api-1.94.0/windmill_api/api/oauth/list_o_auth_connects.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/oauth/list_o_auth_logins.py` & `windmill_api-1.94.0/windmill_api/api/oauth/list_o_auth_logins.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/oauth/refresh_token.py` & `windmill_api-1.94.0/windmill_api/api/oauth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/resource/create_resource.py` & `windmill_api-1.94.0/windmill_api/api/resource/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/resource/create_resource_type.py` & `windmill_api-1.94.0/windmill_api/api/resource/create_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/resource/delete_resource.py` & `windmill_api-1.94.0/windmill_api/api/resource/delete_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/resource/delete_resource_type.py` & `windmill_api-1.94.0/windmill_api/api/resource/delete_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/resource/exists_resource.py` & `windmill_api-1.94.0/windmill_api/api/resource/exists_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/resource/exists_resource_type.py` & `windmill_api-1.94.0/windmill_api/api/resource/exists_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/resource/get_resource.py` & `windmill_api-1.94.0/windmill_api/api/resource/get_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/resource/get_resource_type.py` & `windmill_api-1.94.0/windmill_api/api/resource/get_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/resource/get_resource_value.py` & `windmill_api-1.94.0/windmill_api/api/resource/get_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/resource/list_resource.py` & `windmill_api-1.94.0/windmill_api/api/resource/list_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/resource/list_resource_type.py` & `windmill_api-1.94.0/windmill_api/api/resource/list_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/resource/list_resource_type_names.py` & `windmill_api-1.94.0/windmill_api/api/resource/list_resource_type_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/resource/update_resource.py` & `windmill_api-1.94.0/windmill_api/api/resource/update_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/resource/update_resource_type.py` & `windmill_api-1.94.0/windmill_api/api/resource/update_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/resource/update_resource_value.py` & `windmill_api-1.94.0/windmill_api/api/resource/update_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/schedule/create_schedule.py` & `windmill_api-1.94.0/windmill_api/api/schedule/create_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/schedule/delete_schedule.py` & `windmill_api-1.94.0/windmill_api/api/schedule/delete_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/schedule/exists_schedule.py` & `windmill_api-1.94.0/windmill_api/api/schedule/exists_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/schedule/get_schedule.py` & `windmill_api-1.94.0/windmill_api/api/schedule/get_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/schedule/list_schedules.py` & `windmill_api-1.94.0/windmill_api/api/schedule/list_schedules.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/schedule/preview_schedule.py` & `windmill_api-1.94.0/windmill_api/api/schedule/preview_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/schedule/set_schedule_enabled.py` & `windmill_api-1.94.0/windmill_api/api/schedule/set_schedule_enabled.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/schedule/update_schedule.py` & `windmill_api-1.94.0/windmill_api/api/schedule/update_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/archive_script_by_hash.py` & `windmill_api-1.94.0/windmill_api/api/script/archive_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/archive_script_by_path.py` & `windmill_api-1.94.0/windmill_api/api/script/archive_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/bash_to_jsonschema.py` & `windmill_api-1.94.0/windmill_api/api/script/bash_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/create_script.py` & `windmill_api-1.94.0/windmill_api/api/script/create_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/delete_script_by_hash.py` & `windmill_api-1.94.0/windmill_api/api/script/delete_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/delete_script_by_path.py` & `windmill_api-1.94.0/windmill_api/api/script/delete_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/deno_to_jsonschema.py` & `windmill_api-1.94.0/windmill_api/api/script/deno_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/exists_script_by_path.py` & `windmill_api-1.94.0/windmill_api/api/script/exists_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/get_hub_script_by_path.py` & `windmill_api-1.94.0/windmill_api/api/script/get_hub_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/get_hub_script_content_by_path.py` & `windmill_api-1.94.0/windmill_api/api/script/get_hub_script_content_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/get_script_by_hash.py` & `windmill_api-1.94.0/windmill_api/api/script/get_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/get_script_by_path.py` & `windmill_api-1.94.0/windmill_api/api/script/get_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/get_script_by_path_with_draft.py` & `windmill_api-1.94.0/windmill_api/api/script/get_script_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/get_script_deployment_status.py` & `windmill_api-1.94.0/windmill_api/api/script/get_script_deployment_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/go_to_jsonschema.py` & `windmill_api-1.94.0/windmill_api/api/script/go_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/list_hub_scripts.py` & `windmill_api-1.94.0/windmill_api/api/script/list_hub_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/list_script_paths.py` & `windmill_api-1.94.0/windmill_api/api/script/list_script_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/list_scripts.py` & `windmill_api-1.94.0/windmill_api/api/script/list_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/python_to_jsonschema.py` & `windmill_api-1.94.0/windmill_api/api/script/python_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/raw_script_by_hash.py` & `windmill_api-1.94.0/windmill_api/api/script/raw_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/raw_script_by_path.py` & `windmill_api-1.94.0/windmill_api/api/script/raw_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/script/raw_script_by_path_tokened.py` & `windmill_api-1.94.0/windmill_api/api/script/raw_script_by_path_tokened.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/settings/backend_version.py` & `windmill_api-1.94.0/windmill_api/api/settings/backend_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/settings/get_open_api_yaml.py` & `windmill_api-1.94.0/windmill_api/api/settings/get_open_api_yaml.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/accept_invite.py` & `windmill_api-1.94.0/windmill_api/api/user/accept_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/create_token.py` & `windmill_api-1.94.0/windmill_api/api/user/create_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/create_token_impersonate.py` & `windmill_api-1.94.0/windmill_api/api/user/create_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/create_user.py` & `windmill_api-1.94.0/windmill_api/api/user/create_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/create_user_globally.py` & `windmill_api-1.94.0/windmill_api/api/user/create_user_globally.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/decline_invite.py` & `windmill_api-1.94.0/windmill_api/api/user/decline_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/delete_token.py` & `windmill_api-1.94.0/windmill_api/api/user/delete_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/delete_user.py` & `windmill_api-1.94.0/windmill_api/api/user/delete_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/get_current_email.py` & `windmill_api-1.94.0/windmill_api/api/user/get_current_email.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/get_usage.py` & `windmill_api-1.94.0/windmill_api/api/user/get_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/global_user_delete.py` & `windmill_api-1.94.0/windmill_api/api/user/global_user_delete.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/global_user_update.py` & `windmill_api-1.94.0/windmill_api/api/user/global_user_update.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/global_whoami.py` & `windmill_api-1.94.0/windmill_api/api/user/global_whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/is_owner_of_path.py` & `windmill_api-1.94.0/windmill_api/api/user/is_owner_of_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/leave_workspace.py` & `windmill_api-1.94.0/windmill_api/api/user/leave_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/list_tokens.py` & `windmill_api-1.94.0/windmill_api/api/user/list_tokens.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/list_usernames.py` & `windmill_api-1.94.0/windmill_api/api/user/list_usernames.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/list_users.py` & `windmill_api-1.94.0/windmill_api/api/user/list_users.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/list_users_as_super_admin.py` & `windmill_api-1.94.0/windmill_api/api/user/list_users_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/list_workspace_invites.py` & `windmill_api-1.94.0/windmill_api/api/user/list_workspace_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/login.py` & `windmill_api-1.94.0/windmill_api/api/user/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/login_with_oauth.py` & `windmill_api-1.94.0/windmill_api/api/user/login_with_oauth.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/logout.py` & `windmill_api-1.94.0/windmill_api/api/user/logout.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/set_password.py` & `windmill_api-1.94.0/windmill_api/api/user/set_password.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/update_user.py` & `windmill_api-1.94.0/windmill_api/api/user/update_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/whoami.py` & `windmill_api-1.94.0/windmill_api/api/user/whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/user/whois.py` & `windmill_api-1.94.0/windmill_api/api/user/whois.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/variable/create_variable.py` & `windmill_api-1.94.0/windmill_api/api/variable/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/variable/delete_variable.py` & `windmill_api-1.94.0/windmill_api/api/variable/delete_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/variable/exists_variable.py` & `windmill_api-1.94.0/windmill_api/api/variable/exists_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/variable/get_variable.py` & `windmill_api-1.94.0/windmill_api/api/variable/get_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/variable/list_contextual_variables.py` & `windmill_api-1.94.0/windmill_api/api/variable/list_contextual_variables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/variable/list_variable.py` & `windmill_api-1.94.0/windmill_api/api/variable/list_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/variable/update_variable.py` & `windmill_api-1.94.0/windmill_api/api/variable/update_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/worker/get_custom_tags.py` & `windmill_api-1.94.0/windmill_api/api/worker/get_custom_tags.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/worker/list_workers.py` & `windmill_api-1.94.0/windmill_api/api/worker/list_workers.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/add_user.py` & `windmill_api-1.94.0/windmill_api/api/workspace/add_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/archive_workspace.py` & `windmill_api-1.94.0/windmill_api/api/workspace/archive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/create_workspace.py` & `windmill_api-1.94.0/windmill_api/api/workspace/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/delete_invite.py` & `windmill_api-1.94.0/windmill_api/api/workspace/delete_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/delete_workspace.py` & `windmill_api-1.94.0/windmill_api/api/workspace/delete_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/edit_auto_invite.py` & `windmill_api-1.94.0/windmill_api/api/workspace/edit_auto_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/edit_slack_command.py` & `windmill_api-1.94.0/windmill_api/api/workspace/edit_slack_command.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/edit_webhook.py` & `windmill_api-1.94.0/windmill_api/api/workspace/edit_webhook.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/exists_username.py` & `windmill_api-1.94.0/windmill_api/api/workspace/exists_username.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/exists_workspace.py` & `windmill_api-1.94.0/windmill_api/api/workspace/exists_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/get_premium_info.py` & `windmill_api-1.94.0/windmill_api/api/workspace/get_premium_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/get_settings.py` & `windmill_api-1.94.0/windmill_api/api/workspace/get_settings.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/invite_user.py` & `windmill_api-1.94.0/windmill_api/api/workspace/invite_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/is_domain_allowed.py` & `windmill_api-1.94.0/windmill_api/api/workspace/is_domain_allowed.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/list_pending_invites.py` & `windmill_api-1.94.0/windmill_api/api/workspace/list_pending_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/list_user_workspaces.py` & `windmill_api-1.94.0/windmill_api/api/workspace/list_user_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/list_workspaces.py` & `windmill_api-1.94.0/windmill_api/api/workspace/list_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/list_workspaces_as_super_admin.py` & `windmill_api-1.94.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/api/workspace/unarchive_workspace.py` & `windmill_api-1.94.0/windmill_api/api/workspace/unarchive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/client.py` & `windmill_api-1.94.0/windmill_api/client.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/accept_invite_json_body.py` & `windmill_api-1.94.0/windmill_api/models/accept_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/add_granular_acls_json_body.py` & `windmill_api-1.94.0/windmill_api/models/add_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/add_owner_to_folder_json_body.py` & `windmill_api-1.94.0/windmill_api/models/add_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/add_user_json_body.py` & `windmill_api-1.94.0/windmill_api/models/add_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/add_user_to_group_json_body.py` & `windmill_api-1.94.0/windmill_api/models/add_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/app_with_last_version.py` & `windmill_api-1.94.0/windmill_api/models/app_with_last_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/app_with_last_version_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/app_with_last_version_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/app_with_last_version_policy.py` & `windmill_api-1.94.0/windmill_api/models/app_with_last_version_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/app_with_last_version_policy_triggerables.py` & `windmill_api-1.94.0/windmill_api/models/app_with_last_version_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py` & `windmill_api-1.94.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/app_with_last_version_w_draft.py` & `windmill_api-1.94.0/windmill_api/models/app_with_last_version_w_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/app_with_last_version_w_draft_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/app_with_last_version_w_draft_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/app_with_last_version_w_draft_policy.py` & `windmill_api-1.94.0/windmill_api/models/app_with_last_version_w_draft_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py` & `windmill_api-1.94.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py` & `windmill_api-1.94.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/archive_flow_by_path_json_body.py` & `windmill_api-1.94.0/windmill_api/models/archive_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/archive_script_by_hash_response_200.py` & `windmill_api-1.94.0/windmill_api/models/archive_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/archive_script_by_hash_response_200_schema.py` & `windmill_api-1.94.0/windmill_api/models/archive_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/audit_log.py` & `windmill_api-1.94.0/windmill_api/models/audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/audit_log_operation.py` & `windmill_api-1.94.0/windmill_api/models/audit_log_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/audit_log_parameters.py` & `windmill_api-1.94.0/windmill_api/models/audit_log_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200.py` & `windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item.py` & `windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.94.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_all.py` & `windmill_api-1.94.0/windmill_api/models/branch_all.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_all_branches_item.py` & `windmill_api-1.94.0/windmill_api/models/branch_all_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_all_branches_item_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one.py` & `windmill_api-1.94.0/windmill_api/models/branch_one.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_branches_item.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_branches_item_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_default_item.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_default_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_default_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_default_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_default_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_default_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_default_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/branch_one_default_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/branch_one_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/cancel_queued_job_json_body.py` & `windmill_api-1.94.0/windmill_api/models/cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/cancel_suspended_job_post_json_body.py` & `windmill_api-1.94.0/windmill_api/models/cancel_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job.py` & `windmill_api-1.94.0/windmill_api/models/completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_args.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_flow_status.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_failure_module_branchall.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_failure_module_iterator.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_modules_item_branchall.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_modules_item_iterator.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_flow_status_retry.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/connect_callback_json_body.py` & `windmill_api-1.94.0/windmill_api/models/connect_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/connect_callback_response_200.py` & `windmill_api-1.94.0/windmill_api/models/connect_callback_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/connect_slack_callback_json_body.py` & `windmill_api-1.94.0/windmill_api/models/connect_slack_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/contextual_variable.py` & `windmill_api-1.94.0/windmill_api/models/contextual_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_account_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_account_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_app_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_app_json_body_policy.py` & `windmill_api-1.94.0/windmill_api/models/create_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_app_json_body_policy_triggerables.py` & `windmill_api-1.94.0/windmill_api/models/create_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.94.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_draft_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_draft_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_flow_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_folder_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_group_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_input.py` & `windmill_api-1.94.0/windmill_api/models/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_input_args.py` & `windmill_api-1.94.0/windmill_api/models/create_input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_input_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_input_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_input_json_body_args.py` & `windmill_api-1.94.0/windmill_api/models/create_input_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_resource.py` & `windmill_api-1.94.0/windmill_api/models/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_resource_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_resource_type_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_schedule_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_schedule_json_body_args.py` & `windmill_api-1.94.0/windmill_api/models/create_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_script_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_script_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_script_json_body_schema.py` & `windmill_api-1.94.0/windmill_api/models/create_script_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_token_impersonate_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_token_impersonate_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_token_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_user_globally_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_user_globally_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_user_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_variable.py` & `windmill_api-1.94.0/windmill_api/models/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_variable_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_workspace.py` & `windmill_api-1.94.0/windmill_api/models/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/create_workspace_json_body.py` & `windmill_api-1.94.0/windmill_api/models/create_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/decline_invite_json_body.py` & `windmill_api-1.94.0/windmill_api/models/decline_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_args.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_invite_json_body.py` & `windmill_api-1.94.0/windmill_api/models/delete_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_script_by_hash_response_200.py` & `windmill_api-1.94.0/windmill_api/models/delete_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/delete_script_by_hash_response_200_schema.py` & `windmill_api-1.94.0/windmill_api/models/delete_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200.py` & `windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item.py` & `windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.94.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/edit_auto_invite_json_body.py` & `windmill_api-1.94.0/windmill_api/models/edit_auto_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/edit_resource.py` & `windmill_api-1.94.0/windmill_api/models/edit_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/edit_resource_type.py` & `windmill_api-1.94.0/windmill_api/models/edit_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/edit_schedule.py` & `windmill_api-1.94.0/windmill_api/models/edit_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/edit_schedule_args.py` & `windmill_api-1.94.0/windmill_api/models/edit_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/edit_slack_command_json_body.py` & `windmill_api-1.94.0/windmill_api/models/edit_slack_command_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/edit_variable.py` & `windmill_api-1.94.0/windmill_api/models/edit_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/edit_webhook_json_body.py` & `windmill_api-1.94.0/windmill_api/models/edit_webhook_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/edit_workspace_user.py` & `windmill_api-1.94.0/windmill_api/models/edit_workspace_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/execute_component_json_body.py` & `windmill_api-1.94.0/windmill_api/models/execute_component_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py` & `windmill_api-1.94.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/execute_component_json_body_raw_code.py` & `windmill_api-1.94.0/windmill_api/models/execute_component_json_body_raw_code.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/exists_username_json_body.py` & `windmill_api-1.94.0/windmill_api/models/exists_username_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/exists_workspace_json_body.py` & `windmill_api-1.94.0/windmill_api/models/exists_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow.py` & `windmill_api-1.94.0/windmill_api/models/flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/flow_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_metadata.py` & `windmill_api-1.94.0/windmill_api/models/flow_metadata.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_metadata_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/flow_metadata_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module.py` & `windmill_api-1.94.0/windmill_api/models/flow_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_0.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_0_input_transforms.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_1.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_1_input_transforms.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_2.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_2_input_transforms.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_module_value_2_type_6.py` & `windmill_api-1.94.0/windmill_api/models/flow_module_value_2_type_6.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_args.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_failure_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_preview_value_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/flow_preview_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_schema.py` & `windmill_api-1.94.0/windmill_api/models/flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status.py` & `windmill_api-1.94.0/windmill_api/models/flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_failure_module_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_failure_module_branch_chosen.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_failure_module_branchall.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_failure_module_iterator.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_module.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_module_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_module_branch_chosen.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_module_branchall.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_module_iterator.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_modules_item_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_modules_item_branch_chosen.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_modules_item_branchall.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_modules_item_iterator.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_status_retry.py` & `windmill_api-1.94.0/windmill_api/models/flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value.py` & `windmill_api-1.94.0/windmill_api/models/flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_failure_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/flow_value_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/folder.py` & `windmill_api-1.94.0/windmill_api/models/folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/folder_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/folder_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/force_cancel_queued_job_json_body.py` & `windmill_api-1.94.0/windmill_api/models/force_cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/forloop_flow.py` & `windmill_api-1.94.0/windmill_api/models/forloop_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/forloop_flow_iterator_type_0.py` & `windmill_api-1.94.0/windmill_api/models/forloop_flow_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/forloop_flow_iterator_type_1.py` & `windmill_api-1.94.0/windmill_api/models/forloop_flow_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/forloop_flow_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/forloop_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_app_by_path_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_app_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_app_by_path_response_200_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_app_by_path_response_200_policy.py` & `windmill_api-1.94.0/windmill_api/models/get_app_by_path_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py` & `windmill_api-1.94.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.94.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_app_by_path_with_draft_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_app_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py` & `windmill_api-1.94.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py` & `windmill_api-1.94.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.94.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_app_by_version_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_app_by_version_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_app_by_version_response_200_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_app_by_version_response_200_policy.py` & `windmill_api-1.94.0/windmill_api/models/get_app_by_version_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py` & `windmill_api-1.94.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.94.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_audit_log_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_audit_log_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_audit_log_response_200_operation.py` & `windmill_api-1.94.0/windmill_api/models/get_audit_log_response_200_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_audit_log_response_200_parameters.py` & `windmill_api-1.94.0/windmill_api/models/get_audit_log_response_200_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_args.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_schema.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_input_history_by_path_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py` & `windmill_api-1.94.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_folder_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_folder_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_folder_response_200_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/get_folder_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_folder_usage_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_folder_usage_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_granular_acls_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_granular_acls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_group_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_group_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_group_response_200_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/get_group_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_app_by_id_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_app_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_app_by_id_response_200_app.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_app_by_id_response_200_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_hub_script_by_path_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_hub_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_input_history_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/get_input_history_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_input_history_response_200_item_args.py` & `windmill_api-1.94.0/windmill_api/models/get_input_history_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_job_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_job_updates_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_job_updates_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_premium_info_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_premium_info_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_public_app_by_secret_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_public_app_by_secret_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_public_app_by_secret_response_200_policy.py` & `windmill_api-1.94.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py` & `windmill_api-1.94.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.94.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_resource_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_resource_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_resource_response_200_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/get_resource_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_resource_type_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_resource_type_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_resume_urls_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_resume_urls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_schedule_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_schedule_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_schedule_response_200_args.py` & `windmill_api-1.94.0/windmill_api/models/get_schedule_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_schedule_response_200_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/get_schedule_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_script_by_hash_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_script_by_hash_response_200_schema.py` & `windmill_api-1.94.0/windmill_api/models/get_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_script_by_path_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_script_by_path_response_200_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_script_by_path_response_200_schema.py` & `windmill_api-1.94.0/windmill_api/models/get_script_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_script_by_path_with_draft_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_script_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py` & `windmill_api-1.94.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py` & `windmill_api-1.94.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py` & `windmill_api-1.94.0/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_script_deployment_status_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_script_deployment_status_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_settings_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_suspended_job_flow_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_suspended_job_flow_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_suspended_job_flow_response_200_job.py` & `windmill_api-1.94.0/windmill_api/models/get_suspended_job_flow_response_200_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_variable_response_200.py` & `windmill_api-1.94.0/windmill_api/models/get_variable_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/get_variable_response_200_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/get_variable_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/global_user_info.py` & `windmill_api-1.94.0/windmill_api/models/global_user_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/global_user_update_json_body.py` & `windmill_api-1.94.0/windmill_api/models/global_user_update_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/global_whoami_response_200.py` & `windmill_api-1.94.0/windmill_api/models/global_whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200.py` & `windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item.py` & `windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.94.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/group.py` & `windmill_api-1.94.0/windmill_api/models/group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/group_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/group_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/identity.py` & `windmill_api-1.94.0/windmill_api/models/identity.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/input_.py` & `windmill_api-1.94.0/windmill_api/models/input_.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/input_args.py` & `windmill_api-1.94.0/windmill_api/models/input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/input_transform_type_0.py` & `windmill_api-1.94.0/windmill_api/models/input_transform_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/input_transform_type_1.py` & `windmill_api-1.94.0/windmill_api/models/input_transform_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/invite_user_json_body.py` & `windmill_api-1.94.0/windmill_api/models/invite_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/javascript_transform.py` & `windmill_api-1.94.0/windmill_api/models/javascript_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/job.py` & `windmill_api-1.94.0/windmill_api/models/job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_apps_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_apps_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_apps_response_200_item_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/list_apps_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_audit_logs_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_audit_logs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_audit_logs_response_200_item_operation.py` & `windmill_api-1.94.0/windmill_api/models/list_audit_logs_response_200_item_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_audit_logs_response_200_item_parameters.py` & `windmill_api-1.94.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_args.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_contextual_variables_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_contextual_variables_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_flows_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_flows_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_folders_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_folders_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_folders_response_200_item_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/list_folders_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_groups_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_groups_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_groups_response_200_item_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/list_groups_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_hub_apps_response_200.py` & `windmill_api-1.94.0/windmill_api/models/list_hub_apps_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_hub_apps_response_200_apps_item.py` & `windmill_api-1.94.0/windmill_api/models/list_hub_apps_response_200_apps_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_hub_flows_response_200.py` & `windmill_api-1.94.0/windmill_api/models/list_hub_flows_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_hub_flows_response_200_flows_item.py` & `windmill_api-1.94.0/windmill_api/models/list_hub_flows_response_200_flows_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_hub_scripts_response_200.py` & `windmill_api-1.94.0/windmill_api/models/list_hub_scripts_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_hub_scripts_response_200_asks_item.py` & `windmill_api-1.94.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_inputs_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_inputs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_inputs_response_200_item_args.py` & `windmill_api-1.94.0/windmill_api/models/list_inputs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_jobs_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_pending_invites_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_pending_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_args.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_flow_status_retry.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_resource_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_resource_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_resource_response_200_item_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/list_resource_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_resource_type_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_resource_type_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_schedules_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_schedules_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_schedules_response_200_item_args.py` & `windmill_api-1.94.0/windmill_api/models/list_schedules_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_schedules_response_200_item_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_scripts_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_scripts_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_scripts_response_200_item_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_scripts_response_200_item_schema.py` & `windmill_api-1.94.0/windmill_api/models/list_scripts_response_200_item_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_tokens_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_tokens_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_user_workspaces_response_200.py` & `windmill_api-1.94.0/windmill_api/models/list_user_workspaces_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py` & `windmill_api-1.94.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_users_as_super_admin_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_users_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_users_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_users_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_users_response_200_item_usage.py` & `windmill_api-1.94.0/windmill_api/models/list_users_response_200_item_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_variable_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_variable_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_variable_response_200_item_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/list_variable_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_workers_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_workers_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_workspace_invites_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_workspace_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/list_workspaces_response_200_item.py` & `windmill_api-1.94.0/windmill_api/models/list_workspaces_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/listable_app.py` & `windmill_api-1.94.0/windmill_api/models/listable_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/listable_app_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/listable_app_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/listable_resource.py` & `windmill_api-1.94.0/windmill_api/models/listable_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/listable_resource_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/listable_resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/listable_variable.py` & `windmill_api-1.94.0/windmill_api/models/listable_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/listable_variable_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/listable_variable_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/login.py` & `windmill_api-1.94.0/windmill_api/models/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/login_json_body.py` & `windmill_api-1.94.0/windmill_api/models/login_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/login_with_oauth_json_body.py` & `windmill_api-1.94.0/windmill_api/models/login_with_oauth_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/main_arg_signature.py` & `windmill_api-1.94.0/windmill_api/models/main_arg_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item.py` & `windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_1.py` & `windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_2.py` & `windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_3.py` & `windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py` & `windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_4.py` & `windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.94.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/new_schedule.py` & `windmill_api-1.94.0/windmill_api/models/new_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/new_schedule_args.py` & `windmill_api-1.94.0/windmill_api/models/new_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/new_script.py` & `windmill_api-1.94.0/windmill_api/models/new_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/new_script_schema.py` & `windmill_api-1.94.0/windmill_api/models/new_script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/new_script_with_draft.py` & `windmill_api-1.94.0/windmill_api/models/new_script_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/new_script_with_draft_draft.py` & `windmill_api-1.94.0/windmill_api/models/new_script_with_draft_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/new_script_with_draft_draft_schema.py` & `windmill_api-1.94.0/windmill_api/models/new_script_with_draft_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/new_script_with_draft_schema.py` & `windmill_api-1.94.0/windmill_api/models/new_script_with_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/new_token.py` & `windmill_api-1.94.0/windmill_api/models/new_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/new_token_impersonate.py` & `windmill_api-1.94.0/windmill_api/models/new_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/new_user.py` & `windmill_api-1.94.0/windmill_api/models/new_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow.py` & `windmill_api-1.94.0/windmill_api/models/open_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_schema.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_failure_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_value_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_schema.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/path_flow.py` & `windmill_api-1.94.0/windmill_api/models/path_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/path_flow_input_transforms.py` & `windmill_api-1.94.0/windmill_api/models/path_flow_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py` & `windmill_api-1.94.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py` & `windmill_api-1.94.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/path_script.py` & `windmill_api-1.94.0/windmill_api/models/path_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/path_script_input_transforms.py` & `windmill_api-1.94.0/windmill_api/models/path_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/path_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.94.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/path_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.94.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/policy.py` & `windmill_api-1.94.0/windmill_api/models/policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/policy_triggerables.py` & `windmill_api-1.94.0/windmill_api/models/policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/policy_triggerables_additional_property.py` & `windmill_api-1.94.0/windmill_api/models/policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/preview.py` & `windmill_api-1.94.0/windmill_api/models/preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/preview_args.py` & `windmill_api-1.94.0/windmill_api/models/preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/preview_schedule_json_body.py` & `windmill_api-1.94.0/windmill_api/models/preview_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200.py` & `windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item.py` & `windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.94.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job.py` & `windmill_api-1.94.0/windmill_api/models/queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_args.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_flow_status.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_failure_module_branchall.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_failure_module_iterator.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_modules_item_branchall.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_modules_item_iterator.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_flow_status_retry.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/raw_script.py` & `windmill_api-1.94.0/windmill_api/models/raw_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/raw_script_input_transforms.py` & `windmill_api-1.94.0/windmill_api/models/raw_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.94.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.94.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/refresh_token_json_body.py` & `windmill_api-1.94.0/windmill_api/models/refresh_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/remove_granular_acls_json_body.py` & `windmill_api-1.94.0/windmill_api/models/remove_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/remove_owner_to_folder_json_body.py` & `windmill_api-1.94.0/windmill_api/models/remove_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/remove_user_to_group_json_body.py` & `windmill_api-1.94.0/windmill_api/models/remove_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/resource.py` & `windmill_api-1.94.0/windmill_api/models/resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/resource_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/resource_type.py` & `windmill_api-1.94.0/windmill_api/models/resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/resume_suspended_flow_as_owner_json_body.py` & `windmill_api-1.94.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/resume_suspended_job_post_json_body.py` & `windmill_api-1.94.0/windmill_api/models/resume_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/retry.py` & `windmill_api-1.94.0/windmill_api/models/retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_by_path_json_body.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_args.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_script_by_hash_json_body.py` & `windmill_api-1.94.0/windmill_api/models/run_script_by_hash_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_script_by_path_json_body.py` & `windmill_api-1.94.0/windmill_api/models/run_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_script_preview_json_body.py` & `windmill_api-1.94.0/windmill_api/models/run_script_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_script_preview_json_body_args.py` & `windmill_api-1.94.0/windmill_api/models/run_script_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_wait_result_flow_by_path_json_body.py` & `windmill_api-1.94.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/run_wait_result_script_by_path_json_body.py` & `windmill_api-1.94.0/windmill_api/models/run_wait_result_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/schedule.py` & `windmill_api-1.94.0/windmill_api/models/schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/schedule_args.py` & `windmill_api-1.94.0/windmill_api/models/schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/schedule_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/schedule_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/script.py` & `windmill_api-1.94.0/windmill_api/models/script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/script_args.py` & `windmill_api-1.94.0/windmill_api/models/script_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/script_extra_perms.py` & `windmill_api-1.94.0/windmill_api/models/script_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/script_schema.py` & `windmill_api-1.94.0/windmill_api/models/script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/set_password_json_body.py` & `windmill_api-1.94.0/windmill_api/models/set_password_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/set_schedule_enabled_json_body.py` & `windmill_api-1.94.0/windmill_api/models/set_schedule_enabled_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/slack_token.py` & `windmill_api-1.94.0/windmill_api/models/slack_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/slack_token_bot.py` & `windmill_api-1.94.0/windmill_api/models/slack_token_bot.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/star_json_body.py` & `windmill_api-1.94.0/windmill_api/models/star_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/static_transform.py` & `windmill_api-1.94.0/windmill_api/models/static_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/token_response.py` & `windmill_api-1.94.0/windmill_api/models/token_response.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/truncated_token.py` & `windmill_api-1.94.0/windmill_api/models/truncated_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/unstar_json_body.py` & `windmill_api-1.94.0/windmill_api/models/unstar_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_app_json_body.py` & `windmill_api-1.94.0/windmill_api/models/update_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_app_json_body_policy.py` & `windmill_api-1.94.0/windmill_api/models/update_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_app_json_body_policy_triggerables.py` & `windmill_api-1.94.0/windmill_api/models/update_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.94.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_schema.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_retry.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py` & `windmill_api-1.94.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_folder_json_body.py` & `windmill_api-1.94.0/windmill_api/models/update_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_group_json_body.py` & `windmill_api-1.94.0/windmill_api/models/update_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_input.py` & `windmill_api-1.94.0/windmill_api/models/update_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_input_json_body.py` & `windmill_api-1.94.0/windmill_api/models/update_input_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_resource_json_body.py` & `windmill_api-1.94.0/windmill_api/models/update_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_resource_type_json_body.py` & `windmill_api-1.94.0/windmill_api/models/update_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_resource_value_json_body.py` & `windmill_api-1.94.0/windmill_api/models/update_resource_value_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_schedule_json_body.py` & `windmill_api-1.94.0/windmill_api/models/update_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_schedule_json_body_args.py` & `windmill_api-1.94.0/windmill_api/models/update_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_user_json_body.py` & `windmill_api-1.94.0/windmill_api/models/update_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/update_variable_json_body.py` & `windmill_api-1.94.0/windmill_api/models/update_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/usage.py` & `windmill_api-1.94.0/windmill_api/models/usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/user.py` & `windmill_api-1.94.0/windmill_api/models/user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/user_usage.py` & `windmill_api-1.94.0/windmill_api/models/user_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/user_workspace_list.py` & `windmill_api-1.94.0/windmill_api/models/user_workspace_list.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/user_workspace_list_workspaces_item.py` & `windmill_api-1.94.0/windmill_api/models/user_workspace_list_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/whoami_response_200.py` & `windmill_api-1.94.0/windmill_api/models/whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/whoami_response_200_usage.py` & `windmill_api-1.94.0/windmill_api/models/whoami_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/whois_response_200.py` & `windmill_api-1.94.0/windmill_api/models/whois_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/whois_response_200_usage.py` & `windmill_api-1.94.0/windmill_api/models/whois_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/worker_ping.py` & `windmill_api-1.94.0/windmill_api/models/worker_ping.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/workspace.py` & `windmill_api-1.94.0/windmill_api/models/workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/models/workspace_invite.py` & `windmill_api-1.94.0/windmill_api/models/workspace_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/windmill_api/types.py` & `windmill_api-1.94.0/windmill_api/types.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.93.1/setup.py` & `windmill_api-1.94.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=21.3.0', 'httpx>=0.15.4,<0.24.0', 'python-dateutil>=2.8.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'windmill-api',
-    'version': '1.93.1',
+    'version': '1.94.0',
     'description': 'A client library for accessing Windmill API',
     'long_description': '# Autogenerated Windmill OpenApi Client\nThis is the raw autogenerated api client. You are most likely more interested in [wmill](https://pypi.org/project/wmill/) which leverages this client to offer an user friendly experience. We use [this openapi python client generator](https://github.com/openapi-generators/openapi-python-client/)\n\n# windmill-api\nA client library for accessing Windmill API\n\n## Usage\nFirst, create a client:\n\n```python\nfrom windmill_api import Client\n\nclient = Client(base_url="https://api.example.com")\n```\n\nIf the endpoints you\'re going to hit require authentication, use `AuthenticatedClient` instead:\n\n```python\nfrom windmill_api import AuthenticatedClient\n\nclient = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = get_my_data_model.sync(client=client)\n# or if you need more info (e.g. status_code)\nresponse: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)\n```\n\nOr do the same thing with an async version:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = await get_my_data_model.asyncio(client=client)\nresponse: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)\n```\n\nBy default, when you\'re calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken",\n    verify_ssl="/path/to/certificate_bundle.pem",\n)\n```\n\nYou can also disable certificate validation altogether, but beware that **this is a security risk**.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken", \n    verify_ssl=False\n)\n```\n\nThings to know:\n1. Every path/method combo becomes a Python module with four functions:\n    1. `sync`: Blocking request that returns parsed data (if successful) or `None`\n    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.\n    1. `asyncio`: Like `sync` but async instead of blocking\n    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking\n\n1. All path/query params, and bodies become method arguments.\n1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)\n1. Any endpoint which did not have a tag will be in `windmill_api.api.default`\n\n',
     'author': 'Ruben Fiszel',
     'author_email': 'ruben@windmill.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `windmill_api-1.93.1/PKG-INFO` & `windmill_api-1.94.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windmill-api
-Version: 1.93.1
+Version: 1.94.0
 Summary: A client library for accessing Windmill API
 License: Apache-2.0
 Author: Ruben Fiszel
 Author-email: ruben@windmill.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

