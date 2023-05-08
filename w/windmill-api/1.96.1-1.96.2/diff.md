# Comparing `tmp/windmill_api-1.96.1.tar.gz` & `tmp/windmill_api-1.96.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windmill_api-1.96.1.tar", max compression
+gzip compressed data, was "windmill_api-1.96.2.tar", max compression
```

## Comparing `windmill_api-1.96.1.tar` & `windmill_api-1.96.2.tar`

### file list

```diff
@@ -1,1302 +1,1302 @@
--rw-r--r--   0        0        0    11348 2023-05-08 19:21:20.939801 windmill_api-1.96.1/LICENSE
--rw-r--r--   0        0        0     2952 2023-05-08 19:21:20.943801 windmill_api-1.96.1/README.md
--rw-r--r--   0        0        0      717 2023-05-08 19:21:20.939801 windmill_api-1.96.1/pyproject.toml
--rw-r--r--   0        0        0      100 2023-05-08 19:20:47.203207 windmill_api-1.96.1/windmill_api/__init__.py
--rw-r--r--   0        0        0       47 2023-05-08 19:20:47.699214 windmill_api-1.96.1/windmill_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.831216 windmill_api-1.96.1/windmill_api/api/app/__init__.py
--rw-r--r--   0        0        0     1999 2023-05-08 19:20:58.411395 windmill_api-1.96.1/windmill_api/api/app/create_app.py
--rw-r--r--   0        0        0     1769 2023-05-08 19:20:58.415395 windmill_api-1.96.1/windmill_api/api/app/delete_app.py
--rw-r--r--   0        0        0     2214 2023-05-08 19:20:58.443395 windmill_api-1.96.1/windmill_api/api/app/execute_component.py
--rw-r--r--   0        0        0     2782 2023-05-08 19:20:58.479396 windmill_api-1.96.1/windmill_api/api/app/exists_app.py
--rw-r--r--   0        0        0     3020 2023-05-08 19:20:58.483396 windmill_api-1.96.1/windmill_api/api/app/get_app_by_path.py
--rw-r--r--   0        0        0     3187 2023-05-08 19:20:58.531397 windmill_api-1.96.1/windmill_api/api/app/get_app_by_path_with_draft.py
--rw-r--r--   0        0        0     3031 2023-05-08 19:20:58.523397 windmill_api-1.96.1/windmill_api/api/app/get_app_by_version.py
--rw-r--r--   0        0        0     2649 2023-05-08 19:20:58.579398 windmill_api-1.96.1/windmill_api/api/app/get_hub_app_by_id.py
--rw-r--r--   0        0        0     3168 2023-05-08 19:20:58.587398 windmill_api-1.96.1/windmill_api/api/app/get_public_app_by_secret.py
--rw-r--r--   0        0        0     1797 2023-05-08 19:20:58.607398 windmill_api-1.96.1/windmill_api/api/app/get_public_secret_of_app.py
--rw-r--r--   0        0        0     7289 2023-05-08 19:20:58.675399 windmill_api-1.96.1/windmill_api/api/app/list_apps.py
--rw-r--r--   0        0        0     2405 2023-05-08 19:20:58.643399 windmill_api-1.96.1/windmill_api/api/app/list_hub_apps.py
--rw-r--r--   0        0        0     2140 2023-05-08 19:20:58.679400 windmill_api-1.96.1/windmill_api/api/app/update_app.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.739215 windmill_api-1.96.1/windmill_api/api/audit/__init__.py
--rw-r--r--   0        0        0     3065 2023-05-08 19:20:58.715400 windmill_api-1.96.1/windmill_api/api/audit/get_audit_log.py
--rw-r--r--   0        0        0     8723 2023-05-08 19:20:58.787402 windmill_api-1.96.1/windmill_api/api/audit/list_audit_logs.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.891217 windmill_api-1.96.1/windmill_api/api/capture/__init__.py
--rw-r--r--   0        0        0     1796 2023-05-08 19:20:58.747401 windmill_api-1.96.1/windmill_api/api/capture/create_capture.py
--rw-r--r--   0        0        0     1790 2023-05-08 19:20:58.775401 windmill_api-1.96.1/windmill_api/api/capture/get_capture.py
--rw-r--r--   0        0        0     1799 2023-05-08 19:20:58.807402 windmill_api-1.96.1/windmill_api/api/capture/update_capture.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.843216 windmill_api-1.96.1/windmill_api/api/draft/__init__.py
--rw-r--r--   0        0        0     2019 2023-05-08 19:20:58.815402 windmill_api-1.96.1/windmill_api/api/draft/create_draft.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.891217 windmill_api-1.96.1/windmill_api/api/favorite/__init__.py
--rw-r--r--   0        0        0     1964 2023-05-08 19:20:58.843403 windmill_api-1.96.1/windmill_api/api/favorite/star.py
--rw-r--r--   0        0        0     1984 2023-05-08 19:20:58.847403 windmill_api-1.96.1/windmill_api/api/favorite/unstar.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.799216 windmill_api-1.96.1/windmill_api/api/flow/__init__.py
--rw-r--r--   0        0        0     2220 2023-05-08 19:20:58.879403 windmill_api-1.96.1/windmill_api/api/flow/archive_flow_by_path.py
--rw-r--r--   0        0        0     2009 2023-05-08 19:20:58.875403 windmill_api-1.96.1/windmill_api/api/flow/create_flow.py
--rw-r--r--   0        0        0     1788 2023-05-08 19:20:58.931404 windmill_api-1.96.1/windmill_api/api/flow/delete_flow_by_path.py
--rw-r--r--   0        0        0     2755 2023-05-08 19:20:58.919404 windmill_api-1.96.1/windmill_api/api/flow/exists_flow_by_path.py
--rw-r--r--   0        0        0     3036 2023-05-08 19:20:58.987405 windmill_api-1.96.1/windmill_api/api/flow/get_flow_by_path.py
--rw-r--r--   0        0        0     3205 2023-05-08 19:20:58.971405 windmill_api-1.96.1/windmill_api/api/flow/get_flow_by_path_with_draft.py
--rw-r--r--   0        0        0     4827 2023-05-08 19:20:59.031406 windmill_api-1.96.1/windmill_api/api/flow/get_flow_input_history_by_path.py
--rw-r--r--   0        0        0     2667 2023-05-08 19:20:59.023406 windmill_api-1.96.1/windmill_api/api/flow/get_hub_flow_by_id.py
--rw-r--r--   0        0        0     1668 2023-05-08 19:20:59.055407 windmill_api-1.96.1/windmill_api/api/flow/list_flow_paths.py
--rw-r--r--   0        0        0     7969 2023-05-08 19:20:59.123408 windmill_api-1.96.1/windmill_api/api/flow/list_flows.py
--rw-r--r--   0        0        0     2423 2023-05-08 19:20:59.091407 windmill_api-1.96.1/windmill_api/api/flow/list_hub_flows.py
--rw-r--r--   0        0        0     2150 2023-05-08 19:20:59.123408 windmill_api-1.96.1/windmill_api/api/flow/update_flow.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.883217 windmill_api-1.96.1/windmill_api/api/folder/__init__.py
--rw-r--r--   0        0        0     2214 2023-05-08 19:20:59.159408 windmill_api-1.96.1/windmill_api/api/folder/add_owner_to_folder.py
--rw-r--r--   0        0        0     2029 2023-05-08 19:20:59.151408 windmill_api-1.96.1/windmill_api/api/folder/create_folder.py
--rw-r--r--   0        0        0     1778 2023-05-08 19:20:59.179409 windmill_api-1.96.1/windmill_api/api/folder/delete_folder.py
--rw-r--r--   0        0        0     2960 2023-05-08 19:20:59.203409 windmill_api-1.96.1/windmill_api/api/folder/get_folder.py
--rw-r--r--   0        0        0     3055 2023-05-08 19:20:59.219410 windmill_api-1.96.1/windmill_api/api/folder/get_folder_usage.py
--rw-r--r--   0        0        0     3405 2023-05-08 19:20:59.255410 windmill_api-1.96.1/windmill_api/api/folder/list_folder_names.py
--rw-r--r--   0        0        0     4251 2023-05-08 19:20:59.303411 windmill_api-1.96.1/windmill_api/api/folder/list_folders.py
--rw-r--r--   0        0        0     2244 2023-05-08 19:20:59.287411 windmill_api-1.96.1/windmill_api/api/folder/remove_owner_to_folder.py
--rw-r--r--   0        0        0     2170 2023-05-08 19:20:59.355412 windmill_api-1.96.1/windmill_api/api/folder/update_folder.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.887217 windmill_api-1.96.1/windmill_api/api/granular_acl/__init__.py
--rw-r--r--   0        0        0     2480 2023-05-08 19:20:59.335412 windmill_api-1.96.1/windmill_api/api/granular_acl/add_granular_acls.py
--rw-r--r--   0        0        0     3526 2023-05-08 19:20:59.375413 windmill_api-1.96.1/windmill_api/api/granular_acl/get_granular_acls.py
--rw-r--r--   0        0        0     2545 2023-05-08 19:20:59.391413 windmill_api-1.96.1/windmill_api/api/granular_acl/remove_granular_acls.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.875217 windmill_api-1.96.1/windmill_api/api/group/__init__.py
--rw-r--r--   0        0        0     2194 2023-05-08 19:20:59.407413 windmill_api-1.96.1/windmill_api/api/group/add_user_to_group.py
--rw-r--r--   0        0        0     2019 2023-05-08 19:20:59.423413 windmill_api-1.96.1/windmill_api/api/group/create_group.py
--rw-r--r--   0        0        0     1775 2023-05-08 19:20:59.435414 windmill_api-1.96.1/windmill_api/api/group/delete_group.py
--rw-r--r--   0        0        0     2942 2023-05-08 19:20:59.467414 windmill_api-1.96.1/windmill_api/api/group/get_group.py
--rw-r--r--   0        0        0     3400 2023-05-08 19:20:59.483415 windmill_api-1.96.1/windmill_api/api/group/list_group_names.py
--rw-r--r--   0        0        0     4233 2023-05-08 19:20:59.543416 windmill_api-1.96.1/windmill_api/api/group/list_groups.py
--rw-r--r--   0        0        0     2224 2023-05-08 19:20:59.511415 windmill_api-1.96.1/windmill_api/api/group/remove_user_to_group.py
--rw-r--r--   0        0        0     2160 2023-05-08 19:20:59.559416 windmill_api-1.96.1/windmill_api/api/group/update_group.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.891217 windmill_api-1.96.1/windmill_api/api/input_/__init__.py
--rw-r--r--   0        0        0     3338 2023-05-08 19:20:59.595417 windmill_api-1.96.1/windmill_api/api/input_/create_input.py
--rw-r--r--   0        0        0     1811 2023-05-08 19:20:59.587417 windmill_api-1.96.1/windmill_api/api/input_/delete_input.py
--rw-r--r--   0        0        0     6187 2023-05-08 19:20:59.683418 windmill_api-1.96.1/windmill_api/api/input_/get_input_history.py
--rw-r--r--   0        0        0     6010 2023-05-08 19:20:59.667418 windmill_api-1.96.1/windmill_api/api/input_/list_inputs.py
--rw-r--r--   0        0        0     2025 2023-05-08 19:20:59.699418 windmill_api-1.96.1/windmill_api/api/input_/update_input.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.843216 windmill_api-1.96.1/windmill_api/api/job/__init__.py
--rw-r--r--   0        0        0     2181 2023-05-08 19:20:59.715419 windmill_api-1.96.1/windmill_api/api/job/cancel_queued_job.py
--rw-r--r--   0        0        0     2687 2023-05-08 19:20:59.779420 windmill_api-1.96.1/windmill_api/api/job/cancel_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-05-08 19:20:59.759420 windmill_api-1.96.1/windmill_api/api/job/cancel_suspended_job_post.py
--rw-r--r--   0        0        0     2535 2023-05-08 19:20:59.799420 windmill_api-1.96.1/windmill_api/api/job/create_job_signature.py
--rw-r--r--   0        0        0     3217 2023-05-08 19:20:59.819421 windmill_api-1.96.1/windmill_api/api/job/delete_completed_job.py
--rw-r--r--   0        0        0     2235 2023-05-08 19:20:59.831421 windmill_api-1.96.1/windmill_api/api/job/force_cancel_queued_job.py
--rw-r--r--   0        0        0     3034 2023-05-08 19:20:59.859421 windmill_api-1.96.1/windmill_api/api/job/get_completed_job.py
--rw-r--r--   0        0        0     1784 2023-05-08 19:20:59.863422 windmill_api-1.96.1/windmill_api/api/job/get_completed_job_result.py
--rw-r--r--   0        0        0     2868 2023-05-08 19:20:59.903422 windmill_api-1.96.1/windmill_api/api/job/get_job.py
--rw-r--r--   0        0        0     4305 2023-05-08 19:20:59.919422 windmill_api-1.96.1/windmill_api/api/job/get_job_updates.py
--rw-r--r--   0        0        0     4306 2023-05-08 19:20:59.959423 windmill_api-1.96.1/windmill_api/api/job/get_resume_urls.py
--rw-r--r--   0        0        0     4601 2023-05-08 19:20:59.975424 windmill_api-1.96.1/windmill_api/api/job/get_suspended_job_flow.py
--rw-r--r--   0        0        0    13065 2023-05-08 19:21:00.147427 windmill_api-1.96.1/windmill_api/api/job/list_completed_jobs.py
--rw-r--r--   0        0        0    12292 2023-05-08 19:21:00.147427 windmill_api-1.96.1/windmill_api/api/job/list_jobs.py
--rw-r--r--   0        0        0    12830 2023-05-08 19:21:00.295430 windmill_api-1.96.1/windmill_api/api/job/list_queue.py
--rw-r--r--   0        0        0     2067 2023-05-08 19:21:00.179427 windmill_api-1.96.1/windmill_api/api/job/result_by_id.py
--rw-r--r--   0        0        0     2313 2023-05-08 19:21:00.211428 windmill_api-1.96.1/windmill_api/api/job/resume_suspended_flow_as_owner.py
--rw-r--r--   0        0        0     2994 2023-05-08 19:21:00.255429 windmill_api-1.96.1/windmill_api/api/job/resume_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-05-08 19:21:00.303430 windmill_api-1.96.1/windmill_api/api/job/resume_suspended_job_post.py
--rw-r--r--   0        0        0     4566 2023-05-08 19:21:00.351431 windmill_api-1.96.1/windmill_api/api/job/run_flow_by_path.py
--rw-r--r--   0        0        0     3037 2023-05-08 19:21:00.343430 windmill_api-1.96.1/windmill_api/api/job/run_flow_preview.py
--rw-r--r--   0        0        0     4594 2023-05-08 19:21:00.403432 windmill_api-1.96.1/windmill_api/api/job/run_script_by_hash.py
--rw-r--r--   0        0        0     4200 2023-05-08 19:21:00.447432 windmill_api-1.96.1/windmill_api/api/job/run_script_by_path.py
--rw-r--r--   0        0        0     3050 2023-05-08 19:21:00.447432 windmill_api-1.96.1/windmill_api/api/job/run_script_preview.py
--rw-r--r--   0        0        0     3215 2023-05-08 19:21:00.491433 windmill_api-1.96.1/windmill_api/api/job/run_wait_result_flow_by_path.py
--rw-r--r--   0        0        0     3521 2023-05-08 19:21:00.491433 windmill_api-1.96.1/windmill_api/api/job/run_wait_result_script_by_path.py
--rw-r--r--   0        0        0     3356 2023-05-08 19:21:00.567435 windmill_api-1.96.1/windmill_api/api/job/run_wait_result_script_by_path_get.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.771215 windmill_api-1.96.1/windmill_api/api/oauth/__init__.py
--rw-r--r--   0        0        0     3506 2023-05-08 19:21:00.535434 windmill_api-1.96.1/windmill_api/api/oauth/connect_callback.py
--rw-r--r--   0        0        0     2118 2023-05-08 19:21:00.563434 windmill_api-1.96.1/windmill_api/api/oauth/connect_slack_callback.py
--rw-r--r--   0        0        0     2056 2023-05-08 19:21:00.591435 windmill_api-1.96.1/windmill_api/api/oauth/create_account.py
--rw-r--r--   0        0        0     1764 2023-05-08 19:21:00.611435 windmill_api-1.96.1/windmill_api/api/oauth/disconnect_account.py
--rw-r--r--   0        0        0     1649 2023-05-08 19:21:00.619435 windmill_api-1.96.1/windmill_api/api/oauth/disconnect_slack.py
--rw-r--r--   0        0        0     1426 2023-05-08 19:21:00.639436 windmill_api-1.96.1/windmill_api/api/oauth/list_o_auth_connects.py
--rw-r--r--   0        0        0     2162 2023-05-08 19:21:00.655436 windmill_api-1.96.1/windmill_api/api/oauth/list_o_auth_logins.py
--rw-r--r--   0        0        0     2151 2023-05-08 19:21:00.671436 windmill_api-1.96.1/windmill_api/api/oauth/refresh_token.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.867217 windmill_api-1.96.1/windmill_api/api/raw_app/__init__.py
--rw-r--r--   0        0        0     2033 2023-05-08 19:21:00.683437 windmill_api-1.96.1/windmill_api/api/raw_app/create_raw_app.py
--rw-r--r--   0        0        0     1781 2023-05-08 19:21:00.703437 windmill_api-1.96.1/windmill_api/api/raw_app/delete_raw_app.py
--rw-r--r--   0        0        0     2786 2023-05-08 19:21:00.723437 windmill_api-1.96.1/windmill_api/api/raw_app/exists_raw_app.py
--rw-r--r--   0        0        0     1979 2023-05-08 19:21:00.735438 windmill_api-1.96.1/windmill_api/api/raw_app/get_raw_app_data.py
--rw-r--r--   0        0        0     7349 2023-05-08 19:21:00.831439 windmill_api-1.96.1/windmill_api/api/raw_app/list_raw_apps.py
--rw-r--r--   0        0        0     2166 2023-05-08 19:21:00.767438 windmill_api-1.96.1/windmill_api/api/raw_app/update_raw_app.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.775215 windmill_api-1.96.1/windmill_api/api/resource/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-08 19:21:00.799439 windmill_api-1.96.1/windmill_api/api/resource/create_resource.py
--rw-r--r--   0        0        0     2093 2023-05-08 19:21:00.831439 windmill_api-1.96.1/windmill_api/api/resource/create_resource_type.py
--rw-r--r--   0        0        0     1784 2023-05-08 19:21:00.859440 windmill_api-1.96.1/windmill_api/api/resource/delete_resource.py
--rw-r--r--   0        0        0     1799 2023-05-08 19:21:00.859440 windmill_api-1.96.1/windmill_api/api/resource/delete_resource_type.py
--rw-r--r--   0        0        0     2763 2023-05-08 19:21:00.919441 windmill_api-1.96.1/windmill_api/api/resource/exists_resource.py
--rw-r--r--   0        0        0     2788 2023-05-08 19:21:00.903441 windmill_api-1.96.1/windmill_api/api/resource/exists_resource_type.py
--rw-r--r--   0        0        0     2996 2023-05-08 19:21:00.943441 windmill_api-1.96.1/windmill_api/api/resource/get_resource.py
--rw-r--r--   0        0        0     3074 2023-05-08 19:21:00.959442 windmill_api-1.96.1/windmill_api/api/resource/get_resource_type.py
--rw-r--r--   0        0        0     1790 2023-05-08 19:21:00.975442 windmill_api-1.96.1/windmill_api/api/resource/get_resource_value.py
--rw-r--r--   0        0        0     5732 2023-05-08 19:21:01.027443 windmill_api-1.96.1/windmill_api/api/resource/list_resource.py
--rw-r--r--   0        0        0     3149 2023-05-08 19:21:01.015443 windmill_api-1.96.1/windmill_api/api/resource/list_resource_type.py
--rw-r--r--   0        0        0     2600 2023-05-08 19:21:01.059444 windmill_api-1.96.1/windmill_api/api/resource/list_resource_type_names.py
--rw-r--r--   0        0        0     2190 2023-05-08 19:21:01.059444 windmill_api-1.96.1/windmill_api/api/resource/update_resource.py
--rw-r--r--   0        0        0     2234 2023-05-08 19:21:01.123445 windmill_api-1.96.1/windmill_api/api/resource/update_resource_type.py
--rw-r--r--   0        0        0     2244 2023-05-08 19:21:01.087444 windmill_api-1.96.1/windmill_api/api/resource/update_resource_value.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.871217 windmill_api-1.96.1/windmill_api/api/schedule/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-08 19:21:01.119445 windmill_api-1.96.1/windmill_api/api/schedule/create_schedule.py
--rw-r--r--   0        0        0     1784 2023-05-08 19:21:01.147445 windmill_api-1.96.1/windmill_api/api/schedule/delete_schedule.py
--rw-r--r--   0        0        0     2763 2023-05-08 19:21:01.163446 windmill_api-1.96.1/windmill_api/api/schedule/exists_schedule.py
--rw-r--r--   0        0        0     2996 2023-05-08 19:21:01.187446 windmill_api-1.96.1/windmill_api/api/schedule/get_schedule.py
--rw-r--r--   0        0        0     4287 2023-05-08 19:21:01.223447 windmill_api-1.96.1/windmill_api/api/schedule/list_schedules.py
--rw-r--r--   0        0        0     3217 2023-05-08 19:21:01.227447 windmill_api-1.96.1/windmill_api/api/schedule/preview_schedule.py
--rw-r--r--   0        0        0     2233 2023-05-08 19:21:01.255447 windmill_api-1.96.1/windmill_api/api/schedule/set_schedule_enabled.py
--rw-r--r--   0        0        0     2190 2023-05-08 19:21:01.283448 windmill_api-1.96.1/windmill_api/api/schedule/update_schedule.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.783215 windmill_api-1.96.1/windmill_api/api/script/__init__.py
--rw-r--r--   0        0        0     3165 2023-05-08 19:21:01.299448 windmill_api-1.96.1/windmill_api/api/script/archive_script_by_hash.py
--rw-r--r--   0        0        0     1797 2023-05-08 19:21:01.307448 windmill_api-1.96.1/windmill_api/api/script/archive_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-05-08 19:21:01.343449 windmill_api-1.96.1/windmill_api/api/script/bash_to_jsonschema.py
--rw-r--r--   0        0        0     2029 2023-05-08 19:21:01.335449 windmill_api-1.96.1/windmill_api/api/script/create_script.py
--rw-r--r--   0        0        0     3327 2023-05-08 19:21:01.375450 windmill_api-1.96.1/windmill_api/api/script/delete_script_by_hash.py
--rw-r--r--   0        0        0     2873 2023-05-08 19:21:01.383450 windmill_api-1.96.1/windmill_api/api/script/delete_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-05-08 19:21:01.415450 windmill_api-1.96.1/windmill_api/api/script/deno_to_jsonschema.py
--rw-r--r--   0        0        0     2767 2023-05-08 19:21:01.423450 windmill_api-1.96.1/windmill_api/api/script/exists_script_by_path.py
--rw-r--r--   0        0        0     2802 2023-05-08 19:21:01.451451 windmill_api-1.96.1/windmill_api/api/script/get_hub_script_by_path.py
--rw-r--r--   0        0        0     1607 2023-05-08 19:21:01.455451 windmill_api-1.96.1/windmill_api/api/script/get_hub_script_content_by_path.py
--rw-r--r--   0        0        0     3092 2023-05-08 19:21:01.491452 windmill_api-1.96.1/windmill_api/api/script/get_script_by_hash.py
--rw-r--r--   0        0        0     3074 2023-05-08 19:21:01.515452 windmill_api-1.96.1/windmill_api/api/script/get_script_by_path.py
--rw-r--r--   0        0        0     3241 2023-05-08 19:21:01.531453 windmill_api-1.96.1/windmill_api/api/script/get_script_by_path_with_draft.py
--rw-r--r--   0        0        0     3276 2023-05-08 19:21:01.559453 windmill_api-1.96.1/windmill_api/api/script/get_script_deployment_status.py
--rw-r--r--   0        0        0     2967 2023-05-08 19:21:01.571453 windmill_api-1.96.1/windmill_api/api/script/go_to_jsonschema.py
--rw-r--r--   0        0        0     2459 2023-05-08 19:21:01.595454 windmill_api-1.96.1/windmill_api/api/script/list_hub_scripts.py
--rw-r--r--   0        0        0     1676 2023-05-08 19:21:01.615454 windmill_api-1.96.1/windmill_api/api/script/list_script_paths.py
--rw-r--r--   0        0        0    11165 2023-05-08 19:21:01.727456 windmill_api-1.96.1/windmill_api/api/script/list_scripts.py
--rw-r--r--   0        0        0     3039 2023-05-08 19:21:01.655455 windmill_api-1.96.1/windmill_api/api/script/python_to_jsonschema.py
--rw-r--r--   0        0        0     1784 2023-05-08 19:21:01.679455 windmill_api-1.96.1/windmill_api/api/script/raw_script_by_hash.py
--rw-r--r--   0        0        0     1784 2023-05-08 19:21:01.707456 windmill_api-1.96.1/windmill_api/api/script/raw_script_by_path.py
--rw-r--r--   0        0        0     2119 2023-05-08 19:21:01.739456 windmill_api-1.96.1/windmill_api/api/script/raw_script_by_path_tokened.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.715214 windmill_api-1.96.1/windmill_api/api/settings/__init__.py
--rw-r--r--   0        0        0     1414 2023-05-08 19:21:01.755457 windmill_api-1.96.1/windmill_api/api/settings/backend_version.py
--rw-r--r--   0        0        0     1423 2023-05-08 19:21:01.763457 windmill_api-1.96.1/windmill_api/api/settings/get_open_api_yaml.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.743215 windmill_api-1.96.1/windmill_api/api/user/__init__.py
--rw-r--r--   0        0        0     1857 2023-05-08 19:21:01.787457 windmill_api-1.96.1/windmill_api/api/user/accept_invite.py
--rw-r--r--   0        0        0     1822 2023-05-08 19:21:01.787457 windmill_api-1.96.1/windmill_api/api/user/create_token.py
--rw-r--r--   0        0        0     1991 2023-05-08 19:21:01.835458 windmill_api-1.96.1/windmill_api/api/user/create_token_impersonate.py
--rw-r--r--   0        0        0     2058 2023-05-08 19:21:01.819458 windmill_api-1.96.1/windmill_api/api/user/create_user.py
--rw-r--r--   0        0        0     1863 2023-05-08 19:21:01.843458 windmill_api-1.96.1/windmill_api/api/user/create_user_globally.py
--rw-r--r--   0        0        0     1867 2023-05-08 19:21:01.899459 windmill_api-1.96.1/windmill_api/api/user/decline_invite.py
--rw-r--r--   0        0        0     1674 2023-05-08 19:21:01.871459 windmill_api-1.96.1/windmill_api/api/user/delete_token.py
--rw-r--r--   0        0        0     1872 2023-05-08 19:21:01.899459 windmill_api-1.96.1/windmill_api/api/user/delete_user.py
--rw-r--r--   0        0        0     1454 2023-05-08 19:21:01.923460 windmill_api-1.96.1/windmill_api/api/user/get_current_email.py
--rw-r--r--   0        0        0     1474 2023-05-08 19:21:01.939460 windmill_api-1.96.1/windmill_api/api/user/get_usage.py
--rw-r--r--   0        0        0     1639 2023-05-08 19:21:01.951460 windmill_api-1.96.1/windmill_api/api/user/global_user_delete.py
--rw-r--r--   0        0        0     2060 2023-05-08 19:21:01.967460 windmill_api-1.96.1/windmill_api/api/user/global_user_update.py
--rw-r--r--   0        0        0     2468 2023-05-08 19:21:01.987461 windmill_api-1.96.1/windmill_api/api/user/global_whoami.py
--rw-r--r--   0        0        0     2745 2023-05-08 19:21:02.007461 windmill_api-1.96.1/windmill_api/api/user/is_owner_of_path.py
--rw-r--r--   0        0        0     1646 2023-05-08 19:21:02.015461 windmill_api-1.96.1/windmill_api/api/user/leave_workspace.py
--rw-r--r--   0        0        0     2633 2023-05-08 19:21:02.043462 windmill_api-1.96.1/windmill_api/api/user/list_tokens.py
--rw-r--r--   0        0        0     2552 2023-05-08 19:21:02.055462 windmill_api-1.96.1/windmill_api/api/user/list_usernames.py
--rw-r--r--   0        0        0     3012 2023-05-08 19:21:02.083463 windmill_api-1.96.1/windmill_api/api/user/list_users.py
--rw-r--r--   0        0        0     4222 2023-05-08 19:21:02.111463 windmill_api-1.96.1/windmill_api/api/user/list_users_as_super_admin.py
--rw-r--r--   0        0        0     2829 2023-05-08 19:21:02.119463 windmill_api-1.96.1/windmill_api/api/user/list_workspace_invites.py
--rw-r--r--   0        0        0     1784 2023-05-08 19:21:02.143464 windmill_api-1.96.1/windmill_api/api/user/login.py
--rw-r--r--   0        0        0     2116 2023-05-08 19:21:02.147464 windmill_api-1.96.1/windmill_api/api/user/login_with_oauth.py
--rw-r--r--   0        0        0     1393 2023-05-08 19:21:02.167464 windmill_api-1.96.1/windmill_api/api/user/logout.py
--rw-r--r--   0        0        0     1820 2023-05-08 19:21:02.175464 windmill_api-1.96.1/windmill_api/api/user/set_password.py
--rw-r--r--   0        0        0     2250 2023-05-08 19:21:02.199465 windmill_api-1.96.1/windmill_api/api/user/update_user.py
--rw-r--r--   0        0        0     2652 2023-05-08 19:21:02.211465 windmill_api-1.96.1/windmill_api/api/user/whoami.py
--rw-r--r--   0        0        0     2967 2023-05-08 19:21:02.267466 windmill_api-1.96.1/windmill_api/api/user/whois.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.767215 windmill_api-1.96.1/windmill_api/api/variable/__init__.py
--rw-r--r--   0        0        0     2634 2023-05-08 19:21:02.247466 windmill_api-1.96.1/windmill_api/api/variable/create_variable.py
--rw-r--r--   0        0        0     1784 2023-05-08 19:21:02.295467 windmill_api-1.96.1/windmill_api/api/variable/delete_variable.py
--rw-r--r--   0        0        0     2795 2023-05-08 19:21:02.307467 windmill_api-1.96.1/windmill_api/api/variable/exists_variable.py
--rw-r--r--   0        0        0     3840 2023-05-08 19:21:02.343467 windmill_api-1.96.1/windmill_api/api/variable/get_variable.py
--rw-r--r--   0        0        0     3270 2023-05-08 19:21:02.351468 windmill_api-1.96.1/windmill_api/api/variable/list_contextual_variables.py
--rw-r--r--   0        0        0     3071 2023-05-08 19:21:02.383468 windmill_api-1.96.1/windmill_api/api/variable/list_variable.py
--rw-r--r--   0        0        0     2775 2023-05-08 19:21:02.391468 windmill_api-1.96.1/windmill_api/api/variable/update_variable.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.843216 windmill_api-1.96.1/windmill_api/api/worker/__init__.py
--rw-r--r--   0        0        0     2448 2023-05-08 19:21:02.419469 windmill_api-1.96.1/windmill_api/api/worker/get_custom_tags.py
--rw-r--r--   0        0        0     3896 2023-05-08 19:21:02.447469 windmill_api-1.96.1/windmill_api/api/worker/list_workers.py
--rw-r--r--   0        0        0        0 2023-05-08 19:20:47.755215 windmill_api-1.96.1/windmill_api/api/workspace/__init__.py
--rw-r--r--   0        0        0     2015 2023-05-08 19:21:02.451470 windmill_api-1.96.1/windmill_api/api/workspace/add_user.py
--rw-r--r--   0        0        0     1647 2023-05-08 19:21:02.475470 windmill_api-1.96.1/windmill_api/api/workspace/archive_workspace.py
--rw-r--r--   0        0        0     1856 2023-05-08 19:21:02.479470 windmill_api-1.96.1/windmill_api/api/workspace/create_workspace.py
--rw-r--r--   0        0        0     2049 2023-05-08 19:21:02.507470 windmill_api-1.96.1/windmill_api/api/workspace/delete_invite.py
--rw-r--r--   0        0        0     1688 2023-05-08 19:21:02.503471 windmill_api-1.96.1/windmill_api/api/workspace/delete_workspace.py
--rw-r--r--   0        0        0     2063 2023-05-08 19:21:02.531471 windmill_api-1.96.1/windmill_api/api/workspace/edit_auto_invite.py
--rw-r--r--   0        0        0     2083 2023-05-08 19:21:02.539471 windmill_api-1.96.1/windmill_api/api/workspace/edit_slack_command.py
--rw-r--r--   0        0        0     2029 2023-05-08 19:21:02.563471 windmill_api-1.96.1/windmill_api/api/workspace/edit_webhook.py
--rw-r--r--   0        0        0     1856 2023-05-08 19:21:02.567472 windmill_api-1.96.1/windmill_api/api/workspace/exists_username.py
--rw-r--r--   0        0        0     1856 2023-05-08 19:21:02.587472 windmill_api-1.96.1/windmill_api/api/workspace/exists_workspace.py
--rw-r--r--   0        0        0     2809 2023-05-08 19:21:02.607472 windmill_api-1.96.1/windmill_api/api/workspace/get_premium_info.py
--rw-r--r--   0        0        0     2753 2023-05-08 19:21:02.647473 windmill_api-1.96.1/windmill_api/api/workspace/get_settings.py
--rw-r--r--   0        0        0     2045 2023-05-08 19:21:02.663473 windmill_api-1.96.1/windmill_api/api/workspace/invite_user.py
--rw-r--r--   0        0        0     2176 2023-05-08 19:21:02.679474 windmill_api-1.96.1/windmill_api/api/workspace/is_domain_allowed.py
--rw-r--r--   0        0        0     3255 2023-05-08 19:21:02.707474 windmill_api-1.96.1/windmill_api/api/workspace/list_pending_invites.py
--rw-r--r--   0        0        0     2583 2023-05-08 19:21:02.715474 windmill_api-1.96.1/windmill_api/api/workspace/list_user_workspaces.py
--rw-r--r--   0        0        0     2775 2023-05-08 19:21:02.743475 windmill_api-1.96.1/windmill_api/api/workspace/list_workspaces.py
--rw-r--r--   0        0        0     4311 2023-05-08 19:21:02.767475 windmill_api-1.96.1/windmill_api/api/workspace/list_workspaces_as_super_admin.py
--rw-r--r--   0        0        0     1651 2023-05-08 19:21:02.771475 windmill_api-1.96.1/windmill_api/api/workspace/unarchive_workspace.py
--rw-r--r--   0        0        0     1821 2023-05-08 19:21:02.795476 windmill_api-1.96.1/windmill_api/client.py
--rw-r--r--   0        0        0        1 2023-05-08 19:21:20.935801 windmill_api-1.96.1/windmill_api/models/__init__.py
--rw-r--r--   0        0        0     1667 2023-05-08 19:21:02.819476 windmill_api-1.96.1/windmill_api/models/accept_invite_json_body.py
--rw-r--r--   0        0        0     1710 2023-05-08 19:21:02.847477 windmill_api-1.96.1/windmill_api/models/add_granular_acls_json_body.py
--rw-r--r--   0        0        0      325 2023-05-08 19:20:56.991370 windmill_api-1.96.1/windmill_api/models/add_granular_acls_kind.py
--rw-r--r--   0        0        0     1529 2023-05-08 19:21:02.875477 windmill_api-1.96.1/windmill_api/models/add_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1940 2023-05-08 19:21:02.903478 windmill_api-1.96.1/windmill_api/models/add_user_json_body.py
--rw-r--r--   0        0        0     1552 2023-05-08 19:21:02.923478 windmill_api-1.96.1/windmill_api/models/add_user_to_group_json_body.py
--rw-r--r--   0        0        0     3940 2023-05-08 19:21:02.955479 windmill_api-1.96.1/windmill_api/models/app_with_last_version.py
--rw-r--r--   0        0        0      214 2023-05-08 19:20:57.483378 windmill_api-1.96.1/windmill_api/models/app_with_last_version_execution_mode.py
--rw-r--r--   0        0        0     1248 2023-05-08 19:21:02.987479 windmill_api-1.96.1/windmill_api/models/app_with_last_version_extra_perms.py
--rw-r--r--   0        0        0     3716 2023-05-08 19:21:03.023480 windmill_api-1.96.1/windmill_api/models/app_with_last_version_policy.py
--rw-r--r--   0        0        0      220 2023-05-08 19:20:57.531379 windmill_api-1.96.1/windmill_api/models/app_with_last_version_policy_execution_mode.py
--rw-r--r--   0        0        0     1946 2023-05-08 19:21:03.019480 windmill_api-1.96.1/windmill_api/models/app_with_last_version_policy_triggerables.py
--rw-r--r--   0        0        0     1381 2023-05-08 19:21:03.039480 windmill_api-1.96.1/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4638 2023-05-08 19:21:03.079481 windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft.py
--rw-r--r--   0        0        0      220 2023-05-08 19:20:57.551379 windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_execution_mode.py
--rw-r--r--   0        0        0     1284 2023-05-08 19:21:03.063481 windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_extra_perms.py
--rw-r--r--   0        0        0     3828 2023-05-08 19:21:03.111482 windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_policy.py
--rw-r--r--   0        0        0      226 2023-05-08 19:20:57.095371 windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_policy_execution_mode.py
--rw-r--r--   0        0        0     2020 2023-05-08 19:21:03.103482 windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py
--rw-r--r--   0        0        0     1417 2023-05-08 19:21:03.123482 windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     1569 2023-05-08 19:21:03.139482 windmill_api-1.96.1/windmill_api/models/archive_flow_by_path_json_body.py
--rw-r--r--   0        0        0     7662 2023-05-08 19:21:03.215484 windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1314 2023-05-08 19:21:03.159483 windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      259 2023-05-08 19:20:57.767383 windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      217 2023-05-08 19:20:57.455378 windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1288 2023-05-08 19:21:03.187483 windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     3452 2023-05-08 19:21:03.239484 windmill_api-1.96.1/windmill_api/models/audit_log.py
--rw-r--r--   0        0        0      217 2023-05-08 19:20:57.523379 windmill_api-1.96.1/windmill_api/models/audit_log_action_kind.py
--rw-r--r--   0        0        0      620 2023-05-08 19:20:57.411377 windmill_api-1.96.1/windmill_api/models/audit_log_operation.py
--rw-r--r--   0        0        0     1186 2023-05-08 19:21:03.239484 windmill_api-1.96.1/windmill_api/models/audit_log_parameters.py
--rw-r--r--   0        0        0     2933 2023-05-08 19:21:03.279485 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-05-08 19:21:03.299485 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-05-08 19:20:57.431377 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-05-08 19:21:03.307485 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-05-08 19:21:03.359486 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-05-08 19:21:03.339486 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-05-08 19:21:03.403487 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-05-08 19:20:57.595380 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-05-08 19:21:03.387487 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-05-08 19:21:03.423488 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-05-08 19:20:57.535379 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-05-08 19:21:03.431488 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-05-08 19:20:56.835367 windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2377 2023-05-08 19:21:03.459488 windmill_api-1.96.1/windmill_api/models/branch_all.py
--rw-r--r--   0        0        0     2543 2023-05-08 19:21:03.471488 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item.py
--rw-r--r--   0        0        0     6620 2023-05-08 19:21:03.539490 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-05-08 19:21:03.511489 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-05-08 19:21:03.547490 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-08 19:21:03.571490 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-08 19:21:03.579490 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-08 19:20:57.503378 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-08 19:21:03.599491 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-08 19:20:57.107372 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-08 19:21:03.611491 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-08 19:21:03.627491 windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      146 2023-05-08 19:20:57.035370 windmill_api-1.96.1/windmill_api/models/branch_all_type.py
--rw-r--r--   0        0        0     2670 2023-05-08 19:21:03.651492 windmill_api-1.96.1/windmill_api/models/branch_one.py
--rw-r--r--   0        0        0     2372 2023-05-08 19:21:03.663492 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item.py
--rw-r--r--   0        0        0     6620 2023-05-08 19:21:03.735493 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-05-08 19:21:03.723493 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-05-08 19:21:03.751494 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-08 19:21:03.799494 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-08 19:21:03.779494 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-08 19:20:57.419377 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-08 19:21:03.807494 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-08 19:20:56.975369 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-08 19:21:03.831495 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-08 19:21:03.835495 windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6125 2023-05-08 19:21:03.915496 windmill_api-1.96.1/windmill_api/models/branch_one_default_item.py
--rw-r--r--   0        0        0     2906 2023-05-08 19:21:03.875496 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_retry.py
--rw-r--r--   0        0        0     1863 2023-05-08 19:21:03.903496 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-05-08 19:21:03.935497 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-05-08 19:21:03.947497 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-05-08 19:20:57.107372 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-05-08 19:21:03.963497 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-05-08 19:20:57.679381 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-05-08 19:21:03.995498 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-05-08 19:21:03.991498 windmill_api-1.96.1/windmill_api/models/branch_one_default_item_suspend.py
--rw-r--r--   0        0        0      146 2023-05-08 19:20:57.511379 windmill_api-1.96.1/windmill_api/models/branch_one_type.py
--rw-r--r--   0        0        0     1532 2023-05-08 19:21:04.015498 windmill_api-1.96.1/windmill_api/models/cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     1255 2023-05-08 19:21:04.015498 windmill_api-1.96.1/windmill_api/models/cancel_suspended_job_post_json_body.py
--rw-r--r--   0        0        0    10508 2023-05-08 19:21:04.151501 windmill_api-1.96.1/windmill_api/models/completed_job.py
--rw-r--r--   0        0        0     1176 2023-05-08 19:21:04.035499 windmill_api-1.96.1/windmill_api/models/completed_job_args.py
--rw-r--r--   0        0        0     3265 2023-05-08 19:21:04.103500 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status.py
--rw-r--r--   0        0        0     6800 2023-05-08 19:21:04.187502 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1789 2023-05-08 19:21:04.219502 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2136 2023-05-08 19:21:04.215502 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      202 2023-05-08 19:20:57.691382 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1694 2023-05-08 19:21:04.239503 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2230 2023-05-08 19:21:04.259503 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      360 2023-05-08 19:20:56.955369 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6402 2023-05-08 19:21:04.323504 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1779 2023-05-08 19:21:04.283503 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2116 2023-05-08 19:21:04.311504 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      200 2023-05-08 19:20:56.719365 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1684 2023-05-08 19:21:04.343505 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2220 2023-05-08 19:21:04.355505 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      358 2023-05-08 19:20:57.767383 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2040 2023-05-08 19:21:04.383505 windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_retry.py
--rw-r--r--   0        0        0      310 2023-05-08 19:20:57.187373 windmill_api-1.96.1/windmill_api/models/completed_job_job_kind.py
--rw-r--r--   0        0        0      199 2023-05-08 19:20:56.707365 windmill_api-1.96.1/windmill_api/models/completed_job_language.py
--rw-r--r--   0        0        0     3127 2023-05-08 19:21:04.403506 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow.py
--rw-r--r--   0        0        0     6620 2023-05-08 19:21:04.463507 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3129 2023-05-08 19:21:04.487507 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1929 2023-05-08 19:21:04.495507 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-08 19:21:04.519508 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-08 19:21:04.527508 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-08 19:20:57.279374 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-08 19:21:04.547508 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-08 19:20:57.275375 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-08 19:21:04.559508 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-08 19:21:04.575509 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6544 2023-05-08 19:21:04.675511 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3095 2023-05-08 19:21:04.615510 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1919 2023-05-08 19:21:04.643510 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2223 2023-05-08 19:21:04.675511 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2050 2023-05-08 19:21:04.707511 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      179 2023-05-08 19:20:57.079371 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1917 2023-05-08 19:21:04.703511 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      179 2023-05-08 19:20:57.115372 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1912 2023-05-08 19:21:04.731512 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1963 2023-05-08 19:21:04.739512 windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1572 2023-05-08 19:21:04.755512 windmill_api-1.96.1/windmill_api/models/connect_callback_json_body.py
--rw-r--r--   0        0        0     2533 2023-05-08 19:21:04.779513 windmill_api-1.96.1/windmill_api/models/connect_callback_response_200.py
--rw-r--r--   0        0        0     1600 2023-05-08 19:21:04.783513 windmill_api-1.96.1/windmill_api/models/connect_slack_callback_json_body.py
--rw-r--r--   0        0        0     1753 2023-05-08 19:21:04.807513 windmill_api-1.96.1/windmill_api/models/contextual_variable.py
--rw-r--r--   0        0        0     2147 2023-05-08 19:21:04.811513 windmill_api-1.96.1/windmill_api/models/create_account_json_body.py
--rw-r--r--   0        0        0     2367 2023-05-08 19:21:04.843514 windmill_api-1.96.1/windmill_api/models/create_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-05-08 19:21:04.875514 windmill_api-1.96.1/windmill_api/models/create_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-05-08 19:20:57.775383 windmill_api-1.96.1/windmill_api/models/create_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-05-08 19:21:04.871514 windmill_api-1.96.1/windmill_api/models/create_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-05-08 19:21:04.895515 windmill_api-1.96.1/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     1947 2023-05-08 19:21:04.903515 windmill_api-1.96.1/windmill_api/models/create_draft_json_body.py
--rw-r--r--   0        0        0      183 2023-05-08 19:20:57.231374 windmill_api-1.96.1/windmill_api/models/create_draft_json_body_typ.py
--rw-r--r--   0        0        0     1550 2023-05-08 19:21:04.923515 windmill_api-1.96.1/windmill_api/models/create_flow_json_body.py
--rw-r--r--   0        0        0     2126 2023-05-08 19:21:04.939515 windmill_api-1.96.1/windmill_api/models/create_folder_json_body.py
--rw-r--r--   0        0        0     1697 2023-05-08 19:21:04.951516 windmill_api-1.96.1/windmill_api/models/create_group_json_body.py
--rw-r--r--   0        0        0     1613 2023-05-08 19:21:04.963516 windmill_api-1.96.1/windmill_api/models/create_input.py
--rw-r--r--   0        0        0     1171 2023-05-08 19:21:04.975516 windmill_api-1.96.1/windmill_api/models/create_input_args.py
--rw-r--r--   0        0        0     1701 2023-05-08 19:21:04.991516 windmill_api-1.96.1/windmill_api/models/create_input_json_body.py
--rw-r--r--   0        0        0     1217 2023-05-08 19:21:05.003517 windmill_api-1.96.1/windmill_api/models/create_input_json_body_args.py
--rw-r--r--   0        0        0      214 2023-05-08 19:20:56.735365 windmill_api-1.96.1/windmill_api/models/create_input_runnable_type.py
--rw-r--r--   0        0        0     1732 2023-05-08 19:21:05.019517 windmill_api-1.96.1/windmill_api/models/create_raw_app_json_body.py
--rw-r--r--   0        0        0     2094 2023-05-08 19:21:05.071518 windmill_api-1.96.1/windmill_api/models/create_resource.py
--rw-r--r--   0        0        0     2140 2023-05-08 19:21:05.051518 windmill_api-1.96.1/windmill_api/models/create_resource_json_body.py
--rw-r--r--   0        0        0     2335 2023-05-08 19:21:05.083518 windmill_api-1.96.1/windmill_api/models/create_resource_type_json_body.py
--rw-r--r--   0        0        0     2780 2023-05-08 19:21:05.115519 windmill_api-1.96.1/windmill_api/models/create_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-05-08 19:21:05.103519 windmill_api-1.96.1/windmill_api/models/create_schedule_json_body_args.py
--rw-r--r--   0        0        0     5120 2023-05-08 19:21:05.175520 windmill_api-1.96.1/windmill_api/models/create_script_json_body.py
--rw-r--r--   0        0        0      249 2023-05-08 19:20:57.771383 windmill_api-1.96.1/windmill_api/models/create_script_json_body_kind.py
--rw-r--r--   0        0        0      207 2023-05-08 19:20:56.711365 windmill_api-1.96.1/windmill_api/models/create_script_json_body_language.py
--rw-r--r--   0        0        0     1232 2023-05-08 19:21:05.139519 windmill_api-1.96.1/windmill_api/models/create_script_json_body_schema.py
--rw-r--r--   0        0        0     2534 2023-05-08 19:21:05.179520 windmill_api-1.96.1/windmill_api/models/create_token_impersonate_json_body.py
--rw-r--r--   0        0        0     2169 2023-05-08 19:21:05.239521 windmill_api-1.96.1/windmill_api/models/create_token_json_body.py
--rw-r--r--   0        0        0     2364 2023-05-08 19:21:05.215521 windmill_api-1.96.1/windmill_api/models/create_user_globally_json_body.py
--rw-r--r--   0        0        0     1771 2023-05-08 19:21:05.243521 windmill_api-1.96.1/windmill_api/models/create_user_json_body.py
--rw-r--r--   0        0        0     2493 2023-05-08 19:21:05.275522 windmill_api-1.96.1/windmill_api/models/create_variable.py
--rw-r--r--   0        0        0     2539 2023-05-08 19:21:05.287522 windmill_api-1.96.1/windmill_api/models/create_variable_json_body.py
--rw-r--r--   0        0        0     1678 2023-05-08 19:21:05.303522 windmill_api-1.96.1/windmill_api/models/create_workspace.py
--rw-r--r--   0        0        0     1724 2023-05-08 19:21:05.315523 windmill_api-1.96.1/windmill_api/models/create_workspace_json_body.py
--rw-r--r--   0        0        0     1490 2023-05-08 19:21:05.327523 windmill_api-1.96.1/windmill_api/models/decline_invite_json_body.py
--rw-r--r--   0        0        0    11110 2023-05-08 19:21:05.491526 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200.py
--rw-r--r--   0        0        0     1270 2023-05-08 19:21:05.347523 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3658 2023-05-08 19:21:05.391524 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7442 2023-05-08 19:21:05.475525 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1883 2023-05-08 19:21:05.499526 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2318 2023-05-08 19:21:05.527526 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      219 2023-05-08 19:20:57.307375 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1788 2023-05-08 19:21:05.523526 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2324 2023-05-08 19:21:05.559527 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      377 2023-05-08 19:20:57.507378 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7053 2023-05-08 19:21:05.611528 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1873 2023-05-08 19:21:05.615528 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2298 2023-05-08 19:21:05.647529 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      217 2023-05-08 19:20:56.875368 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1778 2023-05-08 19:21:05.643529 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2314 2023-05-08 19:21:05.679529 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      375 2023-05-08 19:20:56.895368 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2134 2023-05-08 19:21:05.687529 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      327 2023-05-08 19:20:56.715365 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      216 2023-05-08 19:20:57.247374 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3432 2023-05-08 19:21:05.735530 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7425 2023-05-08 19:21:05.771531 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3442 2023-05-08 19:21:05.775531 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2023 2023-05-08 19:21:05.803532 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2327 2023-05-08 19:21:05.807532 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2261 2023-05-08 19:21:05.883533 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      198 2023-05-08 19:20:56.903368 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-08 19:21:05.839532 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      198 2023-05-08 19:20:57.495378 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2016 2023-05-08 19:21:05.867533 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2067 2023-05-08 19:21:05.895533 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7349 2023-05-08 19:21:05.971535 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3408 2023-05-08 19:21:05.935534 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2013 2023-05-08 19:21:05.983535 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2317 2023-05-08 19:21:06.007535 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2241 2023-05-08 19:21:06.015535 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-05-08 19:20:57.479378 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2108 2023-05-08 19:21:06.039536 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-05-08 19:20:57.295375 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2006 2023-05-08 19:21:06.043536 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2057 2023-05-08 19:21:06.075536 windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1783 2023-05-08 19:21:06.071536 windmill_api-1.96.1/windmill_api/models/delete_invite_json_body.py
--rw-r--r--   0        0        0     7636 2023-05-08 19:21:06.163538 windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1309 2023-05-08 19:21:06.095537 windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      258 2023-05-08 19:20:57.307375 windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      216 2023-05-08 19:20:56.795366 windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1283 2023-05-08 19:21:06.123537 windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     2933 2023-05-08 19:21:06.163538 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-05-08 19:21:06.231539 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-05-08 19:20:56.891368 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-05-08 19:21:06.195539 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-05-08 19:21:06.223539 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-05-08 19:21:06.251540 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-05-08 19:21:06.319541 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-05-08 19:20:57.291375 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-05-08 19:21:06.275540 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-05-08 19:21:06.311541 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-05-08 19:20:57.215373 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-05-08 19:21:06.335541 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-05-08 19:20:57.071371 windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     1551 2023-05-08 19:21:06.347541 windmill_api-1.96.1/windmill_api/models/edit_auto_invite_json_body.py
--rw-r--r--   0        0        0     1980 2023-05-08 19:21:06.403542 windmill_api-1.96.1/windmill_api/models/edit_resource.py
--rw-r--r--   0        0        0     1791 2023-05-08 19:21:06.379542 windmill_api-1.96.1/windmill_api/models/edit_resource_type.py
--rw-r--r--   0        0        0     1845 2023-05-08 19:21:06.411543 windmill_api-1.96.1/windmill_api/models/edit_schedule.py
--rw-r--r--   0        0        0     1176 2023-05-08 19:21:06.423543 windmill_api-1.96.1/windmill_api/models/edit_schedule_args.py
--rw-r--r--   0        0        0     1691 2023-05-08 19:21:06.435543 windmill_api-1.96.1/windmill_api/models/edit_slack_command_json_body.py
--rw-r--r--   0        0        0     2260 2023-05-08 19:21:06.459543 windmill_api-1.96.1/windmill_api/models/edit_variable.py
--rw-r--r--   0        0        0     1520 2023-05-08 19:21:06.467543 windmill_api-1.96.1/windmill_api/models/edit_webhook_json_body.py
--rw-r--r--   0        0        0     2058 2023-05-08 19:21:06.491544 windmill_api-1.96.1/windmill_api/models/edit_workspace_user.py
--rw-r--r--   0        0        0     3663 2023-05-08 19:21:06.515544 windmill_api-1.96.1/windmill_api/models/execute_component_json_body.py
--rw-r--r--   0        0        0     1346 2023-05-08 19:21:06.511544 windmill_api-1.96.1/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
--rw-r--r--   0        0        0     1942 2023-05-08 19:21:06.543545 windmill_api-1.96.1/windmill_api/models/execute_component_json_body_raw_code.py
--rw-r--r--   0        0        0     1577 2023-05-08 19:21:06.543545 windmill_api-1.96.1/windmill_api/models/exists_username_json_body.py
--rw-r--r--   0        0        0     1400 2023-05-08 19:21:06.563545 windmill_api-1.96.1/windmill_api/models/exists_workspace_json_body.py
--rw-r--r--   0        0        0     4924 2023-05-08 19:21:06.615546 windmill_api-1.96.1/windmill_api/models/flow.py
--rw-r--r--   0        0        0     1166 2023-05-08 19:21:06.583546 windmill_api-1.96.1/windmill_api/models/flow_extra_perms.py
--rw-r--r--   0        0        0     3707 2023-05-08 19:21:06.635547 windmill_api-1.96.1/windmill_api/models/flow_metadata.py
--rw-r--r--   0        0        0     1209 2023-05-08 19:21:06.639546 windmill_api-1.96.1/windmill_api/models/flow_metadata_extra_perms.py
--rw-r--r--   0        0        0     5729 2023-05-08 19:21:06.715548 windmill_api-1.96.1/windmill_api/models/flow_module.py
--rw-r--r--   0        0        0     2726 2023-05-08 19:21:06.679547 windmill_api-1.96.1/windmill_api/models/flow_module_retry.py
--rw-r--r--   0        0        0     1807 2023-05-08 19:21:06.763549 windmill_api-1.96.1/windmill_api/models/flow_module_retry_constant.py
--rw-r--r--   0        0        0     2111 2023-05-08 19:21:06.787549 windmill_api-1.96.1/windmill_api/models/flow_module_retry_exponential.py
--rw-r--r--   0        0        0     1834 2023-05-08 19:21:06.799549 windmill_api-1.96.1/windmill_api/models/flow_module_sleep_type_0.py
--rw-r--r--   0        0        0      159 2023-05-08 19:20:57.319375 windmill_api-1.96.1/windmill_api/models/flow_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1701 2023-05-08 19:21:06.815550 windmill_api-1.96.1/windmill_api/models/flow_module_sleep_type_1.py
--rw-r--r--   0        0        0      159 2023-05-08 19:20:57.015370 windmill_api-1.96.1/windmill_api/models/flow_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1800 2023-05-08 19:21:06.831550 windmill_api-1.96.1/windmill_api/models/flow_module_stop_after_if.py
--rw-r--r--   0        0        0     1851 2023-05-08 19:21:06.843550 windmill_api-1.96.1/windmill_api/models/flow_module_suspend.py
--rw-r--r--   0        0        0     3292 2023-05-08 19:21:06.879551 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0.py
--rw-r--r--   0        0        0     3564 2023-05-08 19:21:06.879551 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-08 19:21:06.911552 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-08 19:20:57.299375 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-08 19:21:06.915552 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-08 19:20:57.311375 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      208 2023-05-08 19:20:57.103371 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_language.py
--rw-r--r--   0        0        0      158 2023-05-08 19:20:57.667381 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_type.py
--rw-r--r--   0        0        0     2477 2023-05-08 19:21:06.951552 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1.py
--rw-r--r--   0        0        0     3564 2023-05-08 19:21:06.955552 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-08 19:21:06.979553 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-08 19:20:57.743383 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-08 19:21:06.991553 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-08 19:20:57.563379 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      152 2023-05-08 19:20:56.979369 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_type.py
--rw-r--r--   0        0        0     2204 2023-05-08 19:21:07.011553 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2.py
--rw-r--r--   0        0        0     3564 2023-05-08 19:21:07.031554 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-08 19:21:07.043554 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-08 19:20:57.611380 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-08 19:21:07.063554 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-08 19:20:57.599380 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      148 2023-05-08 19:20:56.971369 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_type.py
--rw-r--r--   0        0        0     4138 2023-05-08 19:21:07.099555 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3.py
--rw-r--r--   0        0        0     1990 2023-05-08 19:21:07.091555 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
--rw-r--r--   0        0        0      173 2023-05-08 19:20:57.167373 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
--rw-r--r--   0        0        0     1857 2023-05-08 19:21:07.123555 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
--rw-r--r--   0        0        0      173 2023-05-08 19:20:57.667381 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
--rw-r--r--   0        0        0     6636 2023-05-08 19:21:07.227557 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item.py
--rw-r--r--   0        0        0     3148 2023-05-08 19:21:07.199557 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
--rw-r--r--   0        0        0     1935 2023-05-08 19:21:07.231557 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-05-08 19:21:07.259558 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-05-08 19:21:07.263558 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-08 19:20:57.751383 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-05-08 19:21:07.287558 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-08 19:20:56.707365 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-05-08 19:21:07.295558 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-05-08 19:21:07.315559 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
--rw-r--r--   0        0        0      162 2023-05-08 19:20:57.115372 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_type.py
--rw-r--r--   0        0        0     2934 2023-05-08 19:21:07.339559 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4.py
--rw-r--r--   0        0        0     2508 2023-05-08 19:21:07.351559 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item.py
--rw-r--r--   0        0        0     7243 2023-05-08 19:21:07.427561 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-05-08 19:21:07.391560 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-05-08 19:21:07.419561 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-05-08 19:21:07.451561 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-05-08 19:21:07.459561 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-08 19:20:57.131372 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-05-08 19:21:07.483562 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-08 19:20:57.003370 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-05-08 19:21:07.487562 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-05-08 19:21:07.511562 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6636 2023-05-08 19:21:07.615564 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item.py
--rw-r--r--   0        0        0     3148 2023-05-08 19:21:07.599564 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
--rw-r--r--   0        0        0     1935 2023-05-08 19:21:07.631564 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-05-08 19:21:07.647565 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-05-08 19:21:07.659565 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-08 19:20:56.779366 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-05-08 19:21:07.679565 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-08 19:20:56.883368 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-05-08 19:21:07.687565 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-05-08 19:21:07.711566 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
--rw-r--r--   0        0        0      158 2023-05-08 19:20:56.783366 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_type.py
--rw-r--r--   0        0        0     2577 2023-05-08 19:21:07.727566 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5.py
--rw-r--r--   0        0        0     2679 2023-05-08 19:21:07.747567 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item.py
--rw-r--r--   0        0        0     7243 2023-05-08 19:21:07.811568 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-05-08 19:21:07.787567 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-05-08 19:21:07.815568 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-05-08 19:21:07.843568 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-05-08 19:21:07.847568 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-08 19:20:56.943369 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-05-08 19:21:07.875569 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-08 19:20:57.243374 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-05-08 19:21:07.875569 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-05-08 19:21:07.903569 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      158 2023-05-08 19:20:57.439377 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_type.py
--rw-r--r--   0        0        0     1839 2023-05-08 19:21:07.907569 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_6.py
--rw-r--r--   0        0        0      156 2023-05-08 19:20:57.623381 windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_6_type.py
--rw-r--r--   0        0        0     2009 2023-05-08 19:21:07.991571 windmill_api-1.96.1/windmill_api/models/flow_preview.py
--rw-r--r--   0        0        0     1171 2023-05-08 19:21:07.931570 windmill_api-1.96.1/windmill_api/models/flow_preview_args.py
--rw-r--r--   0        0        0     3074 2023-05-08 19:21:08.015571 windmill_api-1.96.1/windmill_api/models/flow_preview_value.py
--rw-r--r--   0        0        0     6498 2023-05-08 19:21:08.075572 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module.py
--rw-r--r--   0        0        0     3064 2023-05-08 19:21:08.055572 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_retry.py
--rw-r--r--   0        0        0     1911 2023-05-08 19:21:08.087573 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2215 2023-05-08 19:21:08.107573 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2036 2023-05-08 19:21:08.119573 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-08 19:20:57.315375 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1903 2023-05-08 19:21:08.135573 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-08 19:20:56.831367 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1904 2023-05-08 19:21:08.151574 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1955 2023-05-08 19:21:08.163574 windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6422 2023-05-08 19:21:08.247575 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item.py
--rw-r--r--   0        0        0     3030 2023-05-08 19:21:08.203575 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_retry.py
--rw-r--r--   0        0        0     1901 2023-05-08 19:21:08.231575 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2205 2023-05-08 19:21:08.263576 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2016 2023-05-08 19:21:08.279576 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-05-08 19:20:56.923369 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1883 2023-05-08 19:21:08.291576 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-05-08 19:20:56.843367 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1894 2023-05-08 19:21:08.311577 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1945 2023-05-08 19:21:08.319577 windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1143 2023-05-08 19:21:08.335577 windmill_api-1.96.1/windmill_api/models/flow_schema.py
--rw-r--r--   0        0        0     3001 2023-05-08 19:21:08.411579 windmill_api-1.96.1/windmill_api/models/flow_status.py
--rw-r--r--   0        0        0     6370 2023-05-08 19:21:08.471579 windmill_api-1.96.1/windmill_api/models/flow_status_failure_module.py
--rw-r--r--   0        0        0     1723 2023-05-08 19:21:08.439579 windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     1999 2023-05-08 19:21:08.467579 windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      190 2023-05-08 19:20:56.895368 windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1628 2023-05-08 19:21:08.495580 windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2164 2023-05-08 19:21:08.507580 windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      348 2023-05-08 19:20:57.507378 windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_type.py
--rw-r--r--   0        0        0     5808 2023-05-08 19:21:08.575581 windmill_api-1.96.1/windmill_api/models/flow_status_module.py
--rw-r--r--   0        0        0     1685 2023-05-08 19:21:08.535581 windmill_api-1.96.1/windmill_api/models/flow_status_module_approvers_item.py
--rw-r--r--   0        0        0     1925 2023-05-08 19:21:08.563581 windmill_api-1.96.1/windmill_api/models/flow_status_module_branch_chosen.py
--rw-r--r--   0        0        0      183 2023-05-08 19:20:57.563379 windmill_api-1.96.1/windmill_api/models/flow_status_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1590 2023-05-08 19:21:08.591582 windmill_api-1.96.1/windmill_api/models/flow_status_module_branchall.py
--rw-r--r--   0        0        0     2126 2023-05-08 19:21:08.611582 windmill_api-1.96.1/windmill_api/models/flow_status_module_iterator.py
--rw-r--r--   0        0        0      341 2023-05-08 19:20:57.591380 windmill_api-1.96.1/windmill_api/models/flow_status_module_type.py
--rw-r--r--   0        0        0     5981 2023-05-08 19:21:08.679583 windmill_api-1.96.1/windmill_api/models/flow_status_modules_item.py
--rw-r--r--   0        0        0     1713 2023-05-08 19:21:08.639582 windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     1979 2023-05-08 19:21:08.667583 windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      188 2023-05-08 19:20:57.227374 windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1618 2023-05-08 19:21:08.695583 windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2154 2023-05-08 19:21:08.715584 windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      346 2023-05-08 19:20:57.083371 windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_type.py
--rw-r--r--   0        0        0     1974 2023-05-08 19:21:08.795585 windmill_api-1.96.1/windmill_api/models/flow_status_retry.py
--rw-r--r--   0        0        0     2957 2023-05-08 19:21:08.755585 windmill_api-1.96.1/windmill_api/models/flow_value.py
--rw-r--r--   0        0        0     6224 2023-05-08 19:21:08.891587 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module.py
--rw-r--r--   0        0        0     2940 2023-05-08 19:21:08.835586 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1873 2023-05-08 19:21:08.863587 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-05-08 19:21:08.899587 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-05-08 19:21:08.919587 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-05-08 19:20:57.255374 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-05-08 19:21:08.931588 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-05-08 19:20:57.475378 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-05-08 19:21:08.951588 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-05-08 19:21:08.963588 windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6125 2023-05-08 19:21:09.031590 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item.py
--rw-r--r--   0        0        0     2906 2023-05-08 19:21:08.999589 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1863 2023-05-08 19:21:09.031590 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-05-08 19:21:09.063590 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-05-08 19:21:09.059590 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-05-08 19:20:57.083371 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-05-08 19:21:09.091591 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-05-08 19:20:57.275375 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-05-08 19:21:09.095591 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-05-08 19:21:09.123591 windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1858 2023-05-08 19:21:09.123591 windmill_api-1.96.1/windmill_api/models/folder.py
--rw-r--r--   0        0        0     1179 2023-05-08 19:21:09.147592 windmill_api-1.96.1/windmill_api/models/folder_extra_perms.py
--rw-r--r--   0        0        0     1560 2023-05-08 19:21:09.151592 windmill_api-1.96.1/windmill_api/models/force_cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     3807 2023-05-08 19:21:09.199592 windmill_api-1.96.1/windmill_api/models/forloop_flow.py
--rw-r--r--   0        0        0     1874 2023-05-08 19:21:09.183592 windmill_api-1.96.1/windmill_api/models/forloop_flow_iterator_type_0.py
--rw-r--r--   0        0        0      163 2023-05-08 19:20:57.439377 windmill_api-1.96.1/windmill_api/models/forloop_flow_iterator_type_0_type.py
--rw-r--r--   0        0        0     1741 2023-05-08 19:21:09.211593 windmill_api-1.96.1/windmill_api/models/forloop_flow_iterator_type_1.py
--rw-r--r--   0        0        0      163 2023-05-08 19:20:57.319375 windmill_api-1.96.1/windmill_api/models/forloop_flow_iterator_type_1_type.py
--rw-r--r--   0        0        0     6224 2023-05-08 19:21:09.339595 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item.py
--rw-r--r--   0        0        0     2940 2023-05-08 19:21:09.251593 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1873 2023-05-08 19:21:09.327595 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-05-08 19:21:09.363596 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-05-08 19:21:09.367596 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-05-08 19:20:56.743365 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-05-08 19:21:09.391596 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-05-08 19:20:57.691382 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-05-08 19:21:09.399596 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-05-08 19:21:09.419597 windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_suspend.py
--rw-r--r--   0        0        0      152 2023-05-08 19:20:56.927368 windmill_api-1.96.1/windmill_api/models/forloop_flow_type.py
--rw-r--r--   0        0        0     4052 2023-05-08 19:21:09.455597 windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200.py
--rw-r--r--   0        0        0      219 2023-05-08 19:20:57.715382 windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_execution_mode.py
--rw-r--r--   0        0        0     1279 2023-05-08 19:21:09.443597 windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     3811 2023-05-08 19:21:09.491598 windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_policy.py
--rw-r--r--   0        0        0      225 2023-05-08 19:20:57.107372 windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2009 2023-05-08 19:21:09.479598 windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1412 2023-05-08 19:21:09.503598 windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4819 2023-05-08 19:21:09.551599 windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0      228 2023-05-08 19:20:57.555379 windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_execution_mode.py
--rw-r--r--   0        0        0     1330 2023-05-08 19:21:09.527598 windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py
--rw-r--r--   0        0        0     3992 2023-05-08 19:21:09.575599 windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py
--rw-r--r--   0        0        0      234 2023-05-08 19:20:57.139372 windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2160 2023-05-08 19:21:09.579599 windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1463 2023-05-08 19:21:09.595600 windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4112 2023-05-08 19:21:09.627600 windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200.py
--rw-r--r--   0        0        0      222 2023-05-08 19:20:57.175373 windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_execution_mode.py
--rw-r--r--   0        0        0     1294 2023-05-08 19:21:09.619600 windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_extra_perms.py
--rw-r--r--   0        0        0     3862 2023-05-08 19:21:09.723602 windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_policy.py
--rw-r--r--   0        0        0      228 2023-05-08 19:20:57.479378 windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2042 2023-05-08 19:21:09.655601 windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1427 2023-05-08 19:21:09.723602 windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3764 2023-05-08 19:21:09.771603 windmill_api-1.96.1/windmill_api/models/get_audit_log_response_200.py
--rw-r--r--   0        0        0      231 2023-05-08 19:20:57.327376 windmill_api-1.96.1/windmill_api/models/get_audit_log_response_200_action_kind.py
--rw-r--r--   0        0        0      634 2023-05-08 19:20:57.611380 windmill_api-1.96.1/windmill_api/models/get_audit_log_response_200_operation.py
--rw-r--r--   0        0        0     1265 2023-05-08 19:21:09.747602 windmill_api-1.96.1/windmill_api/models/get_audit_log_response_200_parameters.py
--rw-r--r--   0        0        0    11008 2023-05-08 19:21:09.887605 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200.py
--rw-r--r--   0        0        0     1255 2023-05-08 19:21:09.791603 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3595 2023-05-08 19:21:09.831604 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7343 2023-05-08 19:21:09.915605 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1868 2023-05-08 19:21:09.915605 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2288 2023-05-08 19:21:09.943606 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      216 2023-05-08 19:20:56.983369 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1773 2023-05-08 19:21:09.943606 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2309 2023-05-08 19:21:09.975607 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      374 2023-05-08 19:20:56.715365 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6924 2023-05-08 19:21:10.035608 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1858 2023-05-08 19:21:10.003607 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-05-08 19:21:10.027608 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-05-08 19:20:57.211373 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-05-08 19:21:10.115609 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2299 2023-05-08 19:21:10.071608 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      372 2023-05-08 19:20:56.983369 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2119 2023-05-08 19:21:10.175610 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      324 2023-05-08 19:20:56.999370 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      213 2023-05-08 19:20:57.151372 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3375 2023-05-08 19:21:10.159610 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7311 2023-05-08 19:21:10.239611 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3391 2023-05-08 19:21:10.215611 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2008 2023-05-08 19:21:10.243611 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2312 2023-05-08 19:21:10.267612 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2231 2023-05-08 19:21:10.275612 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      195 2023-05-08 19:20:57.003370 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2098 2023-05-08 19:21:10.295612 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      195 2023-05-08 19:20:57.639381 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2001 2023-05-08 19:21:10.307613 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2052 2023-05-08 19:21:10.323613 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7235 2023-05-08 19:21:10.395614 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3357 2023-05-08 19:21:10.363613 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1998 2023-05-08 19:21:10.391614 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-05-08 19:21:10.423615 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-05-08 19:21:10.431615 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-08 19:20:57.303375 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-05-08 19:21:10.503616 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-08 19:20:57.175373 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-05-08 19:21:10.467615 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-05-08 19:21:10.499616 windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     5374 2023-05-08 19:21:10.655619 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200.py
--rw-r--r--   0        0        0     1281 2023-05-08 19:21:10.523616 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     1258 2023-05-08 19:21:10.543617 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_schema.py
--rw-r--r--   0        0        0     3302 2023-05-08 19:21:10.583617 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value.py
--rw-r--r--   0        0        0     7159 2023-05-08 19:21:10.663619 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
--rw-r--r--   0        0        0     3323 2023-05-08 19:21:10.695619 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
--rw-r--r--   0        0        0     1988 2023-05-08 19:21:10.691619 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-05-08 19:21:10.723620 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-05-08 19:21:10.727620 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-05-08 19:20:56.691365 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-05-08 19:21:10.751620 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-05-08 19:20:56.759366 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-05-08 19:21:10.759621 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-05-08 19:21:10.779621 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7066 2023-05-08 19:21:10.843622 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
--rw-r--r--   0        0        0     3289 2023-05-08 19:21:10.819622 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
--rw-r--r--   0        0        0     1978 2023-05-08 19:21:10.895623 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2282 2023-05-08 19:21:10.875623 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2171 2023-05-08 19:21:10.907623 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-05-08 19:20:56.703365 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2038 2023-05-08 19:21:10.923623 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-05-08 19:20:57.107372 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1971 2023-05-08 19:21:10.935624 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2022 2023-05-08 19:21:10.951624 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2093 2023-05-08 19:21:10.967624 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0     5695 2023-05-08 19:21:11.019625 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py
--rw-r--r--   0        0        0     1360 2023-05-08 19:21:11.059626 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py
--rw-r--r--   0        0        0     1337 2023-05-08 19:21:11.039626 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py
--rw-r--r--   0        0        0     3559 2023-05-08 19:21:11.083626 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py
--rw-r--r--   0        0        0     7829 2023-05-08 19:21:11.147627 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py
--rw-r--r--   0        0        0     3606 2023-05-08 19:21:11.119627 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py
--rw-r--r--   0        0        0     2067 2023-05-08 19:21:11.147627 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2371 2023-05-08 19:21:11.183628 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2343 2023-05-08 19:21:11.179628 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      205 2023-05-08 19:20:56.919368 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2210 2023-05-08 19:21:11.207629 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      205 2023-05-08 19:20:57.019370 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2060 2023-05-08 19:21:11.211629 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2111 2023-05-08 19:21:11.291630 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7685 2023-05-08 19:21:11.299630 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py
--rw-r--r--   0        0        0     3542 2023-05-08 19:21:11.335631 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py
--rw-r--r--   0        0        0     2057 2023-05-08 19:21:11.331631 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2361 2023-05-08 19:21:11.367632 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2323 2023-05-08 19:21:11.363631 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      203 2023-05-08 19:20:56.871368 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2190 2023-05-08 19:21:11.391632 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      203 2023-05-08 19:20:57.739382 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2050 2023-05-08 19:21:11.395632 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2101 2023-05-08 19:21:11.419633 windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2756 2023-05-08 19:21:11.503634 windmill_api-1.96.1/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
--rw-r--r--   0        0        0     1337 2023-05-08 19:21:11.439633 windmill_api-1.96.1/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
--rw-r--r--   0        0        0     2010 2023-05-08 19:21:11.471633 windmill_api-1.96.1/windmill_api/models/get_folder_response_200.py
--rw-r--r--   0        0        0     1258 2023-05-08 19:21:11.491634 windmill_api-1.96.1/windmill_api/models/get_folder_response_200_extra_perms.py
--rw-r--r--   0        0        0     2357 2023-05-08 19:21:11.527634 windmill_api-1.96.1/windmill_api/models/get_folder_usage_response_200.py
--rw-r--r--   0        0        0      325 2023-05-08 19:20:56.931369 windmill_api-1.96.1/windmill_api/models/get_granular_acls_kind.py
--rw-r--r--   0        0        0     1235 2023-05-08 19:21:11.523634 windmill_api-1.96.1/windmill_api/models/get_granular_acls_response_200.py
--rw-r--r--   0        0        0     2888 2023-05-08 19:21:11.571635 windmill_api-1.96.1/windmill_api/models/get_group_response_200.py
--rw-r--r--   0        0        0     1253 2023-05-08 19:21:11.547635 windmill_api-1.96.1/windmill_api/models/get_group_response_200_extra_perms.py
--rw-r--r--   0        0        0     1606 2023-05-08 19:21:11.567635 windmill_api-1.96.1/windmill_api/models/get_hub_app_by_id_response_200.py
--rw-r--r--   0        0        0     1634 2023-05-08 19:21:11.595636 windmill_api-1.96.1/windmill_api/models/get_hub_app_by_id_response_200_app.py
--rw-r--r--   0        0        0     1977 2023-05-08 19:21:11.603636 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200.py
--rw-r--r--   0        0        0     2950 2023-05-08 19:21:11.635636 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
--rw-r--r--   0        0        0     1289 2023-05-08 19:21:11.623636 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
--rw-r--r--   0        0        0     3410 2023-05-08 19:21:11.667637 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
--rw-r--r--   0        0        0     7365 2023-05-08 19:21:11.767639 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
--rw-r--r--   0        0        0     3418 2023-05-08 19:21:11.707638 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     2019 2023-05-08 19:21:11.735638 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2323 2023-05-08 19:21:11.771639 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2249 2023-05-08 19:21:11.795639 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-05-08 19:20:57.475378 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2116 2023-05-08 19:21:11.799639 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-05-08 19:20:56.979369 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2012 2023-05-08 19:21:11.823640 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2063 2023-05-08 19:21:11.831640 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7289 2023-05-08 19:21:11.907641 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
--rw-r--r--   0        0        0     3384 2023-05-08 19:21:11.943642 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     2009 2023-05-08 19:21:11.935642 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2313 2023-05-08 19:21:11.967642 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2229 2023-05-08 19:21:11.975642 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      194 2023-05-08 19:20:57.783383 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2096 2023-05-08 19:21:11.995643 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      194 2023-05-08 19:20:57.551379 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2002 2023-05-08 19:21:12.007643 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2053 2023-05-08 19:21:12.023643 windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2698 2023-05-08 19:21:12.047644 windmill_api-1.96.1/windmill_api/models/get_hub_script_by_path_response_200.py
--rw-r--r--   0        0        0      216 2023-05-08 19:20:57.723382 windmill_api-1.96.1/windmill_api/models/get_hub_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     2644 2023-05-08 19:21:12.063644 windmill_api-1.96.1/windmill_api/models/get_input_history_response_200_item.py
--rw-r--r--   0        0        0     1278 2023-05-08 19:21:12.067644 windmill_api-1.96.1/windmill_api/models/get_input_history_response_200_item_args.py
--rw-r--r--   0        0        0      218 2023-05-08 19:20:57.079371 windmill_api-1.96.1/windmill_api/models/get_input_history_runnable_type.py
--rw-r--r--   0        0        0     1852 2023-05-08 19:21:12.159646 windmill_api-1.96.1/windmill_api/models/get_job_response_200.py
--rw-r--r--   0        0        0      188 2023-05-08 19:20:57.259374 windmill_api-1.96.1/windmill_api/models/get_job_response_200_type.py
--rw-r--r--   0        0        0     2364 2023-05-08 19:21:12.107645 windmill_api-1.96.1/windmill_api/models/get_job_updates_response_200.py
--rw-r--r--   0        0        0     1744 2023-05-08 19:21:12.135645 windmill_api-1.96.1/windmill_api/models/get_premium_info_response_200.py
--rw-r--r--   0        0        0     4218 2023-05-08 19:21:12.191646 windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200.py
--rw-r--r--   0        0        0      227 2023-05-08 19:20:56.715365 windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
--rw-r--r--   0        0        0     1322 2023-05-08 19:21:12.183646 windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
--rw-r--r--   0        0        0     3970 2023-05-08 19:21:12.231647 windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_policy.py
--rw-r--r--   0        0        0      233 2023-05-08 19:20:57.147372 windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2131 2023-05-08 19:21:12.219647 windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1455 2023-05-08 19:21:12.239647 windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3533 2023-05-08 19:21:12.279648 windmill_api-1.96.1/windmill_api/models/get_resource_response_200.py
--rw-r--r--   0        0        0     1268 2023-05-08 19:21:12.259647 windmill_api-1.96.1/windmill_api/models/get_resource_response_200_extra_perms.py
--rw-r--r--   0        0        0     2335 2023-05-08 19:21:12.371650 windmill_api-1.96.1/windmill_api/models/get_resource_type_response_200.py
--rw-r--r--   0        0        0     1840 2023-05-08 19:21:12.307648 windmill_api-1.96.1/windmill_api/models/get_resume_urls_response_200.py
--rw-r--r--   0        0        0     4325 2023-05-08 19:21:12.367649 windmill_api-1.96.1/windmill_api/models/get_schedule_response_200.py
--rw-r--r--   0        0        0     1232 2023-05-08 19:21:12.387650 windmill_api-1.96.1/windmill_api/models/get_schedule_response_200_args.py
--rw-r--r--   0        0        0     1268 2023-05-08 19:21:12.391650 windmill_api-1.96.1/windmill_api/models/get_schedule_response_200_extra_perms.py
--rw-r--r--   0        0        0     7558 2023-05-08 19:21:12.479652 windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1294 2023-05-08 19:21:12.411650 windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-08 19:20:57.775383 windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-05-08 19:20:57.239374 windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-05-08 19:21:12.439651 windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     7558 2023-05-08 19:21:12.531652 windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200.py
--rw-r--r--   0        0        0     1294 2023-05-08 19:21:12.571653 windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-08 19:20:57.439377 windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-05-08 19:20:57.255374 windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-05-08 19:21:12.555653 windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200_schema.py
--rw-r--r--   0        0        0     6383 2023-05-08 19:21:12.639654 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0     5608 2023-05-08 19:21:12.643654 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py
--rw-r--r--   0        0        0      269 2023-05-08 19:20:57.035370 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_kind.py
--rw-r--r--   0        0        0      227 2023-05-08 19:20:57.751383 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_language.py
--rw-r--r--   0        0        0     1347 2023-05-08 19:21:12.667655 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py
--rw-r--r--   0        0        0      264 2023-05-08 19:20:56.835367 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_kind.py
--rw-r--r--   0        0        0      222 2023-05-08 19:20:57.735382 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_language.py
--rw-r--r--   0        0        0     1319 2023-05-08 19:21:12.671655 windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py
--rw-r--r--   0        0        0     1922 2023-05-08 19:21:12.695655 windmill_api-1.96.1/windmill_api/models/get_script_deployment_status_response_200.py
--rw-r--r--   0        0        0     4157 2023-05-08 19:21:12.811658 windmill_api-1.96.1/windmill_api/models/get_settings_response_200.py
--rw-r--r--   0        0        0     2428 2023-05-08 19:21:12.727656 windmill_api-1.96.1/windmill_api/models/get_suspended_job_flow_response_200.py
--rw-r--r--   0        0        0     1764 2023-05-08 19:21:12.755656 windmill_api-1.96.1/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
--rw-r--r--   0        0        0     2040 2023-05-08 19:21:12.783657 windmill_api-1.96.1/windmill_api/models/get_suspended_job_flow_response_200_job.py
--rw-r--r--   0        0        0      204 2023-05-08 19:20:56.767366 windmill_api-1.96.1/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
--rw-r--r--   0        0        0     4554 2023-05-08 19:21:12.847658 windmill_api-1.96.1/windmill_api/models/get_variable_response_200.py
--rw-r--r--   0        0        0     1268 2023-05-08 19:21:12.831658 windmill_api-1.96.1/windmill_api/models/get_variable_response_200_extra_perms.py
--rw-r--r--   0        0        0     2647 2023-05-08 19:21:12.875659 windmill_api-1.96.1/windmill_api/models/global_user_info.py
--rw-r--r--   0        0        0      176 2023-05-08 19:20:57.151372 windmill_api-1.96.1/windmill_api/models/global_user_info_login_type.py
--rw-r--r--   0        0        0     1627 2023-05-08 19:21:12.871658 windmill_api-1.96.1/windmill_api/models/global_user_update_json_body.py
--rw-r--r--   0        0        0     2741 2023-05-08 19:21:12.911659 windmill_api-1.96.1/windmill_api/models/global_whoami_response_200.py
--rw-r--r--   0        0        0      185 2023-05-08 19:20:56.875368 windmill_api-1.96.1/windmill_api/models/global_whoami_response_200_login_type.py
--rw-r--r--   0        0        0     2903 2023-05-08 19:21:12.919659 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5478 2023-05-08 19:21:13.039662 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      324 2023-05-08 19:20:57.219374 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1598 2023-05-08 19:21:12.947660 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1663 2023-05-08 19:21:12.971660 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2151 2023-05-08 19:21:13.003661 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3257 2023-05-08 19:21:13.043662 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      342 2023-05-08 19:20:56.719365 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1631 2023-05-08 19:21:13.063662 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3100 2023-05-08 19:21:13.079662 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      333 2023-05-08 19:20:56.903368 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1580 2023-05-08 19:21:13.091663 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      178 2023-05-08 19:20:57.127372 windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2722 2023-05-08 19:21:13.127663 windmill_api-1.96.1/windmill_api/models/group.py
--rw-r--r--   0        0        0     1174 2023-05-08 19:21:13.111663 windmill_api-1.96.1/windmill_api/models/group_extra_perms.py
--rw-r--r--   0        0        0     1689 2023-05-08 19:21:13.139663 windmill_api-1.96.1/windmill_api/models/identity.py
--rw-r--r--   0        0        0      143 2023-05-08 19:20:57.011370 windmill_api-1.96.1/windmill_api/models/identity_type.py
--rw-r--r--   0        0        0     2377 2023-05-08 19:21:13.171664 windmill_api-1.96.1/windmill_api/models/input_.py
--rw-r--r--   0        0        0     1138 2023-05-08 19:21:13.159664 windmill_api-1.96.1/windmill_api/models/input_args.py
--rw-r--r--   0        0        0     1820 2023-05-08 19:21:13.187664 windmill_api-1.96.1/windmill_api/models/input_transform_type_0.py
--rw-r--r--   0        0        0      158 2023-05-08 19:20:57.151372 windmill_api-1.96.1/windmill_api/models/input_transform_type_0_type.py
--rw-r--r--   0        0        0     1687 2023-05-08 19:21:13.275666 windmill_api-1.96.1/windmill_api/models/input_transform_type_1.py
--rw-r--r--   0        0        0      158 2023-05-08 19:20:57.615380 windmill_api-1.96.1/windmill_api/models/input_transform_type_1_type.py
--rw-r--r--   0        0        0     1773 2023-05-08 19:21:13.219665 windmill_api-1.96.1/windmill_api/models/invite_user_json_body.py
--rw-r--r--   0        0        0     1679 2023-05-08 19:21:13.243665 windmill_api-1.96.1/windmill_api/models/javascript_transform.py
--rw-r--r--   0        0        0      158 2023-05-08 19:20:57.163373 windmill_api-1.96.1/windmill_api/models/javascript_transform_type.py
--rw-r--r--   0        0        0     1686 2023-05-08 19:21:13.275666 windmill_api-1.96.1/windmill_api/models/job.py
--rw-r--r--   0        0        0      174 2023-05-08 19:20:57.651381 windmill_api-1.96.1/windmill_api/models/job_type.py
--rw-r--r--   0        0        0     3583 2023-05-08 19:21:13.323667 windmill_api-1.96.1/windmill_api/models/list_apps_response_200_item.py
--rw-r--r--   0        0        0      219 2023-05-08 19:20:56.851367 windmill_api-1.96.1/windmill_api/models/list_apps_response_200_item_execution_mode.py
--rw-r--r--   0        0        0     1276 2023-05-08 19:21:13.299666 windmill_api-1.96.1/windmill_api/models/list_apps_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      218 2023-05-08 19:20:57.307375 windmill_api-1.96.1/windmill_api/models/list_audit_logs_action_kind.py
--rw-r--r--   0        0        0     3896 2023-05-08 19:21:13.411668 windmill_api-1.96.1/windmill_api/models/list_audit_logs_response_200_item.py
--rw-r--r--   0        0        0      237 2023-05-08 19:20:57.723382 windmill_api-1.96.1/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
--rw-r--r--   0        0        0      640 2023-05-08 19:20:57.279374 windmill_api-1.96.1/windmill_api/models/list_audit_logs_response_200_item_operation.py
--rw-r--r--   0        0        0     1298 2023-05-08 19:21:13.351667 windmill_api-1.96.1/windmill_api/models/list_audit_logs_response_200_item_parameters.py
--rw-r--r--   0        0        0    11220 2023-05-08 19:21:13.491670 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item.py
--rw-r--r--   0        0        0     1288 2023-05-08 19:21:13.431669 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_args.py
--rw-r--r--   0        0        0     3736 2023-05-08 19:21:13.475669 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7579 2023-05-08 19:21:13.559671 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1901 2023-05-08 19:21:13.515670 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2352 2023-05-08 19:21:13.543671 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      222 2023-05-08 19:20:56.967369 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1806 2023-05-08 19:21:13.575671 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2342 2023-05-08 19:21:13.595672 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      380 2023-05-08 19:20:57.151372 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7160 2023-05-08 19:21:13.751674 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1891 2023-05-08 19:21:13.623672 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2332 2023-05-08 19:21:13.651672 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      220 2023-05-08 19:20:57.055371 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1796 2023-05-08 19:21:13.675673 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2332 2023-05-08 19:21:13.711674 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      378 2023-05-08 19:20:57.227374 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2152 2023-05-08 19:21:13.743674 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      330 2023-05-08 19:20:57.615380 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
--rw-r--r--   0        0        0      219 2023-05-08 19:20:57.223374 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_language.py
--rw-r--r--   0        0        0     3485 2023-05-08 19:21:13.863676 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7593 2023-05-08 19:21:13.835676 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3498 2023-05-08 19:21:13.875676 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2041 2023-05-08 19:21:13.891677 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2345 2023-05-08 19:21:13.911677 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2295 2023-05-08 19:21:13.919677 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      201 2023-05-08 19:20:56.683364 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2162 2023-05-08 19:21:13.939678 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      201 2023-05-08 19:20:57.347376 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2034 2023-05-08 19:21:13.947678 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2085 2023-05-08 19:21:13.971678 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7471 2023-05-08 19:21:14.031679 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3464 2023-05-08 19:21:14.015679 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2031 2023-05-08 19:21:14.043680 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2335 2023-05-08 19:21:14.063680 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2275 2023-05-08 19:21:14.075680 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      199 2023-05-08 19:20:56.703365 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2142 2023-05-08 19:21:14.091680 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      199 2023-05-08 19:20:57.023370 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2024 2023-05-08 19:21:14.187682 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2075 2023-05-08 19:21:14.119681 windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1865 2023-05-08 19:21:14.151682 windmill_api-1.96.1/windmill_api/models/list_contextual_variables_response_200_item.py
--rw-r--r--   0        0        0     1863 2023-05-08 19:21:14.255683 windmill_api-1.96.1/windmill_api/models/list_flows_response_200_item.py
--rw-r--r--   0        0        0     2074 2023-05-08 19:21:14.231683 windmill_api-1.96.1/windmill_api/models/list_folders_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-05-08 19:21:14.251683 windmill_api-1.96.1/windmill_api/models/list_folders_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2958 2023-05-08 19:21:14.299684 windmill_api-1.96.1/windmill_api/models/list_groups_response_200_item.py
--rw-r--r--   0        0        0     1286 2023-05-08 19:21:14.275683 windmill_api-1.96.1/windmill_api/models/list_groups_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2076 2023-05-08 19:21:14.307684 windmill_api-1.96.1/windmill_api/models/list_hub_apps_response_200.py
--rw-r--r--   0        0        0     2304 2023-05-08 19:21:14.335685 windmill_api-1.96.1/windmill_api/models/list_hub_apps_response_200_apps_item.py
--rw-r--r--   0        0        0     2116 2023-05-08 19:21:14.339685 windmill_api-1.96.1/windmill_api/models/list_hub_flows_response_200.py
--rw-r--r--   0        0        0     2324 2023-05-08 19:21:14.371685 windmill_api-1.96.1/windmill_api/models/list_hub_flows_response_200_flows_item.py
--rw-r--r--   0        0        0     2106 2023-05-08 19:21:14.371685 windmill_api-1.96.1/windmill_api/models/list_hub_scripts_response_200.py
--rw-r--r--   0        0        0     2790 2023-05-08 19:21:14.407686 windmill_api-1.96.1/windmill_api/models/list_hub_scripts_response_200_asks_item.py
--rw-r--r--   0        0        0      262 2023-05-08 19:20:57.403377 windmill_api-1.96.1/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
--rw-r--r--   0        0        0     2590 2023-05-08 19:21:14.411686 windmill_api-1.96.1/windmill_api/models/list_inputs_response_200_item.py
--rw-r--r--   0        0        0     1250 2023-05-08 19:21:14.431686 windmill_api-1.96.1/windmill_api/models/list_inputs_response_200_item_args.py
--rw-r--r--   0        0        0      213 2023-05-08 19:20:57.255374 windmill_api-1.96.1/windmill_api/models/list_inputs_runnable_type.py
--rw-r--r--   0        0        0     1922 2023-05-08 19:21:14.443687 windmill_api-1.96.1/windmill_api/models/list_jobs_response_200_item.py
--rw-r--r--   0        0        0      194 2023-05-08 19:20:56.683364 windmill_api-1.96.1/windmill_api/models/list_jobs_response_200_item_type.py
--rw-r--r--   0        0        0     2076 2023-05-08 19:21:14.463687 windmill_api-1.96.1/windmill_api/models/list_pending_invites_response_200_item.py
--rw-r--r--   0        0        0    12114 2023-05-08 19:21:14.691691 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item.py
--rw-r--r--   0        0        0     1245 2023-05-08 19:21:14.483687 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_args.py
--rw-r--r--   0        0        0     3544 2023-05-08 19:21:14.567689 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7247 2023-05-08 19:21:14.743692 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1858 2023-05-08 19:21:14.715691 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-05-08 19:21:14.747692 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-05-08 19:20:57.787383 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-05-08 19:21:14.771692 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2299 2023-05-08 19:21:14.783692 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      372 2023-05-08 19:20:57.359376 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6858 2023-05-08 19:21:14.855694 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1848 2023-05-08 19:21:14.807693 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2248 2023-05-08 19:21:14.839694 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      212 2023-05-08 19:20:57.599380 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1753 2023-05-08 19:21:14.867694 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2289 2023-05-08 19:21:14.891694 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      370 2023-05-08 19:20:57.107372 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2109 2023-05-08 19:21:14.903695 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      322 2023-05-08 19:20:57.795383 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_job_kind.py
--rw-r--r--   0        0        0      211 2023-05-08 19:20:57.251374 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_language.py
--rw-r--r--   0        0        0     3334 2023-05-08 19:21:14.935695 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7235 2023-05-08 19:21:14.987696 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3357 2023-05-08 19:21:14.975696 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1998 2023-05-08 19:21:15.079698 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-05-08 19:21:15.019697 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-05-08 19:21:15.047697 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-08 19:20:57.459378 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-05-08 19:21:15.079698 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-08 19:20:57.099372 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-05-08 19:21:15.183700 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-05-08 19:21:15.107698 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7159 2023-05-08 19:21:15.191700 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3323 2023-05-08 19:21:15.227700 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1988 2023-05-08 19:21:15.219700 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-05-08 19:21:15.251701 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-05-08 19:21:15.255701 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-05-08 19:20:57.251374 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-05-08 19:21:15.279701 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-05-08 19:20:56.987370 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-05-08 19:21:15.287701 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-05-08 19:21:15.307702 windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     3045 2023-05-08 19:21:15.331702 windmill_api-1.96.1/windmill_api/models/list_raw_apps_response_200_item.py
--rw-r--r--   0        0        0     1294 2023-05-08 19:21:15.327702 windmill_api-1.96.1/windmill_api/models/list_raw_apps_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     4884 2023-05-08 19:21:15.391703 windmill_api-1.96.1/windmill_api/models/list_resource_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-05-08 19:21:15.351703 windmill_api-1.96.1/windmill_api/models/list_resource_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2363 2023-05-08 19:21:15.387703 windmill_api-1.96.1/windmill_api/models/list_resource_type_response_200_item.py
--rw-r--r--   0        0        0     4426 2023-05-08 19:21:15.443704 windmill_api-1.96.1/windmill_api/models/list_schedules_response_200_item.py
--rw-r--r--   0        0        0     1265 2023-05-08 19:21:15.479705 windmill_api-1.96.1/windmill_api/models/list_schedules_response_200_item_args.py
--rw-r--r--   0        0        0     1301 2023-05-08 19:21:15.463704 windmill_api-1.96.1/windmill_api/models/list_schedules_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     7551 2023-05-08 19:21:15.631708 windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-05-08 19:21:15.499705 windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-08 19:20:57.543379 windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item_kind.py
--rw-r--r--   0        0        0      213 2023-05-08 19:20:57.539379 windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item_language.py
--rw-r--r--   0        0        0     1265 2023-05-08 19:21:15.523706 windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item_schema.py
--rw-r--r--   0        0        0     2985 2023-05-08 19:21:15.563706 windmill_api-1.96.1/windmill_api/models/list_tokens_response_200_item.py
--rw-r--r--   0        0        0     2250 2023-05-08 19:21:15.591707 windmill_api-1.96.1/windmill_api/models/list_user_workspaces_response_200.py
--rw-r--r--   0        0        0     1833 2023-05-08 19:21:15.623707 windmill_api-1.96.1/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
--rw-r--r--   0        0        0     2896 2023-05-08 19:21:15.659708 windmill_api-1.96.1/windmill_api/models/list_users_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0      198 2023-05-08 19:20:57.559379 windmill_api-1.96.1/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
--rw-r--r--   0        0        0     4307 2023-05-08 19:21:15.703709 windmill_api-1.96.1/windmill_api/models/list_users_response_200_item.py
--rw-r--r--   0        0        0     1613 2023-05-08 19:21:15.683709 windmill_api-1.96.1/windmill_api/models/list_users_response_200_item_usage.py
--rw-r--r--   0        0        0     4608 2023-05-08 19:21:15.779710 windmill_api-1.96.1/windmill_api/models/list_variable_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-05-08 19:21:15.735709 windmill_api-1.96.1/windmill_api/models/list_variable_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2693 2023-05-08 19:21:15.779710 windmill_api-1.96.1/windmill_api/models/list_workers_response_200_item.py
--rw-r--r--   0        0        0     2086 2023-05-08 19:21:15.811711 windmill_api-1.96.1/windmill_api/models/list_workspace_invites_response_200_item.py
--rw-r--r--   0        0        0     2082 2023-05-08 19:21:15.815711 windmill_api-1.96.1/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0     2013 2023-05-08 19:21:15.847711 windmill_api-1.96.1/windmill_api/models/list_workspaces_response_200_item.py
--rw-r--r--   0        0        0     3388 2023-05-08 19:21:15.859712 windmill_api-1.96.1/windmill_api/models/listable_app.py
--rw-r--r--   0        0        0      207 2023-05-08 19:20:57.343376 windmill_api-1.96.1/windmill_api/models/listable_app_execution_mode.py
--rw-r--r--   0        0        0     1207 2023-05-08 19:21:15.867712 windmill_api-1.96.1/windmill_api/models/listable_app_extra_perms.py
--rw-r--r--   0        0        0     2913 2023-05-08 19:21:15.899712 windmill_api-1.96.1/windmill_api/models/listable_raw_app.py
--rw-r--r--   0        0        0     1225 2023-05-08 19:21:15.887712 windmill_api-1.96.1/windmill_api/models/listable_raw_app_extra_perms.py
--rw-r--r--   0        0        0     4751 2023-05-08 19:21:15.955713 windmill_api-1.96.1/windmill_api/models/listable_resource.py
--rw-r--r--   0        0        0     1232 2023-05-08 19:21:15.919713 windmill_api-1.96.1/windmill_api/models/listable_resource_extra_perms.py
--rw-r--r--   0        0        0     4486 2023-05-08 19:21:16.055715 windmill_api-1.96.1/windmill_api/models/listable_variable.py
--rw-r--r--   0        0        0     1232 2023-05-08 19:21:15.975714 windmill_api-1.96.1/windmill_api/models/listable_variable_extra_perms.py
--rw-r--r--   0        0        0     1513 2023-05-08 19:21:15.999714 windmill_api-1.96.1/windmill_api/models/login.py
--rw-r--r--   0        0        0     1559 2023-05-08 19:21:16.027715 windmill_api-1.96.1/windmill_api/models/login_json_body.py
--rw-r--r--   0        0        0     1739 2023-05-08 19:21:16.127716 windmill_api-1.96.1/windmill_api/models/login_with_oauth_json_body.py
--rw-r--r--   0        0        0     2758 2023-05-08 19:21:16.095716 windmill_api-1.96.1/windmill_api/models/main_arg_signature.py
--rw-r--r--   0        0        0     5099 2023-05-08 19:21:16.151717 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item.py
--rw-r--r--   0        0        0      315 2023-05-08 19:20:57.367376 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1547 2023-05-08 19:21:16.155717 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1612 2023-05-08 19:21:16.179717 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2044 2023-05-08 19:21:16.183717 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3049 2023-05-08 19:21:16.215718 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      333 2023-05-08 19:20:56.815367 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1580 2023-05-08 19:21:16.211718 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     2862 2023-05-08 19:21:16.247718 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
--rw-r--r--   0        0        0      324 2023-05-08 19:20:56.851367 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1529 2023-05-08 19:21:16.239718 windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      169 2023-05-08 19:20:56.815367 windmill_api-1.96.1/windmill_api/models/main_arg_signature_type.py
--rw-r--r--   0        0        0     2662 2023-05-08 19:21:16.279719 windmill_api-1.96.1/windmill_api/models/new_schedule.py
--rw-r--r--   0        0        0     1171 2023-05-08 19:21:16.263719 windmill_api-1.96.1/windmill_api/models/new_schedule_args.py
--rw-r--r--   0        0        0     4866 2023-05-08 19:21:16.339720 windmill_api-1.96.1/windmill_api/models/new_script.py
--rw-r--r--   0        0        0      238 2023-05-08 19:20:57.407377 windmill_api-1.96.1/windmill_api/models/new_script_kind.py
--rw-r--r--   0        0        0      196 2023-05-08 19:20:57.567380 windmill_api-1.96.1/windmill_api/models/new_script_language.py
--rw-r--r--   0        0        0     1171 2023-05-08 19:21:16.303719 windmill_api-1.96.1/windmill_api/models/new_script_schema.py
--rw-r--r--   0        0        0     5879 2023-05-08 19:21:16.467722 windmill_api-1.96.1/windmill_api/models/new_script_with_draft.py
--rw-r--r--   0        0        0     5192 2023-05-08 19:21:16.411721 windmill_api-1.96.1/windmill_api/models/new_script_with_draft_draft.py
--rw-r--r--   0        0        0      252 2023-05-08 19:20:57.027370 windmill_api-1.96.1/windmill_api/models/new_script_with_draft_draft_kind.py
--rw-r--r--   0        0        0      210 2023-05-08 19:20:57.099372 windmill_api-1.96.1/windmill_api/models/new_script_with_draft_draft_language.py
--rw-r--r--   0        0        0     1250 2023-05-08 19:21:16.435722 windmill_api-1.96.1/windmill_api/models/new_script_with_draft_draft_schema.py
--rw-r--r--   0        0        0      247 2023-05-08 19:20:56.739365 windmill_api-1.96.1/windmill_api/models/new_script_with_draft_kind.py
--rw-r--r--   0        0        0      205 2023-05-08 19:20:57.095371 windmill_api-1.96.1/windmill_api/models/new_script_with_draft_language.py
--rw-r--r--   0        0        0     1222 2023-05-08 19:21:16.455722 windmill_api-1.96.1/windmill_api/models/new_script_with_draft_schema.py
--rw-r--r--   0        0        0     2108 2023-05-08 19:21:16.567724 windmill_api-1.96.1/windmill_api/models/new_token.py
--rw-r--r--   0        0        0     2473 2023-05-08 19:21:16.503723 windmill_api-1.96.1/windmill_api/models/new_token_impersonate.py
--rw-r--r--   0        0        0     1710 2023-05-08 19:21:16.531723 windmill_api-1.96.1/windmill_api/models/new_user.py
--rw-r--r--   0        0        0     2584 2023-05-08 19:21:16.571724 windmill_api-1.96.1/windmill_api/models/open_flow.py
--rw-r--r--   0        0        0     1166 2023-05-08 19:21:16.591724 windmill_api-1.96.1/windmill_api/models/open_flow_schema.py
--rw-r--r--   0        0        0     3026 2023-05-08 19:21:16.611725 windmill_api-1.96.1/windmill_api/models/open_flow_value.py
--rw-r--r--   0        0        0     6384 2023-05-08 19:21:16.671726 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module.py
--rw-r--r--   0        0        0     3013 2023-05-08 19:21:16.651725 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1896 2023-05-08 19:21:16.679726 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2200 2023-05-08 19:21:16.703726 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2006 2023-05-08 19:21:16.703726 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      175 2023-05-08 19:20:57.003370 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1873 2023-05-08 19:21:16.731727 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      175 2023-05-08 19:20:57.635381 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1889 2023-05-08 19:21:16.731727 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1940 2023-05-08 19:21:16.759727 windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6308 2023-05-08 19:21:16.899730 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item.py
--rw-r--r--   0        0        0     2979 2023-05-08 19:21:16.799728 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1886 2023-05-08 19:21:16.827729 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2190 2023-05-08 19:21:16.859729 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1986 2023-05-08 19:21:16.887730 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      173 2023-05-08 19:20:57.427377 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1853 2023-05-08 19:21:16.999732 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      173 2023-05-08 19:20:56.835367 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1879 2023-05-08 19:21:16.931730 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1930 2023-05-08 19:21:16.959731 windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2816 2023-05-08 19:21:17.003732 windmill_api-1.96.1/windmill_api/models/open_flow_w_path.py
--rw-r--r--   0        0        0     1197 2023-05-08 19:21:17.023732 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_schema.py
--rw-r--r--   0        0        0     3116 2023-05-08 19:21:17.043733 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value.py
--rw-r--r--   0        0        0     6590 2023-05-08 19:21:17.103733 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module.py
--rw-r--r--   0        0        0     3117 2023-05-08 19:21:17.083733 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
--rw-r--r--   0        0        0     1927 2023-05-08 19:21:17.111734 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2231 2023-05-08 19:21:17.135734 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2073 2023-05-08 19:21:17.139734 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      180 2023-05-08 19:20:56.923369 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1940 2023-05-08 19:21:17.163735 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      180 2023-05-08 19:20:56.887368 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1920 2023-05-08 19:21:17.171735 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1971 2023-05-08 19:21:17.191735 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6514 2023-05-08 19:21:17.247736 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item.py
--rw-r--r--   0        0        0     3074 2023-05-08 19:21:17.231736 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
--rw-r--r--   0        0        0     1917 2023-05-08 19:21:17.259736 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2221 2023-05-08 19:21:17.283737 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2044 2023-05-08 19:21:17.379738 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-08 19:20:57.311375 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1911 2023-05-08 19:21:17.311737 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-08 19:20:57.739382 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1910 2023-05-08 19:21:17.435739 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1961 2023-05-08 19:21:17.407739 windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1989 2023-05-08 19:21:17.435739 windmill_api-1.96.1/windmill_api/models/path_flow.py
--rw-r--r--   0        0        0     3089 2023-05-08 19:21:17.471740 windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms.py
--rw-r--r--   0        0        0     2115 2023-05-08 19:21:17.463740 windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      185 2023-05-08 19:20:56.959369 windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1982 2023-05-08 19:21:17.491740 windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      185 2023-05-08 19:20:56.811367 windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      135 2023-05-08 19:20:57.011370 windmill_api-1.96.1/windmill_api/models/path_flow_type.py
--rw-r--r--   0        0        0     2292 2023-05-08 19:21:17.507741 windmill_api-1.96.1/windmill_api/models/path_script.py
--rw-r--r--   0        0        0     3181 2023-05-08 19:21:17.527741 windmill_api-1.96.1/windmill_api/models/path_script_input_transforms.py
--rw-r--r--   0        0        0     2135 2023-05-08 19:21:17.539741 windmill_api-1.96.1/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      187 2023-05-08 19:20:57.663381 windmill_api-1.96.1/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2002 2023-05-08 19:21:17.555741 windmill_api-1.96.1/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      187 2023-05-08 19:20:57.263374 windmill_api-1.96.1/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      141 2023-05-08 19:20:57.291375 windmill_api-1.96.1/windmill_api/models/path_script_type.py
--rw-r--r--   0        0        0     3390 2023-05-08 19:21:17.591742 windmill_api-1.96.1/windmill_api/models/policy.py
--rw-r--r--   0        0        0      202 2023-05-08 19:20:57.755383 windmill_api-1.96.1/windmill_api/models/policy_execution_mode.py
--rw-r--r--   0        0        0     1709 2023-05-08 19:21:17.579742 windmill_api-1.96.1/windmill_api/models/policy_triggerables.py
--rw-r--r--   0        0        0     1279 2023-05-08 19:21:17.599742 windmill_api-1.96.1/windmill_api/models/policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2359 2023-05-08 19:21:17.631743 windmill_api-1.96.1/windmill_api/models/preview.py
--rw-r--r--   0        0        0     1148 2023-05-08 19:21:17.619742 windmill_api-1.96.1/windmill_api/models/preview_args.py
--rw-r--r--   0        0        0      194 2023-05-08 19:20:57.587380 windmill_api-1.96.1/windmill_api/models/preview_language.py
--rw-r--r--   0        0        0     1642 2023-05-08 19:21:17.647743 windmill_api-1.96.1/windmill_api/models/preview_schedule_json_body.py
--rw-r--r--   0        0        0     2963 2023-05-08 19:21:17.671743 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5679 2023-05-08 19:21:17.707744 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      328 2023-05-08 19:20:56.819367 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1618 2023-05-08 19:21:17.699744 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1683 2023-05-08 19:21:17.727744 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2191 2023-05-08 19:21:17.731745 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3329 2023-05-08 19:21:17.767745 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      346 2023-05-08 19:20:57.507378 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1651 2023-05-08 19:21:17.755745 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3214 2023-05-08 19:21:17.883747 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      337 2023-05-08 19:20:56.699365 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1600 2023-05-08 19:21:17.791746 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      182 2023-05-08 19:20:57.683381 windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0    11580 2023-05-08 19:21:18.035750 windmill_api-1.96.1/windmill_api/models/queued_job.py
--rw-r--r--   0        0        0     1161 2023-05-08 19:21:17.899747 windmill_api-1.96.1/windmill_api/models/queued_job_args.py
--rw-r--r--   0        0        0     3202 2023-05-08 19:21:17.943748 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status.py
--rw-r--r--   0        0        0     6683 2023-05-08 19:21:18.023750 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1774 2023-05-08 19:21:18.051750 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2106 2023-05-08 19:21:18.063750 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      199 2023-05-08 19:20:57.291375 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1679 2023-05-08 19:21:18.075751 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2215 2023-05-08 19:21:18.099751 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      357 2023-05-08 19:20:57.311375 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6294 2023-05-08 19:21:18.155752 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1764 2023-05-08 19:21:18.123751 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2086 2023-05-08 19:21:18.151752 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      197 2023-05-08 19:20:56.903368 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1669 2023-05-08 19:21:18.183752 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2205 2023-05-08 19:21:18.279754 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      355 2023-05-08 19:20:56.691365 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2025 2023-05-08 19:21:18.215753 windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_retry.py
--rw-r--r--   0        0        0      307 2023-05-08 19:20:57.571380 windmill_api-1.96.1/windmill_api/models/queued_job_job_kind.py
--rw-r--r--   0        0        0      196 2023-05-08 19:20:57.035370 windmill_api-1.96.1/windmill_api/models/queued_job_language.py
--rw-r--r--   0        0        0     3079 2023-05-08 19:21:18.259754 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow.py
--rw-r--r--   0        0        0     6506 2023-05-08 19:21:18.447757 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3069 2023-05-08 19:21:18.315755 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1914 2023-05-08 19:21:18.347755 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2218 2023-05-08 19:21:18.379756 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2040 2023-05-08 19:21:18.407756 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-08 19:20:57.419377 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1907 2023-05-08 19:21:18.431757 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-08 19:20:57.347376 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1907 2023-05-08 19:21:18.459757 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1958 2023-05-08 19:21:18.475758 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6430 2023-05-08 19:21:18.535759 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3035 2023-05-08 19:21:18.511758 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1904 2023-05-08 19:21:18.543759 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2208 2023-05-08 19:21:18.567759 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2020 2023-05-08 19:21:18.571759 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-05-08 19:20:57.563379 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1887 2023-05-08 19:21:18.595760 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-05-08 19:20:57.239374 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1897 2023-05-08 19:21:18.599760 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1948 2023-05-08 19:21:18.623760 windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     3028 2023-05-08 19:21:18.643761 windmill_api-1.96.1/windmill_api/models/raw_script.py
--rw-r--r--   0        0        0     3139 2023-05-08 19:21:18.655761 windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms.py
--rw-r--r--   0        0        0     2125 2023-05-08 19:21:18.675761 windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      186 2023-05-08 19:20:57.259374 windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1992 2023-05-08 19:21:18.683761 windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      186 2023-05-08 19:20:57.199373 windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      196 2023-05-08 19:20:57.675381 windmill_api-1.96.1/windmill_api/models/raw_script_language.py
--rw-r--r--   0        0        0      146 2023-05-08 19:20:56.711365 windmill_api-1.96.1/windmill_api/models/raw_script_type.py
--rw-r--r--   0        0        0     1405 2023-05-08 19:21:18.703762 windmill_api-1.96.1/windmill_api/models/refresh_token_json_body.py
--rw-r--r--   0        0        0     1448 2023-05-08 19:21:18.703762 windmill_api-1.96.1/windmill_api/models/remove_granular_acls_json_body.py
--rw-r--r--   0        0        0      328 2023-05-08 19:20:57.075371 windmill_api-1.96.1/windmill_api/models/remove_granular_acls_kind.py
--rw-r--r--   0        0        0     1544 2023-05-08 19:21:18.823764 windmill_api-1.96.1/windmill_api/models/remove_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1567 2023-05-08 19:21:18.731762 windmill_api-1.96.1/windmill_api/models/remove_user_to_group_json_body.py
--rw-r--r--   0        0        0     3367 2023-05-08 19:21:18.863764 windmill_api-1.96.1/windmill_api/models/resource.py
--rw-r--r--   0        0        0     1189 2023-05-08 19:21:18.839764 windmill_api-1.96.1/windmill_api/models/resource_extra_perms.py
--rw-r--r--   0        0        0     2256 2023-05-08 19:21:18.875765 windmill_api-1.96.1/windmill_api/models/resource_type.py
--rw-r--r--   0        0        0     1278 2023-05-08 19:21:18.883765 windmill_api-1.96.1/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
--rw-r--r--   0        0        0     1255 2023-05-08 19:21:18.899765 windmill_api-1.96.1/windmill_api/models/resume_suspended_job_post_json_body.py
--rw-r--r--   0        0        0     2546 2023-05-08 19:21:18.923766 windmill_api-1.96.1/windmill_api/models/retry.py
--rw-r--r--   0        0        0     1751 2023-05-08 19:21:18.927766 windmill_api-1.96.1/windmill_api/models/retry_constant.py
--rw-r--r--   0        0        0     2055 2023-05-08 19:21:18.955766 windmill_api-1.96.1/windmill_api/models/retry_exponential.py
--rw-r--r--   0        0        0     1210 2023-05-08 19:21:18.947766 windmill_api-1.96.1/windmill_api/models/run_flow_by_path_json_body.py
--rw-r--r--   0        0        0     2189 2023-05-08 19:21:18.983767 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body.py
--rw-r--r--   0        0        0     1235 2023-05-08 19:21:18.975767 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_args.py
--rw-r--r--   0        0        0     3265 2023-05-08 19:21:19.015767 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value.py
--rw-r--r--   0        0        0     7049 2023-05-08 19:21:19.063768 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3284 2023-05-08 19:21:19.055768 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1975 2023-05-08 19:21:19.083768 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-05-08 19:21:19.099769 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-05-08 19:21:19.111769 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-05-08 19:20:56.859367 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-05-08 19:21:19.127769 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-05-08 19:20:56.803367 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-05-08 19:21:19.139769 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-05-08 19:21:19.159770 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6939 2023-05-08 19:21:19.219771 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3250 2023-05-08 19:21:19.203770 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1965 2023-05-08 19:21:19.235771 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2269 2023-05-08 19:21:19.251771 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2147 2023-05-08 19:21:19.355773 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      187 2023-05-08 19:20:57.619380 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2014 2023-05-08 19:21:19.371773 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      187 2023-05-08 19:20:57.451377 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1958 2023-05-08 19:21:19.383774 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2009 2023-05-08 19:21:19.399774 windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1220 2023-05-08 19:21:19.403774 windmill_api-1.96.1/windmill_api/models/run_script_by_hash_json_body.py
--rw-r--r--   0        0        0     1220 2023-05-08 19:21:19.419774 windmill_api-1.96.1/windmill_api/models/run_script_by_path_json_body.py
--rw-r--r--   0        0        0     2634 2023-05-08 19:21:19.443775 windmill_api-1.96.1/windmill_api/models/run_script_preview_json_body.py
--rw-r--r--   0        0        0     1245 2023-05-08 19:21:19.439775 windmill_api-1.96.1/windmill_api/models/run_script_preview_json_body_args.py
--rw-r--r--   0        0        0      211 2023-05-08 19:20:57.539379 windmill_api-1.96.1/windmill_api/models/run_script_preview_json_body_language.py
--rw-r--r--   0        0        0     1266 2023-05-08 19:21:19.459775 windmill_api-1.96.1/windmill_api/models/run_wait_result_flow_by_path_json_body.py
--rw-r--r--   0        0        0     1276 2023-05-08 19:21:19.463775 windmill_api-1.96.1/windmill_api/models/run_wait_result_script_by_path_json_body.py
--rw-r--r--   0        0        0      203 2023-05-08 19:20:57.491378 windmill_api-1.96.1/windmill_api/models/runnable_type.py
--rw-r--r--   0        0        0     4086 2023-05-08 19:21:19.519776 windmill_api-1.96.1/windmill_api/models/schedule.py
--rw-r--r--   0        0        0     1153 2023-05-08 19:21:19.483775 windmill_api-1.96.1/windmill_api/models/schedule_args.py
--rw-r--r--   0        0        0     1189 2023-05-08 19:21:19.503776 windmill_api-1.96.1/windmill_api/models/schedule_extra_perms.py
--rw-r--r--   0        0        0     7003 2023-05-08 19:21:19.599778 windmill_api-1.96.1/windmill_api/models/script.py
--rw-r--r--   0        0        0     1143 2023-05-08 19:21:19.535776 windmill_api-1.96.1/windmill_api/models/script_args.py
--rw-r--r--   0        0        0     1179 2023-05-08 19:21:19.555777 windmill_api-1.96.1/windmill_api/models/script_extra_perms.py
--rw-r--r--   0        0        0      235 2023-05-08 19:20:57.415377 windmill_api-1.96.1/windmill_api/models/script_kind.py
--rw-r--r--   0        0        0      193 2023-05-08 19:20:57.627380 windmill_api-1.96.1/windmill_api/models/script_language.py
--rw-r--r--   0        0        0     1153 2023-05-08 19:21:19.579777 windmill_api-1.96.1/windmill_api/models/script_schema.py
--rw-r--r--   0        0        0     1440 2023-05-08 19:21:19.599778 windmill_api-1.96.1/windmill_api/models/set_password_json_body.py
--rw-r--r--   0        0        0     1470 2023-05-08 19:21:19.623778 windmill_api-1.96.1/windmill_api/models/set_schedule_enabled_json_body.py
--rw-r--r--   0        0        0     2032 2023-05-08 19:21:19.631778 windmill_api-1.96.1/windmill_api/models/slack_token.py
--rw-r--r--   0        0        0     1586 2023-05-08 19:21:19.647778 windmill_api-1.96.1/windmill_api/models/slack_token_bot.py
--rw-r--r--   0        0        0     2227 2023-05-08 19:21:19.663779 windmill_api-1.96.1/windmill_api/models/star_json_body.py
--rw-r--r--   0        0        0      209 2023-05-08 19:20:57.551379 windmill_api-1.96.1/windmill_api/models/star_json_body_favorite_kind.py
--rw-r--r--   0        0        0     1772 2023-05-08 19:21:19.679779 windmill_api-1.96.1/windmill_api/models/static_transform.py
--rw-r--r--   0        0        0      154 2023-05-08 19:20:57.327376 windmill_api-1.96.1/windmill_api/models/static_transform_type.py
--rw-r--r--   0        0        0     2462 2023-05-08 19:21:19.703779 windmill_api-1.96.1/windmill_api/models/token_response.py
--rw-r--r--   0        0        0     2921 2023-05-08 19:21:19.719780 windmill_api-1.96.1/windmill_api/models/truncated_token.py
--rw-r--r--   0        0        0     2249 2023-05-08 19:21:19.735780 windmill_api-1.96.1/windmill_api/models/unstar_json_body.py
--rw-r--r--   0        0        0      211 2023-05-08 19:20:57.507378 windmill_api-1.96.1/windmill_api/models/unstar_json_body_favorite_kind.py
--rw-r--r--   0        0        0     2638 2023-05-08 19:21:19.763780 windmill_api-1.96.1/windmill_api/models/update_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-05-08 19:21:19.779781 windmill_api-1.96.1/windmill_api/models/update_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-05-08 19:20:57.155372 windmill_api-1.96.1/windmill_api/models/update_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-05-08 19:21:19.791781 windmill_api-1.96.1/windmill_api/models/update_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-05-08 19:21:19.799781 windmill_api-1.96.1/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-05-08 19:21:19.935783 windmill_api-1.96.1/windmill_api/models/update_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-05-08 19:21:19.819781 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-05-08 19:21:19.859782 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-05-08 19:21:20.043785 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-05-08 19:21:19.975784 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-05-08 19:21:20.007785 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-05-08 19:21:20.039785 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-05-08 19:21:20.067786 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-05-08 19:20:57.519379 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-05-08 19:21:20.071786 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-05-08 19:20:57.667381 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-05-08 19:21:20.099786 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-05-08 19:21:20.099786 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-05-08 19:21:20.179788 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-05-08 19:21:20.139787 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-05-08 19:21:20.171788 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-05-08 19:21:20.199788 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-05-08 19:21:20.207788 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-05-08 19:20:57.235374 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-05-08 19:21:20.227789 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-05-08 19:20:57.423377 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-05-08 19:21:20.239789 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-05-08 19:21:20.255789 windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1949 2023-05-08 19:21:20.375791 windmill_api-1.96.1/windmill_api/models/update_folder_json_body.py
--rw-r--r--   0        0        0     1520 2023-05-08 19:21:20.283789 windmill_api-1.96.1/windmill_api/models/update_group_json_body.py
--rw-r--r--   0        0        0     1670 2023-05-08 19:21:20.307790 windmill_api-1.96.1/windmill_api/models/update_input.py
--rw-r--r--   0        0        0     1716 2023-05-08 19:21:20.335790 windmill_api-1.96.1/windmill_api/models/update_input_json_body.py
--rw-r--r--   0        0        0     1985 2023-05-08 19:21:20.367791 windmill_api-1.96.1/windmill_api/models/update_raw_app_json_body.py
--rw-r--r--   0        0        0     2036 2023-05-08 19:21:20.399792 windmill_api-1.96.1/windmill_api/models/update_resource_json_body.py
--rw-r--r--   0        0        0     1847 2023-05-08 19:21:20.403792 windmill_api-1.96.1/windmill_api/models/update_resource_type_json_body.py
--rw-r--r--   0        0        0     1541 2023-05-08 19:21:20.423792 windmill_api-1.96.1/windmill_api/models/update_resource_value_json_body.py
--rw-r--r--   0        0        0     1953 2023-05-08 19:21:20.435792 windmill_api-1.96.1/windmill_api/models/update_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-05-08 19:21:20.447792 windmill_api-1.96.1/windmill_api/models/update_schedule_json_body_args.py
--rw-r--r--   0        0        0     2066 2023-05-08 19:21:20.467793 windmill_api-1.96.1/windmill_api/models/update_user_json_body.py
--rw-r--r--   0        0        0     2316 2023-05-08 19:21:20.479793 windmill_api-1.96.1/windmill_api/models/update_variable_json_body.py
--rw-r--r--   0        0        0     1478 2023-05-08 19:21:20.495793 windmill_api-1.96.1/windmill_api/models/usage.py
--rw-r--r--   0        0        0     4071 2023-05-08 19:21:20.659796 windmill_api-1.96.1/windmill_api/models/user.py
--rw-r--r--   0        0        0     1501 2023-05-08 19:21:20.523794 windmill_api-1.96.1/windmill_api/models/user_usage.py
--rw-r--r--   0        0        0     2122 2023-05-08 19:21:20.551794 windmill_api-1.96.1/windmill_api/models/user_workspace_list.py
--rw-r--r--   0        0        0     1767 2023-05-08 19:21:20.583795 windmill_api-1.96.1/windmill_api/models/user_workspace_list_workspaces_item.py
--rw-r--r--   0        0        0     4222 2023-05-08 19:21:20.643796 windmill_api-1.96.1/windmill_api/models/whoami_response_200.py
--rw-r--r--   0        0        0     1572 2023-05-08 19:21:20.671796 windmill_api-1.96.1/windmill_api/models/whoami_response_200_usage.py
--rw-r--r--   0        0        0     4211 2023-05-08 19:21:20.719797 windmill_api-1.96.1/windmill_api/models/whois_response_200.py
--rw-r--r--   0        0        0     1567 2023-05-08 19:21:20.691797 windmill_api-1.96.1/windmill_api/models/whois_response_200_usage.py
--rw-r--r--   0        0        0     2604 2023-05-08 19:21:20.731797 windmill_api-1.96.1/windmill_api/models/worker_ping.py
--rw-r--r--   0        0        0     1901 2023-05-08 19:21:20.751798 windmill_api-1.96.1/windmill_api/models/workspace.py
--rw-r--r--   0        0        0     1974 2023-05-08 19:21:20.763798 windmill_api-1.96.1/windmill_api/models/workspace_invite.py
--rw-r--r--   0        0        0       25 2023-05-08 19:20:47.203207 windmill_api-1.96.1/windmill_api/py.typed
--rw-r--r--   0        0        0      939 2023-05-08 19:21:20.767798 windmill_api-1.96.1/windmill_api/types.py
--rw-r--r--   0        0        0     4362 1970-01-01 00:00:00.000000 windmill_api-1.96.1/setup.py
--rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.96.1/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-05-08 21:40:21.025655 windmill_api-1.96.2/LICENSE
+-rw-r--r--   0        0        0     2952 2023-05-08 21:40:21.029655 windmill_api-1.96.2/README.md
+-rw-r--r--   0        0        0      717 2023-05-08 21:40:21.025655 windmill_api-1.96.2/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-05-08 21:39:48.629678 windmill_api-1.96.2/windmill_api/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-08 21:39:49.117673 windmill_api-1.96.2/windmill_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.233673 windmill_api-1.96.2/windmill_api/api/app/__init__.py
+-rw-r--r--   0        0        0     1999 2023-05-08 21:39:59.749666 windmill_api-1.96.2/windmill_api/api/app/create_app.py
+-rw-r--r--   0        0        0     1769 2023-05-08 21:39:59.753666 windmill_api-1.96.2/windmill_api/api/app/delete_app.py
+-rw-r--r--   0        0        0     2214 2023-05-08 21:39:59.789666 windmill_api-1.96.2/windmill_api/api/app/execute_component.py
+-rw-r--r--   0        0        0     2782 2023-05-08 21:39:59.797666 windmill_api-1.96.2/windmill_api/api/app/exists_app.py
+-rw-r--r--   0        0        0     3020 2023-05-08 21:39:59.833666 windmill_api-1.96.2/windmill_api/api/app/get_app_by_path.py
+-rw-r--r--   0        0        0     3187 2023-05-08 21:39:59.837666 windmill_api-1.96.2/windmill_api/api/app/get_app_by_path_with_draft.py
+-rw-r--r--   0        0        0     3031 2023-05-08 21:39:59.873666 windmill_api-1.96.2/windmill_api/api/app/get_app_by_version.py
+-rw-r--r--   0        0        0     2649 2023-05-08 21:39:59.885666 windmill_api-1.96.2/windmill_api/api/app/get_hub_app_by_id.py
+-rw-r--r--   0        0        0     3168 2023-05-08 21:39:59.929666 windmill_api-1.96.2/windmill_api/api/app/get_public_app_by_secret.py
+-rw-r--r--   0        0        0     1797 2023-05-08 21:39:59.913666 windmill_api-1.96.2/windmill_api/api/app/get_public_secret_of_app.py
+-rw-r--r--   0        0        0     7289 2023-05-08 21:40:00.013666 windmill_api-1.96.2/windmill_api/api/app/list_apps.py
+-rw-r--r--   0        0        0     2405 2023-05-08 21:39:59.961666 windmill_api-1.96.2/windmill_api/api/app/list_hub_apps.py
+-rw-r--r--   0        0        0     2140 2023-05-08 21:39:59.993666 windmill_api-1.96.2/windmill_api/api/app/update_app.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.153673 windmill_api-1.96.2/windmill_api/api/audit/__init__.py
+-rw-r--r--   0        0        0     3065 2023-05-08 21:40:00.033666 windmill_api-1.96.2/windmill_api/api/audit/get_audit_log.py
+-rw-r--r--   0        0        0     8723 2023-05-08 21:40:00.129666 windmill_api-1.96.2/windmill_api/api/audit/list_audit_logs.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.289673 windmill_api-1.96.2/windmill_api/api/capture/__init__.py
+-rw-r--r--   0        0        0     1796 2023-05-08 21:40:00.061666 windmill_api-1.96.2/windmill_api/api/capture/create_capture.py
+-rw-r--r--   0        0        0     1790 2023-05-08 21:40:00.089666 windmill_api-1.96.2/windmill_api/api/capture/get_capture.py
+-rw-r--r--   0        0        0     1799 2023-05-08 21:40:00.117666 windmill_api-1.96.2/windmill_api/api/capture/update_capture.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.245673 windmill_api-1.96.2/windmill_api/api/draft/__init__.py
+-rw-r--r--   0        0        0     2019 2023-05-08 21:40:00.145666 windmill_api-1.96.2/windmill_api/api/draft/create_draft.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.293673 windmill_api-1.96.2/windmill_api/api/favorite/__init__.py
+-rw-r--r--   0        0        0     1964 2023-05-08 21:40:00.165666 windmill_api-1.96.2/windmill_api/api/favorite/star.py
+-rw-r--r--   0        0        0     1984 2023-05-08 21:40:00.173666 windmill_api-1.96.2/windmill_api/api/favorite/unstar.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.213673 windmill_api-1.96.2/windmill_api/api/flow/__init__.py
+-rw-r--r--   0        0        0     2220 2023-05-08 21:40:00.197666 windmill_api-1.96.2/windmill_api/api/flow/archive_flow_by_path.py
+-rw-r--r--   0        0        0     2009 2023-05-08 21:40:00.201666 windmill_api-1.96.2/windmill_api/api/flow/create_flow.py
+-rw-r--r--   0        0        0     1788 2023-05-08 21:40:00.229666 windmill_api-1.96.2/windmill_api/api/flow/delete_flow_by_path.py
+-rw-r--r--   0        0        0     2755 2023-05-08 21:40:00.253666 windmill_api-1.96.2/windmill_api/api/flow/exists_flow_by_path.py
+-rw-r--r--   0        0        0     3036 2023-05-08 21:40:00.285666 windmill_api-1.96.2/windmill_api/api/flow/get_flow_by_path.py
+-rw-r--r--   0        0        0     3205 2023-05-08 21:40:00.293666 windmill_api-1.96.2/windmill_api/api/flow/get_flow_by_path_with_draft.py
+-rw-r--r--   0        0        0     4827 2023-05-08 21:40:00.349665 windmill_api-1.96.2/windmill_api/api/flow/get_flow_input_history_by_path.py
+-rw-r--r--   0        0        0     2667 2023-05-08 21:40:00.329666 windmill_api-1.96.2/windmill_api/api/flow/get_hub_flow_by_id.py
+-rw-r--r--   0        0        0     1668 2023-05-08 21:40:00.357665 windmill_api-1.96.2/windmill_api/api/flow/list_flow_paths.py
+-rw-r--r--   0        0        0     7969 2023-05-08 21:40:00.453665 windmill_api-1.96.2/windmill_api/api/flow/list_flows.py
+-rw-r--r--   0        0        0     2423 2023-05-08 21:40:00.389665 windmill_api-1.96.2/windmill_api/api/flow/list_hub_flows.py
+-rw-r--r--   0        0        0     2150 2023-05-08 21:40:00.417665 windmill_api-1.96.2/windmill_api/api/flow/update_flow.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.285673 windmill_api-1.96.2/windmill_api/api/folder/__init__.py
+-rw-r--r--   0        0        0     2214 2023-05-08 21:40:00.449665 windmill_api-1.96.2/windmill_api/api/folder/add_owner_to_folder.py
+-rw-r--r--   0        0        0     2029 2023-05-08 21:40:00.477666 windmill_api-1.96.2/windmill_api/api/folder/create_folder.py
+-rw-r--r--   0        0        0     1778 2023-05-08 21:40:00.485665 windmill_api-1.96.2/windmill_api/api/folder/delete_folder.py
+-rw-r--r--   0        0        0     2960 2023-05-08 21:40:00.521665 windmill_api-1.96.2/windmill_api/api/folder/get_folder.py
+-rw-r--r--   0        0        0     3055 2023-05-08 21:40:00.529665 windmill_api-1.96.2/windmill_api/api/folder/get_folder_usage.py
+-rw-r--r--   0        0        0     3405 2023-05-08 21:40:00.581665 windmill_api-1.96.2/windmill_api/api/folder/list_folder_names.py
+-rw-r--r--   0        0        0     4251 2023-05-08 21:40:00.597665 windmill_api-1.96.2/windmill_api/api/folder/list_folders.py
+-rw-r--r--   0        0        0     2244 2023-05-08 21:40:00.613665 windmill_api-1.96.2/windmill_api/api/folder/remove_owner_to_folder.py
+-rw-r--r--   0        0        0     2170 2023-05-08 21:40:00.629665 windmill_api-1.96.2/windmill_api/api/folder/update_folder.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.289673 windmill_api-1.96.2/windmill_api/api/granular_acl/__init__.py
+-rw-r--r--   0        0        0     2480 2023-05-08 21:40:00.645665 windmill_api-1.96.2/windmill_api/api/granular_acl/add_granular_acls.py
+-rw-r--r--   0        0        0     3526 2023-05-08 21:40:00.697665 windmill_api-1.96.2/windmill_api/api/granular_acl/get_granular_acls.py
+-rw-r--r--   0        0        0     2545 2023-05-08 21:40:00.677665 windmill_api-1.96.2/windmill_api/api/granular_acl/remove_granular_acls.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.277673 windmill_api-1.96.2/windmill_api/api/group/__init__.py
+-rw-r--r--   0        0        0     2194 2023-05-08 21:40:00.709665 windmill_api-1.96.2/windmill_api/api/group/add_user_to_group.py
+-rw-r--r--   0        0        0     2019 2023-05-08 21:40:00.725665 windmill_api-1.96.2/windmill_api/api/group/create_group.py
+-rw-r--r--   0        0        0     1775 2023-05-08 21:40:00.737665 windmill_api-1.96.2/windmill_api/api/group/delete_group.py
+-rw-r--r--   0        0        0     2942 2023-05-08 21:40:00.769665 windmill_api-1.96.2/windmill_api/api/group/get_group.py
+-rw-r--r--   0        0        0     3400 2023-05-08 21:40:00.785665 windmill_api-1.96.2/windmill_api/api/group/list_group_names.py
+-rw-r--r--   0        0        0     4233 2023-05-08 21:40:00.829665 windmill_api-1.96.2/windmill_api/api/group/list_groups.py
+-rw-r--r--   0        0        0     2224 2023-05-08 21:40:00.813665 windmill_api-1.96.2/windmill_api/api/group/remove_user_to_group.py
+-rw-r--r--   0        0        0     2160 2023-05-08 21:40:00.845665 windmill_api-1.96.2/windmill_api/api/group/update_group.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.293673 windmill_api-1.96.2/windmill_api/api/input_/__init__.py
+-rw-r--r--   0        0        0     3338 2023-05-08 21:40:00.877665 windmill_api-1.96.2/windmill_api/api/input_/create_input.py
+-rw-r--r--   0        0        0     1811 2023-05-08 21:40:00.873665 windmill_api-1.96.2/windmill_api/api/input_/delete_input.py
+-rw-r--r--   0        0        0     6187 2023-05-08 21:40:00.957665 windmill_api-1.96.2/windmill_api/api/input_/get_input_history.py
+-rw-r--r--   0        0        0     6010 2023-05-08 21:40:00.953665 windmill_api-1.96.2/windmill_api/api/input_/list_inputs.py
+-rw-r--r--   0        0        0     2025 2023-05-08 21:40:00.985665 windmill_api-1.96.2/windmill_api/api/input_/update_input.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.245673 windmill_api-1.96.2/windmill_api/api/job/__init__.py
+-rw-r--r--   0        0        0     2181 2023-05-08 21:40:00.993665 windmill_api-1.96.2/windmill_api/api/job/cancel_queued_job.py
+-rw-r--r--   0        0        0     2687 2023-05-08 21:40:01.041665 windmill_api-1.96.2/windmill_api/api/job/cancel_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-05-08 21:40:01.033665 windmill_api-1.96.2/windmill_api/api/job/cancel_suspended_job_post.py
+-rw-r--r--   0        0        0     2535 2023-05-08 21:40:01.073665 windmill_api-1.96.2/windmill_api/api/job/create_job_signature.py
+-rw-r--r--   0        0        0     3217 2023-05-08 21:40:01.081665 windmill_api-1.96.2/windmill_api/api/job/delete_completed_job.py
+-rw-r--r--   0        0        0     2235 2023-05-08 21:40:01.105665 windmill_api-1.96.2/windmill_api/api/job/force_cancel_queued_job.py
+-rw-r--r--   0        0        0     3034 2023-05-08 21:40:01.121665 windmill_api-1.96.2/windmill_api/api/job/get_completed_job.py
+-rw-r--r--   0        0        0     1784 2023-05-08 21:40:01.137665 windmill_api-1.96.2/windmill_api/api/job/get_completed_job_result.py
+-rw-r--r--   0        0        0     2868 2023-05-08 21:40:01.157665 windmill_api-1.96.2/windmill_api/api/job/get_job.py
+-rw-r--r--   0        0        0     4305 2023-05-08 21:40:01.197665 windmill_api-1.96.2/windmill_api/api/job/get_job_updates.py
+-rw-r--r--   0        0        0     4306 2023-05-08 21:40:01.213665 windmill_api-1.96.2/windmill_api/api/job/get_resume_urls.py
+-rw-r--r--   0        0        0     4601 2023-05-08 21:40:01.273665 windmill_api-1.96.2/windmill_api/api/job/get_suspended_job_flow.py
+-rw-r--r--   0        0        0    13065 2023-05-08 21:40:01.381665 windmill_api-1.96.2/windmill_api/api/job/list_completed_jobs.py
+-rw-r--r--   0        0        0    12292 2023-05-08 21:40:01.413665 windmill_api-1.96.2/windmill_api/api/job/list_jobs.py
+-rw-r--r--   0        0        0    12830 2023-05-08 21:40:01.533665 windmill_api-1.96.2/windmill_api/api/job/list_queue.py
+-rw-r--r--   0        0        0     2067 2023-05-08 21:40:01.445665 windmill_api-1.96.2/windmill_api/api/job/result_by_id.py
+-rw-r--r--   0        0        0     2313 2023-05-08 21:40:01.477665 windmill_api-1.96.2/windmill_api/api/job/resume_suspended_flow_as_owner.py
+-rw-r--r--   0        0        0     2994 2023-05-08 21:40:01.521664 windmill_api-1.96.2/windmill_api/api/job/resume_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-05-08 21:40:01.565665 windmill_api-1.96.2/windmill_api/api/job/resume_suspended_job_post.py
+-rw-r--r--   0        0        0     4566 2023-05-08 21:40:01.589665 windmill_api-1.96.2/windmill_api/api/job/run_flow_by_path.py
+-rw-r--r--   0        0        0     3037 2023-05-08 21:40:01.609665 windmill_api-1.96.2/windmill_api/api/job/run_flow_preview.py
+-rw-r--r--   0        0        0     4594 2023-05-08 21:40:01.649664 windmill_api-1.96.2/windmill_api/api/job/run_script_by_hash.py
+-rw-r--r--   0        0        0     4200 2023-05-08 21:40:01.685665 windmill_api-1.96.2/windmill_api/api/job/run_script_by_path.py
+-rw-r--r--   0        0        0     3050 2023-05-08 21:40:01.689664 windmill_api-1.96.2/windmill_api/api/job/run_script_preview.py
+-rw-r--r--   0        0        0     3215 2023-05-08 21:40:01.729664 windmill_api-1.96.2/windmill_api/api/job/run_wait_result_flow_by_path.py
+-rw-r--r--   0        0        0     3521 2023-05-08 21:40:01.769664 windmill_api-1.96.2/windmill_api/api/job/run_wait_result_script_by_path.py
+-rw-r--r--   0        0        0     3356 2023-05-08 21:40:01.777664 windmill_api-1.96.2/windmill_api/api/job/run_wait_result_script_by_path_get.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.185673 windmill_api-1.96.2/windmill_api/api/oauth/__init__.py
+-rw-r--r--   0        0        0     3506 2023-05-08 21:40:01.817664 windmill_api-1.96.2/windmill_api/api/oauth/connect_callback.py
+-rw-r--r--   0        0        0     2118 2023-05-08 21:40:01.805664 windmill_api-1.96.2/windmill_api/api/oauth/connect_slack_callback.py
+-rw-r--r--   0        0        0     2056 2023-05-08 21:40:01.837664 windmill_api-1.96.2/windmill_api/api/oauth/create_account.py
+-rw-r--r--   0        0        0     1764 2023-05-08 21:40:01.849664 windmill_api-1.96.2/windmill_api/api/oauth/disconnect_account.py
+-rw-r--r--   0        0        0     1649 2023-05-08 21:40:01.861664 windmill_api-1.96.2/windmill_api/api/oauth/disconnect_slack.py
+-rw-r--r--   0        0        0     1426 2023-05-08 21:40:01.873664 windmill_api-1.96.2/windmill_api/api/oauth/list_o_auth_connects.py
+-rw-r--r--   0        0        0     2162 2023-05-08 21:40:01.897664 windmill_api-1.96.2/windmill_api/api/oauth/list_o_auth_logins.py
+-rw-r--r--   0        0        0     2151 2023-05-08 21:40:01.905664 windmill_api-1.96.2/windmill_api/api/oauth/refresh_token.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.269673 windmill_api-1.96.2/windmill_api/api/raw_app/__init__.py
+-rw-r--r--   0        0        0     2033 2023-05-08 21:40:01.933664 windmill_api-1.96.2/windmill_api/api/raw_app/create_raw_app.py
+-rw-r--r--   0        0        0     1781 2023-05-08 21:40:01.933664 windmill_api-1.96.2/windmill_api/api/raw_app/delete_raw_app.py
+-rw-r--r--   0        0        0     2786 2023-05-08 21:40:01.977664 windmill_api-1.96.2/windmill_api/api/raw_app/exists_raw_app.py
+-rw-r--r--   0        0        0     1979 2023-05-08 21:40:01.961664 windmill_api-1.96.2/windmill_api/api/raw_app/get_raw_app_data.py
+-rw-r--r--   0        0        0     7349 2023-05-08 21:40:02.065664 windmill_api-1.96.2/windmill_api/api/raw_app/list_raw_apps.py
+-rw-r--r--   0        0        0     2166 2023-05-08 21:40:02.005664 windmill_api-1.96.2/windmill_api/api/raw_app/update_raw_app.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.189673 windmill_api-1.96.2/windmill_api/api/resource/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-08 21:40:02.037664 windmill_api-1.96.2/windmill_api/api/resource/create_resource.py
+-rw-r--r--   0        0        0     2093 2023-05-08 21:40:02.069664 windmill_api-1.96.2/windmill_api/api/resource/create_resource_type.py
+-rw-r--r--   0        0        0     1784 2023-05-08 21:40:02.089664 windmill_api-1.96.2/windmill_api/api/resource/delete_resource.py
+-rw-r--r--   0        0        0     1799 2023-05-08 21:40:02.101664 windmill_api-1.96.2/windmill_api/api/resource/delete_resource_type.py
+-rw-r--r--   0        0        0     2763 2023-05-08 21:40:02.129664 windmill_api-1.96.2/windmill_api/api/resource/exists_resource.py
+-rw-r--r--   0        0        0     2788 2023-05-08 21:40:02.153664 windmill_api-1.96.2/windmill_api/api/resource/exists_resource_type.py
+-rw-r--r--   0        0        0     2996 2023-05-08 21:40:02.173664 windmill_api-1.96.2/windmill_api/api/resource/get_resource.py
+-rw-r--r--   0        0        0     3074 2023-05-08 21:40:02.197664 windmill_api-1.96.2/windmill_api/api/resource/get_resource_type.py
+-rw-r--r--   0        0        0     1790 2023-05-08 21:40:02.197664 windmill_api-1.96.2/windmill_api/api/resource/get_resource_value.py
+-rw-r--r--   0        0        0     5732 2023-05-08 21:40:02.273664 windmill_api-1.96.2/windmill_api/api/resource/list_resource.py
+-rw-r--r--   0        0        0     3149 2023-05-08 21:40:02.237664 windmill_api-1.96.2/windmill_api/api/resource/list_resource_type.py
+-rw-r--r--   0        0        0     2600 2023-05-08 21:40:02.277664 windmill_api-1.96.2/windmill_api/api/resource/list_resource_type_names.py
+-rw-r--r--   0        0        0     2190 2023-05-08 21:40:02.305664 windmill_api-1.96.2/windmill_api/api/resource/update_resource.py
+-rw-r--r--   0        0        0     2234 2023-05-08 21:40:02.309664 windmill_api-1.96.2/windmill_api/api/resource/update_resource_type.py
+-rw-r--r--   0        0        0     2244 2023-05-08 21:40:02.337664 windmill_api-1.96.2/windmill_api/api/resource/update_resource_value.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.273673 windmill_api-1.96.2/windmill_api/api/schedule/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-08 21:40:02.353664 windmill_api-1.96.2/windmill_api/api/schedule/create_schedule.py
+-rw-r--r--   0        0        0     1784 2023-05-08 21:40:02.369664 windmill_api-1.96.2/windmill_api/api/schedule/delete_schedule.py
+-rw-r--r--   0        0        0     2763 2023-05-08 21:40:02.393664 windmill_api-1.96.2/windmill_api/api/schedule/exists_schedule.py
+-rw-r--r--   0        0        0     2996 2023-05-08 21:40:02.409664 windmill_api-1.96.2/windmill_api/api/schedule/get_schedule.py
+-rw-r--r--   0        0        0     4287 2023-05-08 21:40:02.449664 windmill_api-1.96.2/windmill_api/api/schedule/list_schedules.py
+-rw-r--r--   0        0        0     3217 2023-05-08 21:40:02.453664 windmill_api-1.96.2/windmill_api/api/schedule/preview_schedule.py
+-rw-r--r--   0        0        0     2233 2023-05-08 21:40:02.481664 windmill_api-1.96.2/windmill_api/api/schedule/set_schedule_enabled.py
+-rw-r--r--   0        0        0     2190 2023-05-08 21:40:02.501664 windmill_api-1.96.2/windmill_api/api/schedule/update_schedule.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.197673 windmill_api-1.96.2/windmill_api/api/script/__init__.py
+-rw-r--r--   0        0        0     3165 2023-05-08 21:40:02.521664 windmill_api-1.96.2/windmill_api/api/script/archive_script_by_hash.py
+-rw-r--r--   0        0        0     1797 2023-05-08 21:40:02.533664 windmill_api-1.96.2/windmill_api/api/script/archive_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-05-08 21:40:02.557664 windmill_api-1.96.2/windmill_api/api/script/bash_to_jsonschema.py
+-rw-r--r--   0        0        0     2029 2023-05-08 21:40:02.561664 windmill_api-1.96.2/windmill_api/api/script/create_script.py
+-rw-r--r--   0        0        0     3327 2023-05-08 21:40:02.597664 windmill_api-1.96.2/windmill_api/api/script/delete_script_by_hash.py
+-rw-r--r--   0        0        0     2873 2023-05-08 21:40:02.605664 windmill_api-1.96.2/windmill_api/api/script/delete_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-05-08 21:40:02.633664 windmill_api-1.96.2/windmill_api/api/script/deno_to_jsonschema.py
+-rw-r--r--   0        0        0     2767 2023-05-08 21:40:02.649664 windmill_api-1.96.2/windmill_api/api/script/exists_script_by_path.py
+-rw-r--r--   0        0        0     2802 2023-05-08 21:40:02.685664 windmill_api-1.96.2/windmill_api/api/script/get_hub_script_by_path.py
+-rw-r--r--   0        0        0     1607 2023-05-08 21:40:02.677664 windmill_api-1.96.2/windmill_api/api/script/get_hub_script_content_by_path.py
+-rw-r--r--   0        0        0     3092 2023-05-08 21:40:02.717664 windmill_api-1.96.2/windmill_api/api/script/get_script_by_hash.py
+-rw-r--r--   0        0        0     3074 2023-05-08 21:40:02.725664 windmill_api-1.96.2/windmill_api/api/script/get_script_by_path.py
+-rw-r--r--   0        0        0     3241 2023-05-08 21:40:02.761664 windmill_api-1.96.2/windmill_api/api/script/get_script_by_path_with_draft.py
+-rw-r--r--   0        0        0     3276 2023-05-08 21:40:02.765663 windmill_api-1.96.2/windmill_api/api/script/get_script_deployment_status.py
+-rw-r--r--   0        0        0     2967 2023-05-08 21:40:02.801663 windmill_api-1.96.2/windmill_api/api/script/go_to_jsonschema.py
+-rw-r--r--   0        0        0     2459 2023-05-08 21:40:02.809664 windmill_api-1.96.2/windmill_api/api/script/list_hub_scripts.py
+-rw-r--r--   0        0        0     1676 2023-05-08 21:40:02.841663 windmill_api-1.96.2/windmill_api/api/script/list_script_paths.py
+-rw-r--r--   0        0        0    11165 2023-05-08 21:40:02.941663 windmill_api-1.96.2/windmill_api/api/script/list_scripts.py
+-rw-r--r--   0        0        0     3039 2023-05-08 21:40:02.881663 windmill_api-1.96.2/windmill_api/api/script/python_to_jsonschema.py
+-rw-r--r--   0        0        0     1784 2023-05-08 21:40:02.909664 windmill_api-1.96.2/windmill_api/api/script/raw_script_by_hash.py
+-rw-r--r--   0        0        0     1784 2023-05-08 21:40:02.937663 windmill_api-1.96.2/windmill_api/api/script/raw_script_by_path.py
+-rw-r--r--   0        0        0     2119 2023-05-08 21:40:02.981663 windmill_api-1.96.2/windmill_api/api/script/raw_script_by_path_tokened.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.129673 windmill_api-1.96.2/windmill_api/api/settings/__init__.py
+-rw-r--r--   0        0        0     1414 2023-05-08 21:40:02.965663 windmill_api-1.96.2/windmill_api/api/settings/backend_version.py
+-rw-r--r--   0        0        0     1423 2023-05-08 21:40:02.989663 windmill_api-1.96.2/windmill_api/api/settings/get_open_api_yaml.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.157673 windmill_api-1.96.2/windmill_api/api/user/__init__.py
+-rw-r--r--   0        0        0     1857 2023-05-08 21:40:03.013663 windmill_api-1.96.2/windmill_api/api/user/accept_invite.py
+-rw-r--r--   0        0        0     1822 2023-05-08 21:40:03.033663 windmill_api-1.96.2/windmill_api/api/user/create_token.py
+-rw-r--r--   0        0        0     1991 2023-05-08 21:40:03.041663 windmill_api-1.96.2/windmill_api/api/user/create_token_impersonate.py
+-rw-r--r--   0        0        0     2058 2023-05-08 21:40:03.061663 windmill_api-1.96.2/windmill_api/api/user/create_user.py
+-rw-r--r--   0        0        0     1863 2023-05-08 21:40:03.069663 windmill_api-1.96.2/windmill_api/api/user/create_user_globally.py
+-rw-r--r--   0        0        0     1867 2023-05-08 21:40:03.089663 windmill_api-1.96.2/windmill_api/api/user/decline_invite.py
+-rw-r--r--   0        0        0     1674 2023-05-08 21:40:03.097663 windmill_api-1.96.2/windmill_api/api/user/delete_token.py
+-rw-r--r--   0        0        0     1872 2023-05-08 21:40:03.117663 windmill_api-1.96.2/windmill_api/api/user/delete_user.py
+-rw-r--r--   0        0        0     1454 2023-05-08 21:40:03.125663 windmill_api-1.96.2/windmill_api/api/user/get_current_email.py
+-rw-r--r--   0        0        0     1474 2023-05-08 21:40:03.141663 windmill_api-1.96.2/windmill_api/api/user/get_usage.py
+-rw-r--r--   0        0        0     1639 2023-05-08 21:40:03.153663 windmill_api-1.96.2/windmill_api/api/user/global_user_delete.py
+-rw-r--r--   0        0        0     2060 2023-05-08 21:40:03.169663 windmill_api-1.96.2/windmill_api/api/user/global_user_update.py
+-rw-r--r--   0        0        0     2468 2023-05-08 21:40:03.189663 windmill_api-1.96.2/windmill_api/api/user/global_whoami.py
+-rw-r--r--   0        0        0     2745 2023-05-08 21:40:03.209663 windmill_api-1.96.2/windmill_api/api/user/is_owner_of_path.py
+-rw-r--r--   0        0        0     1646 2023-05-08 21:40:03.225663 windmill_api-1.96.2/windmill_api/api/user/leave_workspace.py
+-rw-r--r--   0        0        0     2633 2023-05-08 21:40:03.245663 windmill_api-1.96.2/windmill_api/api/user/list_tokens.py
+-rw-r--r--   0        0        0     2552 2023-05-08 21:40:03.265663 windmill_api-1.96.2/windmill_api/api/user/list_usernames.py
+-rw-r--r--   0        0        0     3012 2023-05-08 21:40:03.285663 windmill_api-1.96.2/windmill_api/api/user/list_users.py
+-rw-r--r--   0        0        0     4222 2023-05-08 21:40:03.321663 windmill_api-1.96.2/windmill_api/api/user/list_users_as_super_admin.py
+-rw-r--r--   0        0        0     2829 2023-05-08 21:40:03.321663 windmill_api-1.96.2/windmill_api/api/user/list_workspace_invites.py
+-rw-r--r--   0        0        0     1784 2023-05-08 21:40:03.361663 windmill_api-1.96.2/windmill_api/api/user/login.py
+-rw-r--r--   0        0        0     2116 2023-05-08 21:40:03.353663 windmill_api-1.96.2/windmill_api/api/user/login_with_oauth.py
+-rw-r--r--   0        0        0     1393 2023-05-08 21:40:03.377663 windmill_api-1.96.2/windmill_api/api/user/logout.py
+-rw-r--r--   0        0        0     1820 2023-05-08 21:40:03.385663 windmill_api-1.96.2/windmill_api/api/user/set_password.py
+-rw-r--r--   0        0        0     2250 2023-05-08 21:40:03.413663 windmill_api-1.96.2/windmill_api/api/user/update_user.py
+-rw-r--r--   0        0        0     2652 2023-05-08 21:40:03.421663 windmill_api-1.96.2/windmill_api/api/user/whoami.py
+-rw-r--r--   0        0        0     2967 2023-05-08 21:40:03.457663 windmill_api-1.96.2/windmill_api/api/user/whois.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.181673 windmill_api-1.96.2/windmill_api/api/variable/__init__.py
+-rw-r--r--   0        0        0     2634 2023-05-08 21:40:03.457663 windmill_api-1.96.2/windmill_api/api/variable/create_variable.py
+-rw-r--r--   0        0        0     1784 2023-05-08 21:40:03.485663 windmill_api-1.96.2/windmill_api/api/variable/delete_variable.py
+-rw-r--r--   0        0        0     2795 2023-05-08 21:40:03.497663 windmill_api-1.96.2/windmill_api/api/variable/exists_variable.py
+-rw-r--r--   0        0        0     3840 2023-05-08 21:40:03.537663 windmill_api-1.96.2/windmill_api/api/variable/get_variable.py
+-rw-r--r--   0        0        0     3270 2023-05-08 21:40:03.537663 windmill_api-1.96.2/windmill_api/api/variable/list_contextual_variables.py
+-rw-r--r--   0        0        0     3071 2023-05-08 21:40:03.593663 windmill_api-1.96.2/windmill_api/api/variable/list_variable.py
+-rw-r--r--   0        0        0     2775 2023-05-08 21:40:03.577663 windmill_api-1.96.2/windmill_api/api/variable/update_variable.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.245673 windmill_api-1.96.2/windmill_api/api/worker/__init__.py
+-rw-r--r--   0        0        0     2448 2023-05-08 21:40:03.617663 windmill_api-1.96.2/windmill_api/api/worker/get_custom_tags.py
+-rw-r--r--   0        0        0     3896 2023-05-08 21:40:03.645663 windmill_api-1.96.2/windmill_api/api/worker/list_workers.py
+-rw-r--r--   0        0        0        0 2023-05-08 21:39:49.173673 windmill_api-1.96.2/windmill_api/api/workspace/__init__.py
+-rw-r--r--   0        0        0     2015 2023-05-08 21:40:03.649663 windmill_api-1.96.2/windmill_api/api/workspace/add_user.py
+-rw-r--r--   0        0        0     1647 2023-05-08 21:40:03.673663 windmill_api-1.96.2/windmill_api/api/workspace/archive_workspace.py
+-rw-r--r--   0        0        0     1856 2023-05-08 21:40:03.677663 windmill_api-1.96.2/windmill_api/api/workspace/create_workspace.py
+-rw-r--r--   0        0        0     2049 2023-05-08 21:40:03.701663 windmill_api-1.96.2/windmill_api/api/workspace/delete_invite.py
+-rw-r--r--   0        0        0     1688 2023-05-08 21:40:03.717663 windmill_api-1.96.2/windmill_api/api/workspace/delete_workspace.py
+-rw-r--r--   0        0        0     2063 2023-05-08 21:40:03.729663 windmill_api-1.96.2/windmill_api/api/workspace/edit_auto_invite.py
+-rw-r--r--   0        0        0     2083 2023-05-08 21:40:03.749663 windmill_api-1.96.2/windmill_api/api/workspace/edit_slack_command.py
+-rw-r--r--   0        0        0     2029 2023-05-08 21:40:03.757663 windmill_api-1.96.2/windmill_api/api/workspace/edit_webhook.py
+-rw-r--r--   0        0        0     1856 2023-05-08 21:40:03.777663 windmill_api-1.96.2/windmill_api/api/workspace/exists_username.py
+-rw-r--r--   0        0        0     1856 2023-05-08 21:40:03.785663 windmill_api-1.96.2/windmill_api/api/workspace/exists_workspace.py
+-rw-r--r--   0        0        0     2809 2023-05-08 21:40:03.817663 windmill_api-1.96.2/windmill_api/api/workspace/get_premium_info.py
+-rw-r--r--   0        0        0     2753 2023-05-08 21:40:03.821663 windmill_api-1.96.2/windmill_api/api/workspace/get_settings.py
+-rw-r--r--   0        0        0     2045 2023-05-08 21:40:03.845663 windmill_api-1.96.2/windmill_api/api/workspace/invite_user.py
+-rw-r--r--   0        0        0     2176 2023-05-08 21:40:03.857663 windmill_api-1.96.2/windmill_api/api/workspace/is_domain_allowed.py
+-rw-r--r--   0        0        0     3255 2023-05-08 21:40:03.889663 windmill_api-1.96.2/windmill_api/api/workspace/list_pending_invites.py
+-rw-r--r--   0        0        0     2583 2023-05-08 21:40:03.901663 windmill_api-1.96.2/windmill_api/api/workspace/list_user_workspaces.py
+-rw-r--r--   0        0        0     2775 2023-05-08 21:40:03.929663 windmill_api-1.96.2/windmill_api/api/workspace/list_workspaces.py
+-rw-r--r--   0        0        0     4311 2023-05-08 21:40:03.957663 windmill_api-1.96.2/windmill_api/api/workspace/list_workspaces_as_super_admin.py
+-rw-r--r--   0        0        0     1651 2023-05-08 21:40:03.957663 windmill_api-1.96.2/windmill_api/api/workspace/unarchive_workspace.py
+-rw-r--r--   0        0        0     1821 2023-05-08 21:40:03.985663 windmill_api-1.96.2/windmill_api/client.py
+-rw-r--r--   0        0        0        1 2023-05-08 21:40:21.021655 windmill_api-1.96.2/windmill_api/models/__init__.py
+-rw-r--r--   0        0        0     1667 2023-05-08 21:40:04.013662 windmill_api-1.96.2/windmill_api/models/accept_invite_json_body.py
+-rw-r--r--   0        0        0     1710 2023-05-08 21:40:04.041663 windmill_api-1.96.2/windmill_api/models/add_granular_acls_json_body.py
+-rw-r--r--   0        0        0      325 2023-05-08 21:39:58.381667 windmill_api-1.96.2/windmill_api/models/add_granular_acls_kind.py
+-rw-r--r--   0        0        0     1529 2023-05-08 21:40:04.093663 windmill_api-1.96.2/windmill_api/models/add_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1940 2023-05-08 21:40:04.101662 windmill_api-1.96.2/windmill_api/models/add_user_json_body.py
+-rw-r--r--   0        0        0     1552 2023-05-08 21:40:04.121662 windmill_api-1.96.2/windmill_api/models/add_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3940 2023-05-08 21:40:04.153663 windmill_api-1.96.2/windmill_api/models/app_with_last_version.py
+-rw-r--r--   0        0        0      214 2023-05-08 21:39:58.857667 windmill_api-1.96.2/windmill_api/models/app_with_last_version_execution_mode.py
+-rw-r--r--   0        0        0     1248 2023-05-08 21:40:04.141662 windmill_api-1.96.2/windmill_api/models/app_with_last_version_extra_perms.py
+-rw-r--r--   0        0        0     3716 2023-05-08 21:40:04.193663 windmill_api-1.96.2/windmill_api/models/app_with_last_version_policy.py
+-rw-r--r--   0        0        0      220 2023-05-08 21:39:58.901667 windmill_api-1.96.2/windmill_api/models/app_with_last_version_policy_execution_mode.py
+-rw-r--r--   0        0        0     1946 2023-05-08 21:40:04.181662 windmill_api-1.96.2/windmill_api/models/app_with_last_version_policy_triggerables.py
+-rw-r--r--   0        0        0     1381 2023-05-08 21:40:04.217662 windmill_api-1.96.2/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4638 2023-05-08 21:40:04.257662 windmill_api-1.96.2/windmill_api/models/app_with_last_version_w_draft.py
+-rw-r--r--   0        0        0      220 2023-05-08 21:39:58.917667 windmill_api-1.96.2/windmill_api/models/app_with_last_version_w_draft_execution_mode.py
+-rw-r--r--   0        0        0     1284 2023-05-08 21:40:04.241662 windmill_api-1.96.2/windmill_api/models/app_with_last_version_w_draft_extra_perms.py
+-rw-r--r--   0        0        0     3828 2023-05-08 21:40:04.289662 windmill_api-1.96.2/windmill_api/models/app_with_last_version_w_draft_policy.py
+-rw-r--r--   0        0        0      226 2023-05-08 21:39:58.481667 windmill_api-1.96.2/windmill_api/models/app_with_last_version_w_draft_policy_execution_mode.py
+-rw-r--r--   0        0        0     2020 2023-05-08 21:40:04.285662 windmill_api-1.96.2/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py
+-rw-r--r--   0        0        0     1417 2023-05-08 21:40:04.305662 windmill_api-1.96.2/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1569 2023-05-08 21:40:04.313662 windmill_api-1.96.2/windmill_api/models/archive_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     7662 2023-05-08 21:40:04.409662 windmill_api-1.96.2/windmill_api/models/archive_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1314 2023-05-08 21:40:04.333662 windmill_api-1.96.2/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      259 2023-05-08 21:39:59.125666 windmill_api-1.96.2/windmill_api/models/archive_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      217 2023-05-08 21:39:58.825667 windmill_api-1.96.2/windmill_api/models/archive_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1288 2023-05-08 21:40:04.357662 windmill_api-1.96.2/windmill_api/models/archive_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     3452 2023-05-08 21:40:04.405662 windmill_api-1.96.2/windmill_api/models/audit_log.py
+-rw-r--r--   0        0        0      217 2023-05-08 21:39:58.889667 windmill_api-1.96.2/windmill_api/models/audit_log_action_kind.py
+-rw-r--r--   0        0        0      620 2023-05-08 21:39:58.785667 windmill_api-1.96.2/windmill_api/models/audit_log_operation.py
+-rw-r--r--   0        0        0     1186 2023-05-08 21:40:04.429662 windmill_api-1.96.2/windmill_api/models/audit_log_parameters.py
+-rw-r--r--   0        0        0     2933 2023-05-08 21:40:04.453662 windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-05-08 21:40:04.485662 windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-05-08 21:39:58.801667 windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-05-08 21:40:04.497662 windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-05-08 21:40:04.513662 windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-05-08 21:40:04.529662 windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-05-08 21:40:04.549662 windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-05-08 21:39:58.961667 windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-05-08 21:40:04.557662 windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-05-08 21:40:04.601662 windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-05-08 21:39:58.901667 windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-05-08 21:40:04.585662 windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-08 21:39:58.229667 windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2377 2023-05-08 21:40:04.625662 windmill_api-1.96.2/windmill_api/models/branch_all.py
+-rw-r--r--   0        0        0     2543 2023-05-08 21:40:04.637662 windmill_api-1.96.2/windmill_api/models/branch_all_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-05-08 21:40:04.709662 windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-05-08 21:40:04.677662 windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-08 21:40:04.705662 windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-08 21:40:04.741662 windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-08 21:40:04.741662 windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-08 21:39:58.873667 windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-08 21:40:04.769662 windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-08 21:39:58.493667 windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-08 21:40:04.773662 windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-08 21:40:04.797662 windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-05-08 21:39:58.421667 windmill_api-1.96.2/windmill_api/models/branch_all_type.py
+-rw-r--r--   0        0        0     2670 2023-05-08 21:40:04.817662 windmill_api-1.96.2/windmill_api/models/branch_one.py
+-rw-r--r--   0        0        0     2372 2023-05-08 21:40:04.833662 windmill_api-1.96.2/windmill_api/models/branch_one_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-05-08 21:40:04.913662 windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-05-08 21:40:04.873662 windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-08 21:40:04.901662 windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-08 21:40:04.949662 windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-08 21:40:04.941662 windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-08 21:39:58.793667 windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-08 21:40:04.977662 windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-08 21:39:58.365667 windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-08 21:40:04.981662 windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-08 21:40:05.009662 windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6125 2023-05-08 21:40:05.069662 windmill_api-1.96.2/windmill_api/models/branch_one_default_item.py
+-rw-r--r--   0        0        0     2906 2023-05-08 21:40:05.053662 windmill_api-1.96.2/windmill_api/models/branch_one_default_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-05-08 21:40:05.081662 windmill_api-1.96.2/windmill_api/models/branch_one_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-05-08 21:40:05.105662 windmill_api-1.96.2/windmill_api/models/branch_one_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-05-08 21:40:05.109662 windmill_api-1.96.2/windmill_api/models/branch_one_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-05-08 21:39:58.489667 windmill_api-1.96.2/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-05-08 21:40:05.137662 windmill_api-1.96.2/windmill_api/models/branch_one_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-08 21:39:59.041667 windmill_api-1.96.2/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-05-08 21:40:05.141662 windmill_api-1.96.2/windmill_api/models/branch_one_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-05-08 21:40:05.165662 windmill_api-1.96.2/windmill_api/models/branch_one_default_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-05-08 21:39:58.881667 windmill_api-1.96.2/windmill_api/models/branch_one_type.py
+-rw-r--r--   0        0        0     1532 2023-05-08 21:40:05.173662 windmill_api-1.96.2/windmill_api/models/cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     1255 2023-05-08 21:40:05.185662 windmill_api-1.96.2/windmill_api/models/cancel_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0    10508 2023-05-08 21:40:05.329661 windmill_api-1.96.2/windmill_api/models/completed_job.py
+-rw-r--r--   0        0        0     1176 2023-05-08 21:40:05.205662 windmill_api-1.96.2/windmill_api/models/completed_job_args.py
+-rw-r--r--   0        0        0     3265 2023-05-08 21:40:05.249662 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status.py
+-rw-r--r--   0        0        0     6800 2023-05-08 21:40:05.349661 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1789 2023-05-08 21:40:05.361662 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2136 2023-05-08 21:40:05.377662 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      202 2023-05-08 21:39:59.053666 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1694 2023-05-08 21:40:05.389661 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2230 2023-05-08 21:40:05.413661 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      360 2023-05-08 21:39:58.345667 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6402 2023-05-08 21:40:05.477661 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1779 2023-05-08 21:40:05.437662 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2116 2023-05-08 21:40:05.469661 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      200 2023-05-08 21:39:58.121667 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1684 2023-05-08 21:40:05.497661 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2220 2023-05-08 21:40:05.517661 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      358 2023-05-08 21:39:59.125666 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2040 2023-05-08 21:40:05.529661 windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_retry.py
+-rw-r--r--   0        0        0      310 2023-05-08 21:39:58.569667 windmill_api-1.96.2/windmill_api/models/completed_job_job_kind.py
+-rw-r--r--   0        0        0      199 2023-05-08 21:39:58.109667 windmill_api-1.96.2/windmill_api/models/completed_job_language.py
+-rw-r--r--   0        0        0     3127 2023-05-08 21:40:05.569661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow.py
+-rw-r--r--   0        0        0     6620 2023-05-08 21:40:05.609661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3129 2023-05-08 21:40:05.613661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-08 21:40:05.641661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-08 21:40:05.673661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-08 21:40:05.669661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-08 21:39:58.657667 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-08 21:40:05.717661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-08 21:39:58.653667 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-08 21:40:05.705661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-08 21:40:05.737661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6544 2023-05-08 21:40:05.797661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3095 2023-05-08 21:40:05.777661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1919 2023-05-08 21:40:05.809661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2223 2023-05-08 21:40:05.829661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2050 2023-05-08 21:40:05.841661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      179 2023-05-08 21:39:58.461667 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1917 2023-05-08 21:40:05.857661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      179 2023-05-08 21:39:58.497667 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1912 2023-05-08 21:40:05.873661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1963 2023-05-08 21:40:05.885661 windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1572 2023-05-08 21:40:05.901661 windmill_api-1.96.2/windmill_api/models/connect_callback_json_body.py
+-rw-r--r--   0        0        0     2533 2023-05-08 21:40:05.925661 windmill_api-1.96.2/windmill_api/models/connect_callback_response_200.py
+-rw-r--r--   0        0        0     1600 2023-05-08 21:40:05.925661 windmill_api-1.96.2/windmill_api/models/connect_slack_callback_json_body.py
+-rw-r--r--   0        0        0     1753 2023-05-08 21:40:05.953661 windmill_api-1.96.2/windmill_api/models/contextual_variable.py
+-rw-r--r--   0        0        0     2147 2023-05-08 21:40:05.961661 windmill_api-1.96.2/windmill_api/models/create_account_json_body.py
+-rw-r--r--   0        0        0     2367 2023-05-08 21:40:05.989661 windmill_api-1.96.2/windmill_api/models/create_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-05-08 21:40:06.013661 windmill_api-1.96.2/windmill_api/models/create_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-05-08 21:39:59.133666 windmill_api-1.96.2/windmill_api/models/create_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-05-08 21:40:06.017661 windmill_api-1.96.2/windmill_api/models/create_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-05-08 21:40:06.037661 windmill_api-1.96.2/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1947 2023-05-08 21:40:06.065661 windmill_api-1.96.2/windmill_api/models/create_draft_json_body.py
+-rw-r--r--   0        0        0      183 2023-05-08 21:39:58.609667 windmill_api-1.96.2/windmill_api/models/create_draft_json_body_typ.py
+-rw-r--r--   0        0        0     1550 2023-05-08 21:40:06.105661 windmill_api-1.96.2/windmill_api/models/create_flow_json_body.py
+-rw-r--r--   0        0        0     2126 2023-05-08 21:40:06.101661 windmill_api-1.96.2/windmill_api/models/create_folder_json_body.py
+-rw-r--r--   0        0        0     1697 2023-05-08 21:40:06.129661 windmill_api-1.96.2/windmill_api/models/create_group_json_body.py
+-rw-r--r--   0        0        0     1613 2023-05-08 21:40:06.133661 windmill_api-1.96.2/windmill_api/models/create_input.py
+-rw-r--r--   0        0        0     1171 2023-05-08 21:40:06.149661 windmill_api-1.96.2/windmill_api/models/create_input_args.py
+-rw-r--r--   0        0        0     1701 2023-05-08 21:40:06.161661 windmill_api-1.96.2/windmill_api/models/create_input_json_body.py
+-rw-r--r--   0        0        0     1217 2023-05-08 21:40:06.169661 windmill_api-1.96.2/windmill_api/models/create_input_json_body_args.py
+-rw-r--r--   0        0        0      214 2023-05-08 21:39:58.137667 windmill_api-1.96.2/windmill_api/models/create_input_runnable_type.py
+-rw-r--r--   0        0        0     1732 2023-05-08 21:40:06.197661 windmill_api-1.96.2/windmill_api/models/create_raw_app_json_body.py
+-rw-r--r--   0        0        0     2094 2023-05-08 21:40:06.201661 windmill_api-1.96.2/windmill_api/models/create_resource.py
+-rw-r--r--   0        0        0     2140 2023-05-08 21:40:06.229661 windmill_api-1.96.2/windmill_api/models/create_resource_json_body.py
+-rw-r--r--   0        0        0     2335 2023-05-08 21:40:06.237661 windmill_api-1.96.2/windmill_api/models/create_resource_type_json_body.py
+-rw-r--r--   0        0        0     2780 2023-05-08 21:40:06.273661 windmill_api-1.96.2/windmill_api/models/create_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-08 21:40:06.261661 windmill_api-1.96.2/windmill_api/models/create_schedule_json_body_args.py
+-rw-r--r--   0        0        0     5120 2023-05-08 21:40:06.333661 windmill_api-1.96.2/windmill_api/models/create_script_json_body.py
+-rw-r--r--   0        0        0      249 2023-05-08 21:39:59.133666 windmill_api-1.96.2/windmill_api/models/create_script_json_body_kind.py
+-rw-r--r--   0        0        0      207 2023-05-08 21:39:58.113667 windmill_api-1.96.2/windmill_api/models/create_script_json_body_language.py
+-rw-r--r--   0        0        0     1232 2023-05-08 21:40:06.301661 windmill_api-1.96.2/windmill_api/models/create_script_json_body_schema.py
+-rw-r--r--   0        0        0     2534 2023-05-08 21:40:06.337661 windmill_api-1.96.2/windmill_api/models/create_token_impersonate_json_body.py
+-rw-r--r--   0        0        0     2169 2023-05-08 21:40:06.365661 windmill_api-1.96.2/windmill_api/models/create_token_json_body.py
+-rw-r--r--   0        0        0     2364 2023-05-08 21:40:06.377661 windmill_api-1.96.2/windmill_api/models/create_user_globally_json_body.py
+-rw-r--r--   0        0        0     1771 2023-05-08 21:40:06.393661 windmill_api-1.96.2/windmill_api/models/create_user_json_body.py
+-rw-r--r--   0        0        0     2493 2023-05-08 21:40:06.417661 windmill_api-1.96.2/windmill_api/models/create_variable.py
+-rw-r--r--   0        0        0     2539 2023-05-08 21:40:06.449661 windmill_api-1.96.2/windmill_api/models/create_variable_json_body.py
+-rw-r--r--   0        0        0     1678 2023-05-08 21:40:06.445661 windmill_api-1.96.2/windmill_api/models/create_workspace.py
+-rw-r--r--   0        0        0     1724 2023-05-08 21:40:06.489661 windmill_api-1.96.2/windmill_api/models/create_workspace_json_body.py
+-rw-r--r--   0        0        0     1490 2023-05-08 21:40:06.473661 windmill_api-1.96.2/windmill_api/models/decline_invite_json_body.py
+-rw-r--r--   0        0        0    11110 2023-05-08 21:40:06.613660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200.py
+-rw-r--r--   0        0        0     1270 2023-05-08 21:40:06.509661 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3658 2023-05-08 21:40:06.553660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7442 2023-05-08 21:40:06.641660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1883 2023-05-08 21:40:06.637660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2318 2023-05-08 21:40:06.669660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      219 2023-05-08 21:39:58.685667 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1788 2023-05-08 21:40:06.673660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2324 2023-05-08 21:40:06.705660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      377 2023-05-08 21:39:58.877667 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7053 2023-05-08 21:40:06.761660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1873 2023-05-08 21:40:06.729660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2298 2023-05-08 21:40:06.757660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      217 2023-05-08 21:39:58.269667 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1778 2023-05-08 21:40:06.785660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2314 2023-05-08 21:40:06.797660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      375 2023-05-08 21:39:58.289667 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2134 2023-05-08 21:40:06.841660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      327 2023-05-08 21:39:58.117667 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      216 2023-05-08 21:39:58.625667 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3432 2023-05-08 21:40:06.873660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7425 2023-05-08 21:40:06.925660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3442 2023-05-08 21:40:06.913660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2023 2023-05-08 21:40:06.945660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2327 2023-05-08 21:40:06.957660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2261 2023-05-08 21:40:06.973660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-08 21:39:58.297667 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-08 21:40:06.989660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-08 21:39:58.865667 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2016 2023-05-08 21:40:07.005660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2067 2023-05-08 21:40:07.021660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7349 2023-05-08 21:40:07.089660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3408 2023-05-08 21:40:07.061660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2013 2023-05-08 21:40:07.093660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2317 2023-05-08 21:40:07.121660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2241 2023-05-08 21:40:07.125660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-05-08 21:39:58.849667 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2108 2023-05-08 21:40:07.149660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-05-08 21:39:58.669667 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2006 2023-05-08 21:40:07.161660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2057 2023-05-08 21:40:07.177660 windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1783 2023-05-08 21:40:07.213660 windmill_api-1.96.2/windmill_api/models/delete_invite_json_body.py
+-rw-r--r--   0        0        0     7636 2023-05-08 21:40:07.293660 windmill_api-1.96.2/windmill_api/models/delete_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1309 2023-05-08 21:40:07.233660 windmill_api-1.96.2/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      258 2023-05-08 21:39:58.685667 windmill_api-1.96.2/windmill_api/models/delete_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      216 2023-05-08 21:39:58.193667 windmill_api-1.96.2/windmill_api/models/delete_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1283 2023-05-08 21:40:07.257660 windmill_api-1.96.2/windmill_api/models/delete_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     2933 2023-05-08 21:40:07.301660 windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-05-08 21:40:07.353660 windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-05-08 21:39:58.285667 windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-05-08 21:40:07.329660 windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-05-08 21:40:07.353660 windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-05-08 21:40:07.381660 windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-05-08 21:40:07.393660 windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-05-08 21:39:58.669667 windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-05-08 21:40:07.405660 windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-05-08 21:40:07.437660 windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-05-08 21:39:58.597667 windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-05-08 21:40:07.433660 windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-08 21:39:58.457667 windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     1551 2023-05-08 21:40:07.457660 windmill_api-1.96.2/windmill_api/models/edit_auto_invite_json_body.py
+-rw-r--r--   0        0        0     1980 2023-05-08 21:40:07.469660 windmill_api-1.96.2/windmill_api/models/edit_resource.py
+-rw-r--r--   0        0        0     1791 2023-05-08 21:40:07.489660 windmill_api-1.96.2/windmill_api/models/edit_resource_type.py
+-rw-r--r--   0        0        0     1845 2023-05-08 21:40:07.501660 windmill_api-1.96.2/windmill_api/models/edit_schedule.py
+-rw-r--r--   0        0        0     1176 2023-05-08 21:40:07.509660 windmill_api-1.96.2/windmill_api/models/edit_schedule_args.py
+-rw-r--r--   0        0        0     1691 2023-05-08 21:40:07.529660 windmill_api-1.96.2/windmill_api/models/edit_slack_command_json_body.py
+-rw-r--r--   0        0        0     2260 2023-05-08 21:40:07.545660 windmill_api-1.96.2/windmill_api/models/edit_variable.py
+-rw-r--r--   0        0        0     1520 2023-05-08 21:40:07.553660 windmill_api-1.96.2/windmill_api/models/edit_webhook_json_body.py
+-rw-r--r--   0        0        0     2058 2023-05-08 21:40:07.581660 windmill_api-1.96.2/windmill_api/models/edit_workspace_user.py
+-rw-r--r--   0        0        0     3663 2023-05-08 21:40:07.621660 windmill_api-1.96.2/windmill_api/models/execute_component_json_body.py
+-rw-r--r--   0        0        0     1346 2023-05-08 21:40:07.621660 windmill_api-1.96.2/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
+-rw-r--r--   0        0        0     1942 2023-05-08 21:40:07.649660 windmill_api-1.96.2/windmill_api/models/execute_component_json_body_raw_code.py
+-rw-r--r--   0        0        0     1577 2023-05-08 21:40:07.649660 windmill_api-1.96.2/windmill_api/models/exists_username_json_body.py
+-rw-r--r--   0        0        0     1400 2023-05-08 21:40:07.673660 windmill_api-1.96.2/windmill_api/models/exists_workspace_json_body.py
+-rw-r--r--   0        0        0     4924 2023-05-08 21:40:07.721660 windmill_api-1.96.2/windmill_api/models/flow.py
+-rw-r--r--   0        0        0     1166 2023-05-08 21:40:07.693660 windmill_api-1.96.2/windmill_api/models/flow_extra_perms.py
+-rw-r--r--   0        0        0     3707 2023-05-08 21:40:07.741659 windmill_api-1.96.2/windmill_api/models/flow_metadata.py
+-rw-r--r--   0        0        0     1209 2023-05-08 21:40:07.741659 windmill_api-1.96.2/windmill_api/models/flow_metadata_extra_perms.py
+-rw-r--r--   0        0        0     5729 2023-05-08 21:40:07.821659 windmill_api-1.96.2/windmill_api/models/flow_module.py
+-rw-r--r--   0        0        0     2726 2023-05-08 21:40:07.781659 windmill_api-1.96.2/windmill_api/models/flow_module_retry.py
+-rw-r--r--   0        0        0     1807 2023-05-08 21:40:07.813660 windmill_api-1.96.2/windmill_api/models/flow_module_retry_constant.py
+-rw-r--r--   0        0        0     2111 2023-05-08 21:40:07.845659 windmill_api-1.96.2/windmill_api/models/flow_module_retry_exponential.py
+-rw-r--r--   0        0        0     1834 2023-05-08 21:40:07.853659 windmill_api-1.96.2/windmill_api/models/flow_module_sleep_type_0.py
+-rw-r--r--   0        0        0      159 2023-05-08 21:39:58.697667 windmill_api-1.96.2/windmill_api/models/flow_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1701 2023-05-08 21:40:07.877659 windmill_api-1.96.2/windmill_api/models/flow_module_sleep_type_1.py
+-rw-r--r--   0        0        0      159 2023-05-08 21:39:58.401667 windmill_api-1.96.2/windmill_api/models/flow_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1800 2023-05-08 21:40:07.881659 windmill_api-1.96.2/windmill_api/models/flow_module_stop_after_if.py
+-rw-r--r--   0        0        0     1851 2023-05-08 21:40:07.909659 windmill_api-1.96.2/windmill_api/models/flow_module_suspend.py
+-rw-r--r--   0        0        0     3292 2023-05-08 21:40:07.925659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_0.py
+-rw-r--r--   0        0        0     3564 2023-05-08 21:40:07.945659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-08 21:40:07.953659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-08 21:39:58.673667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-08 21:40:08.001659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-08 21:39:58.685667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      208 2023-05-08 21:39:58.489667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_0_language.py
+-rw-r--r--   0        0        0      158 2023-05-08 21:39:59.029667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_0_type.py
+-rw-r--r--   0        0        0     2477 2023-05-08 21:40:08.017659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_1.py
+-rw-r--r--   0        0        0     3564 2023-05-08 21:40:08.041659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-08 21:40:08.049659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-08 21:39:59.101667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-08 21:40:08.073659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-08 21:39:58.929667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      152 2023-05-08 21:39:58.369667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_1_type.py
+-rw-r--r--   0        0        0     2204 2023-05-08 21:40:08.081659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_2.py
+-rw-r--r--   0        0        0     3564 2023-05-08 21:40:08.113659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-08 21:40:08.109659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-08 21:39:58.977667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-08 21:40:08.141659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-08 21:39:58.965667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      148 2023-05-08 21:39:58.361667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_2_type.py
+-rw-r--r--   0        0        0     4138 2023-05-08 21:40:08.169659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3.py
+-rw-r--r--   0        0        0     1990 2023-05-08 21:40:08.169659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
+-rw-r--r--   0        0        0      173 2023-05-08 21:39:58.549667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1857 2023-05-08 21:40:08.197659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
+-rw-r--r--   0        0        0      173 2023-05-08 21:39:59.029667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6636 2023-05-08 21:40:08.253659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item.py
+-rw-r--r--   0        0        0     3148 2023-05-08 21:40:08.237659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-05-08 21:40:08.265659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-05-08 21:40:08.289659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-05-08 21:40:08.293659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-08 21:39:59.113666 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-05-08 21:40:08.317659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-08 21:39:58.109667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-05-08 21:40:08.325659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-05-08 21:40:08.349659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
+-rw-r--r--   0        0        0      162 2023-05-08 21:39:58.501667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_type.py
+-rw-r--r--   0        0        0     2934 2023-05-08 21:40:08.385659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4.py
+-rw-r--r--   0        0        0     2508 2023-05-08 21:40:08.409659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-05-08 21:40:08.469659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-05-08 21:40:08.449659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-05-08 21:40:08.481659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-05-08 21:40:08.501659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-05-08 21:40:08.509659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-08 21:39:58.513667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-05-08 21:40:08.529659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-08 21:39:58.393667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-05-08 21:40:08.541659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-05-08 21:40:08.561659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6636 2023-05-08 21:40:08.625659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item.py
+-rw-r--r--   0        0        0     3148 2023-05-08 21:40:08.601659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-05-08 21:40:08.629659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-05-08 21:40:08.657659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-05-08 21:40:08.661659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-08 21:39:58.177667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-05-08 21:40:08.689659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-08 21:39:58.281667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-05-08 21:40:08.693659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-05-08 21:40:08.717659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-05-08 21:39:58.185667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_type.py
+-rw-r--r--   0        0        0     2577 2023-05-08 21:40:08.733659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5.py
+-rw-r--r--   0        0        0     2679 2023-05-08 21:40:08.777659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-05-08 21:40:08.845659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-05-08 21:40:08.817659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-05-08 21:40:08.845659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-05-08 21:40:08.877659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-05-08 21:40:08.877659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-08 21:39:58.337667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-05-08 21:40:08.909659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-08 21:39:58.625667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-05-08 21:40:08.909659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-05-08 21:40:08.937659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-05-08 21:39:58.813667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_type.py
+-rw-r--r--   0        0        0     1839 2023-05-08 21:40:08.937659 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_6.py
+-rw-r--r--   0        0        0      156 2023-05-08 21:39:58.989667 windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_6_type.py
+-rw-r--r--   0        0        0     2009 2023-05-08 21:40:08.973659 windmill_api-1.96.2/windmill_api/models/flow_preview.py
+-rw-r--r--   0        0        0     1171 2023-05-08 21:40:08.969659 windmill_api-1.96.2/windmill_api/models/flow_preview_args.py
+-rw-r--r--   0        0        0     3074 2023-05-08 21:40:09.009659 windmill_api-1.96.2/windmill_api/models/flow_preview_value.py
+-rw-r--r--   0        0        0     6498 2023-05-08 21:40:09.053659 windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module.py
+-rw-r--r--   0        0        0     3064 2023-05-08 21:40:09.049659 windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1911 2023-05-08 21:40:09.081659 windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2215 2023-05-08 21:40:09.085659 windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2036 2023-05-08 21:40:09.113659 windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-08 21:39:58.693667 windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1903 2023-05-08 21:40:09.117659 windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-08 21:39:58.229667 windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1904 2023-05-08 21:40:09.141659 windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1955 2023-05-08 21:40:09.169659 windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6422 2023-05-08 21:40:09.257659 windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item.py
+-rw-r--r--   0        0        0     3030 2023-05-08 21:40:09.209658 windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1901 2023-05-08 21:40:09.237659 windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2205 2023-05-08 21:40:09.273659 windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2016 2023-05-08 21:40:09.289658 windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-05-08 21:39:58.317667 windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1883 2023-05-08 21:40:09.301658 windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-05-08 21:39:58.241667 windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1894 2023-05-08 21:40:09.317659 windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1945 2023-05-08 21:40:09.329658 windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1143 2023-05-08 21:40:09.341658 windmill_api-1.96.2/windmill_api/models/flow_schema.py
+-rw-r--r--   0        0        0     3001 2023-05-08 21:40:09.373659 windmill_api-1.96.2/windmill_api/models/flow_status.py
+-rw-r--r--   0        0        0     6370 2023-05-08 21:40:09.425658 windmill_api-1.96.2/windmill_api/models/flow_status_failure_module.py
+-rw-r--r--   0        0        0     1723 2023-05-08 21:40:09.397658 windmill_api-1.96.2/windmill_api/models/flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     1999 2023-05-08 21:40:09.429659 windmill_api-1.96.2/windmill_api/models/flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      190 2023-05-08 21:39:58.289667 windmill_api-1.96.2/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1628 2023-05-08 21:40:09.453658 windmill_api-1.96.2/windmill_api/models/flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2164 2023-05-08 21:40:09.465658 windmill_api-1.96.2/windmill_api/models/flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      348 2023-05-08 21:39:58.877667 windmill_api-1.96.2/windmill_api/models/flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     5808 2023-05-08 21:40:09.541658 windmill_api-1.96.2/windmill_api/models/flow_status_module.py
+-rw-r--r--   0        0        0     1685 2023-05-08 21:40:09.489658 windmill_api-1.96.2/windmill_api/models/flow_status_module_approvers_item.py
+-rw-r--r--   0        0        0     1925 2023-05-08 21:40:09.545658 windmill_api-1.96.2/windmill_api/models/flow_status_module_branch_chosen.py
+-rw-r--r--   0        0        0      183 2023-05-08 21:39:58.929667 windmill_api-1.96.2/windmill_api/models/flow_status_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1590 2023-05-08 21:40:09.605658 windmill_api-1.96.2/windmill_api/models/flow_status_module_branchall.py
+-rw-r--r--   0        0        0     2126 2023-05-08 21:40:09.581658 windmill_api-1.96.2/windmill_api/models/flow_status_module_iterator.py
+-rw-r--r--   0        0        0      341 2023-05-08 21:39:58.957667 windmill_api-1.96.2/windmill_api/models/flow_status_module_type.py
+-rw-r--r--   0        0        0     5981 2023-05-08 21:40:09.665658 windmill_api-1.96.2/windmill_api/models/flow_status_modules_item.py
+-rw-r--r--   0        0        0     1713 2023-05-08 21:40:09.629658 windmill_api-1.96.2/windmill_api/models/flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     1979 2023-05-08 21:40:09.661658 windmill_api-1.96.2/windmill_api/models/flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      188 2023-05-08 21:39:58.609667 windmill_api-1.96.2/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1618 2023-05-08 21:40:09.689658 windmill_api-1.96.2/windmill_api/models/flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2154 2023-05-08 21:40:09.701658 windmill_api-1.96.2/windmill_api/models/flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      346 2023-05-08 21:39:58.469667 windmill_api-1.96.2/windmill_api/models/flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     1974 2023-05-08 21:40:09.725658 windmill_api-1.96.2/windmill_api/models/flow_status_retry.py
+-rw-r--r--   0        0        0     2957 2023-05-08 21:40:09.741658 windmill_api-1.96.2/windmill_api/models/flow_value.py
+-rw-r--r--   0        0        0     6224 2023-05-08 21:40:09.805658 windmill_api-1.96.2/windmill_api/models/flow_value_failure_module.py
+-rw-r--r--   0        0        0     2940 2023-05-08 21:40:09.781658 windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1873 2023-05-08 21:40:09.813658 windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-05-08 21:40:09.841658 windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-05-08 21:40:09.841658 windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-05-08 21:39:58.637667 windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-05-08 21:40:09.869658 windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-05-08 21:39:58.845667 windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-05-08 21:40:09.873658 windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-05-08 21:40:09.901658 windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6125 2023-05-08 21:40:09.981658 windmill_api-1.96.2/windmill_api/models/flow_value_modules_item.py
+-rw-r--r--   0        0        0     2906 2023-05-08 21:40:09.941658 windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-05-08 21:40:09.997658 windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-05-08 21:40:10.013658 windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-05-08 21:40:10.025658 windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-05-08 21:39:58.469667 windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-05-08 21:40:10.045658 windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-08 21:39:58.653667 windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-05-08 21:40:10.053658 windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-05-08 21:40:10.073658 windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1858 2023-05-08 21:40:10.085658 windmill_api-1.96.2/windmill_api/models/folder.py
+-rw-r--r--   0        0        0     1179 2023-05-08 21:40:10.097658 windmill_api-1.96.2/windmill_api/models/folder_extra_perms.py
+-rw-r--r--   0        0        0     1560 2023-05-08 21:40:10.109658 windmill_api-1.96.2/windmill_api/models/force_cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     3807 2023-05-08 21:40:10.149658 windmill_api-1.96.2/windmill_api/models/forloop_flow.py
+-rw-r--r--   0        0        0     1874 2023-05-08 21:40:10.137658 windmill_api-1.96.2/windmill_api/models/forloop_flow_iterator_type_0.py
+-rw-r--r--   0        0        0      163 2023-05-08 21:39:58.813667 windmill_api-1.96.2/windmill_api/models/forloop_flow_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1741 2023-05-08 21:40:10.165658 windmill_api-1.96.2/windmill_api/models/forloop_flow_iterator_type_1.py
+-rw-r--r--   0        0        0      163 2023-05-08 21:39:58.697667 windmill_api-1.96.2/windmill_api/models/forloop_flow_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6224 2023-05-08 21:40:10.233658 windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item.py
+-rw-r--r--   0        0        0     2940 2023-05-08 21:40:10.205658 windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1873 2023-05-08 21:40:10.233658 windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-05-08 21:40:10.269658 windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-05-08 21:40:10.261658 windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-05-08 21:39:58.145667 windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-05-08 21:40:10.293658 windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-05-08 21:39:59.053666 windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-05-08 21:40:10.325658 windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-05-08 21:40:10.321658 windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0      152 2023-05-08 21:39:58.321667 windmill_api-1.96.2/windmill_api/models/forloop_flow_type.py
+-rw-r--r--   0        0        0     4052 2023-05-08 21:40:10.377658 windmill_api-1.96.2/windmill_api/models/get_app_by_path_response_200.py
+-rw-r--r--   0        0        0      219 2023-05-08 21:39:59.077667 windmill_api-1.96.2/windmill_api/models/get_app_by_path_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1279 2023-05-08 21:40:10.349658 windmill_api-1.96.2/windmill_api/models/get_app_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3811 2023-05-08 21:40:10.429658 windmill_api-1.96.2/windmill_api/models/get_app_by_path_response_200_policy.py
+-rw-r--r--   0        0        0      225 2023-05-08 21:39:58.493667 windmill_api-1.96.2/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2009 2023-05-08 21:40:10.401658 windmill_api-1.96.2/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1412 2023-05-08 21:40:10.421658 windmill_api-1.96.2/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4819 2023-05-08 21:40:10.481658 windmill_api-1.96.2/windmill_api/models/get_app_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0      228 2023-05-08 21:39:58.921667 windmill_api-1.96.2/windmill_api/models/get_app_by_path_with_draft_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1330 2023-05-08 21:40:10.453658 windmill_api-1.96.2/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3992 2023-05-08 21:40:10.501658 windmill_api-1.96.2/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py
+-rw-r--r--   0        0        0      234 2023-05-08 21:39:58.521667 windmill_api-1.96.2/windmill_api/models/get_app_by_path_with_draft_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2160 2023-05-08 21:40:10.513658 windmill_api-1.96.2/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1463 2023-05-08 21:40:10.525658 windmill_api-1.96.2/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4112 2023-05-08 21:40:10.561658 windmill_api-1.96.2/windmill_api/models/get_app_by_version_response_200.py
+-rw-r--r--   0        0        0      222 2023-05-08 21:39:58.557667 windmill_api-1.96.2/windmill_api/models/get_app_by_version_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1294 2023-05-08 21:40:10.549658 windmill_api-1.96.2/windmill_api/models/get_app_by_version_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3862 2023-05-08 21:40:10.597658 windmill_api-1.96.2/windmill_api/models/get_app_by_version_response_200_policy.py
+-rw-r--r--   0        0        0      228 2023-05-08 21:39:58.853667 windmill_api-1.96.2/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2042 2023-05-08 21:40:10.589658 windmill_api-1.96.2/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1427 2023-05-08 21:40:10.609658 windmill_api-1.96.2/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3764 2023-05-08 21:40:10.649658 windmill_api-1.96.2/windmill_api/models/get_audit_log_response_200.py
+-rw-r--r--   0        0        0      231 2023-05-08 21:39:58.705667 windmill_api-1.96.2/windmill_api/models/get_audit_log_response_200_action_kind.py
+-rw-r--r--   0        0        0      634 2023-05-08 21:39:58.977667 windmill_api-1.96.2/windmill_api/models/get_audit_log_response_200_operation.py
+-rw-r--r--   0        0        0     1265 2023-05-08 21:40:10.633658 windmill_api-1.96.2/windmill_api/models/get_audit_log_response_200_parameters.py
+-rw-r--r--   0        0        0    11008 2023-05-08 21:40:10.805657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200.py
+-rw-r--r--   0        0        0     1255 2023-05-08 21:40:10.669658 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3595 2023-05-08 21:40:10.717658 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7343 2023-05-08 21:40:10.833658 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1868 2023-05-08 21:40:10.833658 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2288 2023-05-08 21:40:10.861657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      216 2023-05-08 21:39:58.373667 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1773 2023-05-08 21:40:10.865657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2309 2023-05-08 21:40:10.897657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      374 2023-05-08 21:39:58.117667 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6924 2023-05-08 21:40:10.949658 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1858 2023-05-08 21:40:10.925658 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-05-08 21:40:10.953657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-05-08 21:39:58.593667 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-05-08 21:40:10.977657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2299 2023-05-08 21:40:10.997657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      372 2023-05-08 21:39:58.373667 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2119 2023-05-08 21:40:11.021657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      324 2023-05-08 21:39:58.389667 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      213 2023-05-08 21:39:58.533667 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3375 2023-05-08 21:40:11.045657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7311 2023-05-08 21:40:11.105657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3391 2023-05-08 21:40:11.117657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2008 2023-05-08 21:40:11.137657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2312 2023-05-08 21:40:11.149657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2231 2023-05-08 21:40:11.169657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      195 2023-05-08 21:39:58.393667 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2098 2023-05-08 21:40:11.177657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      195 2023-05-08 21:39:59.001667 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2001 2023-05-08 21:40:11.237657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2052 2023-05-08 21:40:11.209657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7235 2023-05-08 21:40:11.293657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3357 2023-05-08 21:40:11.277657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1998 2023-05-08 21:40:11.309657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-05-08 21:40:11.325657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-05-08 21:40:11.337657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-08 21:39:58.677667 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-05-08 21:40:11.353657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-08 21:39:58.557667 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-05-08 21:40:11.369657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-05-08 21:40:11.385657 windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     5374 2023-05-08 21:40:11.441657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200.py
+-rw-r--r--   0        0        0     1281 2023-05-08 21:40:11.405657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1258 2023-05-08 21:40:11.425657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     3302 2023-05-08 21:40:11.493657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value.py
+-rw-r--r--   0        0        0     7159 2023-05-08 21:40:11.525657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
+-rw-r--r--   0        0        0     3323 2023-05-08 21:40:11.533657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1988 2023-05-08 21:40:11.553657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-05-08 21:40:11.565657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-05-08 21:40:11.629657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-05-08 21:39:58.097667 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-05-08 21:40:11.593657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-05-08 21:39:58.161667 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-05-08 21:40:11.625657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-05-08 21:40:11.657657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7066 2023-05-08 21:40:11.713657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
+-rw-r--r--   0        0        0     3289 2023-05-08 21:40:11.697657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1978 2023-05-08 21:40:11.725657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2282 2023-05-08 21:40:11.745657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2171 2023-05-08 21:40:11.757657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-05-08 21:39:58.105667 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2038 2023-05-08 21:40:11.777657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-05-08 21:39:58.489667 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1971 2023-05-08 21:40:11.785657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2022 2023-05-08 21:40:11.805657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2093 2023-05-08 21:40:11.817657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0     5695 2023-05-08 21:40:11.877657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py
+-rw-r--r--   0        0        0     1360 2023-05-08 21:40:11.861657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py
+-rw-r--r--   0        0        0     1337 2023-05-08 21:40:11.881657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py
+-rw-r--r--   0        0        0     3559 2023-05-08 21:40:11.921657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py
+-rw-r--r--   0        0        0     7829 2023-05-08 21:40:11.965657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py
+-rw-r--r--   0        0        0     3606 2023-05-08 21:40:11.961657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2067 2023-05-08 21:40:12.033657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2371 2023-05-08 21:40:11.997657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2343 2023-05-08 21:40:12.029657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      205 2023-05-08 21:39:58.313667 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2210 2023-05-08 21:40:12.057657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      205 2023-05-08 21:39:58.405667 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2060 2023-05-08 21:40:12.061657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2111 2023-05-08 21:40:12.089657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7685 2023-05-08 21:40:12.145657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py
+-rw-r--r--   0        0        0     3542 2023-05-08 21:40:12.129657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2057 2023-05-08 21:40:12.161657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2361 2023-05-08 21:40:12.177657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2323 2023-05-08 21:40:12.193657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      203 2023-05-08 21:39:58.269667 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2190 2023-05-08 21:40:12.205657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      203 2023-05-08 21:39:59.101667 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2050 2023-05-08 21:40:12.249657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2101 2023-05-08 21:40:12.237657 windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2756 2023-05-08 21:40:12.273657 windmill_api-1.96.2/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
+-rw-r--r--   0        0        0     1337 2023-05-08 21:40:12.269657 windmill_api-1.96.2/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
+-rw-r--r--   0        0        0     2010 2023-05-08 21:40:12.305657 windmill_api-1.96.2/windmill_api/models/get_folder_response_200.py
+-rw-r--r--   0        0        0     1258 2023-05-08 21:40:12.297657 windmill_api-1.96.2/windmill_api/models/get_folder_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2357 2023-05-08 21:40:12.333657 windmill_api-1.96.2/windmill_api/models/get_folder_usage_response_200.py
+-rw-r--r--   0        0        0      325 2023-05-08 21:39:58.321667 windmill_api-1.96.2/windmill_api/models/get_granular_acls_kind.py
+-rw-r--r--   0        0        0     1235 2023-05-08 21:40:12.329657 windmill_api-1.96.2/windmill_api/models/get_granular_acls_response_200.py
+-rw-r--r--   0        0        0     2888 2023-05-08 21:40:12.373657 windmill_api-1.96.2/windmill_api/models/get_group_response_200.py
+-rw-r--r--   0        0        0     1253 2023-05-08 21:40:12.353657 windmill_api-1.96.2/windmill_api/models/get_group_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1606 2023-05-08 21:40:12.413657 windmill_api-1.96.2/windmill_api/models/get_hub_app_by_id_response_200.py
+-rw-r--r--   0        0        0     1634 2023-05-08 21:40:12.401657 windmill_api-1.96.2/windmill_api/models/get_hub_app_by_id_response_200_app.py
+-rw-r--r--   0        0        0     1977 2023-05-08 21:40:12.433657 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200.py
+-rw-r--r--   0        0        0     2950 2023-05-08 21:40:12.453657 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
+-rw-r--r--   0        0        0     1289 2023-05-08 21:40:12.453657 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
+-rw-r--r--   0        0        0     3410 2023-05-08 21:40:12.493656 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
+-rw-r--r--   0        0        0     7365 2023-05-08 21:40:12.537657 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3418 2023-05-08 21:40:12.537657 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2019 2023-05-08 21:40:12.565657 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2323 2023-05-08 21:40:12.573656 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2249 2023-05-08 21:40:12.593656 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-05-08 21:39:58.845667 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2116 2023-05-08 21:40:12.601657 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-05-08 21:39:58.369667 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2012 2023-05-08 21:40:12.625656 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2063 2023-05-08 21:40:12.661656 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7289 2023-05-08 21:40:12.709656 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
+-rw-r--r--   0        0        0     3384 2023-05-08 21:40:12.705656 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2009 2023-05-08 21:40:12.733657 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2313 2023-05-08 21:40:12.741656 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2229 2023-05-08 21:40:12.765656 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      194 2023-05-08 21:39:59.141667 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2096 2023-05-08 21:40:12.813656 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      194 2023-05-08 21:39:58.921667 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2002 2023-05-08 21:40:12.793656 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2053 2023-05-08 21:40:12.821656 windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2698 2023-05-08 21:40:12.853656 windmill_api-1.96.2/windmill_api/models/get_hub_script_by_path_response_200.py
+-rw-r--r--   0        0        0      216 2023-05-08 21:39:59.085667 windmill_api-1.96.2/windmill_api/models/get_hub_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     2644 2023-05-08 21:40:12.861656 windmill_api-1.96.2/windmill_api/models/get_input_history_response_200_item.py
+-rw-r--r--   0        0        0     1278 2023-05-08 21:40:12.873656 windmill_api-1.96.2/windmill_api/models/get_input_history_response_200_item_args.py
+-rw-r--r--   0        0        0      218 2023-05-08 21:39:58.465667 windmill_api-1.96.2/windmill_api/models/get_input_history_runnable_type.py
+-rw-r--r--   0        0        0     1852 2023-05-08 21:40:12.897656 windmill_api-1.96.2/windmill_api/models/get_job_response_200.py
+-rw-r--r--   0        0        0      188 2023-05-08 21:39:58.637667 windmill_api-1.96.2/windmill_api/models/get_job_response_200_type.py
+-rw-r--r--   0        0        0     2364 2023-05-08 21:40:12.913656 windmill_api-1.96.2/windmill_api/models/get_job_updates_response_200.py
+-rw-r--r--   0        0        0     1744 2023-05-08 21:40:12.925656 windmill_api-1.96.2/windmill_api/models/get_premium_info_response_200.py
+-rw-r--r--   0        0        0     4218 2023-05-08 21:40:12.969656 windmill_api-1.96.2/windmill_api/models/get_public_app_by_secret_response_200.py
+-rw-r--r--   0        0        0      227 2023-05-08 21:39:58.117667 windmill_api-1.96.2/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1322 2023-05-08 21:40:12.945656 windmill_api-1.96.2/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3970 2023-05-08 21:40:12.993656 windmill_api-1.96.2/windmill_api/models/get_public_app_by_secret_response_200_policy.py
+-rw-r--r--   0        0        0      233 2023-05-08 21:39:58.529667 windmill_api-1.96.2/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2131 2023-05-08 21:40:12.997656 windmill_api-1.96.2/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1455 2023-05-08 21:40:13.045656 windmill_api-1.96.2/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3533 2023-05-08 21:40:13.045656 windmill_api-1.96.2/windmill_api/models/get_resource_response_200.py
+-rw-r--r--   0        0        0     1268 2023-05-08 21:40:13.065656 windmill_api-1.96.2/windmill_api/models/get_resource_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2335 2023-05-08 21:40:13.081656 windmill_api-1.96.2/windmill_api/models/get_resource_type_response_200.py
+-rw-r--r--   0        0        0     1840 2023-05-08 21:40:13.093656 windmill_api-1.96.2/windmill_api/models/get_resume_urls_response_200.py
+-rw-r--r--   0        0        0     4325 2023-05-08 21:40:13.141656 windmill_api-1.96.2/windmill_api/models/get_schedule_response_200.py
+-rw-r--r--   0        0        0     1232 2023-05-08 21:40:13.117656 windmill_api-1.96.2/windmill_api/models/get_schedule_response_200_args.py
+-rw-r--r--   0        0        0     1268 2023-05-08 21:40:13.137656 windmill_api-1.96.2/windmill_api/models/get_schedule_response_200_extra_perms.py
+-rw-r--r--   0        0        0     7558 2023-05-08 21:40:13.233656 windmill_api-1.96.2/windmill_api/models/get_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-08 21:40:13.161656 windmill_api-1.96.2/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-08 21:39:59.133666 windmill_api-1.96.2/windmill_api/models/get_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-05-08 21:39:58.621667 windmill_api-1.96.2/windmill_api/models/get_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-05-08 21:40:13.181656 windmill_api-1.96.2/windmill_api/models/get_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     7558 2023-05-08 21:40:13.317656 windmill_api-1.96.2/windmill_api/models/get_script_by_path_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-08 21:40:13.257656 windmill_api-1.96.2/windmill_api/models/get_script_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-08 21:39:58.809667 windmill_api-1.96.2/windmill_api/models/get_script_by_path_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-05-08 21:39:58.633667 windmill_api-1.96.2/windmill_api/models/get_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-05-08 21:40:13.281656 windmill_api-1.96.2/windmill_api/models/get_script_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     6383 2023-05-08 21:40:13.365656 windmill_api-1.96.2/windmill_api/models/get_script_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0     5608 2023-05-08 21:40:13.393656 windmill_api-1.96.2/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py
+-rw-r--r--   0        0        0      269 2023-05-08 21:39:58.425667 windmill_api-1.96.2/windmill_api/models/get_script_by_path_with_draft_response_200_draft_kind.py
+-rw-r--r--   0        0        0      227 2023-05-08 21:39:59.109666 windmill_api-1.96.2/windmill_api/models/get_script_by_path_with_draft_response_200_draft_language.py
+-rw-r--r--   0        0        0     1347 2023-05-08 21:40:13.393656 windmill_api-1.96.2/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py
+-rw-r--r--   0        0        0      264 2023-05-08 21:39:58.233667 windmill_api-1.96.2/windmill_api/models/get_script_by_path_with_draft_response_200_kind.py
+-rw-r--r--   0        0        0      222 2023-05-08 21:39:59.097667 windmill_api-1.96.2/windmill_api/models/get_script_by_path_with_draft_response_200_language.py
+-rw-r--r--   0        0        0     1319 2023-05-08 21:40:13.413656 windmill_api-1.96.2/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py
+-rw-r--r--   0        0        0     1922 2023-05-08 21:40:13.457656 windmill_api-1.96.2/windmill_api/models/get_script_deployment_status_response_200.py
+-rw-r--r--   0        0        0     4157 2023-05-08 21:40:13.469656 windmill_api-1.96.2/windmill_api/models/get_settings_response_200.py
+-rw-r--r--   0        0        0     2428 2023-05-08 21:40:13.489656 windmill_api-1.96.2/windmill_api/models/get_suspended_job_flow_response_200.py
+-rw-r--r--   0        0        0     1764 2023-05-08 21:40:13.497656 windmill_api-1.96.2/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
+-rw-r--r--   0        0        0     2040 2023-05-08 21:40:13.521656 windmill_api-1.96.2/windmill_api/models/get_suspended_job_flow_response_200_job.py
+-rw-r--r--   0        0        0      204 2023-05-08 21:39:58.169667 windmill_api-1.96.2/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
+-rw-r--r--   0        0        0     4554 2023-05-08 21:40:13.557656 windmill_api-1.96.2/windmill_api/models/get_variable_response_200.py
+-rw-r--r--   0        0        0     1268 2023-05-08 21:40:13.541656 windmill_api-1.96.2/windmill_api/models/get_variable_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2647 2023-05-08 21:40:13.585656 windmill_api-1.96.2/windmill_api/models/global_user_info.py
+-rw-r--r--   0        0        0      176 2023-05-08 21:39:58.533667 windmill_api-1.96.2/windmill_api/models/global_user_info_login_type.py
+-rw-r--r--   0        0        0     1627 2023-05-08 21:40:13.585656 windmill_api-1.96.2/windmill_api/models/global_user_update_json_body.py
+-rw-r--r--   0        0        0     2741 2023-05-08 21:40:13.625656 windmill_api-1.96.2/windmill_api/models/global_whoami_response_200.py
+-rw-r--r--   0        0        0      185 2023-05-08 21:39:58.269667 windmill_api-1.96.2/windmill_api/models/global_whoami_response_200_login_type.py
+-rw-r--r--   0        0        0     2903 2023-05-08 21:40:13.669656 windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5478 2023-05-08 21:40:13.685656 windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      324 2023-05-08 21:39:58.601667 windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1598 2023-05-08 21:40:13.697656 windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1663 2023-05-08 21:40:13.713656 windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2151 2023-05-08 21:40:13.725656 windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3257 2023-05-08 21:40:13.753656 windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      342 2023-05-08 21:39:58.121667 windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1631 2023-05-08 21:40:13.749656 windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3100 2023-05-08 21:40:13.785656 windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      333 2023-05-08 21:39:58.297667 windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1580 2023-05-08 21:40:13.781656 windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-08 21:39:58.513667 windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2722 2023-05-08 21:40:13.857656 windmill_api-1.96.2/windmill_api/models/group.py
+-rw-r--r--   0        0        0     1174 2023-05-08 21:40:13.805656 windmill_api-1.96.2/windmill_api/models/group_extra_perms.py
+-rw-r--r--   0        0        0     1689 2023-05-08 21:40:13.833656 windmill_api-1.96.2/windmill_api/models/identity.py
+-rw-r--r--   0        0        0      143 2023-05-08 21:39:58.401667 windmill_api-1.96.2/windmill_api/models/identity_type.py
+-rw-r--r--   0        0        0     2377 2023-05-08 21:40:13.873656 windmill_api-1.96.2/windmill_api/models/input_.py
+-rw-r--r--   0        0        0     1138 2023-05-08 21:40:13.877656 windmill_api-1.96.2/windmill_api/models/input_args.py
+-rw-r--r--   0        0        0     1820 2023-05-08 21:40:13.905656 windmill_api-1.96.2/windmill_api/models/input_transform_type_0.py
+-rw-r--r--   0        0        0      158 2023-05-08 21:39:58.537667 windmill_api-1.96.2/windmill_api/models/input_transform_type_0_type.py
+-rw-r--r--   0        0        0     1687 2023-05-08 21:40:13.909656 windmill_api-1.96.2/windmill_api/models/input_transform_type_1.py
+-rw-r--r--   0        0        0      158 2023-05-08 21:39:58.981667 windmill_api-1.96.2/windmill_api/models/input_transform_type_1_type.py
+-rw-r--r--   0        0        0     1773 2023-05-08 21:40:13.933656 windmill_api-1.96.2/windmill_api/models/invite_user_json_body.py
+-rw-r--r--   0        0        0     1679 2023-05-08 21:40:13.937656 windmill_api-1.96.2/windmill_api/models/javascript_transform.py
+-rw-r--r--   0        0        0      158 2023-05-08 21:39:58.545667 windmill_api-1.96.2/windmill_api/models/javascript_transform_type.py
+-rw-r--r--   0        0        0     1686 2023-05-08 21:40:13.965656 windmill_api-1.96.2/windmill_api/models/job.py
+-rw-r--r--   0        0        0      174 2023-05-08 21:39:59.013666 windmill_api-1.96.2/windmill_api/models/job_type.py
+-rw-r--r--   0        0        0     3583 2023-05-08 21:40:13.985656 windmill_api-1.96.2/windmill_api/models/list_apps_response_200_item.py
+-rw-r--r--   0        0        0      219 2023-05-08 21:39:58.245667 windmill_api-1.96.2/windmill_api/models/list_apps_response_200_item_execution_mode.py
+-rw-r--r--   0        0        0     1276 2023-05-08 21:40:13.985656 windmill_api-1.96.2/windmill_api/models/list_apps_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      218 2023-05-08 21:39:58.681667 windmill_api-1.96.2/windmill_api/models/list_audit_logs_action_kind.py
+-rw-r--r--   0        0        0     3896 2023-05-08 21:40:14.033656 windmill_api-1.96.2/windmill_api/models/list_audit_logs_response_200_item.py
+-rw-r--r--   0        0        0      237 2023-05-08 21:39:59.085667 windmill_api-1.96.2/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
+-rw-r--r--   0        0        0      640 2023-05-08 21:39:58.657667 windmill_api-1.96.2/windmill_api/models/list_audit_logs_response_200_item_operation.py
+-rw-r--r--   0        0        0     1298 2023-05-08 21:40:14.013656 windmill_api-1.96.2/windmill_api/models/list_audit_logs_response_200_item_parameters.py
+-rw-r--r--   0        0        0    11220 2023-05-08 21:40:14.149655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item.py
+-rw-r--r--   0        0        0     1288 2023-05-08 21:40:14.057656 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_args.py
+-rw-r--r--   0        0        0     3736 2023-05-08 21:40:14.101656 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7579 2023-05-08 21:40:14.225655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1901 2023-05-08 21:40:14.177656 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2352 2023-05-08 21:40:14.205655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      222 2023-05-08 21:39:58.357667 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1806 2023-05-08 21:40:14.277655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2342 2023-05-08 21:40:14.261655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      380 2023-05-08 21:39:58.533667 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7160 2023-05-08 21:40:14.345656 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1891 2023-05-08 21:40:14.301655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2332 2023-05-08 21:40:14.333655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      220 2023-05-08 21:39:58.445667 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1796 2023-05-08 21:40:14.361655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2332 2023-05-08 21:40:14.381655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      378 2023-05-08 21:39:58.609667 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2152 2023-05-08 21:40:14.397655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      330 2023-05-08 21:39:58.981667 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      219 2023-05-08 21:39:58.605667 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_language.py
+-rw-r--r--   0        0        0     3485 2023-05-08 21:40:14.425655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7593 2023-05-08 21:40:14.481655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3498 2023-05-08 21:40:14.465655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2041 2023-05-08 21:40:14.493655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2345 2023-05-08 21:40:14.517655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2295 2023-05-08 21:40:14.521655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      201 2023-05-08 21:39:58.085667 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2162 2023-05-08 21:40:14.545655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      201 2023-05-08 21:39:58.721667 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2034 2023-05-08 21:40:14.597655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2085 2023-05-08 21:40:14.577655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7471 2023-05-08 21:40:14.701655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3464 2023-05-08 21:40:14.637655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2031 2023-05-08 21:40:14.665655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2335 2023-05-08 21:40:14.697655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2275 2023-05-08 21:40:14.729655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      199 2023-05-08 21:39:58.105667 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2142 2023-05-08 21:40:14.733655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      199 2023-05-08 21:39:58.409667 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2024 2023-05-08 21:40:14.757655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2075 2023-05-08 21:40:14.761655 windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1865 2023-05-08 21:40:14.785655 windmill_api-1.96.2/windmill_api/models/list_contextual_variables_response_200_item.py
+-rw-r--r--   0        0        0     1863 2023-05-08 21:40:14.793655 windmill_api-1.96.2/windmill_api/models/list_flows_response_200_item.py
+-rw-r--r--   0        0        0     2074 2023-05-08 21:40:14.813655 windmill_api-1.96.2/windmill_api/models/list_folders_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-05-08 21:40:14.813655 windmill_api-1.96.2/windmill_api/models/list_folders_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2958 2023-05-08 21:40:14.861655 windmill_api-1.96.2/windmill_api/models/list_groups_response_200_item.py
+-rw-r--r--   0        0        0     1286 2023-05-08 21:40:14.833655 windmill_api-1.96.2/windmill_api/models/list_groups_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2076 2023-05-08 21:40:14.865655 windmill_api-1.96.2/windmill_api/models/list_hub_apps_response_200.py
+-rw-r--r--   0        0        0     2304 2023-05-08 21:40:14.897655 windmill_api-1.96.2/windmill_api/models/list_hub_apps_response_200_apps_item.py
+-rw-r--r--   0        0        0     2116 2023-05-08 21:40:14.897655 windmill_api-1.96.2/windmill_api/models/list_hub_flows_response_200.py
+-rw-r--r--   0        0        0     2324 2023-05-08 21:40:14.933655 windmill_api-1.96.2/windmill_api/models/list_hub_flows_response_200_flows_item.py
+-rw-r--r--   0        0        0     2106 2023-05-08 21:40:14.929655 windmill_api-1.96.2/windmill_api/models/list_hub_scripts_response_200.py
+-rw-r--r--   0        0        0     2790 2023-05-08 21:40:14.969655 windmill_api-1.96.2/windmill_api/models/list_hub_scripts_response_200_asks_item.py
+-rw-r--r--   0        0        0      262 2023-05-08 21:39:58.777667 windmill_api-1.96.2/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
+-rw-r--r--   0        0        0     2590 2023-05-08 21:40:14.973655 windmill_api-1.96.2/windmill_api/models/list_inputs_response_200_item.py
+-rw-r--r--   0        0        0     1250 2023-05-08 21:40:14.989655 windmill_api-1.96.2/windmill_api/models/list_inputs_response_200_item_args.py
+-rw-r--r--   0        0        0      213 2023-05-08 21:39:58.633667 windmill_api-1.96.2/windmill_api/models/list_inputs_runnable_type.py
+-rw-r--r--   0        0        0     1922 2023-05-08 21:40:15.009655 windmill_api-1.96.2/windmill_api/models/list_jobs_response_200_item.py
+-rw-r--r--   0        0        0      194 2023-05-08 21:39:58.089667 windmill_api-1.96.2/windmill_api/models/list_jobs_response_200_item_type.py
+-rw-r--r--   0        0        0     2076 2023-05-08 21:40:15.021655 windmill_api-1.96.2/windmill_api/models/list_pending_invites_response_200_item.py
+-rw-r--r--   0        0        0    12114 2023-05-08 21:40:15.209655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item.py
+-rw-r--r--   0        0        0     1245 2023-05-08 21:40:15.089655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_args.py
+-rw-r--r--   0        0        0     3544 2023-05-08 21:40:15.133655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7247 2023-05-08 21:40:15.217655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1858 2023-05-08 21:40:15.237655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-05-08 21:40:15.245655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-05-08 21:39:59.145666 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-05-08 21:40:15.265655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2299 2023-05-08 21:40:15.281655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      372 2023-05-08 21:39:58.733667 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6858 2023-05-08 21:40:15.353655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1848 2023-05-08 21:40:15.309655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2248 2023-05-08 21:40:15.337655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      212 2023-05-08 21:39:58.965667 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1753 2023-05-08 21:40:15.365655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2289 2023-05-08 21:40:15.393655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      370 2023-05-08 21:39:58.493667 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2109 2023-05-08 21:40:15.397655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      322 2023-05-08 21:39:59.153666 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      211 2023-05-08 21:39:58.629667 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_language.py
+-rw-r--r--   0        0        0     3334 2023-05-08 21:40:15.437655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7235 2023-05-08 21:40:15.521655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3357 2023-05-08 21:40:15.529655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1998 2023-05-08 21:40:15.553655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-05-08 21:40:15.561655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-05-08 21:40:15.581655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-08 21:39:58.829667 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-05-08 21:40:15.593655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-08 21:39:58.481667 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-05-08 21:40:15.613655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-05-08 21:40:15.621655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7159 2023-05-08 21:40:15.693655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3323 2023-05-08 21:40:15.665655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1988 2023-05-08 21:40:15.693655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-05-08 21:40:15.729655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-05-08 21:40:15.721655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-05-08 21:39:58.629667 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-05-08 21:40:15.753655 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-05-08 21:39:58.377667 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-05-08 21:40:15.761654 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-05-08 21:40:15.781654 windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     3045 2023-05-08 21:40:15.801654 windmill_api-1.96.2/windmill_api/models/list_raw_apps_response_200_item.py
+-rw-r--r--   0        0        0     1294 2023-05-08 21:40:15.801654 windmill_api-1.96.2/windmill_api/models/list_raw_apps_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     4884 2023-05-08 21:40:15.909654 windmill_api-1.96.2/windmill_api/models/list_resource_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-05-08 21:40:15.821655 windmill_api-1.96.2/windmill_api/models/list_resource_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2363 2023-05-08 21:40:15.857654 windmill_api-1.96.2/windmill_api/models/list_resource_type_response_200_item.py
+-rw-r--r--   0        0        0     4426 2023-05-08 21:40:15.953654 windmill_api-1.96.2/windmill_api/models/list_schedules_response_200_item.py
+-rw-r--r--   0        0        0     1265 2023-05-08 21:40:15.933654 windmill_api-1.96.2/windmill_api/models/list_schedules_response_200_item_args.py
+-rw-r--r--   0        0        0     1301 2023-05-08 21:40:15.949654 windmill_api-1.96.2/windmill_api/models/list_schedules_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     7551 2023-05-08 21:40:16.045654 windmill_api-1.96.2/windmill_api/models/list_scripts_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-05-08 21:40:15.977655 windmill_api-1.96.2/windmill_api/models/list_scripts_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-08 21:39:58.909667 windmill_api-1.96.2/windmill_api/models/list_scripts_response_200_item_kind.py
+-rw-r--r--   0        0        0      213 2023-05-08 21:39:58.905667 windmill_api-1.96.2/windmill_api/models/list_scripts_response_200_item_language.py
+-rw-r--r--   0        0        0     1265 2023-05-08 21:40:16.001654 windmill_api-1.96.2/windmill_api/models/list_scripts_response_200_item_schema.py
+-rw-r--r--   0        0        0     2985 2023-05-08 21:40:16.065654 windmill_api-1.96.2/windmill_api/models/list_tokens_response_200_item.py
+-rw-r--r--   0        0        0     2250 2023-05-08 21:40:16.073654 windmill_api-1.96.2/windmill_api/models/list_user_workspaces_response_200.py
+-rw-r--r--   0        0        0     1833 2023-05-08 21:40:16.105654 windmill_api-1.96.2/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
+-rw-r--r--   0        0        0     2896 2023-05-08 21:40:16.169654 windmill_api-1.96.2/windmill_api/models/list_users_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0      198 2023-05-08 21:39:58.929667 windmill_api-1.96.2/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
+-rw-r--r--   0        0        0     4307 2023-05-08 21:40:16.169654 windmill_api-1.96.2/windmill_api/models/list_users_response_200_item.py
+-rw-r--r--   0        0        0     1613 2023-05-08 21:40:16.193654 windmill_api-1.96.2/windmill_api/models/list_users_response_200_item_usage.py
+-rw-r--r--   0        0        0     4608 2023-05-08 21:40:16.233654 windmill_api-1.96.2/windmill_api/models/list_variable_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-05-08 21:40:16.213654 windmill_api-1.96.2/windmill_api/models/list_variable_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2693 2023-05-08 21:40:16.301654 windmill_api-1.96.2/windmill_api/models/list_workers_response_200_item.py
+-rw-r--r--   0        0        0     2086 2023-05-08 21:40:16.265654 windmill_api-1.96.2/windmill_api/models/list_workspace_invites_response_200_item.py
+-rw-r--r--   0        0        0     2082 2023-05-08 21:40:16.297654 windmill_api-1.96.2/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0     2013 2023-05-08 21:40:16.329654 windmill_api-1.96.2/windmill_api/models/list_workspaces_response_200_item.py
+-rw-r--r--   0        0        0     3388 2023-05-08 21:40:16.345654 windmill_api-1.96.2/windmill_api/models/listable_app.py
+-rw-r--r--   0        0        0      207 2023-05-08 21:39:58.717667 windmill_api-1.96.2/windmill_api/models/listable_app_execution_mode.py
+-rw-r--r--   0        0        0     1207 2023-05-08 21:40:16.353654 windmill_api-1.96.2/windmill_api/models/listable_app_extra_perms.py
+-rw-r--r--   0        0        0     2913 2023-05-08 21:40:16.389654 windmill_api-1.96.2/windmill_api/models/listable_raw_app.py
+-rw-r--r--   0        0        0     1225 2023-05-08 21:40:16.409654 windmill_api-1.96.2/windmill_api/models/listable_raw_app_extra_perms.py
+-rw-r--r--   0        0        0     4751 2023-05-08 21:40:16.453654 windmill_api-1.96.2/windmill_api/models/listable_resource.py
+-rw-r--r--   0        0        0     1232 2023-05-08 21:40:16.429654 windmill_api-1.96.2/windmill_api/models/listable_resource_extra_perms.py
+-rw-r--r--   0        0        0     4486 2023-05-08 21:40:16.493654 windmill_api-1.96.2/windmill_api/models/listable_variable.py
+-rw-r--r--   0        0        0     1232 2023-05-08 21:40:16.473654 windmill_api-1.96.2/windmill_api/models/listable_variable_extra_perms.py
+-rw-r--r--   0        0        0     1513 2023-05-08 21:40:16.513654 windmill_api-1.96.2/windmill_api/models/login.py
+-rw-r--r--   0        0        0     1559 2023-05-08 21:40:16.517654 windmill_api-1.96.2/windmill_api/models/login_json_body.py
+-rw-r--r--   0        0        0     1739 2023-05-08 21:40:16.541654 windmill_api-1.96.2/windmill_api/models/login_with_oauth_json_body.py
+-rw-r--r--   0        0        0     2758 2023-05-08 21:40:16.561654 windmill_api-1.96.2/windmill_api/models/main_arg_signature.py
+-rw-r--r--   0        0        0     5099 2023-05-08 21:40:16.601654 windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item.py
+-rw-r--r--   0        0        0      315 2023-05-08 21:39:58.741667 windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1547 2023-05-08 21:40:16.585654 windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1612 2023-05-08 21:40:16.613654 windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2044 2023-05-08 21:40:16.625654 windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3049 2023-05-08 21:40:16.649654 windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      333 2023-05-08 21:39:58.213667 windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1580 2023-05-08 21:40:16.653654 windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     2862 2023-05-08 21:40:16.685654 windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      324 2023-05-08 21:39:58.249667 windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1529 2023-05-08 21:40:16.681654 windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-08 21:39:58.213667 windmill_api-1.96.2/windmill_api/models/main_arg_signature_type.py
+-rw-r--r--   0        0        0     2662 2023-05-08 21:40:16.769654 windmill_api-1.96.2/windmill_api/models/new_schedule.py
+-rw-r--r--   0        0        0     1171 2023-05-08 21:40:16.705654 windmill_api-1.96.2/windmill_api/models/new_schedule_args.py
+-rw-r--r--   0        0        0     4866 2023-05-08 21:40:16.817654 windmill_api-1.96.2/windmill_api/models/new_script.py
+-rw-r--r--   0        0        0      238 2023-05-08 21:39:58.781667 windmill_api-1.96.2/windmill_api/models/new_script_kind.py
+-rw-r--r--   0        0        0      196 2023-05-08 21:39:58.933667 windmill_api-1.96.2/windmill_api/models/new_script_language.py
+-rw-r--r--   0        0        0     1171 2023-05-08 21:40:16.793654 windmill_api-1.96.2/windmill_api/models/new_script_schema.py
+-rw-r--r--   0        0        0     5879 2023-05-08 21:40:16.877654 windmill_api-1.96.2/windmill_api/models/new_script_with_draft.py
+-rw-r--r--   0        0        0     5192 2023-05-08 21:40:16.889654 windmill_api-1.96.2/windmill_api/models/new_script_with_draft_draft.py
+-rw-r--r--   0        0        0      252 2023-05-08 21:39:58.413667 windmill_api-1.96.2/windmill_api/models/new_script_with_draft_draft_kind.py
+-rw-r--r--   0        0        0      210 2023-05-08 21:39:58.485667 windmill_api-1.96.2/windmill_api/models/new_script_with_draft_draft_language.py
+-rw-r--r--   0        0        0     1250 2023-05-08 21:40:16.901654 windmill_api-1.96.2/windmill_api/models/new_script_with_draft_draft_schema.py
+-rw-r--r--   0        0        0      247 2023-05-08 21:39:58.141667 windmill_api-1.96.2/windmill_api/models/new_script_with_draft_kind.py
+-rw-r--r--   0        0        0      205 2023-05-08 21:39:58.481667 windmill_api-1.96.2/windmill_api/models/new_script_with_draft_language.py
+-rw-r--r--   0        0        0     1222 2023-05-08 21:40:16.913654 windmill_api-1.96.2/windmill_api/models/new_script_with_draft_schema.py
+-rw-r--r--   0        0        0     2108 2023-05-08 21:40:16.953654 windmill_api-1.96.2/windmill_api/models/new_token.py
+-rw-r--r--   0        0        0     2473 2023-05-08 21:40:16.953654 windmill_api-1.96.2/windmill_api/models/new_token_impersonate.py
+-rw-r--r--   0        0        0     1710 2023-05-08 21:40:16.981654 windmill_api-1.96.2/windmill_api/models/new_user.py
+-rw-r--r--   0        0        0     2584 2023-05-08 21:40:16.997654 windmill_api-1.96.2/windmill_api/models/open_flow.py
+-rw-r--r--   0        0        0     1166 2023-05-08 21:40:17.001654 windmill_api-1.96.2/windmill_api/models/open_flow_schema.py
+-rw-r--r--   0        0        0     3026 2023-05-08 21:40:17.041654 windmill_api-1.96.2/windmill_api/models/open_flow_value.py
+-rw-r--r--   0        0        0     6384 2023-05-08 21:40:17.089654 windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3013 2023-05-08 21:40:17.081654 windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1896 2023-05-08 21:40:17.109654 windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2200 2023-05-08 21:40:17.121654 windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2006 2023-05-08 21:40:17.137654 windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      175 2023-05-08 21:39:58.389667 windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1873 2023-05-08 21:40:17.193654 windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      175 2023-05-08 21:39:58.997667 windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1889 2023-05-08 21:40:17.169654 windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1940 2023-05-08 21:40:17.197654 windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6308 2023-05-08 21:40:17.273654 windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item.py
+-rw-r--r--   0        0        0     2979 2023-05-08 21:40:17.237654 windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1886 2023-05-08 21:40:17.265654 windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2190 2023-05-08 21:40:17.297654 windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1986 2023-05-08 21:40:17.305654 windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      173 2023-05-08 21:39:58.801667 windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1853 2023-05-08 21:40:17.325654 windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      173 2023-05-08 21:39:58.229667 windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1879 2023-05-08 21:40:17.333654 windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1930 2023-05-08 21:40:17.409654 windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2816 2023-05-08 21:40:17.377654 windmill_api-1.96.2/windmill_api/models/open_flow_w_path.py
+-rw-r--r--   0        0        0     1197 2023-05-08 21:40:17.401654 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_schema.py
+-rw-r--r--   0        0        0     3116 2023-05-08 21:40:17.441655 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value.py
+-rw-r--r--   0        0        0     6590 2023-05-08 21:40:17.489654 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module.py
+-rw-r--r--   0        0        0     3117 2023-05-08 21:40:17.481655 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1927 2023-05-08 21:40:17.513655 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2231 2023-05-08 21:40:17.521654 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2073 2023-05-08 21:40:17.545654 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      180 2023-05-08 21:39:58.317667 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1940 2023-05-08 21:40:17.549655 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-08 21:39:58.281667 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1920 2023-05-08 21:40:17.617654 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1971 2023-05-08 21:40:17.581654 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6514 2023-05-08 21:40:17.661655 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item.py
+-rw-r--r--   0        0        0     3074 2023-05-08 21:40:17.657655 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1917 2023-05-08 21:40:17.689654 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2221 2023-05-08 21:40:17.693654 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2044 2023-05-08 21:40:17.717655 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-08 21:39:58.685667 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1911 2023-05-08 21:40:17.725654 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-08 21:39:59.101667 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1910 2023-05-08 21:40:17.749655 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1961 2023-05-08 21:40:17.797654 windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1989 2023-05-08 21:40:17.777655 windmill_api-1.96.2/windmill_api/models/path_flow.py
+-rw-r--r--   0        0        0     3089 2023-05-08 21:40:17.817654 windmill_api-1.96.2/windmill_api/models/path_flow_input_transforms.py
+-rw-r--r--   0        0        0     2115 2023-05-08 21:40:17.825655 windmill_api-1.96.2/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      185 2023-05-08 21:39:58.349667 windmill_api-1.96.2/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1982 2023-05-08 21:40:17.845655 windmill_api-1.96.2/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      185 2023-05-08 21:39:58.209667 windmill_api-1.96.2/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      135 2023-05-08 21:39:58.401667 windmill_api-1.96.2/windmill_api/models/path_flow_type.py
+-rw-r--r--   0        0        0     2292 2023-05-08 21:40:17.865655 windmill_api-1.96.2/windmill_api/models/path_script.py
+-rw-r--r--   0        0        0     3181 2023-05-08 21:40:17.881655 windmill_api-1.96.2/windmill_api/models/path_script_input_transforms.py
+-rw-r--r--   0        0        0     2135 2023-05-08 21:40:17.893654 windmill_api-1.96.2/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      187 2023-05-08 21:39:59.025667 windmill_api-1.96.2/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2002 2023-05-08 21:40:17.913655 windmill_api-1.96.2/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      187 2023-05-08 21:39:58.641667 windmill_api-1.96.2/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      141 2023-05-08 21:39:58.669667 windmill_api-1.96.2/windmill_api/models/path_script_type.py
+-rw-r--r--   0        0        0     3390 2023-05-08 21:40:17.941655 windmill_api-1.96.2/windmill_api/models/policy.py
+-rw-r--r--   0        0        0      202 2023-05-08 21:39:59.113666 windmill_api-1.96.2/windmill_api/models/policy_execution_mode.py
+-rw-r--r--   0        0        0     1709 2023-05-08 21:40:17.937655 windmill_api-1.96.2/windmill_api/models/policy_triggerables.py
+-rw-r--r--   0        0        0     1279 2023-05-08 21:40:17.957655 windmill_api-1.96.2/windmill_api/models/policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2359 2023-05-08 21:40:17.981655 windmill_api-1.96.2/windmill_api/models/preview.py
+-rw-r--r--   0        0        0     1148 2023-05-08 21:40:17.977655 windmill_api-1.96.2/windmill_api/models/preview_args.py
+-rw-r--r--   0        0        0      194 2023-05-08 21:39:58.953667 windmill_api-1.96.2/windmill_api/models/preview_language.py
+-rw-r--r--   0        0        0     1642 2023-05-08 21:40:18.005655 windmill_api-1.96.2/windmill_api/models/preview_schedule_json_body.py
+-rw-r--r--   0        0        0     2963 2023-05-08 21:40:18.061655 windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5679 2023-05-08 21:40:18.065655 windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      328 2023-05-08 21:39:58.217667 windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1618 2023-05-08 21:40:18.089655 windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1683 2023-05-08 21:40:18.093654 windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2191 2023-05-08 21:40:18.117655 windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3329 2023-05-08 21:40:18.129655 windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      346 2023-05-08 21:39:58.877667 windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1651 2023-05-08 21:40:18.145655 windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3214 2023-05-08 21:40:18.165655 windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      337 2023-05-08 21:39:58.101667 windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1600 2023-05-08 21:40:18.173655 windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      182 2023-05-08 21:39:59.045667 windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0    11580 2023-05-08 21:40:18.381655 windmill_api-1.96.2/windmill_api/models/queued_job.py
+-rw-r--r--   0        0        0     1161 2023-05-08 21:40:18.193655 windmill_api-1.96.2/windmill_api/models/queued_job_args.py
+-rw-r--r--   0        0        0     3202 2023-05-08 21:40:18.237655 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status.py
+-rw-r--r--   0        0        0     6683 2023-05-08 21:40:18.321655 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1774 2023-05-08 21:40:18.349655 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2106 2023-05-08 21:40:18.377655 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      199 2023-05-08 21:39:58.669667 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1679 2023-05-08 21:40:18.405655 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2215 2023-05-08 21:40:18.417655 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      357 2023-05-08 21:39:58.685667 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6294 2023-05-08 21:40:18.533655 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1764 2023-05-08 21:40:18.441655 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2086 2023-05-08 21:40:18.469655 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      197 2023-05-08 21:39:58.297667 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1669 2023-05-08 21:40:18.497655 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2205 2023-05-08 21:40:18.533655 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      355 2023-05-08 21:39:58.093667 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2025 2023-05-08 21:40:18.565655 windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_retry.py
+-rw-r--r--   0        0        0      307 2023-05-08 21:39:58.937667 windmill_api-1.96.2/windmill_api/models/queued_job_job_kind.py
+-rw-r--r--   0        0        0      196 2023-05-08 21:39:58.425667 windmill_api-1.96.2/windmill_api/models/queued_job_language.py
+-rw-r--r--   0        0        0     3079 2023-05-08 21:40:18.581655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow.py
+-rw-r--r--   0        0        0     6506 2023-05-08 21:40:18.645655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3069 2023-05-08 21:40:18.621655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1914 2023-05-08 21:40:18.653655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2218 2023-05-08 21:40:18.737655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2040 2023-05-08 21:40:18.681655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-08 21:39:58.789667 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1907 2023-05-08 21:40:18.709655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-08 21:39:58.725667 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1907 2023-05-08 21:40:18.741655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1958 2023-05-08 21:40:18.765655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6430 2023-05-08 21:40:18.873655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3035 2023-05-08 21:40:18.805655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1904 2023-05-08 21:40:18.837655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2208 2023-05-08 21:40:18.869655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2020 2023-05-08 21:40:18.897655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-05-08 21:39:58.929667 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1887 2023-05-08 21:40:18.901655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-05-08 21:39:58.617667 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1897 2023-05-08 21:40:18.929655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1948 2023-05-08 21:40:18.929655 windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     3028 2023-05-08 21:40:18.973655 windmill_api-1.96.2/windmill_api/models/raw_script.py
+-rw-r--r--   0        0        0     3139 2023-05-08 21:40:18.965655 windmill_api-1.96.2/windmill_api/models/raw_script_input_transforms.py
+-rw-r--r--   0        0        0     2125 2023-05-08 21:40:18.997655 windmill_api-1.96.2/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      186 2023-05-08 21:39:58.637667 windmill_api-1.96.2/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1992 2023-05-08 21:40:19.001655 windmill_api-1.96.2/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      186 2023-05-08 21:39:58.581667 windmill_api-1.96.2/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      196 2023-05-08 21:39:59.041667 windmill_api-1.96.2/windmill_api/models/raw_script_language.py
+-rw-r--r--   0        0        0      146 2023-05-08 21:39:58.113667 windmill_api-1.96.2/windmill_api/models/raw_script_type.py
+-rw-r--r--   0        0        0     1405 2023-05-08 21:40:19.025655 windmill_api-1.96.2/windmill_api/models/refresh_token_json_body.py
+-rw-r--r--   0        0        0     1448 2023-05-08 21:40:19.025655 windmill_api-1.96.2/windmill_api/models/remove_granular_acls_json_body.py
+-rw-r--r--   0        0        0      328 2023-05-08 21:39:58.461667 windmill_api-1.96.2/windmill_api/models/remove_granular_acls_kind.py
+-rw-r--r--   0        0        0     1544 2023-05-08 21:40:19.053655 windmill_api-1.96.2/windmill_api/models/remove_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1567 2023-05-08 21:40:19.053655 windmill_api-1.96.2/windmill_api/models/remove_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3367 2023-05-08 21:40:19.101655 windmill_api-1.96.2/windmill_api/models/resource.py
+-rw-r--r--   0        0        0     1189 2023-05-08 21:40:19.073655 windmill_api-1.96.2/windmill_api/models/resource_extra_perms.py
+-rw-r--r--   0        0        0     2256 2023-05-08 21:40:19.109655 windmill_api-1.96.2/windmill_api/models/resource_type.py
+-rw-r--r--   0        0        0     1278 2023-05-08 21:40:19.121655 windmill_api-1.96.2/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
+-rw-r--r--   0        0        0     1255 2023-05-08 21:40:19.129655 windmill_api-1.96.2/windmill_api/models/resume_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0     2546 2023-05-08 21:40:19.161655 windmill_api-1.96.2/windmill_api/models/retry.py
+-rw-r--r--   0        0        0     1751 2023-05-08 21:40:19.161655 windmill_api-1.96.2/windmill_api/models/retry_constant.py
+-rw-r--r--   0        0        0     2055 2023-05-08 21:40:19.193655 windmill_api-1.96.2/windmill_api/models/retry_exponential.py
+-rw-r--r--   0        0        0     1210 2023-05-08 21:40:19.181655 windmill_api-1.96.2/windmill_api/models/run_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     2189 2023-05-08 21:40:19.213655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body.py
+-rw-r--r--   0        0        0     1235 2023-05-08 21:40:19.217655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_args.py
+-rw-r--r--   0        0        0     3265 2023-05-08 21:40:19.257655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value.py
+-rw-r--r--   0        0        0     7049 2023-05-08 21:40:19.301655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3284 2023-05-08 21:40:19.297655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1975 2023-05-08 21:40:19.325655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2279 2023-05-08 21:40:19.333655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2167 2023-05-08 21:40:19.421655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-05-08 21:39:58.257667 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2034 2023-05-08 21:40:19.365655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-05-08 21:39:58.201667 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1968 2023-05-08 21:40:19.393655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2019 2023-05-08 21:40:19.425655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6939 2023-05-08 21:40:19.505655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3250 2023-05-08 21:40:19.513655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1965 2023-05-08 21:40:19.533655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2269 2023-05-08 21:40:19.549655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2147 2023-05-08 21:40:19.561655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      187 2023-05-08 21:39:58.985667 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2014 2023-05-08 21:40:19.577655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      187 2023-05-08 21:39:58.821667 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1958 2023-05-08 21:40:19.593655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2009 2023-05-08 21:40:19.609655 windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1220 2023-05-08 21:40:19.609655 windmill_api-1.96.2/windmill_api/models/run_script_by_hash_json_body.py
+-rw-r--r--   0        0        0     1220 2023-05-08 21:40:19.629655 windmill_api-1.96.2/windmill_api/models/run_script_by_path_json_body.py
+-rw-r--r--   0        0        0     2634 2023-05-08 21:40:19.649655 windmill_api-1.96.2/windmill_api/models/run_script_preview_json_body.py
+-rw-r--r--   0        0        0     1245 2023-05-08 21:40:19.649655 windmill_api-1.96.2/windmill_api/models/run_script_preview_json_body_args.py
+-rw-r--r--   0        0        0      211 2023-05-08 21:39:58.905667 windmill_api-1.96.2/windmill_api/models/run_script_preview_json_body_language.py
+-rw-r--r--   0        0        0     1266 2023-05-08 21:40:19.669655 windmill_api-1.96.2/windmill_api/models/run_wait_result_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     1276 2023-05-08 21:40:19.673655 windmill_api-1.96.2/windmill_api/models/run_wait_result_script_by_path_json_body.py
+-rw-r--r--   0        0        0      203 2023-05-08 21:39:58.861667 windmill_api-1.96.2/windmill_api/models/runnable_type.py
+-rw-r--r--   0        0        0     4086 2023-05-08 21:40:19.729655 windmill_api-1.96.2/windmill_api/models/schedule.py
+-rw-r--r--   0        0        0     1153 2023-05-08 21:40:19.693655 windmill_api-1.96.2/windmill_api/models/schedule_args.py
+-rw-r--r--   0        0        0     1189 2023-05-08 21:40:19.713655 windmill_api-1.96.2/windmill_api/models/schedule_extra_perms.py
+-rw-r--r--   0        0        0     7003 2023-05-08 21:40:19.809655 windmill_api-1.96.2/windmill_api/models/script.py
+-rw-r--r--   0        0        0     1143 2023-05-08 21:40:19.749655 windmill_api-1.96.2/windmill_api/models/script_args.py
+-rw-r--r--   0        0        0     1179 2023-05-08 21:40:19.769655 windmill_api-1.96.2/windmill_api/models/script_extra_perms.py
+-rw-r--r--   0        0        0      235 2023-05-08 21:39:58.789667 windmill_api-1.96.2/windmill_api/models/script_kind.py
+-rw-r--r--   0        0        0      193 2023-05-08 21:39:58.993667 windmill_api-1.96.2/windmill_api/models/script_language.py
+-rw-r--r--   0        0        0     1153 2023-05-08 21:40:19.793655 windmill_api-1.96.2/windmill_api/models/script_schema.py
+-rw-r--r--   0        0        0     1440 2023-05-08 21:40:19.817655 windmill_api-1.96.2/windmill_api/models/set_password_json_body.py
+-rw-r--r--   0        0        0     1470 2023-05-08 21:40:19.833655 windmill_api-1.96.2/windmill_api/models/set_schedule_enabled_json_body.py
+-rw-r--r--   0        0        0     2032 2023-05-08 21:40:19.849655 windmill_api-1.96.2/windmill_api/models/slack_token.py
+-rw-r--r--   0        0        0     1586 2023-05-08 21:40:19.857655 windmill_api-1.96.2/windmill_api/models/slack_token_bot.py
+-rw-r--r--   0        0        0     2227 2023-05-08 21:40:19.881655 windmill_api-1.96.2/windmill_api/models/star_json_body.py
+-rw-r--r--   0        0        0      209 2023-05-08 21:39:58.921667 windmill_api-1.96.2/windmill_api/models/star_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     1772 2023-05-08 21:40:19.889655 windmill_api-1.96.2/windmill_api/models/static_transform.py
+-rw-r--r--   0        0        0      154 2023-05-08 21:39:58.701667 windmill_api-1.96.2/windmill_api/models/static_transform_type.py
+-rw-r--r--   0        0        0     2462 2023-05-08 21:40:19.993655 windmill_api-1.96.2/windmill_api/models/token_response.py
+-rw-r--r--   0        0        0     2921 2023-05-08 21:40:19.985655 windmill_api-1.96.2/windmill_api/models/truncated_token.py
+-rw-r--r--   0        0        0     2249 2023-05-08 21:40:20.021655 windmill_api-1.96.2/windmill_api/models/unstar_json_body.py
+-rw-r--r--   0        0        0      211 2023-05-08 21:39:58.877667 windmill_api-1.96.2/windmill_api/models/unstar_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     2638 2023-05-08 21:40:20.033655 windmill_api-1.96.2/windmill_api/models/update_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-05-08 21:40:20.069655 windmill_api-1.96.2/windmill_api/models/update_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-05-08 21:39:58.537667 windmill_api-1.96.2/windmill_api/models/update_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-05-08 21:40:20.061655 windmill_api-1.96.2/windmill_api/models/update_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-05-08 21:40:20.081655 windmill_api-1.96.2/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2896 2023-05-08 21:40:20.113655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body.py
+-rw-r--r--   0        0        0     1222 2023-05-08 21:40:20.101655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_schema.py
+-rw-r--r--   0        0        0     3196 2023-05-08 21:40:20.141655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value.py
+-rw-r--r--   0        0        0     6855 2023-05-08 21:40:20.197655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3211 2023-05-08 21:40:20.185655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1952 2023-05-08 21:40:20.213655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2256 2023-05-08 21:40:20.229655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2123 2023-05-08 21:40:20.241655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      185 2023-05-08 21:39:58.889667 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1990 2023-05-08 21:40:20.261655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      185 2023-05-08 21:39:59.029667 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1945 2023-05-08 21:40:20.269655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1996 2023-05-08 21:40:20.289655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6739 2023-05-08 21:40:20.349655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3177 2023-05-08 21:40:20.329655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1942 2023-05-08 21:40:20.405655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2246 2023-05-08 21:40:20.385655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2103 2023-05-08 21:40:20.413655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      183 2023-05-08 21:39:58.613667 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1970 2023-05-08 21:40:20.433655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      183 2023-05-08 21:39:58.793667 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1935 2023-05-08 21:40:20.441655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1986 2023-05-08 21:40:20.465655 windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1949 2023-05-08 21:40:20.473655 windmill_api-1.96.2/windmill_api/models/update_folder_json_body.py
+-rw-r--r--   0        0        0     1520 2023-05-08 21:40:20.493655 windmill_api-1.96.2/windmill_api/models/update_group_json_body.py
+-rw-r--r--   0        0        0     1670 2023-05-08 21:40:20.501655 windmill_api-1.96.2/windmill_api/models/update_input.py
+-rw-r--r--   0        0        0     1716 2023-05-08 21:40:20.521655 windmill_api-1.96.2/windmill_api/models/update_input_json_body.py
+-rw-r--r--   0        0        0     1985 2023-05-08 21:40:20.533655 windmill_api-1.96.2/windmill_api/models/update_raw_app_json_body.py
+-rw-r--r--   0        0        0     2036 2023-05-08 21:40:20.553655 windmill_api-1.96.2/windmill_api/models/update_resource_json_body.py
+-rw-r--r--   0        0        0     1847 2023-05-08 21:40:20.625655 windmill_api-1.96.2/windmill_api/models/update_resource_type_json_body.py
+-rw-r--r--   0        0        0     1541 2023-05-08 21:40:20.577655 windmill_api-1.96.2/windmill_api/models/update_resource_value_json_body.py
+-rw-r--r--   0        0        0     1953 2023-05-08 21:40:20.609655 windmill_api-1.96.2/windmill_api/models/update_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-08 21:40:20.629655 windmill_api-1.96.2/windmill_api/models/update_schedule_json_body_args.py
+-rw-r--r--   0        0        0     2066 2023-05-08 21:40:20.657655 windmill_api-1.96.2/windmill_api/models/update_user_json_body.py
+-rw-r--r--   0        0        0     2316 2023-05-08 21:40:20.669655 windmill_api-1.96.2/windmill_api/models/update_variable_json_body.py
+-rw-r--r--   0        0        0     1478 2023-05-08 21:40:20.681655 windmill_api-1.96.2/windmill_api/models/usage.py
+-rw-r--r--   0        0        0     4071 2023-05-08 21:40:20.729655 windmill_api-1.96.2/windmill_api/models/user.py
+-rw-r--r--   0        0        0     1501 2023-05-08 21:40:20.705655 windmill_api-1.96.2/windmill_api/models/user_usage.py
+-rw-r--r--   0        0        0     2122 2023-05-08 21:40:20.737655 windmill_api-1.96.2/windmill_api/models/user_workspace_list.py
+-rw-r--r--   0        0        0     1767 2023-05-08 21:40:20.761655 windmill_api-1.96.2/windmill_api/models/user_workspace_list_workspaces_item.py
+-rw-r--r--   0        0        0     4222 2023-05-08 21:40:20.797655 windmill_api-1.96.2/windmill_api/models/whoami_response_200.py
+-rw-r--r--   0        0        0     1572 2023-05-08 21:40:20.785655 windmill_api-1.96.2/windmill_api/models/whoami_response_200_usage.py
+-rw-r--r--   0        0        0     4211 2023-05-08 21:40:20.845655 windmill_api-1.96.2/windmill_api/models/whois_response_200.py
+-rw-r--r--   0        0        0     1567 2023-05-08 21:40:20.825655 windmill_api-1.96.2/windmill_api/models/whois_response_200_usage.py
+-rw-r--r--   0        0        0     2604 2023-05-08 21:40:20.861655 windmill_api-1.96.2/windmill_api/models/worker_ping.py
+-rw-r--r--   0        0        0     1901 2023-05-08 21:40:20.877655 windmill_api-1.96.2/windmill_api/models/workspace.py
+-rw-r--r--   0        0        0     1974 2023-05-08 21:40:20.893655 windmill_api-1.96.2/windmill_api/models/workspace_invite.py
+-rw-r--r--   0        0        0       25 2023-05-08 21:39:48.633678 windmill_api-1.96.2/windmill_api/py.typed
+-rw-r--r--   0        0        0      939 2023-05-08 21:40:20.893655 windmill_api-1.96.2/windmill_api/types.py
+-rw-r--r--   0        0        0     4362 1970-01-01 00:00:00.000000 windmill_api-1.96.2/setup.py
+-rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.96.2/PKG-INFO
```

### Comparing `windmill_api-1.96.1/LICENSE` & `windmill_api-1.96.2/LICENSE`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/README.md` & `windmill_api-1.96.2/README.md`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/pyproject.toml` & `windmill_api-1.96.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "windmill-api"
-version = "1.96.1"
+version = "1.96.2"
 description = "A client library for accessing Windmill API"
 license = "Apache-2.0"
 
 authors = ["Ruben Fiszel <ruben@windmill.dev>"]
 
 readme = "README.md"
 packages = [
```

### Comparing `windmill_api-1.96.1/windmill_api/api/app/create_app.py` & `windmill_api-1.96.2/windmill_api/api/app/create_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/app/delete_app.py` & `windmill_api-1.96.2/windmill_api/api/app/delete_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/app/execute_component.py` & `windmill_api-1.96.2/windmill_api/api/app/execute_component.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/app/exists_app.py` & `windmill_api-1.96.2/windmill_api/api/app/exists_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/app/get_app_by_path.py` & `windmill_api-1.96.2/windmill_api/api/app/get_app_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/app/get_app_by_path_with_draft.py` & `windmill_api-1.96.2/windmill_api/api/app/get_app_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/app/get_app_by_version.py` & `windmill_api-1.96.2/windmill_api/api/app/get_app_by_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/app/get_hub_app_by_id.py` & `windmill_api-1.96.2/windmill_api/api/app/get_hub_app_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/app/get_public_app_by_secret.py` & `windmill_api-1.96.2/windmill_api/api/app/get_public_app_by_secret.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/app/get_public_secret_of_app.py` & `windmill_api-1.96.2/windmill_api/api/app/get_public_secret_of_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/app/list_apps.py` & `windmill_api-1.96.2/windmill_api/api/app/list_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/app/list_hub_apps.py` & `windmill_api-1.96.2/windmill_api/api/app/list_hub_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/app/update_app.py` & `windmill_api-1.96.2/windmill_api/api/app/update_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/audit/get_audit_log.py` & `windmill_api-1.96.2/windmill_api/api/audit/get_audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/audit/list_audit_logs.py` & `windmill_api-1.96.2/windmill_api/api/audit/list_audit_logs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/capture/create_capture.py` & `windmill_api-1.96.2/windmill_api/api/capture/create_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/capture/get_capture.py` & `windmill_api-1.96.2/windmill_api/api/capture/get_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/capture/update_capture.py` & `windmill_api-1.96.2/windmill_api/api/capture/update_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/draft/create_draft.py` & `windmill_api-1.96.2/windmill_api/api/draft/create_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/favorite/star.py` & `windmill_api-1.96.2/windmill_api/api/favorite/star.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/favorite/unstar.py` & `windmill_api-1.96.2/windmill_api/api/favorite/unstar.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/flow/archive_flow_by_path.py` & `windmill_api-1.96.2/windmill_api/api/flow/archive_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/flow/create_flow.py` & `windmill_api-1.96.2/windmill_api/api/flow/create_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/flow/delete_flow_by_path.py` & `windmill_api-1.96.2/windmill_api/api/flow/delete_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/flow/exists_flow_by_path.py` & `windmill_api-1.96.2/windmill_api/api/flow/exists_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/flow/get_flow_by_path.py` & `windmill_api-1.96.2/windmill_api/api/flow/get_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/flow/get_flow_by_path_with_draft.py` & `windmill_api-1.96.2/windmill_api/api/flow/get_flow_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/flow/get_flow_input_history_by_path.py` & `windmill_api-1.96.2/windmill_api/api/flow/get_flow_input_history_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/flow/get_hub_flow_by_id.py` & `windmill_api-1.96.2/windmill_api/api/flow/get_hub_flow_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/flow/list_flow_paths.py` & `windmill_api-1.96.2/windmill_api/api/flow/list_flow_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/flow/list_flows.py` & `windmill_api-1.96.2/windmill_api/api/flow/list_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/flow/list_hub_flows.py` & `windmill_api-1.96.2/windmill_api/api/flow/list_hub_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/flow/update_flow.py` & `windmill_api-1.96.2/windmill_api/api/flow/update_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/folder/add_owner_to_folder.py` & `windmill_api-1.96.2/windmill_api/api/folder/add_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/folder/create_folder.py` & `windmill_api-1.96.2/windmill_api/api/folder/create_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/folder/delete_folder.py` & `windmill_api-1.96.2/windmill_api/api/folder/delete_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/folder/get_folder.py` & `windmill_api-1.96.2/windmill_api/api/folder/get_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/folder/get_folder_usage.py` & `windmill_api-1.96.2/windmill_api/api/folder/get_folder_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/folder/list_folder_names.py` & `windmill_api-1.96.2/windmill_api/api/folder/list_folder_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/folder/list_folders.py` & `windmill_api-1.96.2/windmill_api/api/folder/list_folders.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/folder/remove_owner_to_folder.py` & `windmill_api-1.96.2/windmill_api/api/folder/remove_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/folder/update_folder.py` & `windmill_api-1.96.2/windmill_api/api/folder/update_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/granular_acl/add_granular_acls.py` & `windmill_api-1.96.2/windmill_api/api/granular_acl/add_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/granular_acl/get_granular_acls.py` & `windmill_api-1.96.2/windmill_api/api/granular_acl/get_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/granular_acl/remove_granular_acls.py` & `windmill_api-1.96.2/windmill_api/api/granular_acl/remove_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/group/add_user_to_group.py` & `windmill_api-1.96.2/windmill_api/api/group/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/group/create_group.py` & `windmill_api-1.96.2/windmill_api/api/group/create_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/group/delete_group.py` & `windmill_api-1.96.2/windmill_api/api/group/delete_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/group/get_group.py` & `windmill_api-1.96.2/windmill_api/api/group/get_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/group/list_group_names.py` & `windmill_api-1.96.2/windmill_api/api/group/list_group_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/group/list_groups.py` & `windmill_api-1.96.2/windmill_api/api/group/list_groups.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/group/remove_user_to_group.py` & `windmill_api-1.96.2/windmill_api/api/group/remove_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/group/update_group.py` & `windmill_api-1.96.2/windmill_api/api/group/update_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/input_/create_input.py` & `windmill_api-1.96.2/windmill_api/api/input_/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/input_/delete_input.py` & `windmill_api-1.96.2/windmill_api/api/input_/delete_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/input_/get_input_history.py` & `windmill_api-1.96.2/windmill_api/api/input_/get_input_history.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/input_/list_inputs.py` & `windmill_api-1.96.2/windmill_api/api/input_/list_inputs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/input_/update_input.py` & `windmill_api-1.96.2/windmill_api/api/input_/update_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/cancel_queued_job.py` & `windmill_api-1.96.2/windmill_api/api/job/cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/cancel_suspended_job_get.py` & `windmill_api-1.96.2/windmill_api/api/job/cancel_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/cancel_suspended_job_post.py` & `windmill_api-1.96.2/windmill_api/api/job/cancel_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/create_job_signature.py` & `windmill_api-1.96.2/windmill_api/api/job/create_job_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/delete_completed_job.py` & `windmill_api-1.96.2/windmill_api/api/job/delete_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/force_cancel_queued_job.py` & `windmill_api-1.96.2/windmill_api/api/job/force_cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/get_completed_job.py` & `windmill_api-1.96.2/windmill_api/api/job/get_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/get_completed_job_result.py` & `windmill_api-1.96.2/windmill_api/api/job/get_completed_job_result.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/get_job.py` & `windmill_api-1.96.2/windmill_api/api/job/get_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/get_job_updates.py` & `windmill_api-1.96.2/windmill_api/api/job/get_job_updates.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/get_resume_urls.py` & `windmill_api-1.96.2/windmill_api/api/job/get_resume_urls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/get_suspended_job_flow.py` & `windmill_api-1.96.2/windmill_api/api/job/get_suspended_job_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/list_completed_jobs.py` & `windmill_api-1.96.2/windmill_api/api/job/list_completed_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/list_jobs.py` & `windmill_api-1.96.2/windmill_api/api/job/list_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/list_queue.py` & `windmill_api-1.96.2/windmill_api/api/job/list_queue.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/result_by_id.py` & `windmill_api-1.96.2/windmill_api/api/job/result_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/resume_suspended_flow_as_owner.py` & `windmill_api-1.96.2/windmill_api/api/job/resume_suspended_flow_as_owner.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/resume_suspended_job_get.py` & `windmill_api-1.96.2/windmill_api/api/job/resume_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/resume_suspended_job_post.py` & `windmill_api-1.96.2/windmill_api/api/job/resume_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/run_flow_by_path.py` & `windmill_api-1.96.2/windmill_api/api/job/run_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/run_flow_preview.py` & `windmill_api-1.96.2/windmill_api/api/job/run_flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/run_script_by_hash.py` & `windmill_api-1.96.2/windmill_api/api/job/run_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/run_script_by_path.py` & `windmill_api-1.96.2/windmill_api/api/job/run_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/run_script_preview.py` & `windmill_api-1.96.2/windmill_api/api/job/run_script_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/run_wait_result_flow_by_path.py` & `windmill_api-1.96.2/windmill_api/api/job/run_wait_result_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/run_wait_result_script_by_path.py` & `windmill_api-1.96.2/windmill_api/api/job/run_wait_result_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/job/run_wait_result_script_by_path_get.py` & `windmill_api-1.96.2/windmill_api/api/job/run_wait_result_script_by_path_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/oauth/connect_callback.py` & `windmill_api-1.96.2/windmill_api/api/oauth/connect_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/oauth/connect_slack_callback.py` & `windmill_api-1.96.2/windmill_api/api/oauth/connect_slack_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/oauth/create_account.py` & `windmill_api-1.96.2/windmill_api/api/oauth/create_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/oauth/disconnect_account.py` & `windmill_api-1.96.2/windmill_api/api/oauth/disconnect_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/oauth/disconnect_slack.py` & `windmill_api-1.96.2/windmill_api/api/oauth/disconnect_slack.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/oauth/list_o_auth_connects.py` & `windmill_api-1.96.2/windmill_api/api/oauth/list_o_auth_connects.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/oauth/list_o_auth_logins.py` & `windmill_api-1.96.2/windmill_api/api/oauth/list_o_auth_logins.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/oauth/refresh_token.py` & `windmill_api-1.96.2/windmill_api/api/oauth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/raw_app/create_raw_app.py` & `windmill_api-1.96.2/windmill_api/api/raw_app/create_raw_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/raw_app/delete_raw_app.py` & `windmill_api-1.96.2/windmill_api/api/raw_app/delete_raw_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/raw_app/exists_raw_app.py` & `windmill_api-1.96.2/windmill_api/api/raw_app/exists_raw_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/raw_app/get_raw_app_data.py` & `windmill_api-1.96.2/windmill_api/api/raw_app/get_raw_app_data.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/raw_app/list_raw_apps.py` & `windmill_api-1.96.2/windmill_api/api/raw_app/list_raw_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/raw_app/update_raw_app.py` & `windmill_api-1.96.2/windmill_api/api/raw_app/update_raw_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/resource/create_resource.py` & `windmill_api-1.96.2/windmill_api/api/resource/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/resource/create_resource_type.py` & `windmill_api-1.96.2/windmill_api/api/resource/create_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/resource/delete_resource.py` & `windmill_api-1.96.2/windmill_api/api/resource/delete_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/resource/delete_resource_type.py` & `windmill_api-1.96.2/windmill_api/api/resource/delete_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/resource/exists_resource.py` & `windmill_api-1.96.2/windmill_api/api/resource/exists_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/resource/exists_resource_type.py` & `windmill_api-1.96.2/windmill_api/api/resource/exists_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/resource/get_resource.py` & `windmill_api-1.96.2/windmill_api/api/resource/get_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/resource/get_resource_type.py` & `windmill_api-1.96.2/windmill_api/api/resource/get_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/resource/get_resource_value.py` & `windmill_api-1.96.2/windmill_api/api/resource/get_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/resource/list_resource.py` & `windmill_api-1.96.2/windmill_api/api/resource/list_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/resource/list_resource_type.py` & `windmill_api-1.96.2/windmill_api/api/resource/list_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/resource/list_resource_type_names.py` & `windmill_api-1.96.2/windmill_api/api/resource/list_resource_type_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/resource/update_resource.py` & `windmill_api-1.96.2/windmill_api/api/resource/update_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/resource/update_resource_type.py` & `windmill_api-1.96.2/windmill_api/api/resource/update_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/resource/update_resource_value.py` & `windmill_api-1.96.2/windmill_api/api/resource/update_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/schedule/create_schedule.py` & `windmill_api-1.96.2/windmill_api/api/schedule/create_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/schedule/delete_schedule.py` & `windmill_api-1.96.2/windmill_api/api/schedule/delete_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/schedule/exists_schedule.py` & `windmill_api-1.96.2/windmill_api/api/schedule/exists_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/schedule/get_schedule.py` & `windmill_api-1.96.2/windmill_api/api/schedule/get_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/schedule/list_schedules.py` & `windmill_api-1.96.2/windmill_api/api/schedule/list_schedules.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/schedule/preview_schedule.py` & `windmill_api-1.96.2/windmill_api/api/schedule/preview_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/schedule/set_schedule_enabled.py` & `windmill_api-1.96.2/windmill_api/api/schedule/set_schedule_enabled.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/schedule/update_schedule.py` & `windmill_api-1.96.2/windmill_api/api/schedule/update_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/archive_script_by_hash.py` & `windmill_api-1.96.2/windmill_api/api/script/archive_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/archive_script_by_path.py` & `windmill_api-1.96.2/windmill_api/api/script/archive_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/bash_to_jsonschema.py` & `windmill_api-1.96.2/windmill_api/api/script/bash_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/create_script.py` & `windmill_api-1.96.2/windmill_api/api/script/create_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/delete_script_by_hash.py` & `windmill_api-1.96.2/windmill_api/api/script/delete_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/delete_script_by_path.py` & `windmill_api-1.96.2/windmill_api/api/script/delete_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/deno_to_jsonschema.py` & `windmill_api-1.96.2/windmill_api/api/script/deno_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/exists_script_by_path.py` & `windmill_api-1.96.2/windmill_api/api/script/exists_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/get_hub_script_by_path.py` & `windmill_api-1.96.2/windmill_api/api/script/get_hub_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/get_hub_script_content_by_path.py` & `windmill_api-1.96.2/windmill_api/api/script/get_hub_script_content_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/get_script_by_hash.py` & `windmill_api-1.96.2/windmill_api/api/script/get_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/get_script_by_path.py` & `windmill_api-1.96.2/windmill_api/api/script/get_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/get_script_by_path_with_draft.py` & `windmill_api-1.96.2/windmill_api/api/script/get_script_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/get_script_deployment_status.py` & `windmill_api-1.96.2/windmill_api/api/script/get_script_deployment_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/go_to_jsonschema.py` & `windmill_api-1.96.2/windmill_api/api/script/go_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/list_hub_scripts.py` & `windmill_api-1.96.2/windmill_api/api/script/list_hub_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/list_script_paths.py` & `windmill_api-1.96.2/windmill_api/api/script/list_script_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/list_scripts.py` & `windmill_api-1.96.2/windmill_api/api/script/list_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/python_to_jsonschema.py` & `windmill_api-1.96.2/windmill_api/api/script/python_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/raw_script_by_hash.py` & `windmill_api-1.96.2/windmill_api/api/script/raw_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/raw_script_by_path.py` & `windmill_api-1.96.2/windmill_api/api/script/raw_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/script/raw_script_by_path_tokened.py` & `windmill_api-1.96.2/windmill_api/api/script/raw_script_by_path_tokened.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/settings/backend_version.py` & `windmill_api-1.96.2/windmill_api/api/settings/backend_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/settings/get_open_api_yaml.py` & `windmill_api-1.96.2/windmill_api/api/settings/get_open_api_yaml.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/accept_invite.py` & `windmill_api-1.96.2/windmill_api/api/user/accept_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/create_token.py` & `windmill_api-1.96.2/windmill_api/api/user/create_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/create_token_impersonate.py` & `windmill_api-1.96.2/windmill_api/api/user/create_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/create_user.py` & `windmill_api-1.96.2/windmill_api/api/user/create_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/create_user_globally.py` & `windmill_api-1.96.2/windmill_api/api/user/create_user_globally.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/decline_invite.py` & `windmill_api-1.96.2/windmill_api/api/user/decline_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/delete_token.py` & `windmill_api-1.96.2/windmill_api/api/user/delete_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/delete_user.py` & `windmill_api-1.96.2/windmill_api/api/user/delete_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/get_current_email.py` & `windmill_api-1.96.2/windmill_api/api/user/get_current_email.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/get_usage.py` & `windmill_api-1.96.2/windmill_api/api/user/get_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/global_user_delete.py` & `windmill_api-1.96.2/windmill_api/api/user/global_user_delete.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/global_user_update.py` & `windmill_api-1.96.2/windmill_api/api/user/global_user_update.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/global_whoami.py` & `windmill_api-1.96.2/windmill_api/api/user/global_whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/is_owner_of_path.py` & `windmill_api-1.96.2/windmill_api/api/user/is_owner_of_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/leave_workspace.py` & `windmill_api-1.96.2/windmill_api/api/user/leave_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/list_tokens.py` & `windmill_api-1.96.2/windmill_api/api/user/list_tokens.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/list_usernames.py` & `windmill_api-1.96.2/windmill_api/api/user/list_usernames.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/list_users.py` & `windmill_api-1.96.2/windmill_api/api/user/list_users.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/list_users_as_super_admin.py` & `windmill_api-1.96.2/windmill_api/api/user/list_users_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/list_workspace_invites.py` & `windmill_api-1.96.2/windmill_api/api/user/list_workspace_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/login.py` & `windmill_api-1.96.2/windmill_api/api/user/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/login_with_oauth.py` & `windmill_api-1.96.2/windmill_api/api/user/login_with_oauth.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/logout.py` & `windmill_api-1.96.2/windmill_api/api/user/logout.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/set_password.py` & `windmill_api-1.96.2/windmill_api/api/user/set_password.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/update_user.py` & `windmill_api-1.96.2/windmill_api/api/user/update_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/whoami.py` & `windmill_api-1.96.2/windmill_api/api/user/whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/user/whois.py` & `windmill_api-1.96.2/windmill_api/api/user/whois.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/variable/create_variable.py` & `windmill_api-1.96.2/windmill_api/api/variable/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/variable/delete_variable.py` & `windmill_api-1.96.2/windmill_api/api/variable/delete_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/variable/exists_variable.py` & `windmill_api-1.96.2/windmill_api/api/variable/exists_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/variable/get_variable.py` & `windmill_api-1.96.2/windmill_api/api/variable/get_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/variable/list_contextual_variables.py` & `windmill_api-1.96.2/windmill_api/api/variable/list_contextual_variables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/variable/list_variable.py` & `windmill_api-1.96.2/windmill_api/api/variable/list_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/variable/update_variable.py` & `windmill_api-1.96.2/windmill_api/api/variable/update_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/worker/get_custom_tags.py` & `windmill_api-1.96.2/windmill_api/api/worker/get_custom_tags.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/worker/list_workers.py` & `windmill_api-1.96.2/windmill_api/api/worker/list_workers.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/add_user.py` & `windmill_api-1.96.2/windmill_api/api/workspace/add_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/archive_workspace.py` & `windmill_api-1.96.2/windmill_api/api/workspace/archive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/create_workspace.py` & `windmill_api-1.96.2/windmill_api/api/workspace/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/delete_invite.py` & `windmill_api-1.96.2/windmill_api/api/workspace/delete_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/delete_workspace.py` & `windmill_api-1.96.2/windmill_api/api/workspace/delete_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/edit_auto_invite.py` & `windmill_api-1.96.2/windmill_api/api/workspace/edit_auto_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/edit_slack_command.py` & `windmill_api-1.96.2/windmill_api/api/workspace/edit_slack_command.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/edit_webhook.py` & `windmill_api-1.96.2/windmill_api/api/workspace/edit_webhook.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/exists_username.py` & `windmill_api-1.96.2/windmill_api/api/workspace/exists_username.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/exists_workspace.py` & `windmill_api-1.96.2/windmill_api/api/workspace/exists_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/get_premium_info.py` & `windmill_api-1.96.2/windmill_api/api/workspace/get_premium_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/get_settings.py` & `windmill_api-1.96.2/windmill_api/api/workspace/get_settings.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/invite_user.py` & `windmill_api-1.96.2/windmill_api/api/workspace/invite_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/is_domain_allowed.py` & `windmill_api-1.96.2/windmill_api/api/workspace/is_domain_allowed.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/list_pending_invites.py` & `windmill_api-1.96.2/windmill_api/api/workspace/list_pending_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/list_user_workspaces.py` & `windmill_api-1.96.2/windmill_api/api/workspace/list_user_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/list_workspaces.py` & `windmill_api-1.96.2/windmill_api/api/workspace/list_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/list_workspaces_as_super_admin.py` & `windmill_api-1.96.2/windmill_api/api/workspace/list_workspaces_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/api/workspace/unarchive_workspace.py` & `windmill_api-1.96.2/windmill_api/api/workspace/unarchive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/client.py` & `windmill_api-1.96.2/windmill_api/client.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/accept_invite_json_body.py` & `windmill_api-1.96.2/windmill_api/models/accept_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/add_granular_acls_json_body.py` & `windmill_api-1.96.2/windmill_api/models/add_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/add_owner_to_folder_json_body.py` & `windmill_api-1.96.2/windmill_api/models/add_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/add_user_json_body.py` & `windmill_api-1.96.2/windmill_api/models/add_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/add_user_to_group_json_body.py` & `windmill_api-1.96.2/windmill_api/models/add_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/app_with_last_version.py` & `windmill_api-1.96.2/windmill_api/models/app_with_last_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/app_with_last_version_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/app_with_last_version_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/app_with_last_version_policy.py` & `windmill_api-1.96.2/windmill_api/models/app_with_last_version_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/app_with_last_version_policy_triggerables.py` & `windmill_api-1.96.2/windmill_api/models/app_with_last_version_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py` & `windmill_api-1.96.2/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft.py` & `windmill_api-1.96.2/windmill_api/models/app_with_last_version_w_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/app_with_last_version_w_draft_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_policy.py` & `windmill_api-1.96.2/windmill_api/models/app_with_last_version_w_draft_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py` & `windmill_api-1.96.2/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py` & `windmill_api-1.96.2/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/archive_flow_by_path_json_body.py` & `windmill_api-1.96.2/windmill_api/models/archive_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200.py` & `windmill_api-1.96.2/windmill_api/models/archive_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/archive_script_by_hash_response_200_schema.py` & `windmill_api-1.96.2/windmill_api/models/archive_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/audit_log.py` & `windmill_api-1.96.2/windmill_api/models/audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/audit_log_operation.py` & `windmill_api-1.96.2/windmill_api/models/audit_log_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/audit_log_parameters.py` & `windmill_api-1.96.2/windmill_api/models/audit_log_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200.py` & `windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item.py` & `windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.96.2/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_all.py` & `windmill_api-1.96.2/windmill_api/models/branch_all.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item.py` & `windmill_api-1.96.2/windmill_api/models/branch_all_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_all_branches_item_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/branch_all_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one.py` & `windmill_api-1.96.2/windmill_api/models/branch_one.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_branches_item_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_default_item.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_default_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_default_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_default_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_default_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_default_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_default_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/branch_one_default_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/branch_one_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/cancel_queued_job_json_body.py` & `windmill_api-1.96.2/windmill_api/models/cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/cancel_suspended_job_post_json_body.py` & `windmill_api-1.96.2/windmill_api/models/cancel_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job.py` & `windmill_api-1.96.2/windmill_api/models/completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_args.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_branchall.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_failure_module_iterator.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_branchall.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_modules_item_iterator.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_flow_status_retry.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/connect_callback_json_body.py` & `windmill_api-1.96.2/windmill_api/models/connect_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/connect_callback_response_200.py` & `windmill_api-1.96.2/windmill_api/models/connect_callback_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/connect_slack_callback_json_body.py` & `windmill_api-1.96.2/windmill_api/models/connect_slack_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/contextual_variable.py` & `windmill_api-1.96.2/windmill_api/models/contextual_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_account_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_account_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_app_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_app_json_body_policy.py` & `windmill_api-1.96.2/windmill_api/models/create_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_app_json_body_policy_triggerables.py` & `windmill_api-1.96.2/windmill_api/models/create_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.96.2/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_draft_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_draft_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_flow_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_folder_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_group_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_input.py` & `windmill_api-1.96.2/windmill_api/models/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_input_args.py` & `windmill_api-1.96.2/windmill_api/models/create_input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_input_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_input_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_input_json_body_args.py` & `windmill_api-1.96.2/windmill_api/models/create_input_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_raw_app_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_raw_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_resource.py` & `windmill_api-1.96.2/windmill_api/models/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_resource_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_resource_type_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_schedule_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_schedule_json_body_args.py` & `windmill_api-1.96.2/windmill_api/models/create_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_script_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_script_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_script_json_body_schema.py` & `windmill_api-1.96.2/windmill_api/models/create_script_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_token_impersonate_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_token_impersonate_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_token_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_user_globally_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_user_globally_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_user_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_variable.py` & `windmill_api-1.96.2/windmill_api/models/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_variable_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_workspace.py` & `windmill_api-1.96.2/windmill_api/models/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/create_workspace_json_body.py` & `windmill_api-1.96.2/windmill_api/models/create_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/decline_invite_json_body.py` & `windmill_api-1.96.2/windmill_api/models/decline_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_args.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_invite_json_body.py` & `windmill_api-1.96.2/windmill_api/models/delete_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200.py` & `windmill_api-1.96.2/windmill_api/models/delete_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/delete_script_by_hash_response_200_schema.py` & `windmill_api-1.96.2/windmill_api/models/delete_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200.py` & `windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item.py` & `windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.96.2/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/edit_auto_invite_json_body.py` & `windmill_api-1.96.2/windmill_api/models/edit_auto_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/edit_resource.py` & `windmill_api-1.96.2/windmill_api/models/edit_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/edit_resource_type.py` & `windmill_api-1.96.2/windmill_api/models/edit_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/edit_schedule.py` & `windmill_api-1.96.2/windmill_api/models/edit_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/edit_schedule_args.py` & `windmill_api-1.96.2/windmill_api/models/edit_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/edit_slack_command_json_body.py` & `windmill_api-1.96.2/windmill_api/models/edit_slack_command_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/edit_variable.py` & `windmill_api-1.96.2/windmill_api/models/edit_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/edit_webhook_json_body.py` & `windmill_api-1.96.2/windmill_api/models/edit_webhook_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/edit_workspace_user.py` & `windmill_api-1.96.2/windmill_api/models/edit_workspace_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/execute_component_json_body.py` & `windmill_api-1.96.2/windmill_api/models/execute_component_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py` & `windmill_api-1.96.2/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/execute_component_json_body_raw_code.py` & `windmill_api-1.96.2/windmill_api/models/execute_component_json_body_raw_code.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/exists_username_json_body.py` & `windmill_api-1.96.2/windmill_api/models/exists_username_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/exists_workspace_json_body.py` & `windmill_api-1.96.2/windmill_api/models/exists_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow.py` & `windmill_api-1.96.2/windmill_api/models/flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/flow_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_metadata.py` & `windmill_api-1.96.2/windmill_api/models/flow_metadata.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_metadata_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/flow_metadata_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module.py` & `windmill_api-1.96.2/windmill_api/models/flow_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_0_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_1_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_2_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_module_value_2_type_6.py` & `windmill_api-1.96.2/windmill_api/models/flow_module_value_2_type_6.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_args.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_failure_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_preview_value_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/flow_preview_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_schema.py` & `windmill_api-1.96.2/windmill_api/models/flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status.py` & `windmill_api-1.96.2/windmill_api/models/flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_branchall.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_failure_module_iterator.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_module.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_module_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_module_branch_chosen.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_module_branchall.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_module_iterator.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_branchall.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_modules_item_iterator.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_status_retry.py` & `windmill_api-1.96.2/windmill_api/models/flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value.py` & `windmill_api-1.96.2/windmill_api/models/flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_failure_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/flow_value_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/folder.py` & `windmill_api-1.96.2/windmill_api/models/folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/folder_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/folder_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/force_cancel_queued_job_json_body.py` & `windmill_api-1.96.2/windmill_api/models/force_cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/forloop_flow.py` & `windmill_api-1.96.2/windmill_api/models/forloop_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/forloop_flow_iterator_type_0.py` & `windmill_api-1.96.2/windmill_api/models/forloop_flow_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/forloop_flow_iterator_type_1.py` & `windmill_api-1.96.2/windmill_api/models/forloop_flow_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/forloop_flow_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/forloop_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_app_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/get_app_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_policy.py` & `windmill_api-1.96.2/windmill_api/models/get_app_by_path_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py` & `windmill_api-1.96.2/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.96.2/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_app_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py` & `windmill_api-1.96.2/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py` & `windmill_api-1.96.2/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.96.2/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_app_by_version_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/get_app_by_version_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_policy.py` & `windmill_api-1.96.2/windmill_api/models/get_app_by_version_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py` & `windmill_api-1.96.2/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.96.2/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_audit_log_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_audit_log_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_audit_log_response_200_operation.py` & `windmill_api-1.96.2/windmill_api/models/get_audit_log_response_200_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_audit_log_response_200_parameters.py` & `windmill_api-1.96.2/windmill_api/models/get_audit_log_response_200_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_args.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_schema.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_input_history_by_path_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_input_history_by_path_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py` & `windmill_api-1.96.2/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_folder_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_folder_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_folder_response_200_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/get_folder_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_folder_usage_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_folder_usage_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_granular_acls_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_granular_acls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_group_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_group_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_group_response_200_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/get_group_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_app_by_id_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_app_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_app_by_id_response_200_app.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_app_by_id_response_200_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_hub_script_by_path_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_hub_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_input_history_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/get_input_history_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_input_history_response_200_item_args.py` & `windmill_api-1.96.2/windmill_api/models/get_input_history_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_job_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_job_updates_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_job_updates_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_premium_info_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_premium_info_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_public_app_by_secret_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_policy.py` & `windmill_api-1.96.2/windmill_api/models/get_public_app_by_secret_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py` & `windmill_api-1.96.2/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.96.2/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_resource_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_resource_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_resource_response_200_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/get_resource_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_resource_type_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_resource_type_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_resume_urls_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_resume_urls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_schedule_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_schedule_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_schedule_response_200_args.py` & `windmill_api-1.96.2/windmill_api/models/get_schedule_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_schedule_response_200_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/get_schedule_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/get_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_script_by_hash_response_200_schema.py` & `windmill_api-1.96.2/windmill_api/models/get_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/get_script_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_script_by_path_response_200_schema.py` & `windmill_api-1.96.2/windmill_api/models/get_script_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_script_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py` & `windmill_api-1.96.2/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py` & `windmill_api-1.96.2/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py` & `windmill_api-1.96.2/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_script_deployment_status_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_script_deployment_status_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_settings_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_suspended_job_flow_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_suspended_job_flow_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_suspended_job_flow_response_200_job.py` & `windmill_api-1.96.2/windmill_api/models/get_suspended_job_flow_response_200_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_variable_response_200.py` & `windmill_api-1.96.2/windmill_api/models/get_variable_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/get_variable_response_200_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/get_variable_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/global_user_info.py` & `windmill_api-1.96.2/windmill_api/models/global_user_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/global_user_update_json_body.py` & `windmill_api-1.96.2/windmill_api/models/global_user_update_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/global_whoami_response_200.py` & `windmill_api-1.96.2/windmill_api/models/global_whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200.py` & `windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item.py` & `windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.96.2/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/group.py` & `windmill_api-1.96.2/windmill_api/models/group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/group_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/group_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/identity.py` & `windmill_api-1.96.2/windmill_api/models/identity.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/input_.py` & `windmill_api-1.96.2/windmill_api/models/input_.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/input_args.py` & `windmill_api-1.96.2/windmill_api/models/input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/input_transform_type_0.py` & `windmill_api-1.96.2/windmill_api/models/input_transform_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/input_transform_type_1.py` & `windmill_api-1.96.2/windmill_api/models/input_transform_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/invite_user_json_body.py` & `windmill_api-1.96.2/windmill_api/models/invite_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/javascript_transform.py` & `windmill_api-1.96.2/windmill_api/models/javascript_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/job.py` & `windmill_api-1.96.2/windmill_api/models/job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_apps_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_apps_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_apps_response_200_item_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/list_apps_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_audit_logs_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_audit_logs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_audit_logs_response_200_item_operation.py` & `windmill_api-1.96.2/windmill_api/models/list_audit_logs_response_200_item_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_audit_logs_response_200_item_parameters.py` & `windmill_api-1.96.2/windmill_api/models/list_audit_logs_response_200_item_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_args.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_contextual_variables_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_contextual_variables_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_flows_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_flows_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_folders_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_folders_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_folders_response_200_item_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/list_folders_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_groups_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_groups_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_groups_response_200_item_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/list_groups_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_hub_apps_response_200.py` & `windmill_api-1.96.2/windmill_api/models/list_hub_apps_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_hub_apps_response_200_apps_item.py` & `windmill_api-1.96.2/windmill_api/models/list_hub_apps_response_200_apps_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_hub_flows_response_200.py` & `windmill_api-1.96.2/windmill_api/models/list_hub_flows_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_hub_flows_response_200_flows_item.py` & `windmill_api-1.96.2/windmill_api/models/list_hub_flows_response_200_flows_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_hub_scripts_response_200.py` & `windmill_api-1.96.2/windmill_api/models/list_hub_scripts_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_hub_scripts_response_200_asks_item.py` & `windmill_api-1.96.2/windmill_api/models/list_hub_scripts_response_200_asks_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_inputs_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_inputs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_inputs_response_200_item_args.py` & `windmill_api-1.96.2/windmill_api/models/list_inputs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_jobs_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_pending_invites_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_pending_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_args.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_flow_status_retry.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_raw_apps_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_raw_apps_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_raw_apps_response_200_item_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/list_raw_apps_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_resource_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_resource_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_resource_response_200_item_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/list_resource_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_resource_type_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_resource_type_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_schedules_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_schedules_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_schedules_response_200_item_args.py` & `windmill_api-1.96.2/windmill_api/models/list_schedules_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_schedules_response_200_item_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/list_schedules_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_scripts_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/list_scripts_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_scripts_response_200_item_schema.py` & `windmill_api-1.96.2/windmill_api/models/list_scripts_response_200_item_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_tokens_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_tokens_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_user_workspaces_response_200.py` & `windmill_api-1.96.2/windmill_api/models/list_user_workspaces_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py` & `windmill_api-1.96.2/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_users_as_super_admin_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_users_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_users_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_users_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_users_response_200_item_usage.py` & `windmill_api-1.96.2/windmill_api/models/list_users_response_200_item_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_variable_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_variable_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_variable_response_200_item_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/list_variable_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_workers_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_workers_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_workspace_invites_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_workspace_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/list_workspaces_response_200_item.py` & `windmill_api-1.96.2/windmill_api/models/list_workspaces_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/listable_app.py` & `windmill_api-1.96.2/windmill_api/models/listable_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/listable_app_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/listable_app_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/listable_raw_app.py` & `windmill_api-1.96.2/windmill_api/models/listable_raw_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/listable_raw_app_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/listable_raw_app_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/listable_resource.py` & `windmill_api-1.96.2/windmill_api/models/listable_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/listable_resource_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/listable_resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/listable_variable.py` & `windmill_api-1.96.2/windmill_api/models/listable_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/listable_variable_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/listable_variable_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/login.py` & `windmill_api-1.96.2/windmill_api/models/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/login_json_body.py` & `windmill_api-1.96.2/windmill_api/models/login_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/login_with_oauth_json_body.py` & `windmill_api-1.96.2/windmill_api/models/login_with_oauth_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/main_arg_signature.py` & `windmill_api-1.96.2/windmill_api/models/main_arg_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item.py` & `windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_1.py` & `windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_2.py` & `windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_3.py` & `windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py` & `windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_4.py` & `windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.96.2/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/new_schedule.py` & `windmill_api-1.96.2/windmill_api/models/new_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/new_schedule_args.py` & `windmill_api-1.96.2/windmill_api/models/new_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/new_script.py` & `windmill_api-1.96.2/windmill_api/models/new_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/new_script_schema.py` & `windmill_api-1.96.2/windmill_api/models/new_script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/new_script_with_draft.py` & `windmill_api-1.96.2/windmill_api/models/new_script_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/new_script_with_draft_draft.py` & `windmill_api-1.96.2/windmill_api/models/new_script_with_draft_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/new_script_with_draft_draft_schema.py` & `windmill_api-1.96.2/windmill_api/models/new_script_with_draft_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/new_script_with_draft_schema.py` & `windmill_api-1.96.2/windmill_api/models/new_script_with_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/new_token.py` & `windmill_api-1.96.2/windmill_api/models/new_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/new_token_impersonate.py` & `windmill_api-1.96.2/windmill_api/models/new_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/new_user.py` & `windmill_api-1.96.2/windmill_api/models/new_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow.py` & `windmill_api-1.96.2/windmill_api/models/open_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_schema.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_failure_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_value_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_schema.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/path_flow.py` & `windmill_api-1.96.2/windmill_api/models/path_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms.py` & `windmill_api-1.96.2/windmill_api/models/path_flow_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.2/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.2/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/path_script.py` & `windmill_api-1.96.2/windmill_api/models/path_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/path_script_input_transforms.py` & `windmill_api-1.96.2/windmill_api/models/path_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/path_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.2/windmill_api/models/path_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/path_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.2/windmill_api/models/path_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/policy.py` & `windmill_api-1.96.2/windmill_api/models/policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/policy_triggerables.py` & `windmill_api-1.96.2/windmill_api/models/policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/policy_triggerables_additional_property.py` & `windmill_api-1.96.2/windmill_api/models/policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/preview.py` & `windmill_api-1.96.2/windmill_api/models/preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/preview_args.py` & `windmill_api-1.96.2/windmill_api/models/preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/preview_schedule_json_body.py` & `windmill_api-1.96.2/windmill_api/models/preview_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200.py` & `windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item.py` & `windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.96.2/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job.py` & `windmill_api-1.96.2/windmill_api/models/queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_args.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_branchall.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_failure_module_iterator.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_branchall.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_modules_item_iterator.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_flow_status_retry.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/raw_script.py` & `windmill_api-1.96.2/windmill_api/models/raw_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms.py` & `windmill_api-1.96.2/windmill_api/models/raw_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.96.2/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.96.2/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/refresh_token_json_body.py` & `windmill_api-1.96.2/windmill_api/models/refresh_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/remove_granular_acls_json_body.py` & `windmill_api-1.96.2/windmill_api/models/remove_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/remove_owner_to_folder_json_body.py` & `windmill_api-1.96.2/windmill_api/models/remove_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/remove_user_to_group_json_body.py` & `windmill_api-1.96.2/windmill_api/models/remove_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/resource.py` & `windmill_api-1.96.2/windmill_api/models/resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/resource_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/resource_type.py` & `windmill_api-1.96.2/windmill_api/models/resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/resume_suspended_flow_as_owner_json_body.py` & `windmill_api-1.96.2/windmill_api/models/resume_suspended_flow_as_owner_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/resume_suspended_job_post_json_body.py` & `windmill_api-1.96.2/windmill_api/models/resume_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/retry.py` & `windmill_api-1.96.2/windmill_api/models/retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_by_path_json_body.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_args.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_script_by_hash_json_body.py` & `windmill_api-1.96.2/windmill_api/models/run_script_by_hash_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_script_by_path_json_body.py` & `windmill_api-1.96.2/windmill_api/models/run_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_script_preview_json_body.py` & `windmill_api-1.96.2/windmill_api/models/run_script_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_script_preview_json_body_args.py` & `windmill_api-1.96.2/windmill_api/models/run_script_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_wait_result_flow_by_path_json_body.py` & `windmill_api-1.96.2/windmill_api/models/run_wait_result_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/run_wait_result_script_by_path_json_body.py` & `windmill_api-1.96.2/windmill_api/models/run_wait_result_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/schedule.py` & `windmill_api-1.96.2/windmill_api/models/schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/schedule_args.py` & `windmill_api-1.96.2/windmill_api/models/schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/schedule_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/schedule_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/script.py` & `windmill_api-1.96.2/windmill_api/models/script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/script_args.py` & `windmill_api-1.96.2/windmill_api/models/script_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/script_extra_perms.py` & `windmill_api-1.96.2/windmill_api/models/script_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/script_schema.py` & `windmill_api-1.96.2/windmill_api/models/script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/set_password_json_body.py` & `windmill_api-1.96.2/windmill_api/models/set_password_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/set_schedule_enabled_json_body.py` & `windmill_api-1.96.2/windmill_api/models/set_schedule_enabled_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/slack_token.py` & `windmill_api-1.96.2/windmill_api/models/slack_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/slack_token_bot.py` & `windmill_api-1.96.2/windmill_api/models/slack_token_bot.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/star_json_body.py` & `windmill_api-1.96.2/windmill_api/models/star_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/static_transform.py` & `windmill_api-1.96.2/windmill_api/models/static_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/token_response.py` & `windmill_api-1.96.2/windmill_api/models/token_response.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/truncated_token.py` & `windmill_api-1.96.2/windmill_api/models/truncated_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/unstar_json_body.py` & `windmill_api-1.96.2/windmill_api/models/unstar_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_app_json_body.py` & `windmill_api-1.96.2/windmill_api/models/update_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_app_json_body_policy.py` & `windmill_api-1.96.2/windmill_api/models/update_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_app_json_body_policy_triggerables.py` & `windmill_api-1.96.2/windmill_api/models/update_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.96.2/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_schema.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_retry.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py` & `windmill_api-1.96.2/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_folder_json_body.py` & `windmill_api-1.96.2/windmill_api/models/update_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_group_json_body.py` & `windmill_api-1.96.2/windmill_api/models/update_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_input.py` & `windmill_api-1.96.2/windmill_api/models/update_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_input_json_body.py` & `windmill_api-1.96.2/windmill_api/models/update_input_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_raw_app_json_body.py` & `windmill_api-1.96.2/windmill_api/models/update_raw_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_resource_json_body.py` & `windmill_api-1.96.2/windmill_api/models/update_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_resource_type_json_body.py` & `windmill_api-1.96.2/windmill_api/models/update_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_resource_value_json_body.py` & `windmill_api-1.96.2/windmill_api/models/update_resource_value_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_schedule_json_body.py` & `windmill_api-1.96.2/windmill_api/models/update_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_schedule_json_body_args.py` & `windmill_api-1.96.2/windmill_api/models/update_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_user_json_body.py` & `windmill_api-1.96.2/windmill_api/models/update_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/update_variable_json_body.py` & `windmill_api-1.96.2/windmill_api/models/update_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/usage.py` & `windmill_api-1.96.2/windmill_api/models/usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/user.py` & `windmill_api-1.96.2/windmill_api/models/user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/user_usage.py` & `windmill_api-1.96.2/windmill_api/models/user_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/user_workspace_list.py` & `windmill_api-1.96.2/windmill_api/models/user_workspace_list.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/user_workspace_list_workspaces_item.py` & `windmill_api-1.96.2/windmill_api/models/user_workspace_list_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/whoami_response_200.py` & `windmill_api-1.96.2/windmill_api/models/whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/whoami_response_200_usage.py` & `windmill_api-1.96.2/windmill_api/models/whoami_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/whois_response_200.py` & `windmill_api-1.96.2/windmill_api/models/whois_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/whois_response_200_usage.py` & `windmill_api-1.96.2/windmill_api/models/whois_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/worker_ping.py` & `windmill_api-1.96.2/windmill_api/models/worker_ping.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/workspace.py` & `windmill_api-1.96.2/windmill_api/models/workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/models/workspace_invite.py` & `windmill_api-1.96.2/windmill_api/models/workspace_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/windmill_api/types.py` & `windmill_api-1.96.2/windmill_api/types.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.1/setup.py` & `windmill_api-1.96.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=21.3.0', 'httpx>=0.15.4,<0.24.0', 'python-dateutil>=2.8.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'windmill-api',
-    'version': '1.96.1',
+    'version': '1.96.2',
     'description': 'A client library for accessing Windmill API',
     'long_description': '# Autogenerated Windmill OpenApi Client\nThis is the raw autogenerated api client. You are most likely more interested in [wmill](https://pypi.org/project/wmill/) which leverages this client to offer an user friendly experience. We use [this openapi python client generator](https://github.com/openapi-generators/openapi-python-client/)\n\n# windmill-api\nA client library for accessing Windmill API\n\n## Usage\nFirst, create a client:\n\n```python\nfrom windmill_api import Client\n\nclient = Client(base_url="https://api.example.com")\n```\n\nIf the endpoints you\'re going to hit require authentication, use `AuthenticatedClient` instead:\n\n```python\nfrom windmill_api import AuthenticatedClient\n\nclient = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = get_my_data_model.sync(client=client)\n# or if you need more info (e.g. status_code)\nresponse: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)\n```\n\nOr do the same thing with an async version:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = await get_my_data_model.asyncio(client=client)\nresponse: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)\n```\n\nBy default, when you\'re calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken",\n    verify_ssl="/path/to/certificate_bundle.pem",\n)\n```\n\nYou can also disable certificate validation altogether, but beware that **this is a security risk**.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken", \n    verify_ssl=False\n)\n```\n\nThings to know:\n1. Every path/method combo becomes a Python module with four functions:\n    1. `sync`: Blocking request that returns parsed data (if successful) or `None`\n    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.\n    1. `asyncio`: Like `sync` but async instead of blocking\n    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking\n\n1. All path/query params, and bodies become method arguments.\n1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)\n1. Any endpoint which did not have a tag will be in `windmill_api.api.default`\n\n',
     'author': 'Ruben Fiszel',
     'author_email': 'ruben@windmill.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `windmill_api-1.96.1/PKG-INFO` & `windmill_api-1.96.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windmill-api
-Version: 1.96.1
+Version: 1.96.2
 Summary: A client library for accessing Windmill API
 License: Apache-2.0
 Author: Ruben Fiszel
 Author-email: ruben@windmill.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

