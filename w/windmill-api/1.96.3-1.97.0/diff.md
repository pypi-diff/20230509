# Comparing `tmp/windmill_api-1.96.3.tar.gz` & `tmp/windmill_api-1.97.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windmill_api-1.96.3.tar", max compression
+gzip compressed data, was "windmill_api-1.97.0.tar", max compression
```

## Comparing `windmill_api-1.96.3.tar` & `windmill_api-1.97.0.tar`

### file list

```diff
@@ -1,1302 +1,1302 @@
--rw-r--r--   0        0        0    11348 2023-05-08 23:22:04.179093 windmill_api-1.96.3/LICENSE
--rw-r--r--   0        0        0     2952 2023-05-08 23:22:04.183093 windmill_api-1.96.3/README.md
--rw-r--r--   0        0        0      717 2023-05-08 23:22:04.183093 windmill_api-1.96.3/pyproject.toml
--rw-r--r--   0        0        0      100 2023-05-08 23:21:32.598631 windmill_api-1.96.3/windmill_api/__init__.py
--rw-r--r--   0        0        0       47 2023-05-08 23:21:33.090638 windmill_api-1.96.3/windmill_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.214640 windmill_api-1.96.3/windmill_api/api/app/__init__.py
--rw-r--r--   0        0        0     1999 2023-05-08 23:21:43.570794 windmill_api-1.96.3/windmill_api/api/app/create_app.py
--rw-r--r--   0        0        0     1769 2023-05-08 23:21:43.562794 windmill_api-1.96.3/windmill_api/api/app/delete_app.py
--rw-r--r--   0        0        0     2214 2023-05-08 23:21:43.594794 windmill_api-1.96.3/windmill_api/api/app/execute_component.py
--rw-r--r--   0        0        0     2782 2023-05-08 23:21:43.626795 windmill_api-1.96.3/windmill_api/api/app/exists_app.py
--rw-r--r--   0        0        0     3020 2023-05-08 23:21:43.630795 windmill_api-1.96.3/windmill_api/api/app/get_app_by_path.py
--rw-r--r--   0        0        0     3187 2023-05-08 23:21:43.666795 windmill_api-1.96.3/windmill_api/api/app/get_app_by_path_with_draft.py
--rw-r--r--   0        0        0     3031 2023-05-08 23:21:43.670795 windmill_api-1.96.3/windmill_api/api/app/get_app_by_version.py
--rw-r--r--   0        0        0     2649 2023-05-08 23:21:43.714796 windmill_api-1.96.3/windmill_api/api/app/get_hub_app_by_id.py
--rw-r--r--   0        0        0     3168 2023-05-08 23:21:43.718796 windmill_api-1.96.3/windmill_api/api/app/get_public_app_by_secret.py
--rw-r--r--   0        0        0     1797 2023-05-08 23:21:43.742796 windmill_api-1.96.3/windmill_api/api/app/get_public_secret_of_app.py
--rw-r--r--   0        0        0     7289 2023-05-08 23:21:43.810797 windmill_api-1.96.3/windmill_api/api/app/list_apps.py
--rw-r--r--   0        0        0     2405 2023-05-08 23:21:43.774797 windmill_api-1.96.3/windmill_api/api/app/list_hub_apps.py
--rw-r--r--   0        0        0     2140 2023-05-08 23:21:43.806797 windmill_api-1.96.3/windmill_api/api/app/update_app.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.130638 windmill_api-1.96.3/windmill_api/api/audit/__init__.py
--rw-r--r--   0        0        0     3065 2023-05-08 23:21:43.842798 windmill_api-1.96.3/windmill_api/api/audit/get_audit_log.py
--rw-r--r--   0        0        0     8723 2023-05-08 23:21:43.914799 windmill_api-1.96.3/windmill_api/api/audit/list_audit_logs.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.270641 windmill_api-1.96.3/windmill_api/api/capture/__init__.py
--rw-r--r--   0        0        0     1796 2023-05-08 23:21:43.870798 windmill_api-1.96.3/windmill_api/api/capture/create_capture.py
--rw-r--r--   0        0        0     1790 2023-05-08 23:21:43.898799 windmill_api-1.96.3/windmill_api/api/capture/get_capture.py
--rw-r--r--   0        0        0     1799 2023-05-08 23:21:43.930799 windmill_api-1.96.3/windmill_api/api/capture/update_capture.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.222640 windmill_api-1.96.3/windmill_api/api/draft/__init__.py
--rw-r--r--   0        0        0     2019 2023-05-08 23:21:43.938799 windmill_api-1.96.3/windmill_api/api/draft/create_draft.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.274641 windmill_api-1.96.3/windmill_api/api/favorite/__init__.py
--rw-r--r--   0        0        0     1964 2023-05-08 23:21:43.958799 windmill_api-1.96.3/windmill_api/api/favorite/star.py
--rw-r--r--   0        0        0     1984 2023-05-08 23:21:43.970800 windmill_api-1.96.3/windmill_api/api/favorite/unstar.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.186639 windmill_api-1.96.3/windmill_api/api/flow/__init__.py
--rw-r--r--   0        0        0     2220 2023-05-08 23:21:43.990800 windmill_api-1.96.3/windmill_api/api/flow/archive_flow_by_path.py
--rw-r--r--   0        0        0     2009 2023-05-08 23:21:43.998800 windmill_api-1.96.3/windmill_api/api/flow/create_flow.py
--rw-r--r--   0        0        0     1788 2023-05-08 23:21:44.018800 windmill_api-1.96.3/windmill_api/api/flow/delete_flow_by_path.py
--rw-r--r--   0        0        0     2755 2023-05-08 23:21:44.062801 windmill_api-1.96.3/windmill_api/api/flow/exists_flow_by_path.py
--rw-r--r--   0        0        0     3036 2023-05-08 23:21:44.066801 windmill_api-1.96.3/windmill_api/api/flow/get_flow_by_path.py
--rw-r--r--   0        0        0     3205 2023-05-08 23:21:44.106802 windmill_api-1.96.3/windmill_api/api/flow/get_flow_by_path_with_draft.py
--rw-r--r--   0        0        0     4827 2023-05-08 23:21:44.122802 windmill_api-1.96.3/windmill_api/api/flow/get_flow_input_history_by_path.py
--rw-r--r--   0        0        0     2667 2023-05-08 23:21:44.142802 windmill_api-1.96.3/windmill_api/api/flow/get_hub_flow_by_id.py
--rw-r--r--   0        0        0     1668 2023-05-08 23:21:44.150802 windmill_api-1.96.3/windmill_api/api/flow/list_flow_paths.py
--rw-r--r--   0        0        0     7969 2023-05-08 23:21:44.234804 windmill_api-1.96.3/windmill_api/api/flow/list_flows.py
--rw-r--r--   0        0        0     2423 2023-05-08 23:21:44.182803 windmill_api-1.96.3/windmill_api/api/flow/list_hub_flows.py
--rw-r--r--   0        0        0     2150 2023-05-08 23:21:44.210803 windmill_api-1.96.3/windmill_api/api/flow/update_flow.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.262641 windmill_api-1.96.3/windmill_api/api/folder/__init__.py
--rw-r--r--   0        0        0     2214 2023-05-08 23:21:44.246804 windmill_api-1.96.3/windmill_api/api/folder/add_owner_to_folder.py
--rw-r--r--   0        0        0     2029 2023-05-08 23:21:44.262804 windmill_api-1.96.3/windmill_api/api/folder/create_folder.py
--rw-r--r--   0        0        0     1778 2023-05-08 23:21:44.274804 windmill_api-1.96.3/windmill_api/api/folder/delete_folder.py
--rw-r--r--   0        0        0     2960 2023-05-08 23:21:44.298805 windmill_api-1.96.3/windmill_api/api/folder/get_folder.py
--rw-r--r--   0        0        0     3055 2023-05-08 23:21:44.314805 windmill_api-1.96.3/windmill_api/api/folder/get_folder_usage.py
--rw-r--r--   0        0        0     3405 2023-05-08 23:21:44.346805 windmill_api-1.96.3/windmill_api/api/folder/list_folder_names.py
--rw-r--r--   0        0        0     4251 2023-05-08 23:21:44.374806 windmill_api-1.96.3/windmill_api/api/folder/list_folders.py
--rw-r--r--   0        0        0     2244 2023-05-08 23:21:44.394806 windmill_api-1.96.3/windmill_api/api/folder/remove_owner_to_folder.py
--rw-r--r--   0        0        0     2170 2023-05-08 23:21:44.434807 windmill_api-1.96.3/windmill_api/api/folder/update_folder.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.270641 windmill_api-1.96.3/windmill_api/api/granular_acl/__init__.py
--rw-r--r--   0        0        0     2480 2023-05-08 23:21:44.426807 windmill_api-1.96.3/windmill_api/api/granular_acl/add_granular_acls.py
--rw-r--r--   0        0        0     3526 2023-05-08 23:21:44.470807 windmill_api-1.96.3/windmill_api/api/granular_acl/get_granular_acls.py
--rw-r--r--   0        0        0     2545 2023-05-08 23:21:44.466807 windmill_api-1.96.3/windmill_api/api/granular_acl/remove_granular_acls.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.258640 windmill_api-1.96.3/windmill_api/api/group/__init__.py
--rw-r--r--   0        0        0     2194 2023-05-08 23:21:44.502808 windmill_api-1.96.3/windmill_api/api/group/add_user_to_group.py
--rw-r--r--   0        0        0     2019 2023-05-08 23:21:44.494808 windmill_api-1.96.3/windmill_api/api/group/create_group.py
--rw-r--r--   0        0        0     1775 2023-05-08 23:21:44.522808 windmill_api-1.96.3/windmill_api/api/group/delete_group.py
--rw-r--r--   0        0        0     2942 2023-05-08 23:21:44.542808 windmill_api-1.96.3/windmill_api/api/group/get_group.py
--rw-r--r--   0        0        0     3400 2023-05-08 23:21:44.566809 windmill_api-1.96.3/windmill_api/api/group/list_group_names.py
--rw-r--r--   0        0        0     4233 2023-05-08 23:21:44.598809 windmill_api-1.96.3/windmill_api/api/group/list_groups.py
--rw-r--r--   0        0        0     2224 2023-05-08 23:21:44.594809 windmill_api-1.96.3/windmill_api/api/group/remove_user_to_group.py
--rw-r--r--   0        0        0     2160 2023-05-08 23:21:44.626809 windmill_api-1.96.3/windmill_api/api/group/update_group.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.274641 windmill_api-1.96.3/windmill_api/api/input_/__init__.py
--rw-r--r--   0        0        0     3338 2023-05-08 23:21:44.642810 windmill_api-1.96.3/windmill_api/api/input_/create_input.py
--rw-r--r--   0        0        0     1811 2023-05-08 23:21:44.650810 windmill_api-1.96.3/windmill_api/api/input_/delete_input.py
--rw-r--r--   0        0        0     6187 2023-05-08 23:21:44.714811 windmill_api-1.96.3/windmill_api/api/input_/get_input_history.py
--rw-r--r--   0        0        0     6010 2023-05-08 23:21:44.734811 windmill_api-1.96.3/windmill_api/api/input_/list_inputs.py
--rw-r--r--   0        0        0     2025 2023-05-08 23:21:44.766811 windmill_api-1.96.3/windmill_api/api/input_/update_input.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.226640 windmill_api-1.96.3/windmill_api/api/job/__init__.py
--rw-r--r--   0        0        0     2181 2023-05-08 23:21:44.766811 windmill_api-1.96.3/windmill_api/api/job/cancel_queued_job.py
--rw-r--r--   0        0        0     2687 2023-05-08 23:21:44.798812 windmill_api-1.96.3/windmill_api/api/job/cancel_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-05-08 23:21:44.810812 windmill_api-1.96.3/windmill_api/api/job/cancel_suspended_job_post.py
--rw-r--r--   0        0        0     2535 2023-05-08 23:21:44.834812 windmill_api-1.96.3/windmill_api/api/job/create_job_signature.py
--rw-r--r--   0        0        0     3217 2023-05-08 23:21:44.850813 windmill_api-1.96.3/windmill_api/api/job/delete_completed_job.py
--rw-r--r--   0        0        0     2235 2023-05-08 23:21:44.862813 windmill_api-1.96.3/windmill_api/api/job/force_cancel_queued_job.py
--rw-r--r--   0        0        0     3034 2023-05-08 23:21:44.890813 windmill_api-1.96.3/windmill_api/api/job/get_completed_job.py
--rw-r--r--   0        0        0     1784 2023-05-08 23:21:44.890813 windmill_api-1.96.3/windmill_api/api/job/get_completed_job_result.py
--rw-r--r--   0        0        0     2868 2023-05-08 23:21:44.930814 windmill_api-1.96.3/windmill_api/api/job/get_job.py
--rw-r--r--   0        0        0     4305 2023-05-08 23:21:44.942814 windmill_api-1.96.3/windmill_api/api/job/get_job_updates.py
--rw-r--r--   0        0        0     4306 2023-05-08 23:21:44.982815 windmill_api-1.96.3/windmill_api/api/job/get_resume_urls.py
--rw-r--r--   0        0        0     4601 2023-05-08 23:21:44.998815 windmill_api-1.96.3/windmill_api/api/job/get_suspended_job_flow.py
--rw-r--r--   0        0        0    13065 2023-05-08 23:21:45.146817 windmill_api-1.96.3/windmill_api/api/job/list_completed_jobs.py
--rw-r--r--   0        0        0    12292 2023-05-08 23:21:45.150817 windmill_api-1.96.3/windmill_api/api/job/list_jobs.py
--rw-r--r--   0        0        0    12830 2023-05-08 23:21:45.290819 windmill_api-1.96.3/windmill_api/api/job/list_queue.py
--rw-r--r--   0        0        0     2067 2023-05-08 23:21:45.182818 windmill_api-1.96.3/windmill_api/api/job/result_by_id.py
--rw-r--r--   0        0        0     2313 2023-05-08 23:21:45.210818 windmill_api-1.96.3/windmill_api/api/job/resume_suspended_flow_as_owner.py
--rw-r--r--   0        0        0     2994 2023-05-08 23:21:45.254819 windmill_api-1.96.3/windmill_api/api/job/resume_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-05-08 23:21:45.294819 windmill_api-1.96.3/windmill_api/api/job/resume_suspended_job_post.py
--rw-r--r--   0        0        0     4566 2023-05-08 23:21:45.350820 windmill_api-1.96.3/windmill_api/api/job/run_flow_by_path.py
--rw-r--r--   0        0        0     3037 2023-05-08 23:21:45.330820 windmill_api-1.96.3/windmill_api/api/job/run_flow_preview.py
--rw-r--r--   0        0        0     4594 2023-05-08 23:21:45.390821 windmill_api-1.96.3/windmill_api/api/job/run_script_by_hash.py
--rw-r--r--   0        0        0     4200 2023-05-08 23:21:45.434821 windmill_api-1.96.3/windmill_api/api/job/run_script_by_path.py
--rw-r--r--   0        0        0     3050 2023-05-08 23:21:45.426821 windmill_api-1.96.3/windmill_api/api/job/run_script_preview.py
--rw-r--r--   0        0        0     3215 2023-05-08 23:21:45.490822 windmill_api-1.96.3/windmill_api/api/job/run_wait_result_flow_by_path.py
--rw-r--r--   0        0        0     3521 2023-05-08 23:21:45.478822 windmill_api-1.96.3/windmill_api/api/job/run_wait_result_script_by_path.py
--rw-r--r--   0        0        0     3356 2023-05-08 23:21:45.526823 windmill_api-1.96.3/windmill_api/api/job/run_wait_result_script_by_path_get.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.158639 windmill_api-1.96.3/windmill_api/api/oauth/__init__.py
--rw-r--r--   0        0        0     3506 2023-05-08 23:21:45.542823 windmill_api-1.96.3/windmill_api/api/oauth/connect_callback.py
--rw-r--r--   0        0        0     2118 2023-05-08 23:21:45.554823 windmill_api-1.96.3/windmill_api/api/oauth/connect_slack_callback.py
--rw-r--r--   0        0        0     2056 2023-05-08 23:21:45.570824 windmill_api-1.96.3/windmill_api/api/oauth/create_account.py
--rw-r--r--   0        0        0     1764 2023-05-08 23:21:45.582824 windmill_api-1.96.3/windmill_api/api/oauth/disconnect_account.py
--rw-r--r--   0        0        0     1649 2023-05-08 23:21:45.598824 windmill_api-1.96.3/windmill_api/api/oauth/disconnect_slack.py
--rw-r--r--   0        0        0     1426 2023-05-08 23:21:45.602824 windmill_api-1.96.3/windmill_api/api/oauth/list_o_auth_connects.py
--rw-r--r--   0        0        0     2162 2023-05-08 23:21:45.630824 windmill_api-1.96.3/windmill_api/api/oauth/list_o_auth_logins.py
--rw-r--r--   0        0        0     2151 2023-05-08 23:21:45.630824 windmill_api-1.96.3/windmill_api/api/oauth/refresh_token.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.250640 windmill_api-1.96.3/windmill_api/api/raw_app/__init__.py
--rw-r--r--   0        0        0     2033 2023-05-08 23:21:45.658825 windmill_api-1.96.3/windmill_api/api/raw_app/create_raw_app.py
--rw-r--r--   0        0        0     1781 2023-05-08 23:21:45.662825 windmill_api-1.96.3/windmill_api/api/raw_app/delete_raw_app.py
--rw-r--r--   0        0        0     2786 2023-05-08 23:21:45.698825 windmill_api-1.96.3/windmill_api/api/raw_app/exists_raw_app.py
--rw-r--r--   0        0        0     1979 2023-05-08 23:21:45.694825 windmill_api-1.96.3/windmill_api/api/raw_app/get_raw_app_data.py
--rw-r--r--   0        0        0     7349 2023-05-08 23:21:45.778827 windmill_api-1.96.3/windmill_api/api/raw_app/list_raw_apps.py
--rw-r--r--   0        0        0     2166 2023-05-08 23:21:45.726826 windmill_api-1.96.3/windmill_api/api/raw_app/update_raw_app.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.162639 windmill_api-1.96.3/windmill_api/api/resource/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-08 23:21:45.782827 windmill_api-1.96.3/windmill_api/api/resource/create_resource.py
--rw-r--r--   0        0        0     2093 2023-05-08 23:21:45.830827 windmill_api-1.96.3/windmill_api/api/resource/create_resource_type.py
--rw-r--r--   0        0        0     1784 2023-05-08 23:21:45.810827 windmill_api-1.96.3/windmill_api/api/resource/delete_resource.py
--rw-r--r--   0        0        0     1799 2023-05-08 23:21:45.834827 windmill_api-1.96.3/windmill_api/api/resource/delete_resource_type.py
--rw-r--r--   0        0        0     2763 2023-05-08 23:21:45.870828 windmill_api-1.96.3/windmill_api/api/resource/exists_resource.py
--rw-r--r--   0        0        0     2788 2023-05-08 23:21:45.870828 windmill_api-1.96.3/windmill_api/api/resource/exists_resource_type.py
--rw-r--r--   0        0        0     2996 2023-05-08 23:21:45.910828 windmill_api-1.96.3/windmill_api/api/resource/get_resource.py
--rw-r--r--   0        0        0     3074 2023-05-08 23:21:45.910828 windmill_api-1.96.3/windmill_api/api/resource/get_resource_type.py
--rw-r--r--   0        0        0     1790 2023-05-08 23:21:45.934829 windmill_api-1.96.3/windmill_api/api/resource/get_resource_value.py
--rw-r--r--   0        0        0     5732 2023-05-08 23:21:45.974829 windmill_api-1.96.3/windmill_api/api/resource/list_resource.py
--rw-r--r--   0        0        0     3149 2023-05-08 23:21:45.974829 windmill_api-1.96.3/windmill_api/api/resource/list_resource_type.py
--rw-r--r--   0        0        0     2600 2023-05-08 23:21:46.010830 windmill_api-1.96.3/windmill_api/api/resource/list_resource_type_names.py
--rw-r--r--   0        0        0     2190 2023-05-08 23:21:46.006830 windmill_api-1.96.3/windmill_api/api/resource/update_resource.py
--rw-r--r--   0        0        0     2234 2023-05-08 23:21:46.034830 windmill_api-1.96.3/windmill_api/api/resource/update_resource_type.py
--rw-r--r--   0        0        0     2244 2023-05-08 23:21:46.042830 windmill_api-1.96.3/windmill_api/api/resource/update_resource_value.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.254640 windmill_api-1.96.3/windmill_api/api/schedule/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-08 23:21:46.066831 windmill_api-1.96.3/windmill_api/api/schedule/create_schedule.py
--rw-r--r--   0        0        0     1784 2023-05-08 23:21:46.066831 windmill_api-1.96.3/windmill_api/api/schedule/delete_schedule.py
--rw-r--r--   0        0        0     2763 2023-05-08 23:21:46.122832 windmill_api-1.96.3/windmill_api/api/schedule/exists_schedule.py
--rw-r--r--   0        0        0     2996 2023-05-08 23:21:46.106831 windmill_api-1.96.3/windmill_api/api/schedule/get_schedule.py
--rw-r--r--   0        0        0     4287 2023-05-08 23:21:46.178832 windmill_api-1.96.3/windmill_api/api/schedule/list_schedules.py
--rw-r--r--   0        0        0     3217 2023-05-08 23:21:46.158832 windmill_api-1.96.3/windmill_api/api/schedule/preview_schedule.py
--rw-r--r--   0        0        0     2233 2023-05-08 23:21:46.194833 windmill_api-1.96.3/windmill_api/api/schedule/set_schedule_enabled.py
--rw-r--r--   0        0        0     2190 2023-05-08 23:21:46.210833 windmill_api-1.96.3/windmill_api/api/schedule/update_schedule.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.174639 windmill_api-1.96.3/windmill_api/api/script/__init__.py
--rw-r--r--   0        0        0     3165 2023-05-08 23:21:46.234833 windmill_api-1.96.3/windmill_api/api/script/archive_script_by_hash.py
--rw-r--r--   0        0        0     1797 2023-05-08 23:21:46.238833 windmill_api-1.96.3/windmill_api/api/script/archive_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-05-08 23:21:46.266834 windmill_api-1.96.3/windmill_api/api/script/bash_to_jsonschema.py
--rw-r--r--   0        0        0     2029 2023-05-08 23:21:46.266834 windmill_api-1.96.3/windmill_api/api/script/create_script.py
--rw-r--r--   0        0        0     3327 2023-05-08 23:21:46.306834 windmill_api-1.96.3/windmill_api/api/script/delete_script_by_hash.py
--rw-r--r--   0        0        0     2873 2023-05-08 23:21:46.306834 windmill_api-1.96.3/windmill_api/api/script/delete_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-05-08 23:21:46.338835 windmill_api-1.96.3/windmill_api/api/script/deno_to_jsonschema.py
--rw-r--r--   0        0        0     2767 2023-05-08 23:21:46.346835 windmill_api-1.96.3/windmill_api/api/script/exists_script_by_path.py
--rw-r--r--   0        0        0     2802 2023-05-08 23:21:46.378835 windmill_api-1.96.3/windmill_api/api/script/get_hub_script_by_path.py
--rw-r--r--   0        0        0     1607 2023-05-08 23:21:46.370835 windmill_api-1.96.3/windmill_api/api/script/get_hub_script_content_by_path.py
--rw-r--r--   0        0        0     3092 2023-05-08 23:21:46.410836 windmill_api-1.96.3/windmill_api/api/script/get_script_by_hash.py
--rw-r--r--   0        0        0     3074 2023-05-08 23:21:46.414836 windmill_api-1.96.3/windmill_api/api/script/get_script_by_path.py
--rw-r--r--   0        0        0     3241 2023-05-08 23:21:46.466837 windmill_api-1.96.3/windmill_api/api/script/get_script_by_path_with_draft.py
--rw-r--r--   0        0        0     3276 2023-05-08 23:21:46.470837 windmill_api-1.96.3/windmill_api/api/script/get_script_deployment_status.py
--rw-r--r--   0        0        0     2967 2023-05-08 23:21:46.502837 windmill_api-1.96.3/windmill_api/api/script/go_to_jsonschema.py
--rw-r--r--   0        0        0     2459 2023-05-08 23:21:46.502837 windmill_api-1.96.3/windmill_api/api/script/list_hub_scripts.py
--rw-r--r--   0        0        0     1676 2023-05-08 23:21:46.526838 windmill_api-1.96.3/windmill_api/api/script/list_script_paths.py
--rw-r--r--   0        0        0    11165 2023-05-08 23:21:46.630839 windmill_api-1.96.3/windmill_api/api/script/list_scripts.py
--rw-r--r--   0        0        0     3039 2023-05-08 23:21:46.562838 windmill_api-1.96.3/windmill_api/api/script/python_to_jsonschema.py
--rw-r--r--   0        0        0     1784 2023-05-08 23:21:46.586839 windmill_api-1.96.3/windmill_api/api/script/raw_script_by_hash.py
--rw-r--r--   0        0        0     1784 2023-05-08 23:21:46.614839 windmill_api-1.96.3/windmill_api/api/script/raw_script_by_path.py
--rw-r--r--   0        0        0     2119 2023-05-08 23:21:46.642839 windmill_api-1.96.3/windmill_api/api/script/raw_script_by_path_tokened.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.102638 windmill_api-1.96.3/windmill_api/api/settings/__init__.py
--rw-r--r--   0        0        0     1414 2023-05-08 23:21:46.670840 windmill_api-1.96.3/windmill_api/api/settings/backend_version.py
--rw-r--r--   0        0        0     1423 2023-05-08 23:21:46.662840 windmill_api-1.96.3/windmill_api/api/settings/get_open_api_yaml.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.130638 windmill_api-1.96.3/windmill_api/api/user/__init__.py
--rw-r--r--   0        0        0     1857 2023-05-08 23:21:46.690840 windmill_api-1.96.3/windmill_api/api/user/accept_invite.py
--rw-r--r--   0        0        0     1822 2023-05-08 23:21:46.694840 windmill_api-1.96.3/windmill_api/api/user/create_token.py
--rw-r--r--   0        0        0     1991 2023-05-08 23:21:46.714840 windmill_api-1.96.3/windmill_api/api/user/create_token_impersonate.py
--rw-r--r--   0        0        0     2058 2023-05-08 23:21:46.726841 windmill_api-1.96.3/windmill_api/api/user/create_user.py
--rw-r--r--   0        0        0     1863 2023-05-08 23:21:46.754841 windmill_api-1.96.3/windmill_api/api/user/create_user_globally.py
--rw-r--r--   0        0        0     1867 2023-05-08 23:21:46.750841 windmill_api-1.96.3/windmill_api/api/user/decline_invite.py
--rw-r--r--   0        0        0     1674 2023-05-08 23:21:46.778841 windmill_api-1.96.3/windmill_api/api/user/delete_token.py
--rw-r--r--   0        0        0     1872 2023-05-08 23:21:46.782841 windmill_api-1.96.3/windmill_api/api/user/delete_user.py
--rw-r--r--   0        0        0     1454 2023-05-08 23:21:46.802842 windmill_api-1.96.3/windmill_api/api/user/get_current_email.py
--rw-r--r--   0        0        0     1474 2023-05-08 23:21:46.802842 windmill_api-1.96.3/windmill_api/api/user/get_usage.py
--rw-r--r--   0        0        0     1639 2023-05-08 23:21:46.850842 windmill_api-1.96.3/windmill_api/api/user/global_user_delete.py
--rw-r--r--   0        0        0     2060 2023-05-08 23:21:46.830842 windmill_api-1.96.3/windmill_api/api/user/global_user_update.py
--rw-r--r--   0        0        0     2468 2023-05-08 23:21:46.862843 windmill_api-1.96.3/windmill_api/api/user/global_whoami.py
--rw-r--r--   0        0        0     2745 2023-05-08 23:21:46.890843 windmill_api-1.96.3/windmill_api/api/user/is_owner_of_path.py
--rw-r--r--   0        0        0     1646 2023-05-08 23:21:46.886843 windmill_api-1.96.3/windmill_api/api/user/leave_workspace.py
--rw-r--r--   0        0        0     2633 2023-05-08 23:21:46.922844 windmill_api-1.96.3/windmill_api/api/user/list_tokens.py
--rw-r--r--   0        0        0     2552 2023-05-08 23:21:46.930843 windmill_api-1.96.3/windmill_api/api/user/list_usernames.py
--rw-r--r--   0        0        0     3012 2023-05-08 23:21:46.958844 windmill_api-1.96.3/windmill_api/api/user/list_users.py
--rw-r--r--   0        0        0     4222 2023-05-08 23:21:46.982844 windmill_api-1.96.3/windmill_api/api/user/list_users_as_super_admin.py
--rw-r--r--   0        0        0     2829 2023-05-08 23:21:46.994845 windmill_api-1.96.3/windmill_api/api/user/list_workspace_invites.py
--rw-r--r--   0        0        0     1784 2023-05-08 23:21:47.010845 windmill_api-1.96.3/windmill_api/api/user/login.py
--rw-r--r--   0        0        0     2116 2023-05-08 23:21:47.022845 windmill_api-1.96.3/windmill_api/api/user/login_with_oauth.py
--rw-r--r--   0        0        0     1393 2023-05-08 23:21:47.034845 windmill_api-1.96.3/windmill_api/api/user/logout.py
--rw-r--r--   0        0        0     1820 2023-05-08 23:21:47.046845 windmill_api-1.96.3/windmill_api/api/user/set_password.py
--rw-r--r--   0        0        0     2250 2023-05-08 23:21:47.066846 windmill_api-1.96.3/windmill_api/api/user/update_user.py
--rw-r--r--   0        0        0     2652 2023-05-08 23:21:47.098846 windmill_api-1.96.3/windmill_api/api/user/whoami.py
--rw-r--r--   0        0        0     2967 2023-05-08 23:21:47.102846 windmill_api-1.96.3/windmill_api/api/user/whois.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.154639 windmill_api-1.96.3/windmill_api/api/variable/__init__.py
--rw-r--r--   0        0        0     2634 2023-05-08 23:21:47.138847 windmill_api-1.96.3/windmill_api/api/variable/create_variable.py
--rw-r--r--   0        0        0     1784 2023-05-08 23:21:47.130847 windmill_api-1.96.3/windmill_api/api/variable/delete_variable.py
--rw-r--r--   0        0        0     2795 2023-05-08 23:21:47.182847 windmill_api-1.96.3/windmill_api/api/variable/exists_variable.py
--rw-r--r--   0        0        0     3840 2023-05-08 23:21:47.186847 windmill_api-1.96.3/windmill_api/api/variable/get_variable.py
--rw-r--r--   0        0        0     3270 2023-05-08 23:21:47.222848 windmill_api-1.96.3/windmill_api/api/variable/list_contextual_variables.py
--rw-r--r--   0        0        0     3071 2023-05-08 23:21:47.226848 windmill_api-1.96.3/windmill_api/api/variable/list_variable.py
--rw-r--r--   0        0        0     2775 2023-05-08 23:21:47.258849 windmill_api-1.96.3/windmill_api/api/variable/update_variable.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.222640 windmill_api-1.96.3/windmill_api/api/worker/__init__.py
--rw-r--r--   0        0        0     2448 2023-05-08 23:21:47.262848 windmill_api-1.96.3/windmill_api/api/worker/get_custom_tags.py
--rw-r--r--   0        0        0     3896 2023-05-08 23:21:47.310849 windmill_api-1.96.3/windmill_api/api/worker/list_workers.py
--rw-r--r--   0        0        0        0 2023-05-08 23:21:33.146639 windmill_api-1.96.3/windmill_api/api/workspace/__init__.py
--rw-r--r--   0        0        0     2015 2023-05-08 23:21:47.294849 windmill_api-1.96.3/windmill_api/api/workspace/add_user.py
--rw-r--r--   0        0        0     1647 2023-05-08 23:21:47.318849 windmill_api-1.96.3/windmill_api/api/workspace/archive_workspace.py
--rw-r--r--   0        0        0     1856 2023-05-08 23:21:47.334849 windmill_api-1.96.3/windmill_api/api/workspace/create_workspace.py
--rw-r--r--   0        0        0     2049 2023-05-08 23:21:47.350850 windmill_api-1.96.3/windmill_api/api/workspace/delete_invite.py
--rw-r--r--   0        0        0     1688 2023-05-08 23:21:47.358850 windmill_api-1.96.3/windmill_api/api/workspace/delete_workspace.py
--rw-r--r--   0        0        0     2063 2023-05-08 23:21:47.378850 windmill_api-1.96.3/windmill_api/api/workspace/edit_auto_invite.py
--rw-r--r--   0        0        0     2083 2023-05-08 23:21:47.386850 windmill_api-1.96.3/windmill_api/api/workspace/edit_slack_command.py
--rw-r--r--   0        0        0     2029 2023-05-08 23:21:47.422851 windmill_api-1.96.3/windmill_api/api/workspace/edit_webhook.py
--rw-r--r--   0        0        0     1856 2023-05-08 23:21:47.410851 windmill_api-1.96.3/windmill_api/api/workspace/exists_username.py
--rw-r--r--   0        0        0     1856 2023-05-08 23:21:47.438851 windmill_api-1.96.3/windmill_api/api/workspace/exists_workspace.py
--rw-r--r--   0        0        0     2809 2023-05-08 23:21:47.462851 windmill_api-1.96.3/windmill_api/api/workspace/get_premium_info.py
--rw-r--r--   0        0        0     2753 2023-05-08 23:21:47.474852 windmill_api-1.96.3/windmill_api/api/workspace/get_settings.py
--rw-r--r--   0        0        0     2045 2023-05-08 23:21:47.490852 windmill_api-1.96.3/windmill_api/api/workspace/invite_user.py
--rw-r--r--   0        0        0     2176 2023-05-08 23:21:47.518852 windmill_api-1.96.3/windmill_api/api/workspace/is_domain_allowed.py
--rw-r--r--   0        0        0     3255 2023-05-08 23:21:47.530852 windmill_api-1.96.3/windmill_api/api/workspace/list_pending_invites.py
--rw-r--r--   0        0        0     2583 2023-05-08 23:21:47.550853 windmill_api-1.96.3/windmill_api/api/workspace/list_user_workspaces.py
--rw-r--r--   0        0        0     2775 2023-05-08 23:21:47.566853 windmill_api-1.96.3/windmill_api/api/workspace/list_workspaces.py
--rw-r--r--   0        0        0     4311 2023-05-08 23:21:47.602854 windmill_api-1.96.3/windmill_api/api/workspace/list_workspaces_as_super_admin.py
--rw-r--r--   0        0        0     1651 2023-05-08 23:21:47.590853 windmill_api-1.96.3/windmill_api/api/workspace/unarchive_workspace.py
--rw-r--r--   0        0        0     1821 2023-05-08 23:21:47.618854 windmill_api-1.96.3/windmill_api/client.py
--rw-r--r--   0        0        0        1 2023-05-08 23:22:04.171093 windmill_api-1.96.3/windmill_api/models/__init__.py
--rw-r--r--   0        0        0     1667 2023-05-08 23:21:47.642854 windmill_api-1.96.3/windmill_api/models/accept_invite_json_body.py
--rw-r--r--   0        0        0     1710 2023-05-08 23:21:47.670854 windmill_api-1.96.3/windmill_api/models/add_granular_acls_json_body.py
--rw-r--r--   0        0        0      325 2023-05-08 23:21:42.142773 windmill_api-1.96.3/windmill_api/models/add_granular_acls_kind.py
--rw-r--r--   0        0        0     1529 2023-05-08 23:21:47.698855 windmill_api-1.96.3/windmill_api/models/add_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1940 2023-05-08 23:21:47.738855 windmill_api-1.96.3/windmill_api/models/add_user_json_body.py
--rw-r--r--   0        0        0     1552 2023-05-08 23:21:47.738855 windmill_api-1.96.3/windmill_api/models/add_user_to_group_json_body.py
--rw-r--r--   0        0        0     3940 2023-05-08 23:21:47.802857 windmill_api-1.96.3/windmill_api/models/app_with_last_version.py
--rw-r--r--   0        0        0      214 2023-05-08 23:21:42.642780 windmill_api-1.96.3/windmill_api/models/app_with_last_version_execution_mode.py
--rw-r--r--   0        0        0     1248 2023-05-08 23:21:47.762856 windmill_api-1.96.3/windmill_api/models/app_with_last_version_extra_perms.py
--rw-r--r--   0        0        0     3716 2023-05-08 23:21:47.834857 windmill_api-1.96.3/windmill_api/models/app_with_last_version_policy.py
--rw-r--r--   0        0        0      220 2023-05-08 23:21:42.690781 windmill_api-1.96.3/windmill_api/models/app_with_last_version_policy_execution_mode.py
--rw-r--r--   0        0        0     1946 2023-05-08 23:21:47.826857 windmill_api-1.96.3/windmill_api/models/app_with_last_version_policy_triggerables.py
--rw-r--r--   0        0        0     1381 2023-05-08 23:21:47.846857 windmill_api-1.96.3/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4638 2023-05-08 23:21:47.894858 windmill_api-1.96.3/windmill_api/models/app_with_last_version_w_draft.py
--rw-r--r--   0        0        0      220 2023-05-08 23:21:42.706781 windmill_api-1.96.3/windmill_api/models/app_with_last_version_w_draft_execution_mode.py
--rw-r--r--   0        0        0     1284 2023-05-08 23:21:47.870858 windmill_api-1.96.3/windmill_api/models/app_with_last_version_w_draft_extra_perms.py
--rw-r--r--   0        0        0     3828 2023-05-08 23:21:47.914858 windmill_api-1.96.3/windmill_api/models/app_with_last_version_w_draft_policy.py
--rw-r--r--   0        0        0      226 2023-05-08 23:21:42.250774 windmill_api-1.96.3/windmill_api/models/app_with_last_version_w_draft_policy_execution_mode.py
--rw-r--r--   0        0        0     2020 2023-05-08 23:21:47.918858 windmill_api-1.96.3/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py
--rw-r--r--   0        0        0     1417 2023-05-08 23:21:47.930858 windmill_api-1.96.3/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     1569 2023-05-08 23:21:47.946859 windmill_api-1.96.3/windmill_api/models/archive_flow_by_path_json_body.py
--rw-r--r--   0        0        0     7662 2023-05-08 23:21:48.022860 windmill_api-1.96.3/windmill_api/models/archive_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1314 2023-05-08 23:21:47.966859 windmill_api-1.96.3/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      259 2023-05-08 23:21:42.922784 windmill_api-1.96.3/windmill_api/models/archive_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      217 2023-05-08 23:21:42.610780 windmill_api-1.96.3/windmill_api/models/archive_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1288 2023-05-08 23:21:47.990859 windmill_api-1.96.3/windmill_api/models/archive_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     3452 2023-05-08 23:21:48.038860 windmill_api-1.96.3/windmill_api/models/audit_log.py
--rw-r--r--   0        0        0      217 2023-05-08 23:21:42.678781 windmill_api-1.96.3/windmill_api/models/audit_log_action_kind.py
--rw-r--r--   0        0        0      620 2023-05-08 23:21:42.566779 windmill_api-1.96.3/windmill_api/models/audit_log_operation.py
--rw-r--r--   0        0        0     1186 2023-05-08 23:21:48.042860 windmill_api-1.96.3/windmill_api/models/audit_log_parameters.py
--rw-r--r--   0        0        0     2933 2023-05-08 23:21:48.078861 windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-05-08 23:21:48.098861 windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-05-08 23:21:42.586779 windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-05-08 23:21:48.106861 windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-05-08 23:21:48.142861 windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-05-08 23:21:48.134861 windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-05-08 23:21:48.190862 windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-05-08 23:21:42.750782 windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-05-08 23:21:48.166862 windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-05-08 23:21:48.202862 windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-05-08 23:21:42.690781 windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-05-08 23:21:48.218863 windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-05-08 23:21:41.986770 windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2377 2023-05-08 23:21:48.234863 windmill_api-1.96.3/windmill_api/models/branch_all.py
--rw-r--r--   0        0        0     2543 2023-05-08 23:21:48.254863 windmill_api-1.96.3/windmill_api/models/branch_all_branches_item.py
--rw-r--r--   0        0        0     6620 2023-05-08 23:21:48.310864 windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-05-08 23:21:48.290864 windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-05-08 23:21:48.318864 windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-08 23:21:48.342864 windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-08 23:21:48.346865 windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-08 23:21:42.658780 windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-08 23:21:48.374865 windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-08 23:21:42.262774 windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-08 23:21:48.378865 windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-08 23:21:48.398865 windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      146 2023-05-08 23:21:42.186773 windmill_api-1.96.3/windmill_api/models/branch_all_type.py
--rw-r--r--   0        0        0     2670 2023-05-08 23:21:48.418866 windmill_api-1.96.3/windmill_api/models/branch_one.py
--rw-r--r--   0        0        0     2372 2023-05-08 23:21:48.434866 windmill_api-1.96.3/windmill_api/models/branch_one_branches_item.py
--rw-r--r--   0        0        0     6620 2023-05-08 23:21:48.498867 windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-05-08 23:21:48.490867 windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-05-08 23:21:48.518867 windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-08 23:21:48.530867 windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-08 23:21:48.546867 windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-08 23:21:42.574779 windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-08 23:21:48.578868 windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-08 23:21:42.126772 windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-08 23:21:48.574868 windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-08 23:21:48.602868 windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6125 2023-05-08 23:21:48.654869 windmill_api-1.96.3/windmill_api/models/branch_one_default_item.py
--rw-r--r--   0        0        0     2906 2023-05-08 23:21:48.642869 windmill_api-1.96.3/windmill_api/models/branch_one_default_item_retry.py
--rw-r--r--   0        0        0     1863 2023-05-08 23:21:48.678869 windmill_api-1.96.3/windmill_api/models/branch_one_default_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-05-08 23:21:48.682870 windmill_api-1.96.3/windmill_api/models/branch_one_default_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-05-08 23:21:48.710870 windmill_api-1.96.3/windmill_api/models/branch_one_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-05-08 23:21:42.258774 windmill_api-1.96.3/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-05-08 23:21:48.710870 windmill_api-1.96.3/windmill_api/models/branch_one_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-05-08 23:21:42.834783 windmill_api-1.96.3/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-05-08 23:21:48.738870 windmill_api-1.96.3/windmill_api/models/branch_one_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-05-08 23:21:48.742870 windmill_api-1.96.3/windmill_api/models/branch_one_default_item_suspend.py
--rw-r--r--   0        0        0      146 2023-05-08 23:21:42.666780 windmill_api-1.96.3/windmill_api/models/branch_one_type.py
--rw-r--r--   0        0        0     1532 2023-05-08 23:21:48.762871 windmill_api-1.96.3/windmill_api/models/cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     1255 2023-05-08 23:21:48.766871 windmill_api-1.96.3/windmill_api/models/cancel_suspended_job_post_json_body.py
--rw-r--r--   0        0        0    10508 2023-05-08 23:21:48.918873 windmill_api-1.96.3/windmill_api/models/completed_job.py
--rw-r--r--   0        0        0     1176 2023-05-08 23:21:48.786871 windmill_api-1.96.3/windmill_api/models/completed_job_args.py
--rw-r--r--   0        0        0     3265 2023-05-08 23:21:48.826872 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status.py
--rw-r--r--   0        0        0     6800 2023-05-08 23:21:48.930873 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1789 2023-05-08 23:21:48.942873 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2136 2023-05-08 23:21:48.958874 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      202 2023-05-08 23:21:42.850783 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1694 2023-05-08 23:21:48.970874 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2230 2023-05-08 23:21:48.998874 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      360 2023-05-08 23:21:42.106772 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6402 2023-05-08 23:21:49.046875 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1779 2023-05-08 23:21:49.022874 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2116 2023-05-08 23:21:49.054875 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      200 2023-05-08 23:21:41.870769 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1684 2023-05-08 23:21:49.074875 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2220 2023-05-08 23:21:49.090875 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      358 2023-05-08 23:21:42.922784 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2040 2023-05-08 23:21:49.106876 windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_retry.py
--rw-r--r--   0        0        0      310 2023-05-08 23:21:42.342776 windmill_api-1.96.3/windmill_api/models/completed_job_job_kind.py
--rw-r--r--   0        0        0      199 2023-05-08 23:21:41.858768 windmill_api-1.96.3/windmill_api/models/completed_job_language.py
--rw-r--r--   0        0        0     3127 2023-05-08 23:21:49.138876 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow.py
--rw-r--r--   0        0        0     6620 2023-05-08 23:21:49.182877 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3129 2023-05-08 23:21:49.174877 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1929 2023-05-08 23:21:49.202877 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-05-08 23:21:49.214877 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-05-08 23:21:49.258878 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-08 23:21:42.434777 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-05-08 23:21:49.242878 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-08 23:21:42.430777 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-05-08 23:21:49.310879 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-05-08 23:21:49.286878 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6544 2023-05-08 23:21:49.366880 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3095 2023-05-08 23:21:49.350880 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1919 2023-05-08 23:21:49.378880 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2223 2023-05-08 23:21:49.398880 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2050 2023-05-08 23:21:49.402880 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      179 2023-05-08 23:21:42.230774 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1917 2023-05-08 23:21:49.426880 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      179 2023-05-08 23:21:42.266775 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1912 2023-05-08 23:21:49.430881 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1963 2023-05-08 23:21:49.458881 windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1572 2023-05-08 23:21:49.454881 windmill_api-1.96.3/windmill_api/models/connect_callback_json_body.py
--rw-r--r--   0        0        0     2533 2023-05-08 23:21:49.490882 windmill_api-1.96.3/windmill_api/models/connect_callback_response_200.py
--rw-r--r--   0        0        0     1600 2023-05-08 23:21:49.482881 windmill_api-1.96.3/windmill_api/models/connect_slack_callback_json_body.py
--rw-r--r--   0        0        0     1753 2023-05-08 23:21:49.510882 windmill_api-1.96.3/windmill_api/models/contextual_variable.py
--rw-r--r--   0        0        0     2147 2023-05-08 23:21:49.522882 windmill_api-1.96.3/windmill_api/models/create_account_json_body.py
--rw-r--r--   0        0        0     2367 2023-05-08 23:21:49.546882 windmill_api-1.96.3/windmill_api/models/create_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-05-08 23:21:49.566883 windmill_api-1.96.3/windmill_api/models/create_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-05-08 23:21:42.930784 windmill_api-1.96.3/windmill_api/models/create_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-05-08 23:21:49.574883 windmill_api-1.96.3/windmill_api/models/create_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-05-08 23:21:49.586883 windmill_api-1.96.3/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     1947 2023-05-08 23:21:49.622883 windmill_api-1.96.3/windmill_api/models/create_draft_json_body.py
--rw-r--r--   0        0        0      183 2023-05-08 23:21:42.386776 windmill_api-1.96.3/windmill_api/models/create_draft_json_body_typ.py
--rw-r--r--   0        0        0     1550 2023-05-08 23:21:49.610883 windmill_api-1.96.3/windmill_api/models/create_flow_json_body.py
--rw-r--r--   0        0        0     2126 2023-05-08 23:21:49.666884 windmill_api-1.96.3/windmill_api/models/create_folder_json_body.py
--rw-r--r--   0        0        0     1697 2023-05-08 23:21:49.662884 windmill_api-1.96.3/windmill_api/models/create_group_json_body.py
--rw-r--r--   0        0        0     1613 2023-05-08 23:21:49.686884 windmill_api-1.96.3/windmill_api/models/create_input.py
--rw-r--r--   0        0        0     1171 2023-05-08 23:21:49.686884 windmill_api-1.96.3/windmill_api/models/create_input_args.py
--rw-r--r--   0        0        0     1701 2023-05-08 23:21:49.710885 windmill_api-1.96.3/windmill_api/models/create_input_json_body.py
--rw-r--r--   0        0        0     1217 2023-05-08 23:21:49.706885 windmill_api-1.96.3/windmill_api/models/create_input_json_body_args.py
--rw-r--r--   0        0        0      214 2023-05-08 23:21:41.886769 windmill_api-1.96.3/windmill_api/models/create_input_runnable_type.py
--rw-r--r--   0        0        0     1732 2023-05-08 23:21:49.734885 windmill_api-1.96.3/windmill_api/models/create_raw_app_json_body.py
--rw-r--r--   0        0        0     2094 2023-05-08 23:21:49.742885 windmill_api-1.96.3/windmill_api/models/create_resource.py
--rw-r--r--   0        0        0     2140 2023-05-08 23:21:49.766886 windmill_api-1.96.3/windmill_api/models/create_resource_json_body.py
--rw-r--r--   0        0        0     2335 2023-05-08 23:21:49.778886 windmill_api-1.96.3/windmill_api/models/create_resource_type_json_body.py
--rw-r--r--   0        0        0     2780 2023-05-08 23:21:49.806886 windmill_api-1.96.3/windmill_api/models/create_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-05-08 23:21:49.798886 windmill_api-1.96.3/windmill_api/models/create_schedule_json_body_args.py
--rw-r--r--   0        0        0     5120 2023-05-08 23:21:49.874887 windmill_api-1.96.3/windmill_api/models/create_script_json_body.py
--rw-r--r--   0        0        0      249 2023-05-08 23:21:42.930784 windmill_api-1.96.3/windmill_api/models/create_script_json_body_kind.py
--rw-r--r--   0        0        0      207 2023-05-08 23:21:41.862769 windmill_api-1.96.3/windmill_api/models/create_script_json_body_language.py
--rw-r--r--   0        0        0     1232 2023-05-08 23:21:49.826887 windmill_api-1.96.3/windmill_api/models/create_script_json_body_schema.py
--rw-r--r--   0        0        0     2534 2023-05-08 23:21:49.862887 windmill_api-1.96.3/windmill_api/models/create_token_impersonate_json_body.py
--rw-r--r--   0        0        0     2169 2023-05-08 23:21:49.894888 windmill_api-1.96.3/windmill_api/models/create_token_json_body.py
--rw-r--r--   0        0        0     2364 2023-05-08 23:21:49.910888 windmill_api-1.96.3/windmill_api/models/create_user_globally_json_body.py
--rw-r--r--   0        0        0     1771 2023-05-08 23:21:49.918888 windmill_api-1.96.3/windmill_api/models/create_user_json_body.py
--rw-r--r--   0        0        0     2493 2023-05-08 23:21:49.946888 windmill_api-1.96.3/windmill_api/models/create_variable.py
--rw-r--r--   0        0        0     2539 2023-05-08 23:21:49.958888 windmill_api-1.96.3/windmill_api/models/create_variable_json_body.py
--rw-r--r--   0        0        0     1678 2023-05-08 23:21:49.974889 windmill_api-1.96.3/windmill_api/models/create_workspace.py
--rw-r--r--   0        0        0     1724 2023-05-08 23:21:49.982889 windmill_api-1.96.3/windmill_api/models/create_workspace_json_body.py
--rw-r--r--   0        0        0     1490 2023-05-08 23:21:50.022889 windmill_api-1.96.3/windmill_api/models/decline_invite_json_body.py
--rw-r--r--   0        0        0    11110 2023-05-08 23:21:50.134891 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200.py
--rw-r--r--   0        0        0     1270 2023-05-08 23:21:50.042890 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3658 2023-05-08 23:21:50.086890 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7442 2023-05-08 23:21:50.170892 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1883 2023-05-08 23:21:50.158891 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2318 2023-05-08 23:21:50.182892 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      219 2023-05-08 23:21:42.462777 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1788 2023-05-08 23:21:50.198892 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2324 2023-05-08 23:21:50.218892 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      377 2023-05-08 23:21:42.662780 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7053 2023-05-08 23:21:50.282893 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1873 2023-05-08 23:21:50.242893 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2298 2023-05-08 23:21:50.270893 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      217 2023-05-08 23:21:42.030771 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1778 2023-05-08 23:21:50.294893 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2314 2023-05-08 23:21:50.318894 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      375 2023-05-08 23:21:42.046771 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2134 2023-05-08 23:21:50.326894 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      327 2023-05-08 23:21:41.866768 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      216 2023-05-08 23:21:42.402777 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3432 2023-05-08 23:21:50.402895 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7425 2023-05-08 23:21:50.434895 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3442 2023-05-08 23:21:50.442896 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2023 2023-05-08 23:21:50.466896 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2327 2023-05-08 23:21:50.474896 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2261 2023-05-08 23:21:50.494896 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      198 2023-05-08 23:21:42.058771 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-08 23:21:50.498896 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      198 2023-05-08 23:21:42.650780 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2016 2023-05-08 23:21:50.526897 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2067 2023-05-08 23:21:50.526897 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7349 2023-05-08 23:21:50.606898 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3408 2023-05-08 23:21:50.566897 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2013 2023-05-08 23:21:50.590898 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2317 2023-05-08 23:21:50.622898 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2241 2023-05-08 23:21:50.638898 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-05-08 23:21:42.634780 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2108 2023-05-08 23:21:50.650899 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-05-08 23:21:42.450777 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2006 2023-05-08 23:21:50.666899 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2057 2023-05-08 23:21:50.690899 windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1783 2023-05-08 23:21:50.702900 windmill_api-1.96.3/windmill_api/models/delete_invite_json_body.py
--rw-r--r--   0        0        0     7636 2023-05-08 23:21:50.810901 windmill_api-1.96.3/windmill_api/models/delete_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1309 2023-05-08 23:21:50.722900 windmill_api-1.96.3/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      258 2023-05-08 23:21:42.462777 windmill_api-1.96.3/windmill_api/models/delete_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      216 2023-05-08 23:21:41.946770 windmill_api-1.96.3/windmill_api/models/delete_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1283 2023-05-08 23:21:50.770900 windmill_api-1.96.3/windmill_api/models/delete_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     2933 2023-05-08 23:21:50.806901 windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-05-08 23:21:50.866902 windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-05-08 23:21:42.042771 windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-05-08 23:21:50.838901 windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-05-08 23:21:50.862902 windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-05-08 23:21:50.890902 windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-05-08 23:21:50.902902 windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-05-08 23:21:42.446777 windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-05-08 23:21:50.918903 windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-05-08 23:21:50.934903 windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-05-08 23:21:42.370776 windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-05-08 23:21:50.946903 windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-05-08 23:21:42.222774 windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     1551 2023-05-08 23:21:50.962903 windmill_api-1.96.3/windmill_api/models/edit_auto_invite_json_body.py
--rw-r--r--   0        0        0     1980 2023-05-08 23:21:50.978903 windmill_api-1.96.3/windmill_api/models/edit_resource.py
--rw-r--r--   0        0        0     1791 2023-05-08 23:21:50.986904 windmill_api-1.96.3/windmill_api/models/edit_resource_type.py
--rw-r--r--   0        0        0     1845 2023-05-08 23:21:51.006904 windmill_api-1.96.3/windmill_api/models/edit_schedule.py
--rw-r--r--   0        0        0     1176 2023-05-08 23:21:51.006904 windmill_api-1.96.3/windmill_api/models/edit_schedule_args.py
--rw-r--r--   0        0        0     1691 2023-05-08 23:21:51.030904 windmill_api-1.96.3/windmill_api/models/edit_slack_command_json_body.py
--rw-r--r--   0        0        0     2260 2023-05-08 23:21:51.042904 windmill_api-1.96.3/windmill_api/models/edit_variable.py
--rw-r--r--   0        0        0     1520 2023-05-08 23:21:51.054905 windmill_api-1.96.3/windmill_api/models/edit_webhook_json_body.py
--rw-r--r--   0        0        0     2058 2023-05-08 23:21:51.070905 windmill_api-1.96.3/windmill_api/models/edit_workspace_user.py
--rw-r--r--   0        0        0     3663 2023-05-08 23:21:51.102905 windmill_api-1.96.3/windmill_api/models/execute_component_json_body.py
--rw-r--r--   0        0        0     1346 2023-05-08 23:21:51.114905 windmill_api-1.96.3/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
--rw-r--r--   0        0        0     1942 2023-05-08 23:21:51.134906 windmill_api-1.96.3/windmill_api/models/execute_component_json_body_raw_code.py
--rw-r--r--   0        0        0     1577 2023-05-08 23:21:51.142906 windmill_api-1.96.3/windmill_api/models/exists_username_json_body.py
--rw-r--r--   0        0        0     1400 2023-05-08 23:21:51.174906 windmill_api-1.96.3/windmill_api/models/exists_workspace_json_body.py
--rw-r--r--   0        0        0     4924 2023-05-08 23:21:51.206907 windmill_api-1.96.3/windmill_api/models/flow.py
--rw-r--r--   0        0        0     1166 2023-05-08 23:21:51.198907 windmill_api-1.96.3/windmill_api/models/flow_extra_perms.py
--rw-r--r--   0        0        0     3707 2023-05-08 23:21:51.246907 windmill_api-1.96.3/windmill_api/models/flow_metadata.py
--rw-r--r--   0        0        0     1209 2023-05-08 23:21:51.222907 windmill_api-1.96.3/windmill_api/models/flow_metadata_extra_perms.py
--rw-r--r--   0        0        0     5729 2023-05-08 23:21:51.298908 windmill_api-1.96.3/windmill_api/models/flow_module.py
--rw-r--r--   0        0        0     2726 2023-05-08 23:21:51.286908 windmill_api-1.96.3/windmill_api/models/flow_module_retry.py
--rw-r--r--   0        0        0     1807 2023-05-08 23:21:51.322908 windmill_api-1.96.3/windmill_api/models/flow_module_retry_constant.py
--rw-r--r--   0        0        0     2111 2023-05-08 23:21:51.338909 windmill_api-1.96.3/windmill_api/models/flow_module_retry_exponential.py
--rw-r--r--   0        0        0     1834 2023-05-08 23:21:51.350909 windmill_api-1.96.3/windmill_api/models/flow_module_sleep_type_0.py
--rw-r--r--   0        0        0      159 2023-05-08 23:21:42.474778 windmill_api-1.96.3/windmill_api/models/flow_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1701 2023-05-08 23:21:51.366909 windmill_api-1.96.3/windmill_api/models/flow_module_sleep_type_1.py
--rw-r--r--   0        0        0      159 2023-05-08 23:21:42.166773 windmill_api-1.96.3/windmill_api/models/flow_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1800 2023-05-08 23:21:51.382909 windmill_api-1.96.3/windmill_api/models/flow_module_stop_after_if.py
--rw-r--r--   0        0        0     1851 2023-05-08 23:21:51.394909 windmill_api-1.96.3/windmill_api/models/flow_module_suspend.py
--rw-r--r--   0        0        0     3292 2023-05-08 23:21:51.426910 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_0.py
--rw-r--r--   0        0        0     3564 2023-05-08 23:21:51.430910 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-08 23:21:51.466910 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-08 23:21:42.454777 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-08 23:21:51.494911 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-08 23:21:42.466777 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      208 2023-05-08 23:21:42.258774 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_0_language.py
--rw-r--r--   0        0        0      158 2023-05-08 23:21:42.822783 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_0_type.py
--rw-r--r--   0        0        0     2477 2023-05-08 23:21:51.502911 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_1.py
--rw-r--r--   0        0        0     3564 2023-05-08 23:21:51.530912 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-08 23:21:51.554912 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-08 23:21:42.898784 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-08 23:21:51.562912 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-08 23:21:42.718781 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      152 2023-05-08 23:21:42.134772 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_1_type.py
--rw-r--r--   0        0        0     2204 2023-05-08 23:21:51.586912 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_2.py
--rw-r--r--   0        0        0     3564 2023-05-08 23:21:51.594912 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-05-08 23:21:51.614913 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-05-08 23:21:42.766782 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-05-08 23:21:51.622913 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-05-08 23:21:42.758782 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      148 2023-05-08 23:21:42.122772 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_2_type.py
--rw-r--r--   0        0        0     4138 2023-05-08 23:21:51.666913 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3.py
--rw-r--r--   0        0        0     1990 2023-05-08 23:21:51.650913 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
--rw-r--r--   0        0        0      173 2023-05-08 23:21:42.318775 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
--rw-r--r--   0        0        0     1857 2023-05-08 23:21:51.674914 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
--rw-r--r--   0        0        0      173 2023-05-08 23:21:42.822783 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
--rw-r--r--   0        0        0     6636 2023-05-08 23:21:51.750915 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item.py
--rw-r--r--   0        0        0     3148 2023-05-08 23:21:51.714914 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
--rw-r--r--   0        0        0     1935 2023-05-08 23:21:51.742915 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-05-08 23:21:51.770915 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-05-08 23:21:51.778915 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-08 23:21:42.910784 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-05-08 23:21:51.798915 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-08 23:21:41.858768 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-05-08 23:21:51.810916 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-05-08 23:21:51.854916 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
--rw-r--r--   0        0        0      162 2023-05-08 23:21:42.270774 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_type.py
--rw-r--r--   0        0        0     2934 2023-05-08 23:21:51.846916 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4.py
--rw-r--r--   0        0        0     2508 2023-05-08 23:21:51.882917 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item.py
--rw-r--r--   0        0        0     7243 2023-05-08 23:21:51.934917 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-05-08 23:21:51.946917 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-05-08 23:21:51.958918 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-05-08 23:21:51.978918 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-05-08 23:21:51.986918 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-08 23:21:42.286775 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-05-08 23:21:52.006918 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-08 23:21:42.158773 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-05-08 23:21:52.014918 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-05-08 23:21:52.038919 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6636 2023-05-08 23:21:52.090920 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item.py
--rw-r--r--   0        0        0     3148 2023-05-08 23:21:52.078919 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
--rw-r--r--   0        0        0     1935 2023-05-08 23:21:52.106920 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-05-08 23:21:52.122920 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-05-08 23:21:52.138920 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-05-08 23:21:41.930770 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-05-08 23:21:52.150920 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-05-08 23:21:42.038771 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-05-08 23:21:52.166921 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-05-08 23:21:52.214921 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
--rw-r--r--   0        0        0      158 2023-05-08 23:21:41.934769 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_type.py
--rw-r--r--   0        0        0     2577 2023-05-08 23:21:52.202921 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5.py
--rw-r--r--   0        0        0     2679 2023-05-08 23:21:52.242922 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item.py
--rw-r--r--   0        0        0     7243 2023-05-08 23:21:52.294922 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-05-08 23:21:52.282922 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-05-08 23:21:52.334923 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-05-08 23:21:52.330923 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-05-08 23:21:52.358923 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-08 23:21:42.098772 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-05-08 23:21:52.366923 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-08 23:21:42.398776 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-05-08 23:21:52.386924 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-05-08 23:21:52.394924 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      158 2023-05-08 23:21:42.594779 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_type.py
--rw-r--r--   0        0        0     1839 2023-05-08 23:21:52.414924 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_6.py
--rw-r--r--   0        0        0      156 2023-05-08 23:21:42.778782 windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_6_type.py
--rw-r--r--   0        0        0     2009 2023-05-08 23:21:52.426924 windmill_api-1.96.3/windmill_api/models/flow_preview.py
--rw-r--r--   0        0        0     1171 2023-05-08 23:21:52.430925 windmill_api-1.96.3/windmill_api/models/flow_preview_args.py
--rw-r--r--   0        0        0     3074 2023-05-08 23:21:52.470925 windmill_api-1.96.3/windmill_api/models/flow_preview_value.py
--rw-r--r--   0        0        0     6498 2023-05-08 23:21:52.514926 windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module.py
--rw-r--r--   0        0        0     3064 2023-05-08 23:21:52.506925 windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_retry.py
--rw-r--r--   0        0        0     1911 2023-05-08 23:21:52.534926 windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2215 2023-05-08 23:21:52.546926 windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2036 2023-05-08 23:21:52.562926 windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-08 23:21:42.470777 windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1903 2023-05-08 23:21:52.614927 windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-08 23:21:41.982770 windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1904 2023-05-08 23:21:52.590927 windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1955 2023-05-08 23:21:52.618927 windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6422 2023-05-08 23:21:52.694928 windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item.py
--rw-r--r--   0        0        0     3030 2023-05-08 23:21:52.654928 windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_retry.py
--rw-r--r--   0        0        0     1901 2023-05-08 23:21:52.706928 windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2205 2023-05-08 23:21:52.726929 windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2016 2023-05-08 23:21:52.734929 windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-05-08 23:21:42.078772 windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1883 2023-05-08 23:21:52.754929 windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-05-08 23:21:41.998771 windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1894 2023-05-08 23:21:52.762929 windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1945 2023-05-08 23:21:52.786929 windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1143 2023-05-08 23:21:52.782930 windmill_api-1.96.3/windmill_api/models/flow_schema.py
--rw-r--r--   0        0        0     3001 2023-05-08 23:21:52.822930 windmill_api-1.96.3/windmill_api/models/flow_status.py
--rw-r--r--   0        0        0     6370 2023-05-08 23:21:52.870931 windmill_api-1.96.3/windmill_api/models/flow_status_failure_module.py
--rw-r--r--   0        0        0     1723 2023-05-08 23:21:52.846930 windmill_api-1.96.3/windmill_api/models/flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     1999 2023-05-08 23:21:52.874931 windmill_api-1.96.3/windmill_api/models/flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      190 2023-05-08 23:21:42.046771 windmill_api-1.96.3/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1628 2023-05-08 23:21:52.898931 windmill_api-1.96.3/windmill_api/models/flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2164 2023-05-08 23:21:52.910931 windmill_api-1.96.3/windmill_api/models/flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      348 2023-05-08 23:21:42.662780 windmill_api-1.96.3/windmill_api/models/flow_status_failure_module_type.py
--rw-r--r--   0        0        0     5808 2023-05-08 23:21:53.026933 windmill_api-1.96.3/windmill_api/models/flow_status_module.py
--rw-r--r--   0        0        0     1685 2023-05-08 23:21:52.934932 windmill_api-1.96.3/windmill_api/models/flow_status_module_approvers_item.py
--rw-r--r--   0        0        0     1925 2023-05-08 23:21:52.958932 windmill_api-1.96.3/windmill_api/models/flow_status_module_branch_chosen.py
--rw-r--r--   0        0        0      183 2023-05-08 23:21:42.718781 windmill_api-1.96.3/windmill_api/models/flow_status_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1590 2023-05-08 23:21:52.986932 windmill_api-1.96.3/windmill_api/models/flow_status_module_branchall.py
--rw-r--r--   0        0        0     2126 2023-05-08 23:21:53.022933 windmill_api-1.96.3/windmill_api/models/flow_status_module_iterator.py
--rw-r--r--   0        0        0      341 2023-05-08 23:21:42.746782 windmill_api-1.96.3/windmill_api/models/flow_status_module_type.py
--rw-r--r--   0        0        0     5981 2023-05-08 23:21:53.126934 windmill_api-1.96.3/windmill_api/models/flow_status_modules_item.py
--rw-r--r--   0        0        0     1713 2023-05-08 23:21:53.050933 windmill_api-1.96.3/windmill_api/models/flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     1979 2023-05-08 23:21:53.078934 windmill_api-1.96.3/windmill_api/models/flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      188 2023-05-08 23:21:42.382776 windmill_api-1.96.3/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1618 2023-05-08 23:21:53.106934 windmill_api-1.96.3/windmill_api/models/flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2154 2023-05-08 23:21:53.142935 windmill_api-1.96.3/windmill_api/models/flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      346 2023-05-08 23:21:42.238774 windmill_api-1.96.3/windmill_api/models/flow_status_modules_item_type.py
--rw-r--r--   0        0        0     1974 2023-05-08 23:21:53.158935 windmill_api-1.96.3/windmill_api/models/flow_status_retry.py
--rw-r--r--   0        0        0     2957 2023-05-08 23:21:53.186935 windmill_api-1.96.3/windmill_api/models/flow_value.py
--rw-r--r--   0        0        0     6224 2023-05-08 23:21:53.238936 windmill_api-1.96.3/windmill_api/models/flow_value_failure_module.py
--rw-r--r--   0        0        0     2940 2023-05-08 23:21:53.222936 windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1873 2023-05-08 23:21:53.250936 windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-05-08 23:21:53.266936 windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-05-08 23:21:53.282937 windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-05-08 23:21:42.410776 windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-05-08 23:21:53.294937 windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-05-08 23:21:42.630780 windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-05-08 23:21:53.310937 windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-05-08 23:21:53.322937 windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6125 2023-05-08 23:21:53.430939 windmill_api-1.96.3/windmill_api/models/flow_value_modules_item.py
--rw-r--r--   0        0        0     2906 2023-05-08 23:21:53.358938 windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1863 2023-05-08 23:21:53.386938 windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-05-08 23:21:53.446939 windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-05-08 23:21:53.462939 windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-05-08 23:21:42.234774 windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-05-08 23:21:53.474939 windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-05-08 23:21:42.430777 windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-05-08 23:21:53.490940 windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-05-08 23:21:53.502940 windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1858 2023-05-08 23:21:53.522940 windmill_api-1.96.3/windmill_api/models/folder.py
--rw-r--r--   0        0        0     1179 2023-05-08 23:21:53.522940 windmill_api-1.96.3/windmill_api/models/folder_extra_perms.py
--rw-r--r--   0        0        0     1560 2023-05-08 23:21:53.546941 windmill_api-1.96.3/windmill_api/models/force_cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     3807 2023-05-08 23:21:53.566941 windmill_api-1.96.3/windmill_api/models/forloop_flow.py
--rw-r--r--   0        0        0     1874 2023-05-08 23:21:53.574941 windmill_api-1.96.3/windmill_api/models/forloop_flow_iterator_type_0.py
--rw-r--r--   0        0        0      163 2023-05-08 23:21:42.594779 windmill_api-1.96.3/windmill_api/models/forloop_flow_iterator_type_0_type.py
--rw-r--r--   0        0        0     1741 2023-05-08 23:21:53.594941 windmill_api-1.96.3/windmill_api/models/forloop_flow_iterator_type_1.py
--rw-r--r--   0        0        0      163 2023-05-08 23:21:42.474778 windmill_api-1.96.3/windmill_api/models/forloop_flow_iterator_type_1_type.py
--rw-r--r--   0        0        0     6224 2023-05-08 23:21:53.654942 windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item.py
--rw-r--r--   0        0        0     2940 2023-05-08 23:21:53.634942 windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1873 2023-05-08 23:21:53.662942 windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-05-08 23:21:53.686943 windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-05-08 23:21:53.686943 windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-05-08 23:21:41.894769 windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-05-08 23:21:53.714943 windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-05-08 23:21:42.850783 windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-05-08 23:21:53.718943 windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-05-08 23:21:53.742943 windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_suspend.py
--rw-r--r--   0        0        0      152 2023-05-08 23:21:42.078772 windmill_api-1.96.3/windmill_api/models/forloop_flow_type.py
--rw-r--r--   0        0        0     4052 2023-05-08 23:21:53.822944 windmill_api-1.96.3/windmill_api/models/get_app_by_path_response_200.py
--rw-r--r--   0        0        0      219 2023-05-08 23:21:42.874783 windmill_api-1.96.3/windmill_api/models/get_app_by_path_response_200_execution_mode.py
--rw-r--r--   0        0        0     1279 2023-05-08 23:21:53.762944 windmill_api-1.96.3/windmill_api/models/get_app_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     3811 2023-05-08 23:21:53.834945 windmill_api-1.96.3/windmill_api/models/get_app_by_path_response_200_policy.py
--rw-r--r--   0        0        0      225 2023-05-08 23:21:42.262774 windmill_api-1.96.3/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2009 2023-05-08 23:21:53.850945 windmill_api-1.96.3/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1412 2023-05-08 23:21:53.854945 windmill_api-1.96.3/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4819 2023-05-08 23:21:53.910946 windmill_api-1.96.3/windmill_api/models/get_app_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0      228 2023-05-08 23:21:42.710781 windmill_api-1.96.3/windmill_api/models/get_app_by_path_with_draft_response_200_execution_mode.py
--rw-r--r--   0        0        0     1330 2023-05-08 23:21:53.874945 windmill_api-1.96.3/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py
--rw-r--r--   0        0        0     3992 2023-05-08 23:21:53.918946 windmill_api-1.96.3/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py
--rw-r--r--   0        0        0      234 2023-05-08 23:21:42.290775 windmill_api-1.96.3/windmill_api/models/get_app_by_path_with_draft_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2160 2023-05-08 23:21:53.934946 windmill_api-1.96.3/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1463 2023-05-08 23:21:53.938946 windmill_api-1.96.3/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4112 2023-05-08 23:21:53.982947 windmill_api-1.96.3/windmill_api/models/get_app_by_version_response_200.py
--rw-r--r--   0        0        0      222 2023-05-08 23:21:42.330775 windmill_api-1.96.3/windmill_api/models/get_app_by_version_response_200_execution_mode.py
--rw-r--r--   0        0        0     1294 2023-05-08 23:21:53.958947 windmill_api-1.96.3/windmill_api/models/get_app_by_version_response_200_extra_perms.py
--rw-r--r--   0        0        0     3862 2023-05-08 23:21:54.002947 windmill_api-1.96.3/windmill_api/models/get_app_by_version_response_200_policy.py
--rw-r--r--   0        0        0      228 2023-05-08 23:21:42.634780 windmill_api-1.96.3/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2042 2023-05-08 23:21:54.010947 windmill_api-1.96.3/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1427 2023-05-08 23:21:54.022947 windmill_api-1.96.3/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3764 2023-05-08 23:21:54.058948 windmill_api-1.96.3/windmill_api/models/get_audit_log_response_200.py
--rw-r--r--   0        0        0      231 2023-05-08 23:21:42.482778 windmill_api-1.96.3/windmill_api/models/get_audit_log_response_200_action_kind.py
--rw-r--r--   0        0        0      634 2023-05-08 23:21:42.766782 windmill_api-1.96.3/windmill_api/models/get_audit_log_response_200_operation.py
--rw-r--r--   0        0        0     1265 2023-05-08 23:21:54.046948 windmill_api-1.96.3/windmill_api/models/get_audit_log_response_200_parameters.py
--rw-r--r--   0        0        0    11008 2023-05-08 23:21:54.210950 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200.py
--rw-r--r--   0        0        0     1255 2023-05-08 23:21:54.078948 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3595 2023-05-08 23:21:54.118949 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7343 2023-05-08 23:21:54.242951 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1868 2023-05-08 23:21:54.234950 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2288 2023-05-08 23:21:54.262951 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      216 2023-05-08 23:21:42.134772 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1773 2023-05-08 23:21:54.266951 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2309 2023-05-08 23:21:54.298951 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      374 2023-05-08 23:21:41.862769 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6924 2023-05-08 23:21:54.350952 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1858 2023-05-08 23:21:54.322952 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-05-08 23:21:54.350952 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-05-08 23:21:42.366776 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-05-08 23:21:54.374952 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2299 2023-05-08 23:21:54.386953 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      372 2023-05-08 23:21:42.134772 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2119 2023-05-08 23:21:54.410953 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      324 2023-05-08 23:21:42.150773 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      213 2023-05-08 23:21:42.306775 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3375 2023-05-08 23:21:54.426953 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7311 2023-05-08 23:21:54.502954 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3391 2023-05-08 23:21:54.466954 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2008 2023-05-08 23:21:54.494954 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2312 2023-05-08 23:21:54.570955 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2231 2023-05-08 23:21:54.562955 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      195 2023-05-08 23:21:42.154773 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2098 2023-05-08 23:21:54.590956 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      195 2023-05-08 23:21:42.794782 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2001 2023-05-08 23:21:54.602956 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2052 2023-05-08 23:21:54.618956 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7235 2023-05-08 23:21:54.682957 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3357 2023-05-08 23:21:54.658957 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1998 2023-05-08 23:21:54.686957 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-05-08 23:21:54.714957 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-05-08 23:21:54.714957 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-08 23:21:42.458777 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-05-08 23:21:54.738958 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-08 23:21:42.330775 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-05-08 23:21:54.746958 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-05-08 23:21:54.766958 windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     5374 2023-05-08 23:21:54.810959 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200.py
--rw-r--r--   0        0        0     1281 2023-05-08 23:21:54.786959 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     1258 2023-05-08 23:21:54.806959 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_schema.py
--rw-r--r--   0        0        0     3302 2023-05-08 23:21:54.846959 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value.py
--rw-r--r--   0        0        0     7159 2023-05-08 23:21:54.894960 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
--rw-r--r--   0        0        0     3323 2023-05-08 23:21:54.882960 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
--rw-r--r--   0        0        0     1988 2023-05-08 23:21:54.942961 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-05-08 23:21:54.982961 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-05-08 23:21:54.970961 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-05-08 23:21:41.842768 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-05-08 23:21:54.998962 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-05-08 23:21:41.910769 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-05-08 23:21:55.010962 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-05-08 23:21:55.026962 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7066 2023-05-08 23:21:55.094963 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
--rw-r--r--   0        0        0     3289 2023-05-08 23:21:55.066963 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
--rw-r--r--   0        0        0     1978 2023-05-08 23:21:55.094963 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2282 2023-05-08 23:21:55.126963 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2171 2023-05-08 23:21:55.122963 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-05-08 23:21:41.854768 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2038 2023-05-08 23:21:55.150964 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-05-08 23:21:42.258774 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1971 2023-05-08 23:21:55.154964 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2022 2023-05-08 23:21:55.182964 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2093 2023-05-08 23:21:55.182964 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0     5695 2023-05-08 23:21:55.278966 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py
--rw-r--r--   0        0        0     1360 2023-05-08 23:21:55.202964 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py
--rw-r--r--   0        0        0     1337 2023-05-08 23:21:55.218965 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py
--rw-r--r--   0        0        0     3559 2023-05-08 23:21:55.262965 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py
--rw-r--r--   0        0        0     7829 2023-05-08 23:21:55.410967 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py
--rw-r--r--   0        0        0     3606 2023-05-08 23:21:55.358967 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py
--rw-r--r--   0        0        0     2067 2023-05-08 23:21:55.386967 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2371 2023-05-08 23:21:55.418968 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2343 2023-05-08 23:21:55.442968 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      205 2023-05-08 23:21:42.070772 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2210 2023-05-08 23:21:55.446968 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      205 2023-05-08 23:21:42.170773 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2060 2023-05-08 23:21:55.470968 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2111 2023-05-08 23:21:55.474968 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7685 2023-05-08 23:21:55.550969 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py
--rw-r--r--   0        0        0     3542 2023-05-08 23:21:55.514969 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py
--rw-r--r--   0        0        0     2057 2023-05-08 23:21:55.542969 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2361 2023-05-08 23:21:55.574970 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2323 2023-05-08 23:21:55.578970 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      203 2023-05-08 23:21:42.026771 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2190 2023-05-08 23:21:55.606970 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      203 2023-05-08 23:21:42.898784 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2050 2023-05-08 23:21:55.606970 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2101 2023-05-08 23:21:55.634971 windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2756 2023-05-08 23:21:55.642971 windmill_api-1.96.3/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
--rw-r--r--   0        0        0     1337 2023-05-08 23:21:55.654971 windmill_api-1.96.3/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
--rw-r--r--   0        0        0     2010 2023-05-08 23:21:55.674971 windmill_api-1.96.3/windmill_api/models/get_folder_response_200.py
--rw-r--r--   0        0        0     1258 2023-05-08 23:21:55.674971 windmill_api-1.96.3/windmill_api/models/get_folder_response_200_extra_perms.py
--rw-r--r--   0        0        0     2357 2023-05-08 23:21:55.706972 windmill_api-1.96.3/windmill_api/models/get_folder_usage_response_200.py
--rw-r--r--   0        0        0      325 2023-05-08 23:21:42.082772 windmill_api-1.96.3/windmill_api/models/get_granular_acls_kind.py
--rw-r--r--   0        0        0     1235 2023-05-08 23:21:55.734972 windmill_api-1.96.3/windmill_api/models/get_granular_acls_response_200.py
--rw-r--r--   0        0        0     2888 2023-05-08 23:21:55.802973 windmill_api-1.96.3/windmill_api/models/get_group_response_200.py
--rw-r--r--   0        0        0     1253 2023-05-08 23:21:55.754972 windmill_api-1.96.3/windmill_api/models/get_group_response_200_extra_perms.py
--rw-r--r--   0        0        0     1606 2023-05-08 23:21:55.778973 windmill_api-1.96.3/windmill_api/models/get_hub_app_by_id_response_200.py
--rw-r--r--   0        0        0     1634 2023-05-08 23:21:55.806973 windmill_api-1.96.3/windmill_api/models/get_hub_app_by_id_response_200_app.py
--rw-r--r--   0        0        0     1977 2023-05-08 23:21:55.830973 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200.py
--rw-r--r--   0        0        0     2950 2023-05-08 23:21:55.846974 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
--rw-r--r--   0        0        0     1289 2023-05-08 23:21:55.850974 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
--rw-r--r--   0        0        0     3410 2023-05-08 23:21:55.886974 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
--rw-r--r--   0        0        0     7365 2023-05-08 23:21:55.926975 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
--rw-r--r--   0        0        0     3418 2023-05-08 23:21:55.926975 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     2019 2023-05-08 23:21:55.954975 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2323 2023-05-08 23:21:55.958975 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2249 2023-05-08 23:21:55.982976 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-05-08 23:21:42.630780 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2116 2023-05-08 23:21:55.990976 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-05-08 23:21:42.130772 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2012 2023-05-08 23:21:56.010976 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2063 2023-05-08 23:21:56.018976 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7289 2023-05-08 23:21:56.126978 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
--rw-r--r--   0        0        0     3384 2023-05-08 23:21:56.058977 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     2009 2023-05-08 23:21:56.086977 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2313 2023-05-08 23:21:56.118978 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2229 2023-05-08 23:21:56.214979 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      194 2023-05-08 23:21:42.938784 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2096 2023-05-08 23:21:56.154978 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      194 2023-05-08 23:21:42.706781 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2002 2023-05-08 23:21:56.182978 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2053 2023-05-08 23:21:56.214979 windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2698 2023-05-08 23:21:56.254980 windmill_api-1.96.3/windmill_api/models/get_hub_script_by_path_response_200.py
--rw-r--r--   0        0        0      216 2023-05-08 23:21:42.878784 windmill_api-1.96.3/windmill_api/models/get_hub_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     2644 2023-05-08 23:21:56.250980 windmill_api-1.96.3/windmill_api/models/get_input_history_response_200_item.py
--rw-r--r--   0        0        0     1278 2023-05-08 23:21:56.270980 windmill_api-1.96.3/windmill_api/models/get_input_history_response_200_item_args.py
--rw-r--r--   0        0        0      218 2023-05-08 23:21:42.230774 windmill_api-1.96.3/windmill_api/models/get_input_history_runnable_type.py
--rw-r--r--   0        0        0     1852 2023-05-08 23:21:56.286980 windmill_api-1.96.3/windmill_api/models/get_job_response_200.py
--rw-r--r--   0        0        0      188 2023-05-08 23:21:42.414777 windmill_api-1.96.3/windmill_api/models/get_job_response_200_type.py
--rw-r--r--   0        0        0     2364 2023-05-08 23:21:56.306980 windmill_api-1.96.3/windmill_api/models/get_job_updates_response_200.py
--rw-r--r--   0        0        0     1744 2023-05-08 23:21:56.314980 windmill_api-1.96.3/windmill_api/models/get_premium_info_response_200.py
--rw-r--r--   0        0        0     4218 2023-05-08 23:21:56.354981 windmill_api-1.96.3/windmill_api/models/get_public_app_by_secret_response_200.py
--rw-r--r--   0        0        0      227 2023-05-08 23:21:41.862769 windmill_api-1.96.3/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
--rw-r--r--   0        0        0     1322 2023-05-08 23:21:56.334981 windmill_api-1.96.3/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
--rw-r--r--   0        0        0     3970 2023-05-08 23:21:56.382981 windmill_api-1.96.3/windmill_api/models/get_public_app_by_secret_response_200_policy.py
--rw-r--r--   0        0        0      233 2023-05-08 23:21:42.298775 windmill_api-1.96.3/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2131 2023-05-08 23:21:56.382981 windmill_api-1.96.3/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1455 2023-05-08 23:21:56.402982 windmill_api-1.96.3/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3533 2023-05-08 23:21:56.426982 windmill_api-1.96.3/windmill_api/models/get_resource_response_200.py
--rw-r--r--   0        0        0     1268 2023-05-08 23:21:56.418982 windmill_api-1.96.3/windmill_api/models/get_resource_response_200_extra_perms.py
--rw-r--r--   0        0        0     2335 2023-05-08 23:21:56.454983 windmill_api-1.96.3/windmill_api/models/get_resource_type_response_200.py
--rw-r--r--   0        0        0     1840 2023-05-08 23:21:56.454983 windmill_api-1.96.3/windmill_api/models/get_resume_urls_response_200.py
--rw-r--r--   0        0        0     4325 2023-05-08 23:21:56.514983 windmill_api-1.96.3/windmill_api/models/get_schedule_response_200.py
--rw-r--r--   0        0        0     1232 2023-05-08 23:21:56.506983 windmill_api-1.96.3/windmill_api/models/get_schedule_response_200_args.py
--rw-r--r--   0        0        0     1268 2023-05-08 23:21:56.526984 windmill_api-1.96.3/windmill_api/models/get_schedule_response_200_extra_perms.py
--rw-r--r--   0        0        0     7558 2023-05-08 23:21:56.658985 windmill_api-1.96.3/windmill_api/models/get_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1294 2023-05-08 23:21:56.542984 windmill_api-1.96.3/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-08 23:21:42.930784 windmill_api-1.96.3/windmill_api/models/get_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-05-08 23:21:42.394776 windmill_api-1.96.3/windmill_api/models/get_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-05-08 23:21:56.566984 windmill_api-1.96.3/windmill_api/models/get_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     7558 2023-05-08 23:21:56.654985 windmill_api-1.96.3/windmill_api/models/get_script_by_path_response_200.py
--rw-r--r--   0        0        0     1294 2023-05-08 23:21:56.674986 windmill_api-1.96.3/windmill_api/models/get_script_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-08 23:21:42.594779 windmill_api-1.96.3/windmill_api/models/get_script_by_path_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-05-08 23:21:42.410776 windmill_api-1.96.3/windmill_api/models/get_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-05-08 23:21:56.682986 windmill_api-1.96.3/windmill_api/models/get_script_by_path_response_200_schema.py
--rw-r--r--   0        0        0     6383 2023-05-08 23:21:56.754987 windmill_api-1.96.3/windmill_api/models/get_script_by_path_with_draft_response_200.py
--rw-r--r--   0        0        0     5608 2023-05-08 23:21:56.754987 windmill_api-1.96.3/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py
--rw-r--r--   0        0        0      269 2023-05-08 23:21:42.190773 windmill_api-1.96.3/windmill_api/models/get_script_by_path_with_draft_response_200_draft_kind.py
--rw-r--r--   0        0        0      227 2023-05-08 23:21:42.906784 windmill_api-1.96.3/windmill_api/models/get_script_by_path_with_draft_response_200_draft_language.py
--rw-r--r--   0        0        0     1347 2023-05-08 23:21:56.774987 windmill_api-1.96.3/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py
--rw-r--r--   0        0        0      264 2023-05-08 23:21:41.986770 windmill_api-1.96.3/windmill_api/models/get_script_by_path_with_draft_response_200_kind.py
--rw-r--r--   0        0        0      222 2023-05-08 23:21:42.890784 windmill_api-1.96.3/windmill_api/models/get_script_by_path_with_draft_response_200_language.py
--rw-r--r--   0        0        0     1319 2023-05-08 23:21:56.782987 windmill_api-1.96.3/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py
--rw-r--r--   0        0        0     1922 2023-05-08 23:21:56.802987 windmill_api-1.96.3/windmill_api/models/get_script_deployment_status_response_200.py
--rw-r--r--   0        0        0     4157 2023-05-08 23:21:56.878989 windmill_api-1.96.3/windmill_api/models/get_settings_response_200.py
--rw-r--r--   0        0        0     2428 2023-05-08 23:21:56.830988 windmill_api-1.96.3/windmill_api/models/get_suspended_job_flow_response_200.py
--rw-r--r--   0        0        0     1764 2023-05-08 23:21:56.858988 windmill_api-1.96.3/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
--rw-r--r--   0        0        0     2040 2023-05-08 23:21:56.882989 windmill_api-1.96.3/windmill_api/models/get_suspended_job_flow_response_200_job.py
--rw-r--r--   0        0        0      204 2023-05-08 23:21:41.918769 windmill_api-1.96.3/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
--rw-r--r--   0        0        0     4554 2023-05-08 23:21:56.938989 windmill_api-1.96.3/windmill_api/models/get_variable_response_200.py
--rw-r--r--   0        0        0     1268 2023-05-08 23:21:56.902989 windmill_api-1.96.3/windmill_api/models/get_variable_response_200_extra_perms.py
--rw-r--r--   0        0        0     2647 2023-05-08 23:21:56.938989 windmill_api-1.96.3/windmill_api/models/global_user_info.py
--rw-r--r--   0        0        0      176 2023-05-08 23:21:42.306775 windmill_api-1.96.3/windmill_api/models/global_user_info_login_type.py
--rw-r--r--   0        0        0     1627 2023-05-08 23:21:56.966990 windmill_api-1.96.3/windmill_api/models/global_user_update_json_body.py
--rw-r--r--   0        0        0     2741 2023-05-08 23:21:56.978990 windmill_api-1.96.3/windmill_api/models/global_whoami_response_200.py
--rw-r--r--   0        0        0      185 2023-05-08 23:21:42.026771 windmill_api-1.96.3/windmill_api/models/global_whoami_response_200_login_type.py
--rw-r--r--   0        0        0     2903 2023-05-08 23:21:57.006991 windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5478 2023-05-08 23:21:57.034991 windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      324 2023-05-08 23:21:42.374776 windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1598 2023-05-08 23:21:57.090992 windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1663 2023-05-08 23:21:57.062991 windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2151 2023-05-08 23:21:57.086992 windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3257 2023-05-08 23:21:57.122992 windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      342 2023-05-08 23:21:41.870769 windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1631 2023-05-08 23:21:57.118992 windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3100 2023-05-08 23:21:57.154993 windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      333 2023-05-08 23:21:42.054771 windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1580 2023-05-08 23:21:57.146993 windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      178 2023-05-08 23:21:42.282775 windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2722 2023-05-08 23:21:57.190993 windmill_api-1.96.3/windmill_api/models/group.py
--rw-r--r--   0        0        0     1174 2023-05-08 23:21:57.174993 windmill_api-1.96.3/windmill_api/models/group_extra_perms.py
--rw-r--r--   0        0        0     1689 2023-05-08 23:21:57.198993 windmill_api-1.96.3/windmill_api/models/identity.py
--rw-r--r--   0        0        0      143 2023-05-08 23:21:42.166773 windmill_api-1.96.3/windmill_api/models/identity_type.py
--rw-r--r--   0        0        0     2377 2023-05-08 23:21:57.270994 windmill_api-1.96.3/windmill_api/models/input_.py
--rw-r--r--   0        0        0     1138 2023-05-08 23:21:57.218994 windmill_api-1.96.3/windmill_api/models/input_args.py
--rw-r--r--   0        0        0     1820 2023-05-08 23:21:57.246994 windmill_api-1.96.3/windmill_api/models/input_transform_type_0.py
--rw-r--r--   0        0        0      158 2023-05-08 23:21:42.306775 windmill_api-1.96.3/windmill_api/models/input_transform_type_0_type.py
--rw-r--r--   0        0        0     1687 2023-05-08 23:21:57.274994 windmill_api-1.96.3/windmill_api/models/input_transform_type_1.py
--rw-r--r--   0        0        0      158 2023-05-08 23:21:42.770782 windmill_api-1.96.3/windmill_api/models/input_transform_type_1_type.py
--rw-r--r--   0        0        0     1773 2023-05-08 23:21:57.298995 windmill_api-1.96.3/windmill_api/models/invite_user_json_body.py
--rw-r--r--   0        0        0     1679 2023-05-08 23:21:57.302995 windmill_api-1.96.3/windmill_api/models/javascript_transform.py
--rw-r--r--   0        0        0      158 2023-05-08 23:21:42.318775 windmill_api-1.96.3/windmill_api/models/javascript_transform_type.py
--rw-r--r--   0        0        0     1686 2023-05-08 23:21:57.326995 windmill_api-1.96.3/windmill_api/models/job.py
--rw-r--r--   0        0        0      174 2023-05-08 23:21:42.806783 windmill_api-1.96.3/windmill_api/models/job_type.py
--rw-r--r--   0        0        0     3583 2023-05-08 23:21:57.350995 windmill_api-1.96.3/windmill_api/models/list_apps_response_200_item.py
--rw-r--r--   0        0        0      219 2023-05-08 23:21:42.002771 windmill_api-1.96.3/windmill_api/models/list_apps_response_200_item_execution_mode.py
--rw-r--r--   0        0        0     1276 2023-05-08 23:21:57.346995 windmill_api-1.96.3/windmill_api/models/list_apps_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      218 2023-05-08 23:21:42.462777 windmill_api-1.96.3/windmill_api/models/list_audit_logs_action_kind.py
--rw-r--r--   0        0        0     3896 2023-05-08 23:21:57.394996 windmill_api-1.96.3/windmill_api/models/list_audit_logs_response_200_item.py
--rw-r--r--   0        0        0      237 2023-05-08 23:21:42.882784 windmill_api-1.96.3/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
--rw-r--r--   0        0        0      640 2023-05-08 23:21:42.434777 windmill_api-1.96.3/windmill_api/models/list_audit_logs_response_200_item_operation.py
--rw-r--r--   0        0        0     1298 2023-05-08 23:21:57.374996 windmill_api-1.96.3/windmill_api/models/list_audit_logs_response_200_item_parameters.py
--rw-r--r--   0        0        0    11220 2023-05-08 23:21:57.562998 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item.py
--rw-r--r--   0        0        0     1288 2023-05-08 23:21:57.414996 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_args.py
--rw-r--r--   0        0        0     3736 2023-05-08 23:21:57.454997 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7579 2023-05-08 23:21:57.538998 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1901 2023-05-08 23:21:57.562998 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2352 2023-05-08 23:21:57.590999 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      222 2023-05-08 23:21:42.122772 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1806 2023-05-08 23:21:57.590999 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2342 2023-05-08 23:21:57.659000 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      380 2023-05-08 23:21:42.302775 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7160 2023-05-08 23:21:57.675000 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1891 2023-05-08 23:21:57.683000 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2332 2023-05-08 23:21:57.703000 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      220 2023-05-08 23:21:42.210774 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1796 2023-05-08 23:21:57.707001 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2332 2023-05-08 23:21:57.739001 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      378 2023-05-08 23:21:42.382776 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2152 2023-05-08 23:21:57.739001 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      330 2023-05-08 23:21:42.770782 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
--rw-r--r--   0        0        0      219 2023-05-08 23:21:42.378776 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_language.py
--rw-r--r--   0        0        0     3485 2023-05-08 23:21:57.783002 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7593 2023-05-08 23:21:57.823002 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3498 2023-05-08 23:21:57.819002 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2041 2023-05-08 23:21:57.851003 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2345 2023-05-08 23:21:57.851003 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2295 2023-05-08 23:21:57.939004 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      201 2023-05-08 23:21:41.830768 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2162 2023-05-08 23:21:57.879003 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      201 2023-05-08 23:21:42.502778 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2034 2023-05-08 23:21:57.907003 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2085 2023-05-08 23:21:57.935004 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7471 2023-05-08 23:21:58.047006 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3464 2023-05-08 23:21:57.975005 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2031 2023-05-08 23:21:58.007005 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2335 2023-05-08 23:21:58.035005 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2275 2023-05-08 23:21:58.067006 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      199 2023-05-08 23:21:41.854768 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2142 2023-05-08 23:21:58.075006 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      199 2023-05-08 23:21:42.174773 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2024 2023-05-08 23:21:58.095006 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2075 2023-05-08 23:21:58.103006 windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1865 2023-05-08 23:21:58.123007 windmill_api-1.96.3/windmill_api/models/list_contextual_variables_response_200_item.py
--rw-r--r--   0        0        0     1863 2023-05-08 23:21:58.127007 windmill_api-1.96.3/windmill_api/models/list_flows_response_200_item.py
--rw-r--r--   0        0        0     2074 2023-05-08 23:21:58.155007 windmill_api-1.96.3/windmill_api/models/list_folders_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-05-08 23:21:58.147007 windmill_api-1.96.3/windmill_api/models/list_folders_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2958 2023-05-08 23:21:58.191007 windmill_api-1.96.3/windmill_api/models/list_groups_response_200_item.py
--rw-r--r--   0        0        0     1286 2023-05-08 23:21:58.175007 windmill_api-1.96.3/windmill_api/models/list_groups_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2076 2023-05-08 23:21:58.207008 windmill_api-1.96.3/windmill_api/models/list_hub_apps_response_200.py
--rw-r--r--   0        0        0     2304 2023-05-08 23:21:58.223008 windmill_api-1.96.3/windmill_api/models/list_hub_apps_response_200_apps_item.py
--rw-r--r--   0        0        0     2116 2023-05-08 23:21:58.243008 windmill_api-1.96.3/windmill_api/models/list_hub_flows_response_200.py
--rw-r--r--   0        0        0     2324 2023-05-08 23:21:58.255009 windmill_api-1.96.3/windmill_api/models/list_hub_flows_response_200_flows_item.py
--rw-r--r--   0        0        0     2106 2023-05-08 23:21:58.271009 windmill_api-1.96.3/windmill_api/models/list_hub_scripts_response_200.py
--rw-r--r--   0        0        0     2790 2023-05-08 23:21:58.295009 windmill_api-1.96.3/windmill_api/models/list_hub_scripts_response_200_asks_item.py
--rw-r--r--   0        0        0      262 2023-05-08 23:21:42.558779 windmill_api-1.96.3/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
--rw-r--r--   0        0        0     2590 2023-05-08 23:21:58.311009 windmill_api-1.96.3/windmill_api/models/list_inputs_response_200_item.py
--rw-r--r--   0        0        0     1250 2023-05-08 23:21:58.315009 windmill_api-1.96.3/windmill_api/models/list_inputs_response_200_item_args.py
--rw-r--r--   0        0        0      213 2023-05-08 23:21:42.410776 windmill_api-1.96.3/windmill_api/models/list_inputs_runnable_type.py
--rw-r--r--   0        0        0     1922 2023-05-08 23:21:58.379010 windmill_api-1.96.3/windmill_api/models/list_jobs_response_200_item.py
--rw-r--r--   0        0        0      194 2023-05-08 23:21:41.834768 windmill_api-1.96.3/windmill_api/models/list_jobs_response_200_item_type.py
--rw-r--r--   0        0        0     2076 2023-05-08 23:21:58.343010 windmill_api-1.96.3/windmill_api/models/list_pending_invites_response_200_item.py
--rw-r--r--   0        0        0    12114 2023-05-08 23:21:58.555013 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item.py
--rw-r--r--   0        0        0     1245 2023-05-08 23:21:58.399011 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_args.py
--rw-r--r--   0        0        0     3544 2023-05-08 23:21:58.443011 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7247 2023-05-08 23:21:58.523012 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1858 2023-05-08 23:21:58.547013 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-05-08 23:21:58.575013 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-05-08 23:21:42.942784 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-05-08 23:21:58.579013 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2299 2023-05-08 23:21:58.611014 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      372 2023-05-08 23:21:42.518778 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6858 2023-05-08 23:21:58.663014 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1848 2023-05-08 23:21:58.635014 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2248 2023-05-08 23:21:58.659014 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      212 2023-05-08 23:21:42.754782 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1753 2023-05-08 23:21:58.687015 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2289 2023-05-08 23:21:58.695015 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      370 2023-05-08 23:21:42.262774 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2109 2023-05-08 23:21:58.719015 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      322 2023-05-08 23:21:42.950785 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_job_kind.py
--rw-r--r--   0        0        0      211 2023-05-08 23:21:42.406777 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_language.py
--rw-r--r--   0        0        0     3334 2023-05-08 23:21:58.759016 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7235 2023-05-08 23:21:58.823017 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3357 2023-05-08 23:21:58.867017 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1998 2023-05-08 23:21:58.851017 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-05-08 23:21:58.879017 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-05-08 23:21:58.895018 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-05-08 23:21:42.614780 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-05-08 23:21:58.907018 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-05-08 23:21:42.250774 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-05-08 23:21:58.923018 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-05-08 23:21:58.935018 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7159 2023-05-08 23:21:59.003019 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3323 2023-05-08 23:21:58.975019 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1988 2023-05-08 23:21:59.003019 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-05-08 23:21:59.031020 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-05-08 23:21:59.031020 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-05-08 23:21:42.406777 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-05-08 23:21:59.059020 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-05-08 23:21:42.138773 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-05-08 23:21:59.059020 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-05-08 23:21:59.087020 windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     3045 2023-05-08 23:21:59.139021 windmill_api-1.96.3/windmill_api/models/list_raw_apps_response_200_item.py
--rw-r--r--   0        0        0     1294 2023-05-08 23:21:59.107021 windmill_api-1.96.3/windmill_api/models/list_raw_apps_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     4884 2023-05-08 23:21:59.171022 windmill_api-1.96.3/windmill_api/models/list_resource_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-05-08 23:21:59.159021 windmill_api-1.96.3/windmill_api/models/list_resource_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2363 2023-05-08 23:21:59.191022 windmill_api-1.96.3/windmill_api/models/list_resource_type_response_200_item.py
--rw-r--r--   0        0        0     4426 2023-05-08 23:21:59.287023 windmill_api-1.96.3/windmill_api/models/list_schedules_response_200_item.py
--rw-r--r--   0        0        0     1265 2023-05-08 23:21:59.211022 windmill_api-1.96.3/windmill_api/models/list_schedules_response_200_item_args.py
--rw-r--r--   0        0        0     1301 2023-05-08 23:21:59.231022 windmill_api-1.96.3/windmill_api/models/list_schedules_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     7551 2023-05-08 23:21:59.319024 windmill_api-1.96.3/windmill_api/models/list_scripts_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-05-08 23:21:59.307024 windmill_api-1.96.3/windmill_api/models/list_scripts_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      255 2023-05-08 23:21:42.698781 windmill_api-1.96.3/windmill_api/models/list_scripts_response_200_item_kind.py
--rw-r--r--   0        0        0      213 2023-05-08 23:21:42.694781 windmill_api-1.96.3/windmill_api/models/list_scripts_response_200_item_language.py
--rw-r--r--   0        0        0     1265 2023-05-08 23:21:59.331024 windmill_api-1.96.3/windmill_api/models/list_scripts_response_200_item_schema.py
--rw-r--r--   0        0        0     2985 2023-05-08 23:21:59.363024 windmill_api-1.96.3/windmill_api/models/list_tokens_response_200_item.py
--rw-r--r--   0        0        0     2250 2023-05-08 23:21:59.359024 windmill_api-1.96.3/windmill_api/models/list_user_workspaces_response_200.py
--rw-r--r--   0        0        0     1833 2023-05-08 23:21:59.387025 windmill_api-1.96.3/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
--rw-r--r--   0        0        0     2896 2023-05-08 23:21:59.399025 windmill_api-1.96.3/windmill_api/models/list_users_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0      198 2023-05-08 23:21:42.714781 windmill_api-1.96.3/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
--rw-r--r--   0        0        0     4307 2023-05-08 23:21:59.447026 windmill_api-1.96.3/windmill_api/models/list_users_response_200_item.py
--rw-r--r--   0        0        0     1613 2023-05-08 23:21:59.423025 windmill_api-1.96.3/windmill_api/models/list_users_response_200_item_usage.py
--rw-r--r--   0        0        0     4608 2023-05-08 23:21:59.531027 windmill_api-1.96.3/windmill_api/models/list_variable_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-05-08 23:21:59.467026 windmill_api-1.96.3/windmill_api/models/list_variable_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2693 2023-05-08 23:21:59.507027 windmill_api-1.96.3/windmill_api/models/list_workers_response_200_item.py
--rw-r--r--   0        0        0     2086 2023-05-08 23:21:59.535027 windmill_api-1.96.3/windmill_api/models/list_workspace_invites_response_200_item.py
--rw-r--r--   0        0        0     2082 2023-05-08 23:21:59.559027 windmill_api-1.96.3/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0     2013 2023-05-08 23:21:59.567027 windmill_api-1.96.3/windmill_api/models/list_workspaces_response_200_item.py
--rw-r--r--   0        0        0     3388 2023-05-08 23:21:59.607028 windmill_api-1.96.3/windmill_api/models/listable_app.py
--rw-r--r--   0        0        0      207 2023-05-08 23:21:42.498778 windmill_api-1.96.3/windmill_api/models/listable_app_execution_mode.py
--rw-r--r--   0        0        0     1207 2023-05-08 23:21:59.587028 windmill_api-1.96.3/windmill_api/models/listable_app_extra_perms.py
--rw-r--r--   0        0        0     2913 2023-05-08 23:21:59.631028 windmill_api-1.96.3/windmill_api/models/listable_raw_app.py
--rw-r--r--   0        0        0     1225 2023-05-08 23:21:59.623028 windmill_api-1.96.3/windmill_api/models/listable_raw_app_extra_perms.py
--rw-r--r--   0        0        0     4751 2023-05-08 23:21:59.683029 windmill_api-1.96.3/windmill_api/models/listable_resource.py
--rw-r--r--   0        0        0     1232 2023-05-08 23:21:59.647029 windmill_api-1.96.3/windmill_api/models/listable_resource_extra_perms.py
--rw-r--r--   0        0        0     4486 2023-05-08 23:21:59.707029 windmill_api-1.96.3/windmill_api/models/listable_variable.py
--rw-r--r--   0        0        0     1232 2023-05-08 23:21:59.703029 windmill_api-1.96.3/windmill_api/models/listable_variable_extra_perms.py
--rw-r--r--   0        0        0     1513 2023-05-08 23:21:59.731030 windmill_api-1.96.3/windmill_api/models/login.py
--rw-r--r--   0        0        0     1559 2023-05-08 23:21:59.735030 windmill_api-1.96.3/windmill_api/models/login_json_body.py
--rw-r--r--   0        0        0     1739 2023-05-08 23:21:59.759030 windmill_api-1.96.3/windmill_api/models/login_with_oauth_json_body.py
--rw-r--r--   0        0        0     2758 2023-05-08 23:21:59.775030 windmill_api-1.96.3/windmill_api/models/main_arg_signature.py
--rw-r--r--   0        0        0     5099 2023-05-08 23:21:59.815031 windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item.py
--rw-r--r--   0        0        0      315 2023-05-08 23:21:42.522778 windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1547 2023-05-08 23:21:59.799031 windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1612 2023-05-08 23:21:59.887032 windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2044 2023-05-08 23:21:59.891032 windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3049 2023-05-08 23:21:59.927032 windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      333 2023-05-08 23:21:41.966770 windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1580 2023-05-08 23:21:59.915032 windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     2862 2023-05-08 23:21:59.951033 windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
--rw-r--r--   0        0        0      324 2023-05-08 23:21:42.002771 windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1529 2023-05-08 23:21:59.951033 windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      169 2023-05-08 23:21:41.966770 windmill_api-1.96.3/windmill_api/models/main_arg_signature_type.py
--rw-r--r--   0        0        0     2662 2023-05-08 23:21:59.991033 windmill_api-1.96.3/windmill_api/models/new_schedule.py
--rw-r--r--   0        0        0     1171 2023-05-08 23:21:59.971033 windmill_api-1.96.3/windmill_api/models/new_schedule_args.py
--rw-r--r--   0        0        0     4866 2023-05-08 23:22:00.043034 windmill_api-1.96.3/windmill_api/models/new_script.py
--rw-r--r--   0        0        0      238 2023-05-08 23:21:42.562779 windmill_api-1.96.3/windmill_api/models/new_script_kind.py
--rw-r--r--   0        0        0      196 2023-05-08 23:21:42.722781 windmill_api-1.96.3/windmill_api/models/new_script_language.py
--rw-r--r--   0        0        0     1171 2023-05-08 23:22:00.011034 windmill_api-1.96.3/windmill_api/models/new_script_schema.py
--rw-r--r--   0        0        0     5879 2023-05-08 23:22:00.091035 windmill_api-1.96.3/windmill_api/models/new_script_with_draft.py
--rw-r--r--   0        0        0     5192 2023-05-08 23:22:00.111035 windmill_api-1.96.3/windmill_api/models/new_script_with_draft_draft.py
--rw-r--r--   0        0        0      252 2023-05-08 23:21:42.178773 windmill_api-1.96.3/windmill_api/models/new_script_with_draft_draft_kind.py
--rw-r--r--   0        0        0      210 2023-05-08 23:21:42.254774 windmill_api-1.96.3/windmill_api/models/new_script_with_draft_draft_language.py
--rw-r--r--   0        0        0     1250 2023-05-08 23:22:00.115035 windmill_api-1.96.3/windmill_api/models/new_script_with_draft_draft_schema.py
--rw-r--r--   0        0        0      247 2023-05-08 23:21:41.890769 windmill_api-1.96.3/windmill_api/models/new_script_with_draft_kind.py
--rw-r--r--   0        0        0      205 2023-05-08 23:21:42.246774 windmill_api-1.96.3/windmill_api/models/new_script_with_draft_language.py
--rw-r--r--   0        0        0     1222 2023-05-08 23:22:00.131035 windmill_api-1.96.3/windmill_api/models/new_script_with_draft_schema.py
--rw-r--r--   0        0        0     2108 2023-05-08 23:22:00.147035 windmill_api-1.96.3/windmill_api/models/new_token.py
--rw-r--r--   0        0        0     2473 2023-05-08 23:22:00.167036 windmill_api-1.96.3/windmill_api/models/new_token_impersonate.py
--rw-r--r--   0        0        0     1710 2023-05-08 23:22:00.175036 windmill_api-1.96.3/windmill_api/models/new_user.py
--rw-r--r--   0        0        0     2584 2023-05-08 23:22:00.207036 windmill_api-1.96.3/windmill_api/models/open_flow.py
--rw-r--r--   0        0        0     1166 2023-05-08 23:22:00.195036 windmill_api-1.96.3/windmill_api/models/open_flow_schema.py
--rw-r--r--   0        0        0     3026 2023-05-08 23:22:00.299038 windmill_api-1.96.3/windmill_api/models/open_flow_value.py
--rw-r--r--   0        0        0     6384 2023-05-08 23:22:00.335038 windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module.py
--rw-r--r--   0        0        0     3013 2023-05-08 23:22:00.339038 windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1896 2023-05-08 23:22:00.363039 windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2200 2023-05-08 23:22:00.371039 windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2006 2023-05-08 23:22:00.391039 windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      175 2023-05-08 23:21:42.154773 windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1873 2023-05-08 23:22:00.399039 windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      175 2023-05-08 23:21:42.790782 windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1889 2023-05-08 23:22:00.419039 windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1940 2023-05-08 23:22:00.431040 windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6308 2023-05-08 23:22:00.499041 windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item.py
--rw-r--r--   0        0        0     2979 2023-05-08 23:22:00.471040 windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1886 2023-05-08 23:22:00.499041 windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2190 2023-05-08 23:22:00.531041 windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1986 2023-05-08 23:22:00.527041 windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      173 2023-05-08 23:21:42.582779 windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1853 2023-05-08 23:22:00.555041 windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      173 2023-05-08 23:21:41.986770 windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1879 2023-05-08 23:22:00.555041 windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1930 2023-05-08 23:22:00.583042 windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2816 2023-05-08 23:22:00.595042 windmill_api-1.96.3/windmill_api/models/open_flow_w_path.py
--rw-r--r--   0        0        0     1197 2023-05-08 23:22:00.603042 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_schema.py
--rw-r--r--   0        0        0     3116 2023-05-08 23:22:00.683043 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value.py
--rw-r--r--   0        0        0     6590 2023-05-08 23:22:00.731044 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module.py
--rw-r--r--   0        0        0     3117 2023-05-08 23:22:00.723044 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
--rw-r--r--   0        0        0     1927 2023-05-08 23:22:00.751044 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2231 2023-05-08 23:22:00.763044 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2073 2023-05-08 23:22:00.779044 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      180 2023-05-08 23:21:42.074772 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1940 2023-05-08 23:22:00.791045 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      180 2023-05-08 23:21:42.042771 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1920 2023-05-08 23:22:00.811045 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1971 2023-05-08 23:22:00.819045 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6514 2023-05-08 23:22:00.887046 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item.py
--rw-r--r--   0        0        0     3074 2023-05-08 23:22:00.859046 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
--rw-r--r--   0        0        0     1917 2023-05-08 23:22:00.887046 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2221 2023-05-08 23:22:00.919046 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2044 2023-05-08 23:22:00.915047 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-08 23:21:42.466777 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1911 2023-05-08 23:22:00.943047 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-08 23:21:42.898784 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1910 2023-05-08 23:22:00.951047 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1961 2023-05-08 23:22:00.971047 windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1989 2023-05-08 23:22:00.979047 windmill_api-1.96.3/windmill_api/models/path_flow.py
--rw-r--r--   0        0        0     3089 2023-05-08 23:22:01.055049 windmill_api-1.96.3/windmill_api/models/path_flow_input_transforms.py
--rw-r--r--   0        0        0     2115 2023-05-08 23:22:01.007048 windmill_api-1.96.3/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      185 2023-05-08 23:21:42.110772 windmill_api-1.96.3/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1982 2023-05-08 23:22:01.031048 windmill_api-1.96.3/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      185 2023-05-08 23:21:41.962770 windmill_api-1.96.3/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      135 2023-05-08 23:21:42.166773 windmill_api-1.96.3/windmill_api/models/path_flow_type.py
--rw-r--r--   0        0        0     2292 2023-05-08 23:22:01.071049 windmill_api-1.96.3/windmill_api/models/path_script.py
--rw-r--r--   0        0        0     3181 2023-05-08 23:22:01.091049 windmill_api-1.96.3/windmill_api/models/path_script_input_transforms.py
--rw-r--r--   0        0        0     2135 2023-05-08 23:22:01.095049 windmill_api-1.96.3/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      187 2023-05-08 23:21:42.818783 windmill_api-1.96.3/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2002 2023-05-08 23:22:01.119049 windmill_api-1.96.3/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      187 2023-05-08 23:21:42.418777 windmill_api-1.96.3/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      141 2023-05-08 23:21:42.446777 windmill_api-1.96.3/windmill_api/models/path_script_type.py
--rw-r--r--   0        0        0     3390 2023-05-08 23:22:01.147050 windmill_api-1.96.3/windmill_api/models/policy.py
--rw-r--r--   0        0        0      202 2023-05-08 23:21:42.910784 windmill_api-1.96.3/windmill_api/models/policy_execution_mode.py
--rw-r--r--   0        0        0     1709 2023-05-08 23:22:01.143050 windmill_api-1.96.3/windmill_api/models/policy_triggerables.py
--rw-r--r--   0        0        0     1279 2023-05-08 23:22:01.163050 windmill_api-1.96.3/windmill_api/models/policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2359 2023-05-08 23:22:01.183050 windmill_api-1.96.3/windmill_api/models/preview.py
--rw-r--r--   0        0        0     1148 2023-05-08 23:22:01.183050 windmill_api-1.96.3/windmill_api/models/preview_args.py
--rw-r--r--   0        0        0      194 2023-05-08 23:21:42.742781 windmill_api-1.96.3/windmill_api/models/preview_language.py
--rw-r--r--   0        0        0     1642 2023-05-08 23:22:01.207051 windmill_api-1.96.3/windmill_api/models/preview_schedule_json_body.py
--rw-r--r--   0        0        0     2963 2023-05-08 23:22:01.223051 windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5679 2023-05-08 23:22:01.263052 windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      328 2023-05-08 23:21:41.970770 windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1618 2023-05-08 23:22:01.247051 windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1683 2023-05-08 23:22:01.271052 windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2191 2023-05-08 23:22:01.291052 windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3329 2023-05-08 23:22:01.311052 windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      346 2023-05-08 23:21:42.662780 windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1651 2023-05-08 23:22:01.315052 windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3214 2023-05-08 23:22:01.347053 windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      337 2023-05-08 23:21:41.850768 windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1600 2023-05-08 23:22:01.343053 windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      182 2023-05-08 23:21:42.838783 windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0    11580 2023-05-08 23:22:01.547056 windmill_api-1.96.3/windmill_api/models/queued_job.py
--rw-r--r--   0        0        0     1161 2023-05-08 23:22:01.431054 windmill_api-1.96.3/windmill_api/models/queued_job_args.py
--rw-r--r--   0        0        0     3202 2023-05-08 23:22:01.471054 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status.py
--rw-r--r--   0        0        0     6683 2023-05-08 23:22:01.555056 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1774 2023-05-08 23:22:01.575056 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2106 2023-05-08 23:22:01.583056 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      199 2023-05-08 23:21:42.446777 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1679 2023-05-08 23:22:01.599056 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2215 2023-05-08 23:22:01.619057 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      357 2023-05-08 23:21:42.466777 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6294 2023-05-08 23:22:01.679057 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1764 2023-05-08 23:22:01.643057 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2086 2023-05-08 23:22:01.671057 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      197 2023-05-08 23:21:42.054771 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1669 2023-05-08 23:22:01.695058 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2205 2023-05-08 23:22:01.711058 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      355 2023-05-08 23:21:41.838768 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2025 2023-05-08 23:22:01.731058 windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_retry.py
--rw-r--r--   0        0        0      307 2023-05-08 23:21:42.726781 windmill_api-1.96.3/windmill_api/models/queued_job_job_kind.py
--rw-r--r--   0        0        0      196 2023-05-08 23:21:42.190773 windmill_api-1.96.3/windmill_api/models/queued_job_language.py
--rw-r--r--   0        0        0     3079 2023-05-08 23:22:01.755059 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow.py
--rw-r--r--   0        0        0     6506 2023-05-08 23:22:01.875060 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3069 2023-05-08 23:22:01.867060 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1914 2023-05-08 23:22:01.895060 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2218 2023-05-08 23:22:01.907061 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2040 2023-05-08 23:22:01.923061 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-05-08 23:21:42.570779 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1907 2023-05-08 23:22:01.935061 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-05-08 23:21:42.506778 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1907 2023-05-08 23:22:01.951061 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1958 2023-05-08 23:22:01.963061 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6430 2023-05-08 23:22:02.027062 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3035 2023-05-08 23:22:01.999062 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1904 2023-05-08 23:22:02.027062 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2208 2023-05-08 23:22:02.055063 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2020 2023-05-08 23:22:02.055063 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-05-08 23:21:42.718781 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1887 2023-05-08 23:22:02.079063 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-05-08 23:21:42.394776 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1897 2023-05-08 23:22:02.087063 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1948 2023-05-08 23:22:02.107064 windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     3028 2023-05-08 23:22:02.127064 windmill_api-1.96.3/windmill_api/models/raw_script.py
--rw-r--r--   0        0        0     3139 2023-05-08 23:22:02.139064 windmill_api-1.96.3/windmill_api/models/raw_script_input_transforms.py
--rw-r--r--   0        0        0     2125 2023-05-08 23:22:02.155064 windmill_api-1.96.3/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      186 2023-05-08 23:21:42.414777 windmill_api-1.96.3/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1992 2023-05-08 23:22:02.167064 windmill_api-1.96.3/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      186 2023-05-08 23:21:42.354776 windmill_api-1.96.3/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      196 2023-05-08 23:21:42.834783 windmill_api-1.96.3/windmill_api/models/raw_script_language.py
--rw-r--r--   0        0        0      146 2023-05-08 23:21:41.862769 windmill_api-1.96.3/windmill_api/models/raw_script_type.py
--rw-r--r--   0        0        0     1405 2023-05-08 23:22:02.183065 windmill_api-1.96.3/windmill_api/models/refresh_token_json_body.py
--rw-r--r--   0        0        0     1448 2023-05-08 23:22:02.191065 windmill_api-1.96.3/windmill_api/models/remove_granular_acls_json_body.py
--rw-r--r--   0        0        0      328 2023-05-08 23:21:42.230774 windmill_api-1.96.3/windmill_api/models/remove_granular_acls_kind.py
--rw-r--r--   0        0        0     1544 2023-05-08 23:22:02.211065 windmill_api-1.96.3/windmill_api/models/remove_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1567 2023-05-08 23:22:02.279066 windmill_api-1.96.3/windmill_api/models/remove_user_to_group_json_body.py
--rw-r--r--   0        0        0     3367 2023-05-08 23:22:02.259066 windmill_api-1.96.3/windmill_api/models/resource.py
--rw-r--r--   0        0        0     1189 2023-05-08 23:22:02.279066 windmill_api-1.96.3/windmill_api/models/resource_extra_perms.py
--rw-r--r--   0        0        0     2256 2023-05-08 23:22:02.387067 windmill_api-1.96.3/windmill_api/models/resource_type.py
--rw-r--r--   0        0        0     1278 2023-05-08 23:22:02.299066 windmill_api-1.96.3/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
--rw-r--r--   0        0        0     1255 2023-05-08 23:22:02.315066 windmill_api-1.96.3/windmill_api/models/resume_suspended_job_post_json_body.py
--rw-r--r--   0        0        0     2546 2023-05-08 23:22:02.355067 windmill_api-1.96.3/windmill_api/models/retry.py
--rw-r--r--   0        0        0     1751 2023-05-08 23:22:02.383067 windmill_api-1.96.3/windmill_api/models/retry_constant.py
--rw-r--r--   0        0        0     2055 2023-05-08 23:22:02.415068 windmill_api-1.96.3/windmill_api/models/retry_exponential.py
--rw-r--r--   0        0        0     1210 2023-05-08 23:22:02.407068 windmill_api-1.96.3/windmill_api/models/run_flow_by_path_json_body.py
--rw-r--r--   0        0        0     2189 2023-05-08 23:22:02.439068 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body.py
--rw-r--r--   0        0        0     1235 2023-05-08 23:22:02.431068 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_args.py
--rw-r--r--   0        0        0     3265 2023-05-08 23:22:02.471069 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value.py
--rw-r--r--   0        0        0     7049 2023-05-08 23:22:02.519069 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3284 2023-05-08 23:22:02.511069 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1975 2023-05-08 23:22:02.539070 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-05-08 23:22:02.551070 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-05-08 23:22:02.567070 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-05-08 23:21:42.010771 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-05-08 23:22:02.579070 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-05-08 23:21:41.954770 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-05-08 23:22:02.595070 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-05-08 23:22:02.607071 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6939 2023-05-08 23:22:02.735072 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3250 2023-05-08 23:22:02.643071 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1965 2023-05-08 23:22:02.671072 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2269 2023-05-08 23:22:02.703072 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2147 2023-05-08 23:22:02.731073 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      187 2023-05-08 23:21:42.774782 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2014 2023-05-08 23:22:02.759073 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      187 2023-05-08 23:21:42.602779 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1958 2023-05-08 23:22:02.763073 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2009 2023-05-08 23:22:02.783073 windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1220 2023-05-08 23:22:02.783073 windmill_api-1.96.3/windmill_api/models/run_script_by_hash_json_body.py
--rw-r--r--   0        0        0     1220 2023-05-08 23:22:02.803074 windmill_api-1.96.3/windmill_api/models/run_script_by_path_json_body.py
--rw-r--r--   0        0        0     2634 2023-05-08 23:22:02.819074 windmill_api-1.96.3/windmill_api/models/run_script_preview_json_body.py
--rw-r--r--   0        0        0     1245 2023-05-08 23:22:02.823074 windmill_api-1.96.3/windmill_api/models/run_script_preview_json_body_args.py
--rw-r--r--   0        0        0      211 2023-05-08 23:21:42.694781 windmill_api-1.96.3/windmill_api/models/run_script_preview_json_body_language.py
--rw-r--r--   0        0        0     1266 2023-05-08 23:22:02.839074 windmill_api-1.96.3/windmill_api/models/run_wait_result_flow_by_path_json_body.py
--rw-r--r--   0        0        0     1276 2023-05-08 23:22:02.911075 windmill_api-1.96.3/windmill_api/models/run_wait_result_script_by_path_json_body.py
--rw-r--r--   0        0        0      203 2023-05-08 23:21:42.646780 windmill_api-1.96.3/windmill_api/models/runnable_type.py
--rw-r--r--   0        0        0     4086 2023-05-08 23:22:02.899075 windmill_api-1.96.3/windmill_api/models/schedule.py
--rw-r--r--   0        0        0     1153 2023-05-08 23:22:02.919075 windmill_api-1.96.3/windmill_api/models/schedule_args.py
--rw-r--r--   0        0        0     1189 2023-05-08 23:22:02.931075 windmill_api-1.96.3/windmill_api/models/schedule_extra_perms.py
--rw-r--r--   0        0        0     7003 2023-05-08 23:22:03.007076 windmill_api-1.96.3/windmill_api/models/script.py
--rw-r--r--   0        0        0     1143 2023-05-08 23:22:02.951076 windmill_api-1.96.3/windmill_api/models/script_args.py
--rw-r--r--   0        0        0     1179 2023-05-08 23:22:02.971076 windmill_api-1.96.3/windmill_api/models/script_extra_perms.py
--rw-r--r--   0        0        0      235 2023-05-08 23:21:42.570779 windmill_api-1.96.3/windmill_api/models/script_kind.py
--rw-r--r--   0        0        0      193 2023-05-08 23:21:42.782782 windmill_api-1.96.3/windmill_api/models/script_language.py
--rw-r--r--   0        0        0     1153 2023-05-08 23:22:02.991076 windmill_api-1.96.3/windmill_api/models/script_schema.py
--rw-r--r--   0        0        0     1440 2023-05-08 23:22:03.015076 windmill_api-1.96.3/windmill_api/models/set_password_json_body.py
--rw-r--r--   0        0        0     1470 2023-05-08 23:22:03.027077 windmill_api-1.96.3/windmill_api/models/set_schedule_enabled_json_body.py
--rw-r--r--   0        0        0     2032 2023-05-08 23:22:03.047077 windmill_api-1.96.3/windmill_api/models/slack_token.py
--rw-r--r--   0        0        0     1586 2023-05-08 23:22:03.051077 windmill_api-1.96.3/windmill_api/models/slack_token_bot.py
--rw-r--r--   0        0        0     2227 2023-05-08 23:22:03.079077 windmill_api-1.96.3/windmill_api/models/star_json_body.py
--rw-r--r--   0        0        0      209 2023-05-08 23:21:42.706781 windmill_api-1.96.3/windmill_api/models/star_json_body_favorite_kind.py
--rw-r--r--   0        0        0     1772 2023-05-08 23:22:03.151078 windmill_api-1.96.3/windmill_api/models/static_transform.py
--rw-r--r--   0        0        0      154 2023-05-08 23:21:42.482778 windmill_api-1.96.3/windmill_api/models/static_transform_type.py
--rw-r--r--   0        0        0     2462 2023-05-08 23:22:03.119078 windmill_api-1.96.3/windmill_api/models/token_response.py
--rw-r--r--   0        0        0     2921 2023-05-08 23:22:03.159078 windmill_api-1.96.3/windmill_api/models/truncated_token.py
--rw-r--r--   0        0        0     2249 2023-05-08 23:22:03.183079 windmill_api-1.96.3/windmill_api/models/unstar_json_body.py
--rw-r--r--   0        0        0      211 2023-05-08 23:21:42.666780 windmill_api-1.96.3/windmill_api/models/unstar_json_body_favorite_kind.py
--rw-r--r--   0        0        0     2638 2023-05-08 23:22:03.199079 windmill_api-1.96.3/windmill_api/models/update_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-05-08 23:22:03.227079 windmill_api-1.96.3/windmill_api/models/update_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-05-08 23:21:42.306775 windmill_api-1.96.3/windmill_api/models/update_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-05-08 23:22:03.223080 windmill_api-1.96.3/windmill_api/models/update_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-05-08 23:22:03.243080 windmill_api-1.96.3/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-05-08 23:22:03.271080 windmill_api-1.96.3/windmill_api/models/update_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-05-08 23:22:03.263080 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-05-08 23:22:03.303081 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-05-08 23:22:03.347081 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-05-08 23:22:03.339081 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-05-08 23:22:03.367081 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-05-08 23:22:03.379082 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-05-08 23:22:03.395082 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-05-08 23:21:42.678781 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-05-08 23:22:03.407082 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-05-08 23:21:42.822783 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-05-08 23:22:03.423082 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-05-08 23:22:03.435083 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-05-08 23:22:03.575085 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-05-08 23:22:03.471083 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-05-08 23:22:03.499083 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-05-08 23:22:03.595085 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-05-08 23:22:03.607085 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-05-08 23:21:42.390776 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-05-08 23:22:03.619085 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-05-08 23:21:42.578779 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-05-08 23:22:03.635085 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-05-08 23:22:03.647086 windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1949 2023-05-08 23:22:03.663086 windmill_api-1.96.3/windmill_api/models/update_folder_json_body.py
--rw-r--r--   0        0        0     1520 2023-05-08 23:22:03.671086 windmill_api-1.96.3/windmill_api/models/update_group_json_body.py
--rw-r--r--   0        0        0     1670 2023-05-08 23:22:03.691086 windmill_api-1.96.3/windmill_api/models/update_input.py
--rw-r--r--   0        0        0     1716 2023-05-08 23:22:03.699086 windmill_api-1.96.3/windmill_api/models/update_input_json_body.py
--rw-r--r--   0        0        0     1985 2023-05-08 23:22:03.723087 windmill_api-1.96.3/windmill_api/models/update_raw_app_json_body.py
--rw-r--r--   0        0        0     2036 2023-05-08 23:22:03.731087 windmill_api-1.96.3/windmill_api/models/update_resource_json_body.py
--rw-r--r--   0        0        0     1847 2023-05-08 23:22:03.751087 windmill_api-1.96.3/windmill_api/models/update_resource_type_json_body.py
--rw-r--r--   0        0        0     1541 2023-05-08 23:22:03.755087 windmill_api-1.96.3/windmill_api/models/update_resource_value_json_body.py
--rw-r--r--   0        0        0     1953 2023-05-08 23:22:03.779087 windmill_api-1.96.3/windmill_api/models/update_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-05-08 23:22:03.771087 windmill_api-1.96.3/windmill_api/models/update_schedule_json_body_args.py
--rw-r--r--   0        0        0     2066 2023-05-08 23:22:03.803088 windmill_api-1.96.3/windmill_api/models/update_user_json_body.py
--rw-r--r--   0        0        0     2316 2023-05-08 23:22:03.815088 windmill_api-1.96.3/windmill_api/models/update_variable_json_body.py
--rw-r--r--   0        0        0     1478 2023-05-08 23:22:03.831088 windmill_api-1.96.3/windmill_api/models/usage.py
--rw-r--r--   0        0        0     4071 2023-05-08 23:22:03.871089 windmill_api-1.96.3/windmill_api/models/user.py
--rw-r--r--   0        0        0     1501 2023-05-08 23:22:03.855089 windmill_api-1.96.3/windmill_api/models/user_usage.py
--rw-r--r--   0        0        0     2122 2023-05-08 23:22:03.883089 windmill_api-1.96.3/windmill_api/models/user_workspace_list.py
--rw-r--r--   0        0        0     1767 2023-05-08 23:22:03.899089 windmill_api-1.96.3/windmill_api/models/user_workspace_list_workspaces_item.py
--rw-r--r--   0        0        0     4222 2023-05-08 23:22:03.939090 windmill_api-1.96.3/windmill_api/models/whoami_response_200.py
--rw-r--r--   0        0        0     1572 2023-05-08 23:22:03.923089 windmill_api-1.96.3/windmill_api/models/whoami_response_200_usage.py
--rw-r--r--   0        0        0     4211 2023-05-08 23:22:03.979090 windmill_api-1.96.3/windmill_api/models/whois_response_200.py
--rw-r--r--   0        0        0     1567 2023-05-08 23:22:03.963090 windmill_api-1.96.3/windmill_api/models/whois_response_200_usage.py
--rw-r--r--   0        0        0     2604 2023-05-08 23:22:03.999091 windmill_api-1.96.3/windmill_api/models/worker_ping.py
--rw-r--r--   0        0        0     1901 2023-05-08 23:22:04.011091 windmill_api-1.96.3/windmill_api/models/workspace.py
--rw-r--r--   0        0        0     1974 2023-05-08 23:22:04.031091 windmill_api-1.96.3/windmill_api/models/workspace_invite.py
--rw-r--r--   0        0        0       25 2023-05-08 23:21:32.598631 windmill_api-1.96.3/windmill_api/py.typed
--rw-r--r--   0        0        0      939 2023-05-08 23:22:04.023091 windmill_api-1.96.3/windmill_api/types.py
--rw-r--r--   0        0        0     4362 1970-01-01 00:00:00.000000 windmill_api-1.96.3/setup.py
--rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.96.3/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-05-09 11:11:47.102559 windmill_api-1.97.0/LICENSE
+-rw-r--r--   0        0        0     2952 2023-05-09 11:11:47.110559 windmill_api-1.97.0/README.md
+-rw-r--r--   0        0        0      717 2023-05-09 11:11:47.106559 windmill_api-1.97.0/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-05-09 11:11:00.994841 windmill_api-1.97.0/windmill_api/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-09 11:11:01.702835 windmill_api-1.97.0/windmill_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.874834 windmill_api-1.97.0/windmill_api/api/app/__init__.py
+-rw-r--r--   0        0        0     1999 2023-05-09 11:11:15.414741 windmill_api-1.97.0/windmill_api/api/app/create_app.py
+-rw-r--r--   0        0        0     1769 2023-05-09 11:11:15.410741 windmill_api-1.97.0/windmill_api/api/app/delete_app.py
+-rw-r--r--   0        0        0     2214 2023-05-09 11:11:15.454741 windmill_api-1.97.0/windmill_api/api/app/execute_component.py
+-rw-r--r--   0        0        0     2782 2023-05-09 11:11:15.490740 windmill_api-1.97.0/windmill_api/api/app/exists_app.py
+-rw-r--r--   0        0        0     3020 2023-05-09 11:11:15.510740 windmill_api-1.97.0/windmill_api/api/app/get_app_by_path.py
+-rw-r--r--   0        0        0     3187 2023-05-09 11:11:15.546740 windmill_api-1.97.0/windmill_api/api/app/get_app_by_path_with_draft.py
+-rw-r--r--   0        0        0     3031 2023-05-09 11:11:15.566740 windmill_api-1.97.0/windmill_api/api/app/get_app_by_version.py
+-rw-r--r--   0        0        0     2649 2023-05-09 11:11:15.614740 windmill_api-1.97.0/windmill_api/api/app/get_hub_app_by_id.py
+-rw-r--r--   0        0        0     3168 2023-05-09 11:11:15.634739 windmill_api-1.97.0/windmill_api/api/app/get_public_app_by_secret.py
+-rw-r--r--   0        0        0     1797 2023-05-09 11:11:15.650739 windmill_api-1.97.0/windmill_api/api/app/get_public_secret_of_app.py
+-rw-r--r--   0        0        0     7289 2023-05-09 11:11:15.766739 windmill_api-1.97.0/windmill_api/api/app/list_apps.py
+-rw-r--r--   0        0        0     2405 2023-05-09 11:11:15.698739 windmill_api-1.97.0/windmill_api/api/app/list_hub_apps.py
+-rw-r--r--   0        0        0     2140 2023-05-09 11:11:15.738739 windmill_api-1.97.0/windmill_api/api/app/update_app.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.754835 windmill_api-1.97.0/windmill_api/api/audit/__init__.py
+-rw-r--r--   0        0        0     3065 2023-05-09 11:11:15.802739 windmill_api-1.97.0/windmill_api/api/audit/get_audit_log.py
+-rw-r--r--   0        0        0     8723 2023-05-09 11:11:15.914738 windmill_api-1.97.0/windmill_api/api/audit/list_audit_logs.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.954833 windmill_api-1.97.0/windmill_api/api/capture/__init__.py
+-rw-r--r--   0        0        0     1796 2023-05-09 11:11:15.846738 windmill_api-1.97.0/windmill_api/api/capture/create_capture.py
+-rw-r--r--   0        0        0     1790 2023-05-09 11:11:15.890738 windmill_api-1.97.0/windmill_api/api/capture/get_capture.py
+-rw-r--r--   0        0        0     1799 2023-05-09 11:11:15.930738 windmill_api-1.97.0/windmill_api/api/capture/update_capture.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.886834 windmill_api-1.97.0/windmill_api/api/draft/__init__.py
+-rw-r--r--   0        0        0     2019 2023-05-09 11:11:15.954738 windmill_api-1.97.0/windmill_api/api/draft/create_draft.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.954833 windmill_api-1.97.0/windmill_api/api/favorite/__init__.py
+-rw-r--r--   0        0        0     1964 2023-05-09 11:11:15.978737 windmill_api-1.97.0/windmill_api/api/favorite/star.py
+-rw-r--r--   0        0        0     1984 2023-05-09 11:11:15.998737 windmill_api-1.97.0/windmill_api/api/favorite/unstar.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.838834 windmill_api-1.97.0/windmill_api/api/flow/__init__.py
+-rw-r--r--   0        0        0     2220 2023-05-09 11:11:16.026737 windmill_api-1.97.0/windmill_api/api/flow/archive_flow_by_path.py
+-rw-r--r--   0        0        0     2009 2023-05-09 11:11:16.034737 windmill_api-1.97.0/windmill_api/api/flow/create_flow.py
+-rw-r--r--   0        0        0     1788 2023-05-09 11:11:16.066737 windmill_api-1.97.0/windmill_api/api/flow/delete_flow_by_path.py
+-rw-r--r--   0        0        0     2755 2023-05-09 11:11:16.122737 windmill_api-1.97.0/windmill_api/api/flow/exists_flow_by_path.py
+-rw-r--r--   0        0        0     3036 2023-05-09 11:11:16.142736 windmill_api-1.97.0/windmill_api/api/flow/get_flow_by_path.py
+-rw-r--r--   0        0        0     3205 2023-05-09 11:11:16.178736 windmill_api-1.97.0/windmill_api/api/flow/get_flow_by_path_with_draft.py
+-rw-r--r--   0        0        0     4827 2023-05-09 11:11:16.222736 windmill_api-1.97.0/windmill_api/api/flow/get_flow_input_history_by_path.py
+-rw-r--r--   0        0        0     2667 2023-05-09 11:11:16.226736 windmill_api-1.97.0/windmill_api/api/flow/get_hub_flow_by_id.py
+-rw-r--r--   0        0        0     1668 2023-05-09 11:11:16.258736 windmill_api-1.97.0/windmill_api/api/flow/list_flow_paths.py
+-rw-r--r--   0        0        0     7969 2023-05-09 11:11:16.362735 windmill_api-1.97.0/windmill_api/api/flow/list_flows.py
+-rw-r--r--   0        0        0     2423 2023-05-09 11:11:16.306735 windmill_api-1.97.0/windmill_api/api/flow/list_hub_flows.py
+-rw-r--r--   0        0        0     2150 2023-05-09 11:11:16.394735 windmill_api-1.97.0/windmill_api/api/flow/update_flow.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.942833 windmill_api-1.97.0/windmill_api/api/folder/__init__.py
+-rw-r--r--   0        0        0     2214 2023-05-09 11:11:16.410735 windmill_api-1.97.0/windmill_api/api/folder/add_owner_to_folder.py
+-rw-r--r--   0        0        0     2029 2023-05-09 11:11:16.450734 windmill_api-1.97.0/windmill_api/api/folder/create_folder.py
+-rw-r--r--   0        0        0     1778 2023-05-09 11:11:16.498734 windmill_api-1.97.0/windmill_api/api/folder/delete_folder.py
+-rw-r--r--   0        0        0     2960 2023-05-09 11:11:16.510734 windmill_api-1.97.0/windmill_api/api/folder/get_folder.py
+-rw-r--r--   0        0        0     3055 2023-05-09 11:11:16.658733 windmill_api-1.97.0/windmill_api/api/folder/get_folder_usage.py
+-rw-r--r--   0        0        0     3405 2023-05-09 11:11:16.582734 windmill_api-1.97.0/windmill_api/api/folder/list_folder_names.py
+-rw-r--r--   0        0        0     4251 2023-05-09 11:11:16.694733 windmill_api-1.97.0/windmill_api/api/folder/list_folders.py
+-rw-r--r--   0        0        0     2244 2023-05-09 11:11:16.726733 windmill_api-1.97.0/windmill_api/api/folder/remove_owner_to_folder.py
+-rw-r--r--   0        0        0     2170 2023-05-09 11:11:16.754733 windmill_api-1.97.0/windmill_api/api/folder/update_folder.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.950833 windmill_api-1.97.0/windmill_api/api/granular_acl/__init__.py
+-rw-r--r--   0        0        0     2480 2023-05-09 11:11:16.774732 windmill_api-1.97.0/windmill_api/api/granular_acl/add_granular_acls.py
+-rw-r--r--   0        0        0     3526 2023-05-09 11:11:16.822732 windmill_api-1.97.0/windmill_api/api/granular_acl/get_granular_acls.py
+-rw-r--r--   0        0        0     2545 2023-05-09 11:11:16.818732 windmill_api-1.97.0/windmill_api/api/granular_acl/remove_granular_acls.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.934833 windmill_api-1.97.0/windmill_api/api/group/__init__.py
+-rw-r--r--   0        0        0     2194 2023-05-09 11:11:16.866732 windmill_api-1.97.0/windmill_api/api/group/add_user_to_group.py
+-rw-r--r--   0        0        0     2019 2023-05-09 11:11:16.862732 windmill_api-1.97.0/windmill_api/api/group/create_group.py
+-rw-r--r--   0        0        0     1775 2023-05-09 11:11:16.902732 windmill_api-1.97.0/windmill_api/api/group/delete_group.py
+-rw-r--r--   0        0        0     2942 2023-05-09 11:11:16.922732 windmill_api-1.97.0/windmill_api/api/group/get_group.py
+-rw-r--r--   0        0        0     3400 2023-05-09 11:11:16.966731 windmill_api-1.97.0/windmill_api/api/group/list_group_names.py
+-rw-r--r--   0        0        0     4233 2023-05-09 11:11:17.006731 windmill_api-1.97.0/windmill_api/api/group/list_groups.py
+-rw-r--r--   0        0        0     2224 2023-05-09 11:11:17.010731 windmill_api-1.97.0/windmill_api/api/group/remove_user_to_group.py
+-rw-r--r--   0        0        0     2160 2023-05-09 11:11:17.054731 windmill_api-1.97.0/windmill_api/api/group/update_group.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.958833 windmill_api-1.97.0/windmill_api/api/input_/__init__.py
+-rw-r--r--   0        0        0     3338 2023-05-09 11:11:17.078731 windmill_api-1.97.0/windmill_api/api/input_/create_input.py
+-rw-r--r--   0        0        0     1811 2023-05-09 11:11:17.094731 windmill_api-1.97.0/windmill_api/api/input_/delete_input.py
+-rw-r--r--   0        0        0     6187 2023-05-09 11:11:17.198730 windmill_api-1.97.0/windmill_api/api/input_/get_input_history.py
+-rw-r--r--   0        0        0     6010 2023-05-09 11:11:17.198730 windmill_api-1.97.0/windmill_api/api/input_/list_inputs.py
+-rw-r--r--   0        0        0     2025 2023-05-09 11:11:17.238730 windmill_api-1.97.0/windmill_api/api/input_/update_input.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.890833 windmill_api-1.97.0/windmill_api/api/job/__init__.py
+-rw-r--r--   0        0        0     2181 2023-05-09 11:11:17.266730 windmill_api-1.97.0/windmill_api/api/job/cancel_queued_job.py
+-rw-r--r--   0        0        0     2687 2023-05-09 11:11:17.302729 windmill_api-1.97.0/windmill_api/api/job/cancel_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-05-09 11:11:17.330729 windmill_api-1.97.0/windmill_api/api/job/cancel_suspended_job_post.py
+-rw-r--r--   0        0        0     2535 2023-05-09 11:11:17.358729 windmill_api-1.97.0/windmill_api/api/job/create_job_signature.py
+-rw-r--r--   0        0        0     3217 2023-05-09 11:11:17.390729 windmill_api-1.97.0/windmill_api/api/job/delete_completed_job.py
+-rw-r--r--   0        0        0     2235 2023-05-09 11:11:17.402729 windmill_api-1.97.0/windmill_api/api/job/force_cancel_queued_job.py
+-rw-r--r--   0        0        0     3034 2023-05-09 11:11:17.454728 windmill_api-1.97.0/windmill_api/api/job/get_completed_job.py
+-rw-r--r--   0        0        0     1784 2023-05-09 11:11:17.442729 windmill_api-1.97.0/windmill_api/api/job/get_completed_job_result.py
+-rw-r--r--   0        0        0     2868 2023-05-09 11:11:17.502728 windmill_api-1.97.0/windmill_api/api/job/get_job.py
+-rw-r--r--   0        0        0     4305 2023-05-09 11:11:17.538728 windmill_api-1.97.0/windmill_api/api/job/get_job_updates.py
+-rw-r--r--   0        0        0     4306 2023-05-09 11:11:17.582728 windmill_api-1.97.0/windmill_api/api/job/get_resume_urls.py
+-rw-r--r--   0        0        0     4601 2023-05-09 11:11:17.622727 windmill_api-1.97.0/windmill_api/api/job/get_suspended_job_flow.py
+-rw-r--r--   0        0        0    13065 2023-05-09 11:11:17.822726 windmill_api-1.97.0/windmill_api/api/job/list_completed_jobs.py
+-rw-r--r--   0        0        0    12292 2023-05-09 11:11:17.850726 windmill_api-1.97.0/windmill_api/api/job/list_jobs.py
+-rw-r--r--   0        0        0    12830 2023-05-09 11:11:18.026725 windmill_api-1.97.0/windmill_api/api/job/list_queue.py
+-rw-r--r--   0        0        0     2067 2023-05-09 11:11:17.894726 windmill_api-1.97.0/windmill_api/api/job/result_by_id.py
+-rw-r--r--   0        0        0     2313 2023-05-09 11:11:17.934726 windmill_api-1.97.0/windmill_api/api/job/resume_suspended_flow_as_owner.py
+-rw-r--r--   0        0        0     2994 2023-05-09 11:11:17.990725 windmill_api-1.97.0/windmill_api/api/job/resume_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-05-09 11:11:18.050725 windmill_api-1.97.0/windmill_api/api/job/resume_suspended_job_post.py
+-rw-r--r--   0        0        0     4566 2023-05-09 11:11:18.110725 windmill_api-1.97.0/windmill_api/api/job/run_flow_by_path.py
+-rw-r--r--   0        0        0     3037 2023-05-09 11:11:18.110725 windmill_api-1.97.0/windmill_api/api/job/run_flow_preview.py
+-rw-r--r--   0        0        0     4594 2023-05-09 11:11:18.194724 windmill_api-1.97.0/windmill_api/api/job/run_script_by_hash.py
+-rw-r--r--   0        0        0     4200 2023-05-09 11:11:18.186724 windmill_api-1.97.0/windmill_api/api/job/run_script_by_path.py
+-rw-r--r--   0        0        0     3050 2023-05-09 11:11:18.274724 windmill_api-1.97.0/windmill_api/api/job/run_script_preview.py
+-rw-r--r--   0        0        0     3215 2023-05-09 11:11:18.282724 windmill_api-1.97.0/windmill_api/api/job/run_wait_result_flow_by_path.py
+-rw-r--r--   0        0        0     3521 2023-05-09 11:11:18.338723 windmill_api-1.97.0/windmill_api/api/job/run_wait_result_script_by_path.py
+-rw-r--r--   0        0        0     3356 2023-05-09 11:11:18.362723 windmill_api-1.97.0/windmill_api/api/job/run_wait_result_script_by_path_get.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.798834 windmill_api-1.97.0/windmill_api/api/oauth/__init__.py
+-rw-r--r--   0        0        0     3506 2023-05-09 11:11:18.398723 windmill_api-1.97.0/windmill_api/api/oauth/connect_callback.py
+-rw-r--r--   0        0        0     2118 2023-05-09 11:11:18.410723 windmill_api-1.97.0/windmill_api/api/oauth/connect_slack_callback.py
+-rw-r--r--   0        0        0     2056 2023-05-09 11:11:18.438722 windmill_api-1.97.0/windmill_api/api/oauth/create_account.py
+-rw-r--r--   0        0        0     1764 2023-05-09 11:11:18.454723 windmill_api-1.97.0/windmill_api/api/oauth/disconnect_account.py
+-rw-r--r--   0        0        0     1649 2023-05-09 11:11:18.478722 windmill_api-1.97.0/windmill_api/api/oauth/disconnect_slack.py
+-rw-r--r--   0        0        0     1426 2023-05-09 11:11:18.490722 windmill_api-1.97.0/windmill_api/api/oauth/list_o_auth_connects.py
+-rw-r--r--   0        0        0     2162 2023-05-09 11:11:18.526722 windmill_api-1.97.0/windmill_api/api/oauth/list_o_auth_logins.py
+-rw-r--r--   0        0        0     2151 2023-05-09 11:11:18.538722 windmill_api-1.97.0/windmill_api/api/oauth/refresh_token.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.922833 windmill_api-1.97.0/windmill_api/api/raw_app/__init__.py
+-rw-r--r--   0        0        0     2033 2023-05-09 11:11:18.570722 windmill_api-1.97.0/windmill_api/api/raw_app/create_raw_app.py
+-rw-r--r--   0        0        0     1781 2023-05-09 11:11:18.594722 windmill_api-1.97.0/windmill_api/api/raw_app/delete_raw_app.py
+-rw-r--r--   0        0        0     2786 2023-05-09 11:11:18.630721 windmill_api-1.97.0/windmill_api/api/raw_app/exists_raw_app.py
+-rw-r--r--   0        0        0     1979 2023-05-09 11:11:18.638721 windmill_api-1.97.0/windmill_api/api/raw_app/get_raw_app_data.py
+-rw-r--r--   0        0        0     7349 2023-05-09 11:11:18.770721 windmill_api-1.97.0/windmill_api/api/raw_app/list_raw_apps.py
+-rw-r--r--   0        0        0     2166 2023-05-09 11:11:18.682721 windmill_api-1.97.0/windmill_api/api/raw_app/update_raw_app.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.806834 windmill_api-1.97.0/windmill_api/api/resource/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-09 11:11:18.726721 windmill_api-1.97.0/windmill_api/api/resource/create_resource.py
+-rw-r--r--   0        0        0     2093 2023-05-09 11:11:18.766721 windmill_api-1.97.0/windmill_api/api/resource/create_resource_type.py
+-rw-r--r--   0        0        0     1784 2023-05-09 11:11:18.830720 windmill_api-1.97.0/windmill_api/api/resource/delete_resource.py
+-rw-r--r--   0        0        0     1799 2023-05-09 11:11:18.810720 windmill_api-1.97.0/windmill_api/api/resource/delete_resource_type.py
+-rw-r--r--   0        0        0     2763 2023-05-09 11:11:18.866720 windmill_api-1.97.0/windmill_api/api/resource/exists_resource.py
+-rw-r--r--   0        0        0     2788 2023-05-09 11:11:18.886720 windmill_api-1.97.0/windmill_api/api/resource/exists_resource_type.py
+-rw-r--r--   0        0        0     2996 2023-05-09 11:11:18.922720 windmill_api-1.97.0/windmill_api/api/resource/get_resource.py
+-rw-r--r--   0        0        0     3074 2023-05-09 11:11:18.950719 windmill_api-1.97.0/windmill_api/api/resource/get_resource_type.py
+-rw-r--r--   0        0        0     1790 2023-05-09 11:11:18.962719 windmill_api-1.97.0/windmill_api/api/resource/get_resource_value.py
+-rw-r--r--   0        0        0     5732 2023-05-09 11:11:19.054719 windmill_api-1.97.0/windmill_api/api/resource/list_resource.py
+-rw-r--r--   0        0        0     3149 2023-05-09 11:11:19.022719 windmill_api-1.97.0/windmill_api/api/resource/list_resource_type.py
+-rw-r--r--   0        0        0     2600 2023-05-09 11:11:19.078719 windmill_api-1.97.0/windmill_api/api/resource/list_resource_type_names.py
+-rw-r--r--   0        0        0     2190 2023-05-09 11:11:19.102718 windmill_api-1.97.0/windmill_api/api/resource/update_resource.py
+-rw-r--r--   0        0        0     2234 2023-05-09 11:11:19.122718 windmill_api-1.97.0/windmill_api/api/resource/update_resource_type.py
+-rw-r--r--   0        0        0     2244 2023-05-09 11:11:19.150718 windmill_api-1.97.0/windmill_api/api/resource/update_resource_value.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.926833 windmill_api-1.97.0/windmill_api/api/schedule/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-09 11:11:19.174718 windmill_api-1.97.0/windmill_api/api/schedule/create_schedule.py
+-rw-r--r--   0        0        0     1784 2023-05-09 11:11:19.198718 windmill_api-1.97.0/windmill_api/api/schedule/delete_schedule.py
+-rw-r--r--   0        0        0     2763 2023-05-09 11:11:19.254718 windmill_api-1.97.0/windmill_api/api/schedule/exists_schedule.py
+-rw-r--r--   0        0        0     2996 2023-05-09 11:11:19.258718 windmill_api-1.97.0/windmill_api/api/schedule/get_schedule.py
+-rw-r--r--   0        0        0     4287 2023-05-09 11:11:19.342717 windmill_api-1.97.0/windmill_api/api/schedule/list_schedules.py
+-rw-r--r--   0        0        0     3217 2023-05-09 11:11:19.342717 windmill_api-1.97.0/windmill_api/api/schedule/preview_schedule.py
+-rw-r--r--   0        0        0     2233 2023-05-09 11:11:19.394717 windmill_api-1.97.0/windmill_api/api/schedule/set_schedule_enabled.py
+-rw-r--r--   0        0        0     2190 2023-05-09 11:11:19.386717 windmill_api-1.97.0/windmill_api/api/schedule/update_schedule.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.818834 windmill_api-1.97.0/windmill_api/api/script/__init__.py
+-rw-r--r--   0        0        0     3165 2023-05-09 11:11:19.454716 windmill_api-1.97.0/windmill_api/api/script/archive_script_by_hash.py
+-rw-r--r--   0        0        0     1797 2023-05-09 11:11:19.434717 windmill_api-1.97.0/windmill_api/api/script/archive_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-05-09 11:11:19.494716 windmill_api-1.97.0/windmill_api/api/script/bash_to_jsonschema.py
+-rw-r--r--   0        0        0     2029 2023-05-09 11:11:19.498716 windmill_api-1.97.0/windmill_api/api/script/create_script.py
+-rw-r--r--   0        0        0     3327 2023-05-09 11:11:19.550716 windmill_api-1.97.0/windmill_api/api/script/delete_script_by_hash.py
+-rw-r--r--   0        0        0     2873 2023-05-09 11:11:19.558716 windmill_api-1.97.0/windmill_api/api/script/delete_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-05-09 11:11:19.610715 windmill_api-1.97.0/windmill_api/api/script/deno_to_jsonschema.py
+-rw-r--r--   0        0        0     2767 2023-05-09 11:11:19.618715 windmill_api-1.97.0/windmill_api/api/script/exists_script_by_path.py
+-rw-r--r--   0        0        0     2802 2023-05-09 11:11:19.666715 windmill_api-1.97.0/windmill_api/api/script/get_hub_script_by_path.py
+-rw-r--r--   0        0        0     1607 2023-05-09 11:11:19.658715 windmill_api-1.97.0/windmill_api/api/script/get_hub_script_content_by_path.py
+-rw-r--r--   0        0        0     3092 2023-05-09 11:11:19.722715 windmill_api-1.97.0/windmill_api/api/script/get_script_by_hash.py
+-rw-r--r--   0        0        0     3074 2023-05-09 11:11:19.746715 windmill_api-1.97.0/windmill_api/api/script/get_script_by_path.py
+-rw-r--r--   0        0        0     3241 2023-05-09 11:11:19.786714 windmill_api-1.97.0/windmill_api/api/script/get_script_by_path_with_draft.py
+-rw-r--r--   0        0        0     3276 2023-05-09 11:11:19.802714 windmill_api-1.97.0/windmill_api/api/script/get_script_deployment_status.py
+-rw-r--r--   0        0        0     2967 2023-05-09 11:11:19.858714 windmill_api-1.97.0/windmill_api/api/script/go_to_jsonschema.py
+-rw-r--r--   0        0        0     2459 2023-05-09 11:11:19.850714 windmill_api-1.97.0/windmill_api/api/script/list_hub_scripts.py
+-rw-r--r--   0        0        0     1676 2023-05-09 11:11:19.890714 windmill_api-1.97.0/windmill_api/api/script/list_script_paths.py
+-rw-r--r--   0        0        0    11165 2023-05-09 11:11:20.042713 windmill_api-1.97.0/windmill_api/api/script/list_scripts.py
+-rw-r--r--   0        0        0     3039 2023-05-09 11:11:19.942713 windmill_api-1.97.0/windmill_api/api/script/python_to_jsonschema.py
+-rw-r--r--   0        0        0     1784 2023-05-09 11:11:19.982713 windmill_api-1.97.0/windmill_api/api/script/raw_script_by_hash.py
+-rw-r--r--   0        0        0     1784 2023-05-09 11:11:20.022713 windmill_api-1.97.0/windmill_api/api/script/raw_script_by_path.py
+-rw-r--r--   0        0        0     2119 2023-05-09 11:11:20.070713 windmill_api-1.97.0/windmill_api/api/script/raw_script_by_path_tokened.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.718835 windmill_api-1.97.0/windmill_api/api/settings/__init__.py
+-rw-r--r--   0        0        0     1414 2023-05-09 11:11:20.082713 windmill_api-1.97.0/windmill_api/api/settings/backend_version.py
+-rw-r--r--   0        0        0     1423 2023-05-09 11:11:20.102712 windmill_api-1.97.0/windmill_api/api/settings/get_open_api_yaml.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.758834 windmill_api-1.97.0/windmill_api/api/user/__init__.py
+-rw-r--r--   0        0        0     1857 2023-05-09 11:11:20.134712 windmill_api-1.97.0/windmill_api/api/user/accept_invite.py
+-rw-r--r--   0        0        0     1822 2023-05-09 11:11:20.142712 windmill_api-1.97.0/windmill_api/api/user/create_token.py
+-rw-r--r--   0        0        0     1991 2023-05-09 11:11:20.174712 windmill_api-1.97.0/windmill_api/api/user/create_token_impersonate.py
+-rw-r--r--   0        0        0     2058 2023-05-09 11:11:20.202712 windmill_api-1.97.0/windmill_api/api/user/create_user.py
+-rw-r--r--   0        0        0     1863 2023-05-09 11:11:20.222712 windmill_api-1.97.0/windmill_api/api/user/create_user_globally.py
+-rw-r--r--   0        0        0     1867 2023-05-09 11:11:20.250712 windmill_api-1.97.0/windmill_api/api/user/decline_invite.py
+-rw-r--r--   0        0        0     1674 2023-05-09 11:11:20.262712 windmill_api-1.97.0/windmill_api/api/user/delete_token.py
+-rw-r--r--   0        0        0     1872 2023-05-09 11:11:20.294711 windmill_api-1.97.0/windmill_api/api/user/delete_user.py
+-rw-r--r--   0        0        0     1454 2023-05-09 11:11:20.294711 windmill_api-1.97.0/windmill_api/api/user/get_current_email.py
+-rw-r--r--   0        0        0     1474 2023-05-09 11:11:20.326711 windmill_api-1.97.0/windmill_api/api/user/get_usage.py
+-rw-r--r--   0        0        0     1639 2023-05-09 11:11:20.338711 windmill_api-1.97.0/windmill_api/api/user/global_user_delete.py
+-rw-r--r--   0        0        0     2060 2023-05-09 11:11:20.374711 windmill_api-1.97.0/windmill_api/api/user/global_user_update.py
+-rw-r--r--   0        0        0     2468 2023-05-09 11:11:20.414711 windmill_api-1.97.0/windmill_api/api/user/global_whoami.py
+-rw-r--r--   0        0        0     2745 2023-05-09 11:11:20.430710 windmill_api-1.97.0/windmill_api/api/user/is_owner_of_path.py
+-rw-r--r--   0        0        0     1646 2023-05-09 11:11:20.458710 windmill_api-1.97.0/windmill_api/api/user/leave_workspace.py
+-rw-r--r--   0        0        0     2633 2023-05-09 11:11:20.482710 windmill_api-1.97.0/windmill_api/api/user/list_tokens.py
+-rw-r--r--   0        0        0     2552 2023-05-09 11:11:20.518710 windmill_api-1.97.0/windmill_api/api/user/list_usernames.py
+-rw-r--r--   0        0        0     3012 2023-05-09 11:11:20.542710 windmill_api-1.97.0/windmill_api/api/user/list_users.py
+-rw-r--r--   0        0        0     4222 2023-05-09 11:11:20.614709 windmill_api-1.97.0/windmill_api/api/user/list_users_as_super_admin.py
+-rw-r--r--   0        0        0     2829 2023-05-09 11:11:20.594709 windmill_api-1.97.0/windmill_api/api/user/list_workspace_invites.py
+-rw-r--r--   0        0        0     1784 2023-05-09 11:11:20.634709 windmill_api-1.97.0/windmill_api/api/user/login.py
+-rw-r--r--   0        0        0     2116 2023-05-09 11:11:20.658709 windmill_api-1.97.0/windmill_api/api/user/login_with_oauth.py
+-rw-r--r--   0        0        0     1393 2023-05-09 11:11:20.666709 windmill_api-1.97.0/windmill_api/api/user/logout.py
+-rw-r--r--   0        0        0     1820 2023-05-09 11:11:20.702709 windmill_api-1.97.0/windmill_api/api/user/set_password.py
+-rw-r--r--   0        0        0     2250 2023-05-09 11:11:20.730709 windmill_api-1.97.0/windmill_api/api/user/update_user.py
+-rw-r--r--   0        0        0     2652 2023-05-09 11:11:20.762709 windmill_api-1.97.0/windmill_api/api/user/whoami.py
+-rw-r--r--   0        0        0     2967 2023-05-09 11:11:20.790708 windmill_api-1.97.0/windmill_api/api/user/whois.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.790834 windmill_api-1.97.0/windmill_api/api/variable/__init__.py
+-rw-r--r--   0        0        0     2634 2023-05-09 11:11:20.818708 windmill_api-1.97.0/windmill_api/api/variable/create_variable.py
+-rw-r--r--   0        0        0     1784 2023-05-09 11:11:20.834708 windmill_api-1.97.0/windmill_api/api/variable/delete_variable.py
+-rw-r--r--   0        0        0     2795 2023-05-09 11:11:20.882708 windmill_api-1.97.0/windmill_api/api/variable/exists_variable.py
+-rw-r--r--   0        0        0     3840 2023-05-09 11:11:20.910708 windmill_api-1.97.0/windmill_api/api/variable/get_variable.py
+-rw-r--r--   0        0        0     3270 2023-05-09 11:11:20.962707 windmill_api-1.97.0/windmill_api/api/variable/list_contextual_variables.py
+-rw-r--r--   0        0        0     3071 2023-05-09 11:11:20.970707 windmill_api-1.97.0/windmill_api/api/variable/list_variable.py
+-rw-r--r--   0        0        0     2775 2023-05-09 11:11:21.026707 windmill_api-1.97.0/windmill_api/api/variable/update_variable.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.886834 windmill_api-1.97.0/windmill_api/api/worker/__init__.py
+-rw-r--r--   0        0        0     2448 2023-05-09 11:11:21.022707 windmill_api-1.97.0/windmill_api/api/worker/get_custom_tags.py
+-rw-r--r--   0        0        0     3896 2023-05-09 11:11:21.106706 windmill_api-1.97.0/windmill_api/api/worker/list_workers.py
+-rw-r--r--   0        0        0        0 2023-05-09 11:11:01.778834 windmill_api-1.97.0/windmill_api/api/workspace/__init__.py
+-rw-r--r--   0        0        0     2015 2023-05-09 11:11:21.074707 windmill_api-1.97.0/windmill_api/api/workspace/add_user.py
+-rw-r--r--   0        0        0     1647 2023-05-09 11:11:21.118706 windmill_api-1.97.0/windmill_api/api/workspace/archive_workspace.py
+-rw-r--r--   0        0        0     1856 2023-05-09 11:11:21.150706 windmill_api-1.97.0/windmill_api/api/workspace/create_workspace.py
+-rw-r--r--   0        0        0     2049 2023-05-09 11:11:21.166706 windmill_api-1.97.0/windmill_api/api/workspace/delete_invite.py
+-rw-r--r--   0        0        0     1688 2023-05-09 11:11:21.210706 windmill_api-1.97.0/windmill_api/api/workspace/delete_workspace.py
+-rw-r--r--   0        0        0     2063 2023-05-09 11:11:21.210706 windmill_api-1.97.0/windmill_api/api/workspace/edit_auto_invite.py
+-rw-r--r--   0        0        0     2083 2023-05-09 11:11:21.298705 windmill_api-1.97.0/windmill_api/api/workspace/edit_slack_command.py
+-rw-r--r--   0        0        0     2029 2023-05-09 11:11:21.254706 windmill_api-1.97.0/windmill_api/api/workspace/edit_webhook.py
+-rw-r--r--   0        0        0     1856 2023-05-09 11:11:21.294705 windmill_api-1.97.0/windmill_api/api/workspace/exists_username.py
+-rw-r--r--   0        0        0     1856 2023-05-09 11:11:21.338705 windmill_api-1.97.0/windmill_api/api/workspace/exists_workspace.py
+-rw-r--r--   0        0        0     2809 2023-05-09 11:11:21.354705 windmill_api-1.97.0/windmill_api/api/workspace/get_premium_info.py
+-rw-r--r--   0        0        0     2753 2023-05-09 11:11:21.406705 windmill_api-1.97.0/windmill_api/api/workspace/get_settings.py
+-rw-r--r--   0        0        0     2045 2023-05-09 11:11:21.398705 windmill_api-1.97.0/windmill_api/api/workspace/invite_user.py
+-rw-r--r--   0        0        0     2176 2023-05-09 11:11:21.442705 windmill_api-1.97.0/windmill_api/api/workspace/is_domain_allowed.py
+-rw-r--r--   0        0        0     3255 2023-05-09 11:11:21.486704 windmill_api-1.97.0/windmill_api/api/workspace/list_pending_invites.py
+-rw-r--r--   0        0        0     2583 2023-05-09 11:11:21.494704 windmill_api-1.97.0/windmill_api/api/workspace/list_user_workspaces.py
+-rw-r--r--   0        0        0     2775 2023-05-09 11:11:21.542704 windmill_api-1.97.0/windmill_api/api/workspace/list_workspaces.py
+-rw-r--r--   0        0        0     4311 2023-05-09 11:11:21.574704 windmill_api-1.97.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py
+-rw-r--r--   0        0        0     1651 2023-05-09 11:11:21.586704 windmill_api-1.97.0/windmill_api/api/workspace/unarchive_workspace.py
+-rw-r--r--   0        0        0     1821 2023-05-09 11:11:21.614703 windmill_api-1.97.0/windmill_api/client.py
+-rw-r--r--   0        0        0        1 2023-05-09 11:11:47.098559 windmill_api-1.97.0/windmill_api/models/__init__.py
+-rw-r--r--   0        0        0     1667 2023-05-09 11:11:21.650703 windmill_api-1.97.0/windmill_api/models/accept_invite_json_body.py
+-rw-r--r--   0        0        0     1710 2023-05-09 11:11:21.694703 windmill_api-1.97.0/windmill_api/models/add_granular_acls_json_body.py
+-rw-r--r--   0        0        0      325 2023-05-09 11:11:13.490752 windmill_api-1.97.0/windmill_api/models/add_granular_acls_kind.py
+-rw-r--r--   0        0        0     1529 2023-05-09 11:11:21.730703 windmill_api-1.97.0/windmill_api/models/add_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1940 2023-05-09 11:11:21.794702 windmill_api-1.97.0/windmill_api/models/add_user_json_body.py
+-rw-r--r--   0        0        0     1552 2023-05-09 11:11:21.810702 windmill_api-1.97.0/windmill_api/models/add_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3940 2023-05-09 11:11:21.886702 windmill_api-1.97.0/windmill_api/models/app_with_last_version.py
+-rw-r--r--   0        0        0      214 2023-05-09 11:11:14.138749 windmill_api-1.97.0/windmill_api/models/app_with_last_version_execution_mode.py
+-rw-r--r--   0        0        0     1248 2023-05-09 11:11:21.842702 windmill_api-1.97.0/windmill_api/models/app_with_last_version_extra_perms.py
+-rw-r--r--   0        0        0     3716 2023-05-09 11:11:21.938701 windmill_api-1.97.0/windmill_api/models/app_with_last_version_policy.py
+-rw-r--r--   0        0        0      220 2023-05-09 11:11:14.206748 windmill_api-1.97.0/windmill_api/models/app_with_last_version_policy_execution_mode.py
+-rw-r--r--   0        0        0     1946 2023-05-09 11:11:21.926701 windmill_api-1.97.0/windmill_api/models/app_with_last_version_policy_triggerables.py
+-rw-r--r--   0        0        0     1381 2023-05-09 11:11:21.962701 windmill_api-1.97.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4638 2023-05-09 11:11:22.022701 windmill_api-1.97.0/windmill_api/models/app_with_last_version_w_draft.py
+-rw-r--r--   0        0        0      220 2023-05-09 11:11:14.230748 windmill_api-1.97.0/windmill_api/models/app_with_last_version_w_draft_execution_mode.py
+-rw-r--r--   0        0        0     1284 2023-05-09 11:11:21.998701 windmill_api-1.97.0/windmill_api/models/app_with_last_version_w_draft_extra_perms.py
+-rw-r--r--   0        0        0     3828 2023-05-09 11:11:22.070701 windmill_api-1.97.0/windmill_api/models/app_with_last_version_w_draft_policy.py
+-rw-r--r--   0        0        0      226 2023-05-09 11:11:13.630751 windmill_api-1.97.0/windmill_api/models/app_with_last_version_w_draft_policy_execution_mode.py
+-rw-r--r--   0        0        0     2020 2023-05-09 11:11:22.066701 windmill_api-1.97.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py
+-rw-r--r--   0        0        0     1417 2023-05-09 11:11:22.098700 windmill_api-1.97.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1569 2023-05-09 11:11:22.114700 windmill_api-1.97.0/windmill_api/models/archive_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     7662 2023-05-09 11:11:22.238700 windmill_api-1.97.0/windmill_api/models/archive_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1314 2023-05-09 11:11:22.142700 windmill_api-1.97.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      259 2023-05-09 11:11:14.526746 windmill_api-1.97.0/windmill_api/models/archive_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      217 2023-05-09 11:11:14.098749 windmill_api-1.97.0/windmill_api/models/archive_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1288 2023-05-09 11:11:22.182700 windmill_api-1.97.0/windmill_api/models/archive_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     3452 2023-05-09 11:11:22.258700 windmill_api-1.97.0/windmill_api/models/audit_log.py
+-rw-r--r--   0        0        0      217 2023-05-09 11:11:14.190748 windmill_api-1.97.0/windmill_api/models/audit_log_action_kind.py
+-rw-r--r--   0        0        0      620 2023-05-09 11:11:14.042749 windmill_api-1.97.0/windmill_api/models/audit_log_operation.py
+-rw-r--r--   0        0        0     1186 2023-05-09 11:11:22.278699 windmill_api-1.97.0/windmill_api/models/audit_log_parameters.py
+-rw-r--r--   0        0        0     2933 2023-05-09 11:11:22.318699 windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-05-09 11:11:22.390699 windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-05-09 11:11:14.066749 windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-05-09 11:11:22.378699 windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-05-09 11:11:22.426699 windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-05-09 11:11:22.434698 windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-05-09 11:11:22.482698 windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-05-09 11:11:14.286748 windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-05-09 11:11:22.474698 windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-05-09 11:11:22.558698 windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-05-09 11:11:14.206748 windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-05-09 11:11:22.518698 windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-09 11:11:13.278754 windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2377 2023-05-09 11:11:22.574698 windmill_api-1.97.0/windmill_api/models/branch_all.py
+-rw-r--r--   0        0        0     2543 2023-05-09 11:11:22.614697 windmill_api-1.97.0/windmill_api/models/branch_all_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-05-09 11:11:22.698697 windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-05-09 11:11:22.674697 windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-09 11:11:22.718697 windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-09 11:11:22.754696 windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-09 11:11:22.762696 windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-09 11:11:14.166748 windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-09 11:11:22.802696 windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-09 11:11:13.650751 windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-09 11:11:22.802696 windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-09 11:11:22.846696 windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-05-09 11:11:13.550752 windmill_api-1.97.0/windmill_api/models/branch_all_type.py
+-rw-r--r--   0        0        0     2670 2023-05-09 11:11:22.866696 windmill_api-1.97.0/windmill_api/models/branch_one.py
+-rw-r--r--   0        0        0     2372 2023-05-09 11:11:22.902696 windmill_api-1.97.0/windmill_api/models/branch_one_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-05-09 11:11:22.986695 windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-05-09 11:11:22.978695 windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-09 11:11:23.018695 windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-09 11:11:23.038695 windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-09 11:11:23.066695 windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-09 11:11:14.054749 windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-09 11:11:23.114694 windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-09 11:11:13.466753 windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-09 11:11:23.106694 windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-09 11:11:23.150694 windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6125 2023-05-09 11:11:23.234694 windmill_api-1.97.0/windmill_api/models/branch_one_default_item.py
+-rw-r--r--   0        0        0     2906 2023-05-09 11:11:23.210694 windmill_api-1.97.0/windmill_api/models/branch_one_default_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-05-09 11:11:23.254694 windmill_api-1.97.0/windmill_api/models/branch_one_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-05-09 11:11:23.290693 windmill_api-1.97.0/windmill_api/models/branch_one_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-05-09 11:11:23.302693 windmill_api-1.97.0/windmill_api/models/branch_one_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-05-09 11:11:13.646751 windmill_api-1.97.0/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-05-09 11:11:23.342693 windmill_api-1.97.0/windmill_api/models/branch_one_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-09 11:11:14.398747 windmill_api-1.97.0/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-05-09 11:11:23.350693 windmill_api-1.97.0/windmill_api/models/branch_one_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-05-09 11:11:23.390693 windmill_api-1.97.0/windmill_api/models/branch_one_default_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-05-09 11:11:14.178748 windmill_api-1.97.0/windmill_api/models/branch_one_type.py
+-rw-r--r--   0        0        0     1532 2023-05-09 11:11:23.390693 windmill_api-1.97.0/windmill_api/models/cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     1255 2023-05-09 11:11:23.418692 windmill_api-1.97.0/windmill_api/models/cancel_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0    10508 2023-05-09 11:11:23.594691 windmill_api-1.97.0/windmill_api/models/completed_job.py
+-rw-r--r--   0        0        0     1176 2023-05-09 11:11:23.446692 windmill_api-1.97.0/windmill_api/models/completed_job_args.py
+-rw-r--r--   0        0        0     3265 2023-05-09 11:11:23.542692 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status.py
+-rw-r--r--   0        0        0     6800 2023-05-09 11:11:23.670691 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1789 2023-05-09 11:11:23.674691 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2136 2023-05-09 11:11:23.718691 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      202 2023-05-09 11:11:14.422747 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1694 2023-05-09 11:11:23.714691 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2230 2023-05-09 11:11:23.762690 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      360 2023-05-09 11:11:13.442753 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6402 2023-05-09 11:11:23.842690 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1779 2023-05-09 11:11:23.802690 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2116 2023-05-09 11:11:23.842690 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      200 2023-05-09 11:11:13.122755 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1684 2023-05-09 11:11:23.886690 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2220 2023-05-09 11:11:23.898690 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      358 2023-05-09 11:11:14.526746 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2040 2023-05-09 11:11:23.934689 windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_retry.py
+-rw-r--r--   0        0        0      310 2023-05-09 11:11:13.754751 windmill_api-1.97.0/windmill_api/models/completed_job_job_kind.py
+-rw-r--r--   0        0        0      199 2023-05-09 11:11:13.106755 windmill_api-1.97.0/windmill_api/models/completed_job_language.py
+-rw-r--r--   0        0        0     3127 2023-05-09 11:11:23.970689 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow.py
+-rw-r--r--   0        0        0     6620 2023-05-09 11:11:24.110688 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3129 2023-05-09 11:11:24.030689 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1929 2023-05-09 11:11:24.082688 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-05-09 11:11:24.134688 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-05-09 11:11:24.154688 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-09 11:11:13.870750 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-05-09 11:11:24.182688 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-09 11:11:13.866750 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-05-09 11:11:24.198688 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-05-09 11:11:24.262688 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6544 2023-05-09 11:11:24.322687 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3095 2023-05-09 11:11:24.318687 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1919 2023-05-09 11:11:24.362687 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2223 2023-05-09 11:11:24.374687 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2050 2023-05-09 11:11:24.406687 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      179 2023-05-09 11:11:13.606752 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1917 2023-05-09 11:11:24.418686 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      179 2023-05-09 11:11:13.658751 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1912 2023-05-09 11:11:24.454686 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1963 2023-05-09 11:11:24.462686 windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1572 2023-05-09 11:11:24.498686 windmill_api-1.97.0/windmill_api/models/connect_callback_json_body.py
+-rw-r--r--   0        0        0     2533 2023-05-09 11:11:24.514686 windmill_api-1.97.0/windmill_api/models/connect_callback_response_200.py
+-rw-r--r--   0        0        0     1600 2023-05-09 11:11:24.538686 windmill_api-1.97.0/windmill_api/models/connect_slack_callback_json_body.py
+-rw-r--r--   0        0        0     1753 2023-05-09 11:11:24.570685 windmill_api-1.97.0/windmill_api/models/contextual_variable.py
+-rw-r--r--   0        0        0     2147 2023-05-09 11:11:24.586686 windmill_api-1.97.0/windmill_api/models/create_account_json_body.py
+-rw-r--r--   0        0        0     2367 2023-05-09 11:11:24.626685 windmill_api-1.97.0/windmill_api/models/create_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-05-09 11:11:24.662685 windmill_api-1.97.0/windmill_api/models/create_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-05-09 11:11:14.534746 windmill_api-1.97.0/windmill_api/models/create_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-05-09 11:11:24.698685 windmill_api-1.97.0/windmill_api/models/create_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-05-09 11:11:24.694685 windmill_api-1.97.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     1947 2023-05-09 11:11:24.742684 windmill_api-1.97.0/windmill_api/models/create_draft_json_body.py
+-rw-r--r--   0        0        0      183 2023-05-09 11:11:13.810750 windmill_api-1.97.0/windmill_api/models/create_draft_json_body_typ.py
+-rw-r--r--   0        0        0     1550 2023-05-09 11:11:24.738685 windmill_api-1.97.0/windmill_api/models/create_flow_json_body.py
+-rw-r--r--   0        0        0     2126 2023-05-09 11:11:24.794684 windmill_api-1.97.0/windmill_api/models/create_folder_json_body.py
+-rw-r--r--   0        0        0     1697 2023-05-09 11:11:24.786684 windmill_api-1.97.0/windmill_api/models/create_group_json_body.py
+-rw-r--r--   0        0        0     1613 2023-05-09 11:11:24.854684 windmill_api-1.97.0/windmill_api/models/create_input.py
+-rw-r--r--   0        0        0     1171 2023-05-09 11:11:24.822684 windmill_api-1.97.0/windmill_api/models/create_input_args.py
+-rw-r--r--   0        0        0     1701 2023-05-09 11:11:24.862684 windmill_api-1.97.0/windmill_api/models/create_input_json_body.py
+-rw-r--r--   0        0        0     1217 2023-05-09 11:11:24.898684 windmill_api-1.97.0/windmill_api/models/create_input_json_body_args.py
+-rw-r--r--   0        0        0      214 2023-05-09 11:11:13.142754 windmill_api-1.97.0/windmill_api/models/create_input_runnable_type.py
+-rw-r--r--   0        0        0     1732 2023-05-09 11:11:24.910683 windmill_api-1.97.0/windmill_api/models/create_raw_app_json_body.py
+-rw-r--r--   0        0        0     2094 2023-05-09 11:11:24.950683 windmill_api-1.97.0/windmill_api/models/create_resource.py
+-rw-r--r--   0        0        0     2140 2023-05-09 11:11:24.962683 windmill_api-1.97.0/windmill_api/models/create_resource_json_body.py
+-rw-r--r--   0        0        0     2335 2023-05-09 11:11:25.006683 windmill_api-1.97.0/windmill_api/models/create_resource_type_json_body.py
+-rw-r--r--   0        0        0     2780 2023-05-09 11:11:25.022683 windmill_api-1.97.0/windmill_api/models/create_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-09 11:11:25.038683 windmill_api-1.97.0/windmill_api/models/create_schedule_json_body_args.py
+-rw-r--r--   0        0        0     5120 2023-05-09 11:11:25.142682 windmill_api-1.97.0/windmill_api/models/create_script_json_body.py
+-rw-r--r--   0        0        0      249 2023-05-09 11:11:14.534746 windmill_api-1.97.0/windmill_api/models/create_script_json_body_kind.py
+-rw-r--r--   0        0        0      207 2023-05-09 11:11:13.110755 windmill_api-1.97.0/windmill_api/models/create_script_json_body_language.py
+-rw-r--r--   0        0        0     1232 2023-05-09 11:11:25.078683 windmill_api-1.97.0/windmill_api/models/create_script_json_body_schema.py
+-rw-r--r--   0        0        0     2534 2023-05-09 11:11:25.158682 windmill_api-1.97.0/windmill_api/models/create_token_impersonate_json_body.py
+-rw-r--r--   0        0        0     2169 2023-05-09 11:11:25.194682 windmill_api-1.97.0/windmill_api/models/create_token_json_body.py
+-rw-r--r--   0        0        0     2364 2023-05-09 11:11:25.214682 windmill_api-1.97.0/windmill_api/models/create_user_globally_json_body.py
+-rw-r--r--   0        0        0     1771 2023-05-09 11:11:25.258681 windmill_api-1.97.0/windmill_api/models/create_user_json_body.py
+-rw-r--r--   0        0        0     2493 2023-05-09 11:11:25.270681 windmill_api-1.97.0/windmill_api/models/create_variable.py
+-rw-r--r--   0        0        0     2539 2023-05-09 11:11:25.314681 windmill_api-1.97.0/windmill_api/models/create_variable_json_body.py
+-rw-r--r--   0        0        0     1678 2023-05-09 11:11:25.310681 windmill_api-1.97.0/windmill_api/models/create_workspace.py
+-rw-r--r--   0        0        0     1724 2023-05-09 11:11:25.358681 windmill_api-1.97.0/windmill_api/models/create_workspace_json_body.py
+-rw-r--r--   0        0        0     1490 2023-05-09 11:11:25.354681 windmill_api-1.97.0/windmill_api/models/decline_invite_json_body.py
+-rw-r--r--   0        0        0    11110 2023-05-09 11:11:25.574679 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200.py
+-rw-r--r--   0        0        0     1270 2023-05-09 11:11:25.390681 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3658 2023-05-09 11:11:25.482680 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7442 2023-05-09 11:11:25.610679 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1883 2023-05-09 11:11:25.614679 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2318 2023-05-09 11:11:25.658679 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      219 2023-05-09 11:11:13.910750 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1788 2023-05-09 11:11:25.654679 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2324 2023-05-09 11:11:25.706679 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      377 2023-05-09 11:11:14.170748 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7053 2023-05-09 11:11:25.786678 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1873 2023-05-09 11:11:25.746678 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2298 2023-05-09 11:11:25.786678 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      217 2023-05-09 11:11:13.334753 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1778 2023-05-09 11:11:25.862678 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2314 2023-05-09 11:11:25.842678 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      375 2023-05-09 11:11:13.358753 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2134 2023-05-09 11:11:25.898678 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      327 2023-05-09 11:11:13.114755 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      216 2023-05-09 11:11:13.834750 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3432 2023-05-09 11:11:25.938677 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7425 2023-05-09 11:11:26.062677 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3442 2023-05-09 11:11:26.002677 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2023 2023-05-09 11:11:26.050677 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2327 2023-05-09 11:11:26.102676 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2261 2023-05-09 11:11:26.110676 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-09 11:11:13.374753 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-09 11:11:26.150676 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-09 11:11:14.154748 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2016 2023-05-09 11:11:26.150676 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2067 2023-05-09 11:11:26.194676 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7349 2023-05-09 11:11:26.294675 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3408 2023-05-09 11:11:26.258675 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2013 2023-05-09 11:11:26.318675 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2317 2023-05-09 11:11:26.370675 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2241 2023-05-09 11:11:26.362675 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-05-09 11:11:14.130749 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2108 2023-05-09 11:11:26.414674 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-05-09 11:11:13.894750 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2006 2023-05-09 11:11:26.422675 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2057 2023-05-09 11:11:26.462674 windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1783 2023-05-09 11:11:26.522674 windmill_api-1.97.0/windmill_api/models/delete_invite_json_body.py
+-rw-r--r--   0        0        0     7636 2023-05-09 11:11:26.658673 windmill_api-1.97.0/windmill_api/models/delete_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1309 2023-05-09 11:11:26.554674 windmill_api-1.97.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      258 2023-05-09 11:11:13.910750 windmill_api-1.97.0/windmill_api/models/delete_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      216 2023-05-09 11:11:13.222754 windmill_api-1.97.0/windmill_api/models/delete_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1283 2023-05-09 11:11:26.606673 windmill_api-1.97.0/windmill_api/models/delete_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     2933 2023-05-09 11:11:26.670673 windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-05-09 11:11:26.742673 windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-05-09 11:11:13.354753 windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-05-09 11:11:26.706673 windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-05-09 11:11:26.750672 windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-05-09 11:11:26.786672 windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-05-09 11:11:26.810672 windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-05-09 11:11:13.890750 windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-05-09 11:11:26.822672 windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-05-09 11:11:26.874672 windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-05-09 11:11:13.790751 windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-05-09 11:11:26.858672 windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-09 11:11:13.598752 windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     1551 2023-05-09 11:11:26.898671 windmill_api-1.97.0/windmill_api/models/edit_auto_invite_json_body.py
+-rw-r--r--   0        0        0     1980 2023-05-09 11:11:26.922671 windmill_api-1.97.0/windmill_api/models/edit_resource.py
+-rw-r--r--   0        0        0     1791 2023-05-09 11:11:26.942671 windmill_api-1.97.0/windmill_api/models/edit_resource_type.py
+-rw-r--r--   0        0        0     1845 2023-05-09 11:11:26.970671 windmill_api-1.97.0/windmill_api/models/edit_schedule.py
+-rw-r--r--   0        0        0     1176 2023-05-09 11:11:26.974671 windmill_api-1.97.0/windmill_api/models/edit_schedule_args.py
+-rw-r--r--   0        0        0     1691 2023-05-09 11:11:27.010671 windmill_api-1.97.0/windmill_api/models/edit_slack_command_json_body.py
+-rw-r--r--   0        0        0     2260 2023-05-09 11:11:27.022671 windmill_api-1.97.0/windmill_api/models/edit_variable.py
+-rw-r--r--   0        0        0     1520 2023-05-09 11:11:27.050671 windmill_api-1.97.0/windmill_api/models/edit_webhook_json_body.py
+-rw-r--r--   0        0        0     2058 2023-05-09 11:11:27.074670 windmill_api-1.97.0/windmill_api/models/edit_workspace_user.py
+-rw-r--r--   0        0        0     3663 2023-05-09 11:11:27.166670 windmill_api-1.97.0/windmill_api/models/execute_component_json_body.py
+-rw-r--r--   0        0        0     1346 2023-05-09 11:11:27.102670 windmill_api-1.97.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
+-rw-r--r--   0        0        0     1942 2023-05-09 11:11:27.146670 windmill_api-1.97.0/windmill_api/models/execute_component_json_body_raw_code.py
+-rw-r--r--   0        0        0     1577 2023-05-09 11:11:27.206670 windmill_api-1.97.0/windmill_api/models/exists_username_json_body.py
+-rw-r--r--   0        0        0     1400 2023-05-09 11:11:27.198670 windmill_api-1.97.0/windmill_api/models/exists_workspace_json_body.py
+-rw-r--r--   0        0        0     4924 2023-05-09 11:11:27.302669 windmill_api-1.97.0/windmill_api/models/flow.py
+-rw-r--r--   0        0        0     1166 2023-05-09 11:11:27.238669 windmill_api-1.97.0/windmill_api/models/flow_extra_perms.py
+-rw-r--r--   0        0        0     3707 2023-05-09 11:11:27.310669 windmill_api-1.97.0/windmill_api/models/flow_metadata.py
+-rw-r--r--   0        0        0     1209 2023-05-09 11:11:27.334669 windmill_api-1.97.0/windmill_api/models/flow_metadata_extra_perms.py
+-rw-r--r--   0        0        0     5729 2023-05-09 11:11:27.430668 windmill_api-1.97.0/windmill_api/models/flow_module.py
+-rw-r--r--   0        0        0     2726 2023-05-09 11:11:27.398669 windmill_api-1.97.0/windmill_api/models/flow_module_retry.py
+-rw-r--r--   0        0        0     1807 2023-05-09 11:11:27.442668 windmill_api-1.97.0/windmill_api/models/flow_module_retry_constant.py
+-rw-r--r--   0        0        0     2111 2023-05-09 11:11:27.522668 windmill_api-1.97.0/windmill_api/models/flow_module_retry_exponential.py
+-rw-r--r--   0        0        0     1834 2023-05-09 11:11:27.490668 windmill_api-1.97.0/windmill_api/models/flow_module_sleep_type_0.py
+-rw-r--r--   0        0        0      159 2023-05-09 11:11:13.926750 windmill_api-1.97.0/windmill_api/models/flow_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1701 2023-05-09 11:11:27.554668 windmill_api-1.97.0/windmill_api/models/flow_module_sleep_type_1.py
+-rw-r--r--   0        0        0      159 2023-05-09 11:11:13.522752 windmill_api-1.97.0/windmill_api/models/flow_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1800 2023-05-09 11:11:27.570668 windmill_api-1.97.0/windmill_api/models/flow_module_stop_after_if.py
+-rw-r--r--   0        0        0     1851 2023-05-09 11:11:27.598667 windmill_api-1.97.0/windmill_api/models/flow_module_suspend.py
+-rw-r--r--   0        0        0     3292 2023-05-09 11:11:27.638667 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_0.py
+-rw-r--r--   0        0        0     3564 2023-05-09 11:11:27.654667 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-09 11:11:27.686667 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-09 11:11:13.898750 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-09 11:11:27.718667 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-09 11:11:13.914750 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      208 2023-05-09 11:11:13.642752 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_0_language.py
+-rw-r--r--   0        0        0      158 2023-05-09 11:11:14.386747 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_0_type.py
+-rw-r--r--   0        0        0     2477 2023-05-09 11:11:27.750666 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_1.py
+-rw-r--r--   0        0        0     3564 2023-05-09 11:11:27.774666 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-09 11:11:27.838666 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-09 11:11:14.490746 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-09 11:11:27.818666 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-09 11:11:14.246748 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      152 2023-05-09 11:11:13.478752 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_1_type.py
+-rw-r--r--   0        0        0     2204 2023-05-09 11:11:27.862666 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_2.py
+-rw-r--r--   0        0        0     3564 2023-05-09 11:11:27.894666 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-05-09 11:11:27.906665 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-05-09 11:11:14.306748 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-05-09 11:11:27.942665 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-05-09 11:11:14.294747 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      148 2023-05-09 11:11:13.462752 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_2_type.py
+-rw-r--r--   0        0        0     4138 2023-05-09 11:11:27.982665 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3.py
+-rw-r--r--   0        0        0     1990 2023-05-09 11:11:27.986665 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
+-rw-r--r--   0        0        0      173 2023-05-09 11:11:13.726751 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1857 2023-05-09 11:11:28.022665 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
+-rw-r--r--   0        0        0      173 2023-05-09 11:11:14.382747 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6636 2023-05-09 11:11:28.118664 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py
+-rw-r--r--   0        0        0     3148 2023-05-09 11:11:28.094664 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-05-09 11:11:28.138664 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-05-09 11:11:28.170664 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-05-09 11:11:28.182664 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-09 11:11:14.506746 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-05-09 11:11:28.218664 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-09 11:11:13.106755 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-05-09 11:11:28.226664 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-05-09 11:11:28.266663 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
+-rw-r--r--   0        0        0      162 2023-05-09 11:11:13.658751 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_type.py
+-rw-r--r--   0        0        0     2934 2023-05-09 11:11:28.322663 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4.py
+-rw-r--r--   0        0        0     2508 2023-05-09 11:11:28.318663 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-05-09 11:11:28.466662 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-05-09 11:11:28.382663 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-05-09 11:11:28.422662 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-05-09 11:11:28.470662 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-05-09 11:11:28.514662 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-09 11:11:13.682751 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-05-09 11:11:28.510662 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-09 11:11:13.506752 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-05-09 11:11:28.554662 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-05-09 11:11:28.562662 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6636 2023-05-09 11:11:28.670661 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item.py
+-rw-r--r--   0        0        0     3148 2023-05-09 11:11:28.618661 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-05-09 11:11:28.658661 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-05-09 11:11:28.706661 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-05-09 11:11:28.714661 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-05-09 11:11:13.202754 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-05-09 11:11:28.754660 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-05-09 11:11:13.346753 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-05-09 11:11:28.758660 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-05-09 11:11:28.802660 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-05-09 11:11:13.210754 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_type.py
+-rw-r--r--   0        0        0     2577 2023-05-09 11:11:28.866660 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5.py
+-rw-r--r--   0        0        0     2679 2023-05-09 11:11:28.854660 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-05-09 11:11:29.026659 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-05-09 11:11:28.922659 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-05-09 11:11:28.966659 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-05-09 11:11:29.018659 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-05-09 11:11:29.062658 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-09 11:11:13.426753 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-05-09 11:11:29.074658 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-09 11:11:13.830750 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-05-09 11:11:29.110658 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-05-09 11:11:29.122658 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-05-09 11:11:14.082749 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_type.py
+-rw-r--r--   0        0        0     1839 2023-05-09 11:11:29.158658 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_6.py
+-rw-r--r--   0        0        0      156 2023-05-09 11:11:14.326747 windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_6_type.py
+-rw-r--r--   0        0        0     2009 2023-05-09 11:11:29.174658 windmill_api-1.97.0/windmill_api/models/flow_preview.py
+-rw-r--r--   0        0        0     1171 2023-05-09 11:11:29.186658 windmill_api-1.97.0/windmill_api/models/flow_preview_args.py
+-rw-r--r--   0        0        0     3074 2023-05-09 11:11:29.242657 windmill_api-1.97.0/windmill_api/models/flow_preview_value.py
+-rw-r--r--   0        0        0     6498 2023-05-09 11:11:29.314657 windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module.py
+-rw-r--r--   0        0        0     3064 2023-05-09 11:11:29.302657 windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1911 2023-05-09 11:11:29.350657 windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2215 2023-05-09 11:11:29.362657 windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2036 2023-05-09 11:11:29.398656 windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-09 11:11:13.922750 windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1903 2023-05-09 11:11:29.450656 windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-09 11:11:13.274754 windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1904 2023-05-09 11:11:29.446656 windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1955 2023-05-09 11:11:29.506656 windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6422 2023-05-09 11:11:29.574655 windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item.py
+-rw-r--r--   0        0        0     3030 2023-05-09 11:11:29.602655 windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1901 2023-05-09 11:11:29.614655 windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2205 2023-05-09 11:11:29.650655 windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2016 2023-05-09 11:11:29.658655 windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-05-09 11:11:13.398753 windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1883 2023-05-09 11:11:29.698655 windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-05-09 11:11:13.290753 windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1894 2023-05-09 11:11:29.702654 windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1945 2023-05-09 11:11:29.742654 windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1143 2023-05-09 11:11:29.730654 windmill_api-1.97.0/windmill_api/models/flow_schema.py
+-rw-r--r--   0        0        0     3001 2023-05-09 11:11:29.794654 windmill_api-1.97.0/windmill_api/models/flow_status.py
+-rw-r--r--   0        0        0     6370 2023-05-09 11:11:29.866654 windmill_api-1.97.0/windmill_api/models/flow_status_failure_module.py
+-rw-r--r--   0        0        0     1723 2023-05-09 11:11:29.830654 windmill_api-1.97.0/windmill_api/models/flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     1999 2023-05-09 11:11:29.874653 windmill_api-1.97.0/windmill_api/models/flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      190 2023-05-09 11:11:13.362753 windmill_api-1.97.0/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1628 2023-05-09 11:11:29.910653 windmill_api-1.97.0/windmill_api/models/flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2164 2023-05-09 11:11:29.930653 windmill_api-1.97.0/windmill_api/models/flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      348 2023-05-09 11:11:14.170748 windmill_api-1.97.0/windmill_api/models/flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     5808 2023-05-09 11:11:30.038653 windmill_api-1.97.0/windmill_api/models/flow_status_module.py
+-rw-r--r--   0        0        0     1685 2023-05-09 11:11:30.006653 windmill_api-1.97.0/windmill_api/models/flow_status_module_approvers_item.py
+-rw-r--r--   0        0        0     1925 2023-05-09 11:11:30.046652 windmill_api-1.97.0/windmill_api/models/flow_status_module_branch_chosen.py
+-rw-r--r--   0        0        0      183 2023-05-09 11:11:14.246748 windmill_api-1.97.0/windmill_api/models/flow_status_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1590 2023-05-09 11:11:30.082652 windmill_api-1.97.0/windmill_api/models/flow_status_module_branchall.py
+-rw-r--r--   0        0        0     2126 2023-05-09 11:11:30.102652 windmill_api-1.97.0/windmill_api/models/flow_status_module_iterator.py
+-rw-r--r--   0        0        0      341 2023-05-09 11:11:14.282748 windmill_api-1.97.0/windmill_api/models/flow_status_module_type.py
+-rw-r--r--   0        0        0     5981 2023-05-09 11:11:30.242651 windmill_api-1.97.0/windmill_api/models/flow_status_modules_item.py
+-rw-r--r--   0        0        0     1713 2023-05-09 11:11:30.138652 windmill_api-1.97.0/windmill_api/models/flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     1979 2023-05-09 11:11:30.174651 windmill_api-1.97.0/windmill_api/models/flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      188 2023-05-09 11:11:13.806750 windmill_api-1.97.0/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1618 2023-05-09 11:11:30.214651 windmill_api-1.97.0/windmill_api/models/flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2154 2023-05-09 11:11:30.266651 windmill_api-1.97.0/windmill_api/models/flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      346 2023-05-09 11:11:13.618752 windmill_api-1.97.0/windmill_api/models/flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     1974 2023-05-09 11:11:30.294651 windmill_api-1.97.0/windmill_api/models/flow_status_retry.py
+-rw-r--r--   0        0        0     2957 2023-05-09 11:11:30.326651 windmill_api-1.97.0/windmill_api/models/flow_value.py
+-rw-r--r--   0        0        0     6224 2023-05-09 11:11:30.426650 windmill_api-1.97.0/windmill_api/models/flow_value_failure_module.py
+-rw-r--r--   0        0        0     2940 2023-05-09 11:11:30.390650 windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1873 2023-05-09 11:11:30.442650 windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-05-09 11:11:30.478650 windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-05-09 11:11:30.486650 windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-05-09 11:11:13.846750 windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-05-09 11:11:30.526649 windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-05-09 11:11:14.130749 windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-05-09 11:11:30.526649 windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-05-09 11:11:30.570649 windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6125 2023-05-09 11:11:30.678648 windmill_api-1.97.0/windmill_api/models/flow_value_modules_item.py
+-rw-r--r--   0        0        0     2906 2023-05-09 11:11:30.630649 windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-05-09 11:11:30.674648 windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-05-09 11:11:30.762648 windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-05-09 11:11:30.718648 windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-05-09 11:11:13.614752 windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-05-09 11:11:30.770648 windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-09 11:11:13.866750 windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-05-09 11:11:30.806648 windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-05-09 11:11:30.814648 windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1858 2023-05-09 11:11:30.858647 windmill_api-1.97.0/windmill_api/models/folder.py
+-rw-r--r--   0        0        0     1179 2023-05-09 11:11:30.842647 windmill_api-1.97.0/windmill_api/models/folder_extra_perms.py
+-rw-r--r--   0        0        0     1560 2023-05-09 11:11:30.886647 windmill_api-1.97.0/windmill_api/models/force_cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     3807 2023-05-09 11:11:30.934647 windmill_api-1.97.0/windmill_api/models/forloop_flow.py
+-rw-r--r--   0        0        0     1874 2023-05-09 11:11:30.926647 windmill_api-1.97.0/windmill_api/models/forloop_flow_iterator_type_0.py
+-rw-r--r--   0        0        0      163 2023-05-09 11:11:14.082749 windmill_api-1.97.0/windmill_api/models/forloop_flow_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1741 2023-05-09 11:11:30.970647 windmill_api-1.97.0/windmill_api/models/forloop_flow_iterator_type_1.py
+-rw-r--r--   0        0        0      163 2023-05-09 11:11:13.926750 windmill_api-1.97.0/windmill_api/models/forloop_flow_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6224 2023-05-09 11:11:31.062646 windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item.py
+-rw-r--r--   0        0        0     2940 2023-05-09 11:11:31.030646 windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1873 2023-05-09 11:11:31.074646 windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-05-09 11:11:31.166645 windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-05-09 11:11:31.118646 windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-05-09 11:11:13.154754 windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-05-09 11:11:31.158645 windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-05-09 11:11:14.422747 windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-05-09 11:11:31.218645 windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-05-09 11:11:31.210645 windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0      152 2023-05-09 11:11:13.402753 windmill_api-1.97.0/windmill_api/models/forloop_flow_type.py
+-rw-r--r--   0        0        0     4052 2023-05-09 11:11:31.294645 windmill_api-1.97.0/windmill_api/models/get_app_by_path_response_200.py
+-rw-r--r--   0        0        0      219 2023-05-09 11:11:14.454747 windmill_api-1.97.0/windmill_api/models/get_app_by_path_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1279 2023-05-09 11:11:31.250645 windmill_api-1.97.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3811 2023-05-09 11:11:31.358644 windmill_api-1.97.0/windmill_api/models/get_app_by_path_response_200_policy.py
+-rw-r--r--   0        0        0      225 2023-05-09 11:11:13.650751 windmill_api-1.97.0/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2009 2023-05-09 11:11:31.338644 windmill_api-1.97.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1412 2023-05-09 11:11:31.370644 windmill_api-1.97.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4819 2023-05-09 11:11:31.438644 windmill_api-1.97.0/windmill_api/models/get_app_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0      228 2023-05-09 11:11:14.234748 windmill_api-1.97.0/windmill_api/models/get_app_by_path_with_draft_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1330 2023-05-09 11:11:31.402644 windmill_api-1.97.0/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3992 2023-05-09 11:11:31.474644 windmill_api-1.97.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py
+-rw-r--r--   0        0        0      234 2023-05-09 11:11:13.690751 windmill_api-1.97.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2160 2023-05-09 11:11:31.482643 windmill_api-1.97.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1463 2023-05-09 11:11:31.502643 windmill_api-1.97.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4112 2023-05-09 11:11:31.562643 windmill_api-1.97.0/windmill_api/models/get_app_by_version_response_200.py
+-rw-r--r--   0        0        0      222 2023-05-09 11:11:13.738751 windmill_api-1.97.0/windmill_api/models/get_app_by_version_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1294 2023-05-09 11:11:31.538643 windmill_api-1.97.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3862 2023-05-09 11:11:31.610643 windmill_api-1.97.0/windmill_api/models/get_app_by_version_response_200_policy.py
+-rw-r--r--   0        0        0      228 2023-05-09 11:11:14.134749 windmill_api-1.97.0/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2042 2023-05-09 11:11:31.598643 windmill_api-1.97.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1427 2023-05-09 11:11:31.634642 windmill_api-1.97.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3764 2023-05-09 11:11:31.682642 windmill_api-1.97.0/windmill_api/models/get_audit_log_response_200.py
+-rw-r--r--   0        0        0      231 2023-05-09 11:11:13.938750 windmill_api-1.97.0/windmill_api/models/get_audit_log_response_200_action_kind.py
+-rw-r--r--   0        0        0      634 2023-05-09 11:11:14.306748 windmill_api-1.97.0/windmill_api/models/get_audit_log_response_200_operation.py
+-rw-r--r--   0        0        0     1265 2023-05-09 11:11:31.670642 windmill_api-1.97.0/windmill_api/models/get_audit_log_response_200_parameters.py
+-rw-r--r--   0        0        0    11008 2023-05-09 11:11:31.906641 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200.py
+-rw-r--r--   0        0        0     1255 2023-05-09 11:11:31.750642 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3595 2023-05-09 11:11:31.818641 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7343 2023-05-09 11:11:31.942641 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1868 2023-05-09 11:11:31.942641 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2288 2023-05-09 11:11:31.982640 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      216 2023-05-09 11:11:13.478752 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1773 2023-05-09 11:11:31.990640 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2309 2023-05-09 11:11:32.038640 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      374 2023-05-09 11:11:13.114755 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6924 2023-05-09 11:11:32.122640 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1858 2023-05-09 11:11:32.078640 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-05-09 11:11:32.118640 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-05-09 11:11:13.786751 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-05-09 11:11:32.162639 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2299 2023-05-09 11:11:32.174639 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      372 2023-05-09 11:11:13.478752 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2119 2023-05-09 11:11:32.214639 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      324 2023-05-09 11:11:13.502752 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      213 2023-05-09 11:11:13.706751 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3375 2023-05-09 11:11:32.242639 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7311 2023-05-09 11:11:32.338638 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3391 2023-05-09 11:11:32.346638 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2008 2023-05-09 11:11:32.382638 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2312 2023-05-09 11:11:32.394638 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2231 2023-05-09 11:11:32.466637 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      195 2023-05-09 11:11:13.506752 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2098 2023-05-09 11:11:32.438638 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      195 2023-05-09 11:11:14.346747 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2001 2023-05-09 11:11:32.482637 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2052 2023-05-09 11:11:32.506637 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7235 2023-05-09 11:11:32.606636 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3357 2023-05-09 11:11:32.566637 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1998 2023-05-09 11:11:32.614636 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-05-09 11:11:32.658636 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-05-09 11:11:32.658636 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-09 11:11:13.902750 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-05-09 11:11:32.702636 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-09 11:11:13.738751 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-05-09 11:11:32.706636 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-05-09 11:11:32.746636 windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     5374 2023-05-09 11:11:32.806635 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200.py
+-rw-r--r--   0        0        0     1281 2023-05-09 11:11:32.774635 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1258 2023-05-09 11:11:32.806635 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     3302 2023-05-09 11:11:32.914635 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value.py
+-rw-r--r--   0        0        0     7159 2023-05-09 11:11:32.930634 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
+-rw-r--r--   0        0        0     3323 2023-05-09 11:11:32.974634 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1988 2023-05-09 11:11:32.974634 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-05-09 11:11:33.062634 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-05-09 11:11:33.018634 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-05-09 11:11:13.082755 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-05-09 11:11:33.062634 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-05-09 11:11:13.178754 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-05-09 11:11:33.102633 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-05-09 11:11:33.110633 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7066 2023-05-09 11:11:33.226632 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
+-rw-r--r--   0        0        0     3289 2023-05-09 11:11:33.170633 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1978 2023-05-09 11:11:33.214633 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2282 2023-05-09 11:11:33.266632 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2171 2023-05-09 11:11:33.266632 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-05-09 11:11:13.098755 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2038 2023-05-09 11:11:33.310632 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-05-09 11:11:13.646751 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1971 2023-05-09 11:11:33.318632 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2022 2023-05-09 11:11:33.354632 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2093 2023-05-09 11:11:33.366632 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0     5695 2023-05-09 11:11:33.454631 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py
+-rw-r--r--   0        0        0     1360 2023-05-09 11:11:33.394631 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py
+-rw-r--r--   0        0        0     1337 2023-05-09 11:11:33.426631 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py
+-rw-r--r--   0        0        0     3559 2023-05-09 11:11:33.550630 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py
+-rw-r--r--   0        0        0     7829 2023-05-09 11:11:33.634630 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py
+-rw-r--r--   0        0        0     3606 2023-05-09 11:11:33.614630 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2067 2023-05-09 11:11:33.658630 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2371 2023-05-09 11:11:33.682630 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2343 2023-05-09 11:11:33.706630 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      205 2023-05-09 11:11:13.394753 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2210 2023-05-09 11:11:33.726629 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      205 2023-05-09 11:11:13.526752 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2060 2023-05-09 11:11:33.750629 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2111 2023-05-09 11:11:33.770629 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7685 2023-05-09 11:11:33.874629 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py
+-rw-r--r--   0        0        0     3542 2023-05-09 11:11:33.830629 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2057 2023-05-09 11:11:33.874629 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2361 2023-05-09 11:11:33.926628 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2323 2023-05-09 11:11:33.918628 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      203 2023-05-09 11:11:13.330753 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2190 2023-05-09 11:11:33.962628 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      203 2023-05-09 11:11:14.490746 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2050 2023-05-09 11:11:33.970628 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2101 2023-05-09 11:11:34.006628 windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2756 2023-05-09 11:11:34.106627 windmill_api-1.97.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py
+-rw-r--r--   0        0        0     1337 2023-05-09 11:11:34.034628 windmill_api-1.97.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py
+-rw-r--r--   0        0        0     2010 2023-05-09 11:11:34.082627 windmill_api-1.97.0/windmill_api/models/get_folder_response_200.py
+-rw-r--r--   0        0        0     1258 2023-05-09 11:11:34.110627 windmill_api-1.97.0/windmill_api/models/get_folder_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2357 2023-05-09 11:11:34.162627 windmill_api-1.97.0/windmill_api/models/get_folder_usage_response_200.py
+-rw-r--r--   0        0        0      325 2023-05-09 11:11:13.410753 windmill_api-1.97.0/windmill_api/models/get_granular_acls_kind.py
+-rw-r--r--   0        0        0     1235 2023-05-09 11:11:34.146627 windmill_api-1.97.0/windmill_api/models/get_granular_acls_response_200.py
+-rw-r--r--   0        0        0     2888 2023-05-09 11:11:34.262626 windmill_api-1.97.0/windmill_api/models/get_group_response_200.py
+-rw-r--r--   0        0        0     1253 2023-05-09 11:11:34.190626 windmill_api-1.97.0/windmill_api/models/get_group_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1606 2023-05-09 11:11:34.226626 windmill_api-1.97.0/windmill_api/models/get_hub_app_by_id_response_200.py
+-rw-r--r--   0        0        0     1634 2023-05-09 11:11:34.270626 windmill_api-1.97.0/windmill_api/models/get_hub_app_by_id_response_200_app.py
+-rw-r--r--   0        0        0     1977 2023-05-09 11:11:34.306626 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200.py
+-rw-r--r--   0        0        0     2950 2023-05-09 11:11:34.326626 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
+-rw-r--r--   0        0        0     1289 2023-05-09 11:11:34.330626 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
+-rw-r--r--   0        0        0     3410 2023-05-09 11:11:34.390625 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
+-rw-r--r--   0        0        0     7365 2023-05-09 11:11:34.450625 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3418 2023-05-09 11:11:34.450625 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2019 2023-05-09 11:11:34.494625 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2323 2023-05-09 11:11:34.498625 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2249 2023-05-09 11:11:34.542624 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-05-09 11:11:14.126748 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2116 2023-05-09 11:11:34.538624 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-05-09 11:11:13.474753 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2012 2023-05-09 11:11:34.582624 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2063 2023-05-09 11:11:34.586624 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7289 2023-05-09 11:11:34.702623 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
+-rw-r--r--   0        0        0     3384 2023-05-09 11:11:34.646624 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2009 2023-05-09 11:11:34.766623 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2313 2023-05-09 11:11:34.814623 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2229 2023-05-09 11:11:34.814623 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      194 2023-05-09 11:11:14.546746 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2096 2023-05-09 11:11:34.858622 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      194 2023-05-09 11:11:14.230748 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2002 2023-05-09 11:11:34.862622 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2053 2023-05-09 11:11:34.902622 windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2698 2023-05-09 11:11:34.918622 windmill_api-1.97.0/windmill_api/models/get_hub_script_by_path_response_200.py
+-rw-r--r--   0        0        0      216 2023-05-09 11:11:14.462746 windmill_api-1.97.0/windmill_api/models/get_hub_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     2644 2023-05-09 11:11:34.970622 windmill_api-1.97.0/windmill_api/models/get_input_history_response_200_item.py
+-rw-r--r--   0        0        0     1278 2023-05-09 11:11:34.946622 windmill_api-1.97.0/windmill_api/models/get_input_history_response_200_item_args.py
+-rw-r--r--   0        0        0      218 2023-05-09 11:11:13.610752 windmill_api-1.97.0/windmill_api/models/get_input_history_runnable_type.py
+-rw-r--r--   0        0        0     1852 2023-05-09 11:11:34.998622 windmill_api-1.97.0/windmill_api/models/get_job_response_200.py
+-rw-r--r--   0        0        0      188 2023-05-09 11:11:13.846750 windmill_api-1.97.0/windmill_api/models/get_job_response_200_type.py
+-rw-r--r--   0        0        0     2364 2023-05-09 11:11:35.030621 windmill_api-1.97.0/windmill_api/models/get_job_updates_response_200.py
+-rw-r--r--   0        0        0     1744 2023-05-09 11:11:35.038621 windmill_api-1.97.0/windmill_api/models/get_premium_info_response_200.py
+-rw-r--r--   0        0        0     4218 2023-05-09 11:11:35.110621 windmill_api-1.97.0/windmill_api/models/get_public_app_by_secret_response_200.py
+-rw-r--r--   0        0        0      227 2023-05-09 11:11:13.114755 windmill_api-1.97.0/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1322 2023-05-09 11:11:35.070621 windmill_api-1.97.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3970 2023-05-09 11:11:35.142621 windmill_api-1.97.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py
+-rw-r--r--   0        0        0      233 2023-05-09 11:11:13.698751 windmill_api-1.97.0/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2131 2023-05-09 11:11:35.162620 windmill_api-1.97.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1455 2023-05-09 11:11:35.174620 windmill_api-1.97.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3533 2023-05-09 11:11:35.242620 windmill_api-1.97.0/windmill_api/models/get_resource_response_200.py
+-rw-r--r--   0        0        0     1268 2023-05-09 11:11:35.202620 windmill_api-1.97.0/windmill_api/models/get_resource_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2335 2023-05-09 11:11:35.258620 windmill_api-1.97.0/windmill_api/models/get_resource_type_response_200.py
+-rw-r--r--   0        0        0     1840 2023-05-09 11:11:35.278620 windmill_api-1.97.0/windmill_api/models/get_resume_urls_response_200.py
+-rw-r--r--   0        0        0     4325 2023-05-09 11:11:35.342619 windmill_api-1.97.0/windmill_api/models/get_schedule_response_200.py
+-rw-r--r--   0        0        0     1232 2023-05-09 11:11:35.306620 windmill_api-1.97.0/windmill_api/models/get_schedule_response_200_args.py
+-rw-r--r--   0        0        0     1268 2023-05-09 11:11:35.422619 windmill_api-1.97.0/windmill_api/models/get_schedule_response_200_extra_perms.py
+-rw-r--r--   0        0        0     7558 2023-05-09 11:11:35.554618 windmill_api-1.97.0/windmill_api/models/get_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-09 11:11:35.458619 windmill_api-1.97.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-09 11:11:14.538746 windmill_api-1.97.0/windmill_api/models/get_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-05-09 11:11:13.822750 windmill_api-1.97.0/windmill_api/models/get_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-05-09 11:11:35.498618 windmill_api-1.97.0/windmill_api/models/get_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     7558 2023-05-09 11:11:35.646618 windmill_api-1.97.0/windmill_api/models/get_script_by_path_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-09 11:11:35.582618 windmill_api-1.97.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-09 11:11:14.078749 windmill_api-1.97.0/windmill_api/models/get_script_by_path_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-05-09 11:11:13.842750 windmill_api-1.97.0/windmill_api/models/get_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-05-09 11:11:35.618618 windmill_api-1.97.0/windmill_api/models/get_script_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     6383 2023-05-09 11:11:35.734617 windmill_api-1.97.0/windmill_api/models/get_script_by_path_with_draft_response_200.py
+-rw-r--r--   0        0        0     5608 2023-05-09 11:11:35.754617 windmill_api-1.97.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py
+-rw-r--r--   0        0        0      269 2023-05-09 11:11:13.554752 windmill_api-1.97.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_kind.py
+-rw-r--r--   0        0        0      227 2023-05-09 11:11:14.502746 windmill_api-1.97.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_language.py
+-rw-r--r--   0        0        0     1347 2023-05-09 11:11:35.770617 windmill_api-1.97.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py
+-rw-r--r--   0        0        0      264 2023-05-09 11:11:13.278754 windmill_api-1.97.0/windmill_api/models/get_script_by_path_with_draft_response_200_kind.py
+-rw-r--r--   0        0        0      222 2023-05-09 11:11:14.482746 windmill_api-1.97.0/windmill_api/models/get_script_by_path_with_draft_response_200_language.py
+-rw-r--r--   0        0        0     1319 2023-05-09 11:11:35.790617 windmill_api-1.97.0/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py
+-rw-r--r--   0        0        0     1922 2023-05-09 11:11:35.814617 windmill_api-1.97.0/windmill_api/models/get_script_deployment_status_response_200.py
+-rw-r--r--   0        0        0     4157 2023-05-09 11:11:35.874616 windmill_api-1.97.0/windmill_api/models/get_settings_response_200.py
+-rw-r--r--   0        0        0     2428 2023-05-09 11:11:35.858616 windmill_api-1.97.0/windmill_api/models/get_suspended_job_flow_response_200.py
+-rw-r--r--   0        0        0     1764 2023-05-09 11:11:35.898616 windmill_api-1.97.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
+-rw-r--r--   0        0        0     2040 2023-05-09 11:11:35.918616 windmill_api-1.97.0/windmill_api/models/get_suspended_job_flow_response_200_job.py
+-rw-r--r--   0        0        0      204 2023-05-09 11:11:13.186754 windmill_api-1.97.0/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
+-rw-r--r--   0        0        0     4554 2023-05-09 11:11:36.038615 windmill_api-1.97.0/windmill_api/models/get_variable_response_200.py
+-rw-r--r--   0        0        0     1268 2023-05-09 11:11:35.946616 windmill_api-1.97.0/windmill_api/models/get_variable_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2647 2023-05-09 11:11:36.062615 windmill_api-1.97.0/windmill_api/models/global_user_info.py
+-rw-r--r--   0        0        0      176 2023-05-09 11:11:13.706751 windmill_api-1.97.0/windmill_api/models/global_user_info_login_type.py
+-rw-r--r--   0        0        0     1627 2023-05-09 11:11:36.082615 windmill_api-1.97.0/windmill_api/models/global_user_update_json_body.py
+-rw-r--r--   0        0        0     2741 2023-05-09 11:11:36.126614 windmill_api-1.97.0/windmill_api/models/global_whoami_response_200.py
+-rw-r--r--   0        0        0      185 2023-05-09 11:11:13.334753 windmill_api-1.97.0/windmill_api/models/global_whoami_response_200_login_type.py
+-rw-r--r--   0        0        0     2903 2023-05-09 11:11:36.142614 windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5478 2023-05-09 11:11:36.222614 windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      324 2023-05-09 11:11:13.794751 windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1598 2023-05-09 11:11:36.178614 windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1663 2023-05-09 11:11:36.218614 windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2151 2023-05-09 11:11:36.262614 windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3257 2023-05-09 11:11:36.282614 windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      342 2023-05-09 11:11:13.122755 windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1631 2023-05-09 11:11:36.298613 windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3100 2023-05-09 11:11:36.338613 windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      333 2023-05-09 11:11:13.370753 windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1580 2023-05-09 11:11:36.338613 windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-09 11:11:13.678751 windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2722 2023-05-09 11:11:36.402613 windmill_api-1.97.0/windmill_api/models/group.py
+-rw-r--r--   0        0        0     1174 2023-05-09 11:11:36.370613 windmill_api-1.97.0/windmill_api/models/group_extra_perms.py
+-rw-r--r--   0        0        0     1689 2023-05-09 11:11:36.414613 windmill_api-1.97.0/windmill_api/models/identity.py
+-rw-r--r--   0        0        0      143 2023-05-09 11:11:13.518752 windmill_api-1.97.0/windmill_api/models/identity_type.py
+-rw-r--r--   0        0        0     2377 2023-05-09 11:11:36.462612 windmill_api-1.97.0/windmill_api/models/input_.py
+-rw-r--r--   0        0        0     1138 2023-05-09 11:11:36.442613 windmill_api-1.97.0/windmill_api/models/input_args.py
+-rw-r--r--   0        0        0     1820 2023-05-09 11:11:36.486612 windmill_api-1.97.0/windmill_api/models/input_transform_type_0.py
+-rw-r--r--   0        0        0      158 2023-05-09 11:11:13.710751 windmill_api-1.97.0/windmill_api/models/input_transform_type_0_type.py
+-rw-r--r--   0        0        0     1687 2023-05-09 11:11:36.506612 windmill_api-1.97.0/windmill_api/models/input_transform_type_1.py
+-rw-r--r--   0        0        0      158 2023-05-09 11:11:14.314747 windmill_api-1.97.0/windmill_api/models/input_transform_type_1_type.py
+-rw-r--r--   0        0        0     1773 2023-05-09 11:11:36.530612 windmill_api-1.97.0/windmill_api/models/invite_user_json_body.py
+-rw-r--r--   0        0        0     1679 2023-05-09 11:11:36.546612 windmill_api-1.97.0/windmill_api/models/javascript_transform.py
+-rw-r--r--   0        0        0      158 2023-05-09 11:11:13.722751 windmill_api-1.97.0/windmill_api/models/javascript_transform_type.py
+-rw-r--r--   0        0        0     1686 2023-05-09 11:11:36.578612 windmill_api-1.97.0/windmill_api/models/job.py
+-rw-r--r--   0        0        0      174 2023-05-09 11:11:14.362747 windmill_api-1.97.0/windmill_api/models/job_type.py
+-rw-r--r--   0        0        0     3583 2023-05-09 11:11:36.666611 windmill_api-1.97.0/windmill_api/models/list_apps_response_200_item.py
+-rw-r--r--   0        0        0      219 2023-05-09 11:11:13.298754 windmill_api-1.97.0/windmill_api/models/list_apps_response_200_item_execution_mode.py
+-rw-r--r--   0        0        0     1276 2023-05-09 11:11:36.610612 windmill_api-1.97.0/windmill_api/models/list_apps_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      218 2023-05-09 11:11:13.910750 windmill_api-1.97.0/windmill_api/models/list_audit_logs_action_kind.py
+-rw-r--r--   0        0        0     3896 2023-05-09 11:11:36.730611 windmill_api-1.97.0/windmill_api/models/list_audit_logs_response_200_item.py
+-rw-r--r--   0        0        0      237 2023-05-09 11:11:14.466746 windmill_api-1.97.0/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
+-rw-r--r--   0        0        0      640 2023-05-09 11:11:13.874750 windmill_api-1.97.0/windmill_api/models/list_audit_logs_response_200_item_operation.py
+-rw-r--r--   0        0        0     1298 2023-05-09 11:11:36.706611 windmill_api-1.97.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py
+-rw-r--r--   0        0        0    11220 2023-05-09 11:11:36.910610 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item.py
+-rw-r--r--   0        0        0     1288 2023-05-09 11:11:36.758611 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_args.py
+-rw-r--r--   0        0        0     3736 2023-05-09 11:11:36.834610 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7579 2023-05-09 11:11:36.958609 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1901 2023-05-09 11:11:36.946609 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2352 2023-05-09 11:11:36.990609 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      222 2023-05-09 11:11:13.458752 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1806 2023-05-09 11:11:36.998609 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2342 2023-05-09 11:11:37.046609 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      380 2023-05-09 11:11:13.706751 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7160 2023-05-09 11:11:37.130609 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1891 2023-05-09 11:11:37.086609 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2332 2023-05-09 11:11:37.138609 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      220 2023-05-09 11:11:13.578752 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1796 2023-05-09 11:11:37.174609 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2332 2023-05-09 11:11:37.286608 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      378 2023-05-09 11:11:13.806750 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2152 2023-05-09 11:11:37.226609 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      330 2023-05-09 11:11:14.314747 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      219 2023-05-09 11:11:13.802750 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_language.py
+-rw-r--r--   0        0        0     3485 2023-05-09 11:11:37.370608 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7593 2023-05-09 11:11:37.410608 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3498 2023-05-09 11:11:37.430608 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2041 2023-05-09 11:11:37.454608 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2345 2023-05-09 11:11:37.482608 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2295 2023-05-09 11:11:37.498608 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      201 2023-05-09 11:11:13.070755 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2162 2023-05-09 11:11:37.522608 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      201 2023-05-09 11:11:13.966750 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2034 2023-05-09 11:11:37.570608 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2085 2023-05-09 11:11:37.570608 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7471 2023-05-09 11:11:37.694607 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3464 2023-05-09 11:11:37.634607 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2031 2023-05-09 11:11:37.682607 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2335 2023-05-09 11:11:37.726607 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2275 2023-05-09 11:11:37.738607 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      199 2023-05-09 11:11:13.098755 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2142 2023-05-09 11:11:37.770607 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      199 2023-05-09 11:11:13.530752 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2024 2023-05-09 11:11:37.778607 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2075 2023-05-09 11:11:37.810607 windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1865 2023-05-09 11:11:37.882607 windmill_api-1.97.0/windmill_api/models/list_contextual_variables_response_200_item.py
+-rw-r--r--   0        0        0     1863 2023-05-09 11:11:37.854607 windmill_api-1.97.0/windmill_api/models/list_flows_response_200_item.py
+-rw-r--r--   0        0        0     2074 2023-05-09 11:11:37.966606 windmill_api-1.97.0/windmill_api/models/list_folders_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-05-09 11:11:37.914607 windmill_api-1.97.0/windmill_api/models/list_folders_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2958 2023-05-09 11:11:37.974607 windmill_api-1.97.0/windmill_api/models/list_groups_response_200_item.py
+-rw-r--r--   0        0        0     1286 2023-05-09 11:11:37.998607 windmill_api-1.97.0/windmill_api/models/list_groups_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2076 2023-05-09 11:11:38.022606 windmill_api-1.97.0/windmill_api/models/list_hub_apps_response_200.py
+-rw-r--r--   0        0        0     2304 2023-05-09 11:11:38.046606 windmill_api-1.97.0/windmill_api/models/list_hub_apps_response_200_apps_item.py
+-rw-r--r--   0        0        0     2116 2023-05-09 11:11:38.070606 windmill_api-1.97.0/windmill_api/models/list_hub_flows_response_200.py
+-rw-r--r--   0        0        0     2324 2023-05-09 11:11:38.098606 windmill_api-1.97.0/windmill_api/models/list_hub_flows_response_200_flows_item.py
+-rw-r--r--   0        0        0     2106 2023-05-09 11:11:38.118606 windmill_api-1.97.0/windmill_api/models/list_hub_scripts_response_200.py
+-rw-r--r--   0        0        0     2790 2023-05-09 11:11:38.158606 windmill_api-1.97.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py
+-rw-r--r--   0        0        0      262 2023-05-09 11:11:14.034749 windmill_api-1.97.0/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
+-rw-r--r--   0        0        0     2590 2023-05-09 11:11:38.178606 windmill_api-1.97.0/windmill_api/models/list_inputs_response_200_item.py
+-rw-r--r--   0        0        0     1250 2023-05-09 11:11:38.190606 windmill_api-1.97.0/windmill_api/models/list_inputs_response_200_item_args.py
+-rw-r--r--   0        0        0      213 2023-05-09 11:11:13.842750 windmill_api-1.97.0/windmill_api/models/list_inputs_runnable_type.py
+-rw-r--r--   0        0        0     1922 2023-05-09 11:11:38.222606 windmill_api-1.97.0/windmill_api/models/list_jobs_response_200_item.py
+-rw-r--r--   0        0        0      194 2023-05-09 11:11:13.074755 windmill_api-1.97.0/windmill_api/models/list_jobs_response_200_item_type.py
+-rw-r--r--   0        0        0     2076 2023-05-09 11:11:38.238606 windmill_api-1.97.0/windmill_api/models/list_pending_invites_response_200_item.py
+-rw-r--r--   0        0        0    12114 2023-05-09 11:11:38.514605 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item.py
+-rw-r--r--   0        0        0     1245 2023-05-09 11:11:38.266606 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_args.py
+-rw-r--r--   0        0        0     3544 2023-05-09 11:11:38.330606 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7247 2023-05-09 11:11:38.450605 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1858 2023-05-09 11:11:38.530605 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-05-09 11:11:38.554605 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-05-09 11:11:14.550746 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-05-09 11:11:38.570605 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2299 2023-05-09 11:11:38.602605 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      372 2023-05-09 11:11:13.982749 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6858 2023-05-09 11:11:38.682605 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1848 2023-05-09 11:11:38.638605 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2248 2023-05-09 11:11:38.682605 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      212 2023-05-09 11:11:14.290748 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1753 2023-05-09 11:11:38.718605 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2289 2023-05-09 11:11:38.738605 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      370 2023-05-09 11:11:13.650751 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2109 2023-05-09 11:11:38.770604 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      322 2023-05-09 11:11:14.566746 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      211 2023-05-09 11:11:13.834750 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_language.py
+-rw-r--r--   0        0        0     3334 2023-05-09 11:11:38.806604 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7235 2023-05-09 11:11:38.890604 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3357 2023-05-09 11:11:38.866604 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1998 2023-05-09 11:11:38.906604 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-05-09 11:11:38.934604 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-05-09 11:11:38.946604 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-05-09 11:11:14.102749 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-05-09 11:11:38.978604 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-05-09 11:11:13.638751 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-05-09 11:11:38.994604 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-05-09 11:11:39.098604 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7159 2023-05-09 11:11:39.202603 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3323 2023-05-09 11:11:39.158604 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1988 2023-05-09 11:11:39.198603 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-05-09 11:11:39.242603 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-05-09 11:11:39.262603 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-05-09 11:11:13.838750 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-05-09 11:11:39.282603 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-05-09 11:11:13.482752 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-05-09 11:11:39.306603 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-05-09 11:11:39.326603 windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     3045 2023-05-09 11:11:39.366603 windmill_api-1.97.0/windmill_api/models/list_raw_apps_response_200_item.py
+-rw-r--r--   0        0        0     1294 2023-05-09 11:11:39.350603 windmill_api-1.97.0/windmill_api/models/list_raw_apps_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     4884 2023-05-09 11:11:39.454603 windmill_api-1.97.0/windmill_api/models/list_resource_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-05-09 11:11:39.394603 windmill_api-1.97.0/windmill_api/models/list_resource_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2363 2023-05-09 11:11:39.446603 windmill_api-1.97.0/windmill_api/models/list_resource_type_response_200_item.py
+-rw-r--r--   0        0        0     4426 2023-05-09 11:11:39.534602 windmill_api-1.97.0/windmill_api/models/list_schedules_response_200_item.py
+-rw-r--r--   0        0        0     1265 2023-05-09 11:11:39.482603 windmill_api-1.97.0/windmill_api/models/list_schedules_response_200_item_args.py
+-rw-r--r--   0        0        0     1301 2023-05-09 11:11:39.514603 windmill_api-1.97.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     7551 2023-05-09 11:11:39.706602 windmill_api-1.97.0/windmill_api/models/list_scripts_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-05-09 11:11:39.558602 windmill_api-1.97.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-05-09 11:11:14.218748 windmill_api-1.97.0/windmill_api/models/list_scripts_response_200_item_kind.py
+-rw-r--r--   0        0        0      213 2023-05-09 11:11:14.214748 windmill_api-1.97.0/windmill_api/models/list_scripts_response_200_item_language.py
+-rw-r--r--   0        0        0     1265 2023-05-09 11:11:39.594602 windmill_api-1.97.0/windmill_api/models/list_scripts_response_200_item_schema.py
+-rw-r--r--   0        0        0     2985 2023-05-09 11:11:39.730602 windmill_api-1.97.0/windmill_api/models/list_tokens_response_200_item.py
+-rw-r--r--   0        0        0     2250 2023-05-09 11:11:39.750602 windmill_api-1.97.0/windmill_api/models/list_user_workspaces_response_200.py
+-rw-r--r--   0        0        0     1833 2023-05-09 11:11:39.770602 windmill_api-1.97.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
+-rw-r--r--   0        0        0     2896 2023-05-09 11:11:39.806602 windmill_api-1.97.0/windmill_api/models/list_users_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0      198 2023-05-09 11:11:14.242748 windmill_api-1.97.0/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
+-rw-r--r--   0        0        0     4307 2023-05-09 11:11:39.858602 windmill_api-1.97.0/windmill_api/models/list_users_response_200_item.py
+-rw-r--r--   0        0        0     1613 2023-05-09 11:11:39.842602 windmill_api-1.97.0/windmill_api/models/list_users_response_200_item_usage.py
+-rw-r--r--   0        0        0     4608 2023-05-09 11:11:39.934601 windmill_api-1.97.0/windmill_api/models/list_variable_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-05-09 11:11:39.890601 windmill_api-1.97.0/windmill_api/models/list_variable_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2693 2023-05-09 11:11:39.950601 windmill_api-1.97.0/windmill_api/models/list_workers_response_200_item.py
+-rw-r--r--   0        0        0     2086 2023-05-09 11:11:39.974601 windmill_api-1.97.0/windmill_api/models/list_workspace_invites_response_200_item.py
+-rw-r--r--   0        0        0     2082 2023-05-09 11:11:39.990601 windmill_api-1.97.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0     2013 2023-05-09 11:11:40.018601 windmill_api-1.97.0/windmill_api/models/list_workspaces_response_200_item.py
+-rw-r--r--   0        0        0     3388 2023-05-09 11:11:40.062601 windmill_api-1.97.0/windmill_api/models/listable_app.py
+-rw-r--r--   0        0        0      207 2023-05-09 11:11:13.958750 windmill_api-1.97.0/windmill_api/models/listable_app_execution_mode.py
+-rw-r--r--   0        0        0     1207 2023-05-09 11:11:40.050601 windmill_api-1.97.0/windmill_api/models/listable_app_extra_perms.py
+-rw-r--r--   0        0        0     2913 2023-05-09 11:11:40.110601 windmill_api-1.97.0/windmill_api/models/listable_raw_app.py
+-rw-r--r--   0        0        0     1225 2023-05-09 11:11:40.094601 windmill_api-1.97.0/windmill_api/models/listable_raw_app_extra_perms.py
+-rw-r--r--   0        0        0     4751 2023-05-09 11:11:40.190601 windmill_api-1.97.0/windmill_api/models/listable_resource.py
+-rw-r--r--   0        0        0     1232 2023-05-09 11:11:40.138601 windmill_api-1.97.0/windmill_api/models/listable_resource_extra_perms.py
+-rw-r--r--   0        0        0     4486 2023-05-09 11:11:40.278601 windmill_api-1.97.0/windmill_api/models/listable_variable.py
+-rw-r--r--   0        0        0     1232 2023-05-09 11:11:40.218601 windmill_api-1.97.0/windmill_api/models/listable_variable_extra_perms.py
+-rw-r--r--   0        0        0     1513 2023-05-09 11:11:40.254601 windmill_api-1.97.0/windmill_api/models/login.py
+-rw-r--r--   0        0        0     1559 2023-05-09 11:11:40.294601 windmill_api-1.97.0/windmill_api/models/login_json_body.py
+-rw-r--r--   0        0        0     1739 2023-05-09 11:11:40.318601 windmill_api-1.97.0/windmill_api/models/login_with_oauth_json_body.py
+-rw-r--r--   0        0        0     2758 2023-05-09 11:11:40.350600 windmill_api-1.97.0/windmill_api/models/main_arg_signature.py
+-rw-r--r--   0        0        0     5099 2023-05-09 11:11:40.402600 windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item.py
+-rw-r--r--   0        0        0      315 2023-05-09 11:11:13.990749 windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1547 2023-05-09 11:11:40.386600 windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1612 2023-05-09 11:11:40.430600 windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2044 2023-05-09 11:11:40.450600 windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3049 2023-05-09 11:11:40.566600 windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      333 2023-05-09 11:11:13.246754 windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1580 2023-05-09 11:11:40.486600 windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     2862 2023-05-09 11:11:40.542600 windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      324 2023-05-09 11:11:13.302754 windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1529 2023-05-09 11:11:40.578600 windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      169 2023-05-09 11:11:13.250754 windmill_api-1.97.0/windmill_api/models/main_arg_signature_type.py
+-rw-r--r--   0        0        0     2662 2023-05-09 11:11:40.630600 windmill_api-1.97.0/windmill_api/models/new_schedule.py
+-rw-r--r--   0        0        0     1171 2023-05-09 11:11:40.606600 windmill_api-1.97.0/windmill_api/models/new_schedule_args.py
+-rw-r--r--   0        0        0     4866 2023-05-09 11:11:40.714599 windmill_api-1.97.0/windmill_api/models/new_script.py
+-rw-r--r--   0        0        0      238 2023-05-09 11:11:14.038749 windmill_api-1.97.0/windmill_api/models/new_script_kind.py
+-rw-r--r--   0        0        0      196 2023-05-09 11:11:14.250748 windmill_api-1.97.0/windmill_api/models/new_script_language.py
+-rw-r--r--   0        0        0     1171 2023-05-09 11:11:40.682600 windmill_api-1.97.0/windmill_api/models/new_script_schema.py
+-rw-r--r--   0        0        0     5879 2023-05-09 11:11:40.802599 windmill_api-1.97.0/windmill_api/models/new_script_with_draft.py
+-rw-r--r--   0        0        0     5192 2023-05-09 11:11:40.866599 windmill_api-1.97.0/windmill_api/models/new_script_with_draft_draft.py
+-rw-r--r--   0        0        0      252 2023-05-09 11:11:13.538752 windmill_api-1.97.0/windmill_api/models/new_script_with_draft_draft_kind.py
+-rw-r--r--   0        0        0      210 2023-05-09 11:11:13.638751 windmill_api-1.97.0/windmill_api/models/new_script_with_draft_draft_language.py
+-rw-r--r--   0        0        0     1250 2023-05-09 11:11:40.834599 windmill_api-1.97.0/windmill_api/models/new_script_with_draft_draft_schema.py
+-rw-r--r--   0        0        0      247 2023-05-09 11:11:13.150754 windmill_api-1.97.0/windmill_api/models/new_script_with_draft_kind.py
+-rw-r--r--   0        0        0      205 2023-05-09 11:11:13.630751 windmill_api-1.97.0/windmill_api/models/new_script_with_draft_language.py
+-rw-r--r--   0        0        0     1222 2023-05-09 11:11:40.870599 windmill_api-1.97.0/windmill_api/models/new_script_with_draft_schema.py
+-rw-r--r--   0        0        0     2108 2023-05-09 11:11:40.922599 windmill_api-1.97.0/windmill_api/models/new_token.py
+-rw-r--r--   0        0        0     2473 2023-05-09 11:11:40.926599 windmill_api-1.97.0/windmill_api/models/new_token_impersonate.py
+-rw-r--r--   0        0        0     1710 2023-05-09 11:11:40.962598 windmill_api-1.97.0/windmill_api/models/new_user.py
+-rw-r--r--   0        0        0     2584 2023-05-09 11:11:40.986598 windmill_api-1.97.0/windmill_api/models/open_flow.py
+-rw-r--r--   0        0        0     1166 2023-05-09 11:11:40.994598 windmill_api-1.97.0/windmill_api/models/open_flow_schema.py
+-rw-r--r--   0        0        0     3026 2023-05-09 11:11:41.046598 windmill_api-1.97.0/windmill_api/models/open_flow_value.py
+-rw-r--r--   0        0        0     6384 2023-05-09 11:11:41.114597 windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3013 2023-05-09 11:11:41.214597 windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1896 2023-05-09 11:11:41.154597 windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2200 2023-05-09 11:11:41.206597 windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2006 2023-05-09 11:11:41.246597 windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      175 2023-05-09 11:11:13.502752 windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1873 2023-05-09 11:11:41.262596 windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      175 2023-05-09 11:11:14.342747 windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1889 2023-05-09 11:11:41.290596 windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1940 2023-05-09 11:11:41.306596 windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6308 2023-05-09 11:11:41.506595 windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item.py
+-rw-r--r--   0        0        0     2979 2023-05-09 11:11:41.366596 windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1886 2023-05-09 11:11:41.410596 windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2190 2023-05-09 11:11:41.462595 windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1986 2023-05-09 11:11:41.506595 windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      173 2023-05-09 11:11:14.066749 windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1853 2023-05-09 11:11:41.546595 windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      173 2023-05-09 11:11:13.274754 windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1879 2023-05-09 11:11:41.554595 windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1930 2023-05-09 11:11:41.586594 windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2816 2023-05-09 11:11:41.618594 windmill_api-1.97.0/windmill_api/models/open_flow_w_path.py
+-rw-r--r--   0        0        0     1197 2023-05-09 11:11:41.614594 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_schema.py
+-rw-r--r--   0        0        0     3116 2023-05-09 11:11:41.678594 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value.py
+-rw-r--r--   0        0        0     6590 2023-05-09 11:11:41.738594 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module.py
+-rw-r--r--   0        0        0     3117 2023-05-09 11:11:41.738594 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1927 2023-05-09 11:11:41.782593 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2231 2023-05-09 11:11:41.886593 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2073 2023-05-09 11:11:41.826593 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      180 2023-05-09 11:11:13.398753 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1940 2023-05-09 11:11:41.870593 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      180 2023-05-09 11:11:13.350753 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1920 2023-05-09 11:11:41.910593 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1971 2023-05-09 11:11:41.934592 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6514 2023-05-09 11:11:42.118591 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item.py
+-rw-r--r--   0        0        0     3074 2023-05-09 11:11:41.998592 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1917 2023-05-09 11:11:42.046592 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2221 2023-05-09 11:11:42.098591 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2044 2023-05-09 11:11:42.146591 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-09 11:11:13.914750 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1911 2023-05-09 11:11:42.162591 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-09 11:11:14.490746 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1910 2023-05-09 11:11:42.194591 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1961 2023-05-09 11:11:42.210591 windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1989 2023-05-09 11:11:42.238591 windmill_api-1.97.0/windmill_api/models/path_flow.py
+-rw-r--r--   0        0        0     3089 2023-05-09 11:11:42.262590 windmill_api-1.97.0/windmill_api/models/path_flow_input_transforms.py
+-rw-r--r--   0        0        0     2115 2023-05-09 11:11:42.282590 windmill_api-1.97.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      185 2023-05-09 11:11:13.446753 windmill_api-1.97.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1982 2023-05-09 11:11:42.302590 windmill_api-1.97.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      185 2023-05-09 11:11:13.246754 windmill_api-1.97.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      135 2023-05-09 11:11:13.518752 windmill_api-1.97.0/windmill_api/models/path_flow_type.py
+-rw-r--r--   0        0        0     2292 2023-05-09 11:11:42.342590 windmill_api-1.97.0/windmill_api/models/path_script.py
+-rw-r--r--   0        0        0     3181 2023-05-09 11:11:42.354590 windmill_api-1.97.0/windmill_api/models/path_script_input_transforms.py
+-rw-r--r--   0        0        0     2135 2023-05-09 11:11:42.382590 windmill_api-1.97.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      187 2023-05-09 11:11:14.374747 windmill_api-1.97.0/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2002 2023-05-09 11:11:42.398589 windmill_api-1.97.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      187 2023-05-09 11:11:13.854750 windmill_api-1.97.0/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      141 2023-05-09 11:11:13.886750 windmill_api-1.97.0/windmill_api/models/path_script_type.py
+-rw-r--r--   0        0        0     3390 2023-05-09 11:11:42.462589 windmill_api-1.97.0/windmill_api/models/policy.py
+-rw-r--r--   0        0        0      202 2023-05-09 11:11:14.506746 windmill_api-1.97.0/windmill_api/models/policy_execution_mode.py
+-rw-r--r--   0        0        0     1709 2023-05-09 11:11:42.434589 windmill_api-1.97.0/windmill_api/models/policy_triggerables.py
+-rw-r--r--   0        0        0     1279 2023-05-09 11:11:42.462589 windmill_api-1.97.0/windmill_api/models/policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2359 2023-05-09 11:11:42.518589 windmill_api-1.97.0/windmill_api/models/preview.py
+-rw-r--r--   0        0        0     1148 2023-05-09 11:11:42.498589 windmill_api-1.97.0/windmill_api/models/preview_args.py
+-rw-r--r--   0        0        0      194 2023-05-09 11:11:14.278748 windmill_api-1.97.0/windmill_api/models/preview_language.py
+-rw-r--r--   0        0        0     1642 2023-05-09 11:11:42.538589 windmill_api-1.97.0/windmill_api/models/preview_schedule_json_body.py
+-rw-r--r--   0        0        0     2963 2023-05-09 11:11:42.650588 windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5679 2023-05-09 11:11:42.630588 windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      328 2023-05-09 11:11:13.254754 windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1618 2023-05-09 11:11:42.670588 windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1683 2023-05-09 11:11:42.690588 windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2191 2023-05-09 11:11:42.710588 windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3329 2023-05-09 11:11:42.742587 windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      346 2023-05-09 11:11:14.170748 windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1651 2023-05-09 11:11:42.746587 windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3214 2023-05-09 11:11:42.798587 windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      337 2023-05-09 11:11:13.094755 windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1600 2023-05-09 11:11:42.782587 windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      182 2023-05-09 11:11:14.402747 windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0    11580 2023-05-09 11:11:43.114585 windmill_api-1.97.0/windmill_api/models/queued_job.py
+-rw-r--r--   0        0        0     1161 2023-05-09 11:11:42.822587 windmill_api-1.97.0/windmill_api/models/queued_job_args.py
+-rw-r--r--   0        0        0     3202 2023-05-09 11:11:42.890586 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status.py
+-rw-r--r--   0        0        0     6683 2023-05-09 11:11:43.014586 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1774 2023-05-09 11:11:43.050586 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2106 2023-05-09 11:11:43.094585 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      199 2023-05-09 11:11:13.890750 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1679 2023-05-09 11:11:43.134585 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2215 2023-05-09 11:11:43.174585 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      357 2023-05-09 11:11:13.914750 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6294 2023-05-09 11:11:43.330584 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1764 2023-05-09 11:11:43.214584 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2086 2023-05-09 11:11:43.258584 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      197 2023-05-09 11:11:13.370753 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1669 2023-05-09 11:11:43.298584 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2205 2023-05-09 11:11:43.354584 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      355 2023-05-09 11:11:13.082755 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2025 2023-05-09 11:11:43.382583 windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_retry.py
+-rw-r--r--   0        0        0      307 2023-05-09 11:11:14.254748 windmill_api-1.97.0/windmill_api/models/queued_job_job_kind.py
+-rw-r--r--   0        0        0      196 2023-05-09 11:11:13.554752 windmill_api-1.97.0/windmill_api/models/queued_job_language.py
+-rw-r--r--   0        0        0     3079 2023-05-09 11:11:43.422583 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow.py
+-rw-r--r--   0        0        0     6506 2023-05-09 11:11:43.502583 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3069 2023-05-09 11:11:43.582582 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1914 2023-05-09 11:11:43.542582 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2218 2023-05-09 11:11:43.594582 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2040 2023-05-09 11:11:43.630582 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-05-09 11:11:14.050749 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1907 2023-05-09 11:11:43.634582 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-05-09 11:11:13.966750 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1907 2023-05-09 11:11:43.674582 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1958 2023-05-09 11:11:43.678582 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6430 2023-05-09 11:11:43.794581 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3035 2023-05-09 11:11:43.738581 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1904 2023-05-09 11:11:43.778581 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2208 2023-05-09 11:11:43.822581 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2020 2023-05-09 11:11:43.834581 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-05-09 11:11:14.242748 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1887 2023-05-09 11:11:43.950580 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-05-09 11:11:13.822750 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1897 2023-05-09 11:11:43.878580 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1948 2023-05-09 11:11:43.918580 windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     3028 2023-05-09 11:11:43.986580 windmill_api-1.97.0/windmill_api/models/raw_script.py
+-rw-r--r--   0        0        0     3139 2023-05-09 11:11:44.002580 windmill_api-1.97.0/windmill_api/models/raw_script_input_transforms.py
+-rw-r--r--   0        0        0     2125 2023-05-09 11:11:44.026579 windmill_api-1.97.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      186 2023-05-09 11:11:13.846750 windmill_api-1.97.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1992 2023-05-09 11:11:44.046579 windmill_api-1.97.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      186 2023-05-09 11:11:13.770751 windmill_api-1.97.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      196 2023-05-09 11:11:14.398747 windmill_api-1.97.0/windmill_api/models/raw_script_language.py
+-rw-r--r--   0        0        0      146 2023-05-09 11:11:13.110755 windmill_api-1.97.0/windmill_api/models/raw_script_type.py
+-rw-r--r--   0        0        0     1405 2023-05-09 11:11:44.070579 windmill_api-1.97.0/windmill_api/models/refresh_token_json_body.py
+-rw-r--r--   0        0        0     1448 2023-05-09 11:11:44.078579 windmill_api-1.97.0/windmill_api/models/remove_granular_acls_json_body.py
+-rw-r--r--   0        0        0      328 2023-05-09 11:11:13.606752 windmill_api-1.97.0/windmill_api/models/remove_granular_acls_kind.py
+-rw-r--r--   0        0        0     1544 2023-05-09 11:11:44.110579 windmill_api-1.97.0/windmill_api/models/remove_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1567 2023-05-09 11:11:44.118579 windmill_api-1.97.0/windmill_api/models/remove_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3367 2023-05-09 11:11:44.274578 windmill_api-1.97.0/windmill_api/models/resource.py
+-rw-r--r--   0        0        0     1189 2023-05-09 11:11:44.146579 windmill_api-1.97.0/windmill_api/models/resource_extra_perms.py
+-rw-r--r--   0        0        0     2256 2023-05-09 11:11:44.198578 windmill_api-1.97.0/windmill_api/models/resource_type.py
+-rw-r--r--   0        0        0     1278 2023-05-09 11:11:44.234578 windmill_api-1.97.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
+-rw-r--r--   0        0        0     1255 2023-05-09 11:11:44.262578 windmill_api-1.97.0/windmill_api/models/resume_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0     2546 2023-05-09 11:11:44.322578 windmill_api-1.97.0/windmill_api/models/retry.py
+-rw-r--r--   0        0        0     1751 2023-05-09 11:11:44.318578 windmill_api-1.97.0/windmill_api/models/retry_constant.py
+-rw-r--r--   0        0        0     2055 2023-05-09 11:11:44.370577 windmill_api-1.97.0/windmill_api/models/retry_exponential.py
+-rw-r--r--   0        0        0     1210 2023-05-09 11:11:44.354577 windmill_api-1.97.0/windmill_api/models/run_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     2189 2023-05-09 11:11:44.398577 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body.py
+-rw-r--r--   0        0        0     1235 2023-05-09 11:11:44.398577 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_args.py
+-rw-r--r--   0        0        0     3265 2023-05-09 11:11:44.474577 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value.py
+-rw-r--r--   0        0        0     7049 2023-05-09 11:11:44.526576 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3284 2023-05-09 11:11:44.538576 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1975 2023-05-09 11:11:44.574576 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2279 2023-05-09 11:11:44.586576 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2167 2023-05-09 11:11:44.618576 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-05-09 11:11:13.310753 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2034 2023-05-09 11:11:44.630576 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-05-09 11:11:13.234754 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1968 2023-05-09 11:11:44.662576 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2019 2023-05-09 11:11:44.670575 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6939 2023-05-09 11:11:44.894574 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3250 2023-05-09 11:11:44.734575 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1965 2023-05-09 11:11:44.882574 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2269 2023-05-09 11:11:44.930574 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2147 2023-05-09 11:11:44.934574 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      187 2023-05-09 11:11:14.322747 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2014 2023-05-09 11:11:44.970574 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      187 2023-05-09 11:11:14.090749 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1958 2023-05-09 11:11:44.982574 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2009 2023-05-09 11:11:45.010573 windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1220 2023-05-09 11:11:45.010573 windmill_api-1.97.0/windmill_api/models/run_script_by_hash_json_body.py
+-rw-r--r--   0        0        0     1220 2023-05-09 11:11:45.042573 windmill_api-1.97.0/windmill_api/models/run_script_by_path_json_body.py
+-rw-r--r--   0        0        0     2634 2023-05-09 11:11:45.066573 windmill_api-1.97.0/windmill_api/models/run_script_preview_json_body.py
+-rw-r--r--   0        0        0     1245 2023-05-09 11:11:45.074573 windmill_api-1.97.0/windmill_api/models/run_script_preview_json_body_args.py
+-rw-r--r--   0        0        0      211 2023-05-09 11:11:14.210748 windmill_api-1.97.0/windmill_api/models/run_script_preview_json_body_language.py
+-rw-r--r--   0        0        0     1266 2023-05-09 11:11:45.098573 windmill_api-1.97.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     1276 2023-05-09 11:11:45.102573 windmill_api-1.97.0/windmill_api/models/run_wait_result_script_by_path_json_body.py
+-rw-r--r--   0        0        0      203 2023-05-09 11:11:14.150748 windmill_api-1.97.0/windmill_api/models/runnable_type.py
+-rw-r--r--   0        0        0     4086 2023-05-09 11:11:45.190572 windmill_api-1.97.0/windmill_api/models/schedule.py
+-rw-r--r--   0        0        0     1153 2023-05-09 11:11:45.134573 windmill_api-1.97.0/windmill_api/models/schedule_args.py
+-rw-r--r--   0        0        0     1189 2023-05-09 11:11:45.166572 windmill_api-1.97.0/windmill_api/models/schedule_extra_perms.py
+-rw-r--r--   0        0        0     7003 2023-05-09 11:11:45.318571 windmill_api-1.97.0/windmill_api/models/script.py
+-rw-r--r--   0        0        0     1143 2023-05-09 11:11:45.218572 windmill_api-1.97.0/windmill_api/models/script_args.py
+-rw-r--r--   0        0        0     1179 2023-05-09 11:11:45.246572 windmill_api-1.97.0/windmill_api/models/script_extra_perms.py
+-rw-r--r--   0        0        0      235 2023-05-09 11:11:14.050749 windmill_api-1.97.0/windmill_api/models/script_kind.py
+-rw-r--r--   0        0        0      193 2023-05-09 11:11:14.330747 windmill_api-1.97.0/windmill_api/models/script_language.py
+-rw-r--r--   0        0        0     1153 2023-05-09 11:11:45.282571 windmill_api-1.97.0/windmill_api/models/script_schema.py
+-rw-r--r--   0        0        0     1440 2023-05-09 11:11:45.318571 windmill_api-1.97.0/windmill_api/models/set_password_json_body.py
+-rw-r--r--   0        0        0     1470 2023-05-09 11:11:45.354571 windmill_api-1.97.0/windmill_api/models/set_schedule_enabled_json_body.py
+-rw-r--r--   0        0        0     2032 2023-05-09 11:11:45.366571 windmill_api-1.97.0/windmill_api/models/slack_token.py
+-rw-r--r--   0        0        0     1586 2023-05-09 11:11:45.394571 windmill_api-1.97.0/windmill_api/models/slack_token_bot.py
+-rw-r--r--   0        0        0     2227 2023-05-09 11:11:45.418571 windmill_api-1.97.0/windmill_api/models/star_json_body.py
+-rw-r--r--   0        0        0      209 2023-05-09 11:11:14.230748 windmill_api-1.97.0/windmill_api/models/star_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     1772 2023-05-09 11:11:45.446570 windmill_api-1.97.0/windmill_api/models/static_transform.py
+-rw-r--r--   0        0        0      154 2023-05-09 11:11:13.934750 windmill_api-1.97.0/windmill_api/models/static_transform_type.py
+-rw-r--r--   0        0        0     2462 2023-05-09 11:11:45.482570 windmill_api-1.97.0/windmill_api/models/token_response.py
+-rw-r--r--   0        0        0     2921 2023-05-09 11:11:45.514570 windmill_api-1.97.0/windmill_api/models/truncated_token.py
+-rw-r--r--   0        0        0     2249 2023-05-09 11:11:45.534570 windmill_api-1.97.0/windmill_api/models/unstar_json_body.py
+-rw-r--r--   0        0        0      211 2023-05-09 11:11:14.174748 windmill_api-1.97.0/windmill_api/models/unstar_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     2638 2023-05-09 11:11:45.574569 windmill_api-1.97.0/windmill_api/models/update_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-05-09 11:11:45.602569 windmill_api-1.97.0/windmill_api/models/update_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-05-09 11:11:13.710751 windmill_api-1.97.0/windmill_api/models/update_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-05-09 11:11:45.614569 windmill_api-1.97.0/windmill_api/models/update_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-05-09 11:11:45.630569 windmill_api-1.97.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2896 2023-05-09 11:11:45.794568 windmill_api-1.97.0/windmill_api/models/update_flow_json_body.py
+-rw-r--r--   0        0        0     1222 2023-05-09 11:11:45.662569 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_schema.py
+-rw-r--r--   0        0        0     3196 2023-05-09 11:11:45.722568 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value.py
+-rw-r--r--   0        0        0     6855 2023-05-09 11:11:45.906567 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3211 2023-05-09 11:11:45.854567 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1952 2023-05-09 11:11:45.898567 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2256 2023-05-09 11:11:45.942567 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2123 2023-05-09 11:11:45.942567 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      185 2023-05-09 11:11:14.190748 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1990 2023-05-09 11:11:45.982566 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      185 2023-05-09 11:11:14.382747 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1945 2023-05-09 11:11:45.982566 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1996 2023-05-09 11:11:46.026566 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6739 2023-05-09 11:11:46.106566 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3177 2023-05-09 11:11:46.090566 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1942 2023-05-09 11:11:46.130566 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2246 2023-05-09 11:11:46.158565 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2103 2023-05-09 11:11:46.178565 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      183 2023-05-09 11:11:13.818750 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1970 2023-05-09 11:11:46.202565 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      183 2023-05-09 11:11:14.054749 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1935 2023-05-09 11:11:46.218565 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1986 2023-05-09 11:11:46.246565 windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1949 2023-05-09 11:11:46.262565 windmill_api-1.97.0/windmill_api/models/update_folder_json_body.py
+-rw-r--r--   0        0        0     1520 2023-05-09 11:11:46.278565 windmill_api-1.97.0/windmill_api/models/update_group_json_body.py
+-rw-r--r--   0        0        0     1670 2023-05-09 11:11:46.302564 windmill_api-1.97.0/windmill_api/models/update_input.py
+-rw-r--r--   0        0        0     1716 2023-05-09 11:11:46.318564 windmill_api-1.97.0/windmill_api/models/update_input_json_body.py
+-rw-r--r--   0        0        0     1985 2023-05-09 11:11:46.350564 windmill_api-1.97.0/windmill_api/models/update_raw_app_json_body.py
+-rw-r--r--   0        0        0     2036 2023-05-09 11:11:46.362564 windmill_api-1.97.0/windmill_api/models/update_resource_json_body.py
+-rw-r--r--   0        0        0     1847 2023-05-09 11:11:46.390564 windmill_api-1.97.0/windmill_api/models/update_resource_type_json_body.py
+-rw-r--r--   0        0        0     1541 2023-05-09 11:11:46.398564 windmill_api-1.97.0/windmill_api/models/update_resource_value_json_body.py
+-rw-r--r--   0        0        0     1953 2023-05-09 11:11:46.434563 windmill_api-1.97.0/windmill_api/models/update_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-09 11:11:46.426563 windmill_api-1.97.0/windmill_api/models/update_schedule_json_body_args.py
+-rw-r--r--   0        0        0     2066 2023-05-09 11:11:46.474563 windmill_api-1.97.0/windmill_api/models/update_user_json_body.py
+-rw-r--r--   0        0        0     2316 2023-05-09 11:11:46.490563 windmill_api-1.97.0/windmill_api/models/update_variable_json_body.py
+-rw-r--r--   0        0        0     1478 2023-05-09 11:11:46.510563 windmill_api-1.97.0/windmill_api/models/usage.py
+-rw-r--r--   0        0        0     4071 2023-05-09 11:11:46.678562 windmill_api-1.97.0/windmill_api/models/user.py
+-rw-r--r--   0        0        0     1501 2023-05-09 11:11:46.542563 windmill_api-1.97.0/windmill_api/models/user_usage.py
+-rw-r--r--   0        0        0     2122 2023-05-09 11:11:46.678562 windmill_api-1.97.0/windmill_api/models/user_workspace_list.py
+-rw-r--r--   0        0        0     1767 2023-05-09 11:11:46.718562 windmill_api-1.97.0/windmill_api/models/user_workspace_list_workspaces_item.py
+-rw-r--r--   0        0        0     4222 2023-05-09 11:11:46.770561 windmill_api-1.97.0/windmill_api/models/whoami_response_200.py
+-rw-r--r--   0        0        0     1572 2023-05-09 11:11:46.754561 windmill_api-1.97.0/windmill_api/models/whoami_response_200_usage.py
+-rw-r--r--   0        0        0     4211 2023-05-09 11:11:46.842561 windmill_api-1.97.0/windmill_api/models/whois_response_200.py
+-rw-r--r--   0        0        0     1567 2023-05-09 11:11:46.806561 windmill_api-1.97.0/windmill_api/models/whois_response_200_usage.py
+-rw-r--r--   0        0        0     2604 2023-05-09 11:11:46.862560 windmill_api-1.97.0/windmill_api/models/worker_ping.py
+-rw-r--r--   0        0        0     1901 2023-05-09 11:11:46.890560 windmill_api-1.97.0/windmill_api/models/workspace.py
+-rw-r--r--   0        0        0     1974 2023-05-09 11:11:46.902560 windmill_api-1.97.0/windmill_api/models/workspace_invite.py
+-rw-r--r--   0        0        0       25 2023-05-09 11:11:00.994841 windmill_api-1.97.0/windmill_api/py.typed
+-rw-r--r--   0        0        0      939 2023-05-09 11:11:46.910560 windmill_api-1.97.0/windmill_api/types.py
+-rw-r--r--   0        0        0     4362 1970-01-01 00:00:00.000000 windmill_api-1.97.0/setup.py
+-rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.97.0/PKG-INFO
```

### Comparing `windmill_api-1.96.3/LICENSE` & `windmill_api-1.97.0/LICENSE`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/README.md` & `windmill_api-1.97.0/README.md`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/pyproject.toml` & `windmill_api-1.97.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "windmill-api"
-version = "1.96.3"
+version = "1.97.0"
 description = "A client library for accessing Windmill API"
 license = "Apache-2.0"
 
 authors = ["Ruben Fiszel <ruben@windmill.dev>"]
 
 readme = "README.md"
 packages = [
```

### Comparing `windmill_api-1.96.3/windmill_api/api/app/create_app.py` & `windmill_api-1.97.0/windmill_api/api/app/create_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/app/delete_app.py` & `windmill_api-1.97.0/windmill_api/api/app/delete_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/app/execute_component.py` & `windmill_api-1.97.0/windmill_api/api/app/execute_component.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/app/exists_app.py` & `windmill_api-1.97.0/windmill_api/api/app/exists_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/app/get_app_by_path.py` & `windmill_api-1.97.0/windmill_api/api/app/get_app_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/app/get_app_by_path_with_draft.py` & `windmill_api-1.97.0/windmill_api/api/app/get_app_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/app/get_app_by_version.py` & `windmill_api-1.97.0/windmill_api/api/app/get_app_by_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/app/get_hub_app_by_id.py` & `windmill_api-1.97.0/windmill_api/api/app/get_hub_app_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/app/get_public_app_by_secret.py` & `windmill_api-1.97.0/windmill_api/api/app/get_public_app_by_secret.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/app/get_public_secret_of_app.py` & `windmill_api-1.97.0/windmill_api/api/app/get_public_secret_of_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/app/list_apps.py` & `windmill_api-1.97.0/windmill_api/api/app/list_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/app/list_hub_apps.py` & `windmill_api-1.97.0/windmill_api/api/app/list_hub_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/app/update_app.py` & `windmill_api-1.97.0/windmill_api/api/app/update_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/audit/get_audit_log.py` & `windmill_api-1.97.0/windmill_api/api/audit/get_audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/audit/list_audit_logs.py` & `windmill_api-1.97.0/windmill_api/api/audit/list_audit_logs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/capture/create_capture.py` & `windmill_api-1.97.0/windmill_api/api/capture/create_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/capture/get_capture.py` & `windmill_api-1.97.0/windmill_api/api/capture/get_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/capture/update_capture.py` & `windmill_api-1.97.0/windmill_api/api/capture/update_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/draft/create_draft.py` & `windmill_api-1.97.0/windmill_api/api/draft/create_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/favorite/star.py` & `windmill_api-1.97.0/windmill_api/api/favorite/star.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/favorite/unstar.py` & `windmill_api-1.97.0/windmill_api/api/favorite/unstar.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/flow/archive_flow_by_path.py` & `windmill_api-1.97.0/windmill_api/api/flow/archive_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/flow/create_flow.py` & `windmill_api-1.97.0/windmill_api/api/flow/create_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/flow/delete_flow_by_path.py` & `windmill_api-1.97.0/windmill_api/api/flow/delete_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/flow/exists_flow_by_path.py` & `windmill_api-1.97.0/windmill_api/api/flow/exists_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/flow/get_flow_by_path.py` & `windmill_api-1.97.0/windmill_api/api/flow/get_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/flow/get_flow_by_path_with_draft.py` & `windmill_api-1.97.0/windmill_api/api/flow/get_flow_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/flow/get_flow_input_history_by_path.py` & `windmill_api-1.97.0/windmill_api/api/flow/get_flow_input_history_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/flow/get_hub_flow_by_id.py` & `windmill_api-1.97.0/windmill_api/api/flow/get_hub_flow_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/flow/list_flow_paths.py` & `windmill_api-1.97.0/windmill_api/api/flow/list_flow_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/flow/list_flows.py` & `windmill_api-1.97.0/windmill_api/api/flow/list_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/flow/list_hub_flows.py` & `windmill_api-1.97.0/windmill_api/api/flow/list_hub_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/flow/update_flow.py` & `windmill_api-1.97.0/windmill_api/api/flow/update_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/folder/add_owner_to_folder.py` & `windmill_api-1.97.0/windmill_api/api/folder/add_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/folder/create_folder.py` & `windmill_api-1.97.0/windmill_api/api/folder/create_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/folder/delete_folder.py` & `windmill_api-1.97.0/windmill_api/api/folder/delete_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/folder/get_folder.py` & `windmill_api-1.97.0/windmill_api/api/folder/get_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/folder/get_folder_usage.py` & `windmill_api-1.97.0/windmill_api/api/folder/get_folder_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/folder/list_folder_names.py` & `windmill_api-1.97.0/windmill_api/api/folder/list_folder_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/folder/list_folders.py` & `windmill_api-1.97.0/windmill_api/api/folder/list_folders.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/folder/remove_owner_to_folder.py` & `windmill_api-1.97.0/windmill_api/api/folder/remove_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/folder/update_folder.py` & `windmill_api-1.97.0/windmill_api/api/folder/update_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/granular_acl/add_granular_acls.py` & `windmill_api-1.97.0/windmill_api/api/granular_acl/add_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/granular_acl/get_granular_acls.py` & `windmill_api-1.97.0/windmill_api/api/granular_acl/get_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/granular_acl/remove_granular_acls.py` & `windmill_api-1.97.0/windmill_api/api/granular_acl/remove_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/group/add_user_to_group.py` & `windmill_api-1.97.0/windmill_api/api/group/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/group/create_group.py` & `windmill_api-1.97.0/windmill_api/api/group/create_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/group/delete_group.py` & `windmill_api-1.97.0/windmill_api/api/group/delete_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/group/get_group.py` & `windmill_api-1.97.0/windmill_api/api/group/get_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/group/list_group_names.py` & `windmill_api-1.97.0/windmill_api/api/group/list_group_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/group/list_groups.py` & `windmill_api-1.97.0/windmill_api/api/group/list_groups.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/group/remove_user_to_group.py` & `windmill_api-1.97.0/windmill_api/api/group/remove_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/group/update_group.py` & `windmill_api-1.97.0/windmill_api/api/group/update_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/input_/create_input.py` & `windmill_api-1.97.0/windmill_api/api/input_/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/input_/delete_input.py` & `windmill_api-1.97.0/windmill_api/api/input_/delete_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/input_/get_input_history.py` & `windmill_api-1.97.0/windmill_api/api/input_/get_input_history.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/input_/list_inputs.py` & `windmill_api-1.97.0/windmill_api/api/input_/list_inputs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/input_/update_input.py` & `windmill_api-1.97.0/windmill_api/api/input_/update_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/cancel_queued_job.py` & `windmill_api-1.97.0/windmill_api/api/job/cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/cancel_suspended_job_get.py` & `windmill_api-1.97.0/windmill_api/api/job/cancel_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/cancel_suspended_job_post.py` & `windmill_api-1.97.0/windmill_api/api/job/cancel_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/create_job_signature.py` & `windmill_api-1.97.0/windmill_api/api/job/create_job_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/delete_completed_job.py` & `windmill_api-1.97.0/windmill_api/api/job/delete_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/force_cancel_queued_job.py` & `windmill_api-1.97.0/windmill_api/api/job/force_cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/get_completed_job.py` & `windmill_api-1.97.0/windmill_api/api/job/get_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/get_completed_job_result.py` & `windmill_api-1.97.0/windmill_api/api/job/get_completed_job_result.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/get_job.py` & `windmill_api-1.97.0/windmill_api/api/job/get_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/get_job_updates.py` & `windmill_api-1.97.0/windmill_api/api/job/get_job_updates.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/get_resume_urls.py` & `windmill_api-1.97.0/windmill_api/api/job/get_resume_urls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/get_suspended_job_flow.py` & `windmill_api-1.97.0/windmill_api/api/job/get_suspended_job_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/list_completed_jobs.py` & `windmill_api-1.97.0/windmill_api/api/job/list_completed_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/list_jobs.py` & `windmill_api-1.97.0/windmill_api/api/job/list_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/list_queue.py` & `windmill_api-1.97.0/windmill_api/api/job/list_queue.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/result_by_id.py` & `windmill_api-1.97.0/windmill_api/api/job/result_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/resume_suspended_flow_as_owner.py` & `windmill_api-1.97.0/windmill_api/api/job/resume_suspended_flow_as_owner.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/resume_suspended_job_get.py` & `windmill_api-1.97.0/windmill_api/api/job/resume_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/resume_suspended_job_post.py` & `windmill_api-1.97.0/windmill_api/api/job/resume_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/run_flow_by_path.py` & `windmill_api-1.97.0/windmill_api/api/job/run_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/run_flow_preview.py` & `windmill_api-1.97.0/windmill_api/api/job/run_flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/run_script_by_hash.py` & `windmill_api-1.97.0/windmill_api/api/job/run_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/run_script_by_path.py` & `windmill_api-1.97.0/windmill_api/api/job/run_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/run_script_preview.py` & `windmill_api-1.97.0/windmill_api/api/job/run_script_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/run_wait_result_flow_by_path.py` & `windmill_api-1.97.0/windmill_api/api/job/run_wait_result_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/run_wait_result_script_by_path.py` & `windmill_api-1.97.0/windmill_api/api/job/run_wait_result_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/job/run_wait_result_script_by_path_get.py` & `windmill_api-1.97.0/windmill_api/api/job/run_wait_result_script_by_path_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/oauth/connect_callback.py` & `windmill_api-1.97.0/windmill_api/api/oauth/connect_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/oauth/connect_slack_callback.py` & `windmill_api-1.97.0/windmill_api/api/oauth/connect_slack_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/oauth/create_account.py` & `windmill_api-1.97.0/windmill_api/api/oauth/create_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/oauth/disconnect_account.py` & `windmill_api-1.97.0/windmill_api/api/oauth/disconnect_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/oauth/disconnect_slack.py` & `windmill_api-1.97.0/windmill_api/api/oauth/disconnect_slack.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/oauth/list_o_auth_connects.py` & `windmill_api-1.97.0/windmill_api/api/oauth/list_o_auth_connects.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/oauth/list_o_auth_logins.py` & `windmill_api-1.97.0/windmill_api/api/oauth/list_o_auth_logins.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/oauth/refresh_token.py` & `windmill_api-1.97.0/windmill_api/api/oauth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/raw_app/create_raw_app.py` & `windmill_api-1.97.0/windmill_api/api/raw_app/create_raw_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/raw_app/delete_raw_app.py` & `windmill_api-1.97.0/windmill_api/api/raw_app/delete_raw_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/raw_app/exists_raw_app.py` & `windmill_api-1.97.0/windmill_api/api/raw_app/exists_raw_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/raw_app/get_raw_app_data.py` & `windmill_api-1.97.0/windmill_api/api/raw_app/get_raw_app_data.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/raw_app/list_raw_apps.py` & `windmill_api-1.97.0/windmill_api/api/raw_app/list_raw_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/raw_app/update_raw_app.py` & `windmill_api-1.97.0/windmill_api/api/raw_app/update_raw_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/resource/create_resource.py` & `windmill_api-1.97.0/windmill_api/api/resource/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/resource/create_resource_type.py` & `windmill_api-1.97.0/windmill_api/api/resource/create_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/resource/delete_resource.py` & `windmill_api-1.97.0/windmill_api/api/resource/delete_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/resource/delete_resource_type.py` & `windmill_api-1.97.0/windmill_api/api/resource/delete_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/resource/exists_resource.py` & `windmill_api-1.97.0/windmill_api/api/resource/exists_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/resource/exists_resource_type.py` & `windmill_api-1.97.0/windmill_api/api/resource/exists_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/resource/get_resource.py` & `windmill_api-1.97.0/windmill_api/api/resource/get_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/resource/get_resource_type.py` & `windmill_api-1.97.0/windmill_api/api/resource/get_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/resource/get_resource_value.py` & `windmill_api-1.97.0/windmill_api/api/resource/get_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/resource/list_resource.py` & `windmill_api-1.97.0/windmill_api/api/resource/list_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/resource/list_resource_type.py` & `windmill_api-1.97.0/windmill_api/api/resource/list_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/resource/list_resource_type_names.py` & `windmill_api-1.97.0/windmill_api/api/resource/list_resource_type_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/resource/update_resource.py` & `windmill_api-1.97.0/windmill_api/api/resource/update_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/resource/update_resource_type.py` & `windmill_api-1.97.0/windmill_api/api/resource/update_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/resource/update_resource_value.py` & `windmill_api-1.97.0/windmill_api/api/resource/update_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/schedule/create_schedule.py` & `windmill_api-1.97.0/windmill_api/api/schedule/create_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/schedule/delete_schedule.py` & `windmill_api-1.97.0/windmill_api/api/schedule/delete_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/schedule/exists_schedule.py` & `windmill_api-1.97.0/windmill_api/api/schedule/exists_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/schedule/get_schedule.py` & `windmill_api-1.97.0/windmill_api/api/schedule/get_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/schedule/list_schedules.py` & `windmill_api-1.97.0/windmill_api/api/schedule/list_schedules.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/schedule/preview_schedule.py` & `windmill_api-1.97.0/windmill_api/api/schedule/preview_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/schedule/set_schedule_enabled.py` & `windmill_api-1.97.0/windmill_api/api/schedule/set_schedule_enabled.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/schedule/update_schedule.py` & `windmill_api-1.97.0/windmill_api/api/schedule/update_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/archive_script_by_hash.py` & `windmill_api-1.97.0/windmill_api/api/script/archive_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/archive_script_by_path.py` & `windmill_api-1.97.0/windmill_api/api/script/archive_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/bash_to_jsonschema.py` & `windmill_api-1.97.0/windmill_api/api/script/bash_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/create_script.py` & `windmill_api-1.97.0/windmill_api/api/script/create_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/delete_script_by_hash.py` & `windmill_api-1.97.0/windmill_api/api/script/delete_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/delete_script_by_path.py` & `windmill_api-1.97.0/windmill_api/api/script/delete_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/deno_to_jsonschema.py` & `windmill_api-1.97.0/windmill_api/api/script/deno_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/exists_script_by_path.py` & `windmill_api-1.97.0/windmill_api/api/script/exists_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/get_hub_script_by_path.py` & `windmill_api-1.97.0/windmill_api/api/script/get_hub_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/get_hub_script_content_by_path.py` & `windmill_api-1.97.0/windmill_api/api/script/get_hub_script_content_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/get_script_by_hash.py` & `windmill_api-1.97.0/windmill_api/api/script/get_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/get_script_by_path.py` & `windmill_api-1.97.0/windmill_api/api/script/get_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/get_script_by_path_with_draft.py` & `windmill_api-1.97.0/windmill_api/api/script/get_script_by_path_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/get_script_deployment_status.py` & `windmill_api-1.97.0/windmill_api/api/script/get_script_deployment_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/go_to_jsonschema.py` & `windmill_api-1.97.0/windmill_api/api/script/go_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/list_hub_scripts.py` & `windmill_api-1.97.0/windmill_api/api/script/list_hub_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/list_script_paths.py` & `windmill_api-1.97.0/windmill_api/api/script/list_script_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/list_scripts.py` & `windmill_api-1.97.0/windmill_api/api/script/list_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/python_to_jsonschema.py` & `windmill_api-1.97.0/windmill_api/api/script/python_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/raw_script_by_hash.py` & `windmill_api-1.97.0/windmill_api/api/script/raw_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/raw_script_by_path.py` & `windmill_api-1.97.0/windmill_api/api/script/raw_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/script/raw_script_by_path_tokened.py` & `windmill_api-1.97.0/windmill_api/api/script/raw_script_by_path_tokened.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/settings/backend_version.py` & `windmill_api-1.97.0/windmill_api/api/settings/backend_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/settings/get_open_api_yaml.py` & `windmill_api-1.97.0/windmill_api/api/settings/get_open_api_yaml.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/accept_invite.py` & `windmill_api-1.97.0/windmill_api/api/user/accept_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/create_token.py` & `windmill_api-1.97.0/windmill_api/api/user/create_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/create_token_impersonate.py` & `windmill_api-1.97.0/windmill_api/api/user/create_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/create_user.py` & `windmill_api-1.97.0/windmill_api/api/user/create_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/create_user_globally.py` & `windmill_api-1.97.0/windmill_api/api/user/create_user_globally.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/decline_invite.py` & `windmill_api-1.97.0/windmill_api/api/user/decline_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/delete_token.py` & `windmill_api-1.97.0/windmill_api/api/user/delete_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/delete_user.py` & `windmill_api-1.97.0/windmill_api/api/user/delete_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/get_current_email.py` & `windmill_api-1.97.0/windmill_api/api/user/get_current_email.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/get_usage.py` & `windmill_api-1.97.0/windmill_api/api/user/get_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/global_user_delete.py` & `windmill_api-1.97.0/windmill_api/api/user/global_user_delete.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/global_user_update.py` & `windmill_api-1.97.0/windmill_api/api/user/global_user_update.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/global_whoami.py` & `windmill_api-1.97.0/windmill_api/api/user/global_whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/is_owner_of_path.py` & `windmill_api-1.97.0/windmill_api/api/user/is_owner_of_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/leave_workspace.py` & `windmill_api-1.97.0/windmill_api/api/user/leave_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/list_tokens.py` & `windmill_api-1.97.0/windmill_api/api/user/list_tokens.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/list_usernames.py` & `windmill_api-1.97.0/windmill_api/api/user/list_usernames.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/list_users.py` & `windmill_api-1.97.0/windmill_api/api/user/list_users.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/list_users_as_super_admin.py` & `windmill_api-1.97.0/windmill_api/api/user/list_users_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/list_workspace_invites.py` & `windmill_api-1.97.0/windmill_api/api/user/list_workspace_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/login.py` & `windmill_api-1.97.0/windmill_api/api/user/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/login_with_oauth.py` & `windmill_api-1.97.0/windmill_api/api/user/login_with_oauth.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/logout.py` & `windmill_api-1.97.0/windmill_api/api/user/logout.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/set_password.py` & `windmill_api-1.97.0/windmill_api/api/user/set_password.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/update_user.py` & `windmill_api-1.97.0/windmill_api/api/user/update_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/whoami.py` & `windmill_api-1.97.0/windmill_api/api/user/whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/user/whois.py` & `windmill_api-1.97.0/windmill_api/api/user/whois.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/variable/create_variable.py` & `windmill_api-1.97.0/windmill_api/api/variable/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/variable/delete_variable.py` & `windmill_api-1.97.0/windmill_api/api/variable/delete_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/variable/exists_variable.py` & `windmill_api-1.97.0/windmill_api/api/variable/exists_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/variable/get_variable.py` & `windmill_api-1.97.0/windmill_api/api/variable/get_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/variable/list_contextual_variables.py` & `windmill_api-1.97.0/windmill_api/api/variable/list_contextual_variables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/variable/list_variable.py` & `windmill_api-1.97.0/windmill_api/api/variable/list_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/variable/update_variable.py` & `windmill_api-1.97.0/windmill_api/api/variable/update_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/worker/get_custom_tags.py` & `windmill_api-1.97.0/windmill_api/api/worker/get_custom_tags.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/worker/list_workers.py` & `windmill_api-1.97.0/windmill_api/api/worker/list_workers.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/add_user.py` & `windmill_api-1.97.0/windmill_api/api/workspace/add_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/archive_workspace.py` & `windmill_api-1.97.0/windmill_api/api/workspace/archive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/create_workspace.py` & `windmill_api-1.97.0/windmill_api/api/workspace/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/delete_invite.py` & `windmill_api-1.97.0/windmill_api/api/workspace/delete_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/delete_workspace.py` & `windmill_api-1.97.0/windmill_api/api/workspace/delete_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/edit_auto_invite.py` & `windmill_api-1.97.0/windmill_api/api/workspace/edit_auto_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/edit_slack_command.py` & `windmill_api-1.97.0/windmill_api/api/workspace/edit_slack_command.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/edit_webhook.py` & `windmill_api-1.97.0/windmill_api/api/workspace/edit_webhook.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/exists_username.py` & `windmill_api-1.97.0/windmill_api/api/workspace/exists_username.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/exists_workspace.py` & `windmill_api-1.97.0/windmill_api/api/workspace/exists_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/get_premium_info.py` & `windmill_api-1.97.0/windmill_api/api/workspace/get_premium_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/get_settings.py` & `windmill_api-1.97.0/windmill_api/api/workspace/get_settings.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/invite_user.py` & `windmill_api-1.97.0/windmill_api/api/workspace/invite_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/is_domain_allowed.py` & `windmill_api-1.97.0/windmill_api/api/workspace/is_domain_allowed.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/list_pending_invites.py` & `windmill_api-1.97.0/windmill_api/api/workspace/list_pending_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/list_user_workspaces.py` & `windmill_api-1.97.0/windmill_api/api/workspace/list_user_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/list_workspaces.py` & `windmill_api-1.97.0/windmill_api/api/workspace/list_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/list_workspaces_as_super_admin.py` & `windmill_api-1.97.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/api/workspace/unarchive_workspace.py` & `windmill_api-1.97.0/windmill_api/api/workspace/unarchive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/client.py` & `windmill_api-1.97.0/windmill_api/client.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/accept_invite_json_body.py` & `windmill_api-1.97.0/windmill_api/models/accept_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/add_granular_acls_json_body.py` & `windmill_api-1.97.0/windmill_api/models/add_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/add_owner_to_folder_json_body.py` & `windmill_api-1.97.0/windmill_api/models/add_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/add_user_json_body.py` & `windmill_api-1.97.0/windmill_api/models/add_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/add_user_to_group_json_body.py` & `windmill_api-1.97.0/windmill_api/models/add_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/app_with_last_version.py` & `windmill_api-1.97.0/windmill_api/models/app_with_last_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/app_with_last_version_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/app_with_last_version_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/app_with_last_version_policy.py` & `windmill_api-1.97.0/windmill_api/models/app_with_last_version_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/app_with_last_version_policy_triggerables.py` & `windmill_api-1.97.0/windmill_api/models/app_with_last_version_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py` & `windmill_api-1.97.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/app_with_last_version_w_draft.py` & `windmill_api-1.97.0/windmill_api/models/app_with_last_version_w_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/app_with_last_version_w_draft_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/app_with_last_version_w_draft_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/app_with_last_version_w_draft_policy.py` & `windmill_api-1.97.0/windmill_api/models/app_with_last_version_w_draft_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py` & `windmill_api-1.97.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py` & `windmill_api-1.97.0/windmill_api/models/app_with_last_version_w_draft_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/archive_flow_by_path_json_body.py` & `windmill_api-1.97.0/windmill_api/models/archive_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/archive_script_by_hash_response_200.py` & `windmill_api-1.97.0/windmill_api/models/archive_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/archive_script_by_hash_response_200_schema.py` & `windmill_api-1.97.0/windmill_api/models/archive_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/audit_log.py` & `windmill_api-1.97.0/windmill_api/models/audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/audit_log_operation.py` & `windmill_api-1.97.0/windmill_api/models/audit_log_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/audit_log_parameters.py` & `windmill_api-1.97.0/windmill_api/models/audit_log_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200.py` & `windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item.py` & `windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.97.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_all.py` & `windmill_api-1.97.0/windmill_api/models/branch_all.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_all_branches_item.py` & `windmill_api-1.97.0/windmill_api/models/branch_all_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_all_branches_item_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one.py` & `windmill_api-1.97.0/windmill_api/models/branch_one.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_branches_item.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_branches_item_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_default_item.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_default_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_default_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_default_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_default_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_default_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_default_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/branch_one_default_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/branch_one_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/cancel_queued_job_json_body.py` & `windmill_api-1.97.0/windmill_api/models/cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/cancel_suspended_job_post_json_body.py` & `windmill_api-1.97.0/windmill_api/models/cancel_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job.py` & `windmill_api-1.97.0/windmill_api/models/completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_args.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_flow_status.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_failure_module_branchall.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_failure_module_iterator.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_modules_item_branchall.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_modules_item_iterator.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_flow_status_retry.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/connect_callback_json_body.py` & `windmill_api-1.97.0/windmill_api/models/connect_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/connect_callback_response_200.py` & `windmill_api-1.97.0/windmill_api/models/connect_callback_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/connect_slack_callback_json_body.py` & `windmill_api-1.97.0/windmill_api/models/connect_slack_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/contextual_variable.py` & `windmill_api-1.97.0/windmill_api/models/contextual_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_account_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_account_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_app_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_app_json_body_policy.py` & `windmill_api-1.97.0/windmill_api/models/create_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_app_json_body_policy_triggerables.py` & `windmill_api-1.97.0/windmill_api/models/create_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.97.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_draft_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_draft_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_flow_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_folder_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_group_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_input.py` & `windmill_api-1.97.0/windmill_api/models/create_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_input_args.py` & `windmill_api-1.97.0/windmill_api/models/create_input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_input_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_input_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_input_json_body_args.py` & `windmill_api-1.97.0/windmill_api/models/create_input_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_raw_app_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_raw_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_resource.py` & `windmill_api-1.97.0/windmill_api/models/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_resource_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_resource_type_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_schedule_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_schedule_json_body_args.py` & `windmill_api-1.97.0/windmill_api/models/create_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_script_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_script_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_script_json_body_schema.py` & `windmill_api-1.97.0/windmill_api/models/create_script_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_token_impersonate_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_token_impersonate_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_token_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_user_globally_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_user_globally_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_user_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_variable.py` & `windmill_api-1.97.0/windmill_api/models/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_variable_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_workspace.py` & `windmill_api-1.97.0/windmill_api/models/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/create_workspace_json_body.py` & `windmill_api-1.97.0/windmill_api/models/create_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/decline_invite_json_body.py` & `windmill_api-1.97.0/windmill_api/models/decline_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_args.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_invite_json_body.py` & `windmill_api-1.97.0/windmill_api/models/delete_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_script_by_hash_response_200.py` & `windmill_api-1.97.0/windmill_api/models/delete_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/delete_script_by_hash_response_200_schema.py` & `windmill_api-1.97.0/windmill_api/models/delete_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200.py` & `windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item.py` & `windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.97.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/edit_auto_invite_json_body.py` & `windmill_api-1.97.0/windmill_api/models/edit_auto_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/edit_resource.py` & `windmill_api-1.97.0/windmill_api/models/edit_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/edit_resource_type.py` & `windmill_api-1.97.0/windmill_api/models/edit_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/edit_schedule.py` & `windmill_api-1.97.0/windmill_api/models/edit_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/edit_schedule_args.py` & `windmill_api-1.97.0/windmill_api/models/edit_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/edit_slack_command_json_body.py` & `windmill_api-1.97.0/windmill_api/models/edit_slack_command_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/edit_variable.py` & `windmill_api-1.97.0/windmill_api/models/edit_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/edit_webhook_json_body.py` & `windmill_api-1.97.0/windmill_api/models/edit_webhook_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/edit_workspace_user.py` & `windmill_api-1.97.0/windmill_api/models/edit_workspace_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/execute_component_json_body.py` & `windmill_api-1.97.0/windmill_api/models/execute_component_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py` & `windmill_api-1.97.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/execute_component_json_body_raw_code.py` & `windmill_api-1.97.0/windmill_api/models/execute_component_json_body_raw_code.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/exists_username_json_body.py` & `windmill_api-1.97.0/windmill_api/models/exists_username_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/exists_workspace_json_body.py` & `windmill_api-1.97.0/windmill_api/models/exists_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow.py` & `windmill_api-1.97.0/windmill_api/models/flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/flow_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_metadata.py` & `windmill_api-1.97.0/windmill_api/models/flow_metadata.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_metadata_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/flow_metadata_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module.py` & `windmill_api-1.97.0/windmill_api/models/flow_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_0.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_0_input_transforms.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_1.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_1_input_transforms.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_2.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_2_input_transforms.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_module_value_2_type_6.py` & `windmill_api-1.97.0/windmill_api/models/flow_module_value_2_type_6.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_args.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_failure_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_preview_value_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/flow_preview_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_schema.py` & `windmill_api-1.97.0/windmill_api/models/flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status.py` & `windmill_api-1.97.0/windmill_api/models/flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_failure_module_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_failure_module_branch_chosen.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_failure_module_branchall.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_failure_module_iterator.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_module.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_module_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_module_branch_chosen.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_module_branchall.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_module_iterator.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_modules_item_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_modules_item_branch_chosen.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_modules_item_branchall.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_modules_item_iterator.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_status_retry.py` & `windmill_api-1.97.0/windmill_api/models/flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value.py` & `windmill_api-1.97.0/windmill_api/models/flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_failure_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/flow_value_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/folder.py` & `windmill_api-1.97.0/windmill_api/models/folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/folder_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/folder_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/force_cancel_queued_job_json_body.py` & `windmill_api-1.97.0/windmill_api/models/force_cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/forloop_flow.py` & `windmill_api-1.97.0/windmill_api/models/forloop_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/forloop_flow_iterator_type_0.py` & `windmill_api-1.97.0/windmill_api/models/forloop_flow_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/forloop_flow_iterator_type_1.py` & `windmill_api-1.97.0/windmill_api/models/forloop_flow_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/forloop_flow_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/forloop_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_app_by_path_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_app_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_app_by_path_response_200_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_app_by_path_response_200_policy.py` & `windmill_api-1.97.0/windmill_api/models/get_app_by_path_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py` & `windmill_api-1.97.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.97.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_app_by_path_with_draft_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_app_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/get_app_by_path_with_draft_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py` & `windmill_api-1.97.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py` & `windmill_api-1.97.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.97.0/windmill_api/models/get_app_by_path_with_draft_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_app_by_version_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_app_by_version_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_app_by_version_response_200_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_app_by_version_response_200_policy.py` & `windmill_api-1.97.0/windmill_api/models/get_app_by_version_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py` & `windmill_api-1.97.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.97.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_audit_log_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_audit_log_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_audit_log_response_200_operation.py` & `windmill_api-1.97.0/windmill_api/models/get_audit_log_response_200_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_audit_log_response_200_parameters.py` & `windmill_api-1.97.0/windmill_api/models/get_audit_log_response_200_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_args.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_schema.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_by_path_with_draft_response_200_draft_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_input_history_by_path_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_input_history_by_path_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py` & `windmill_api-1.97.0/windmill_api/models/get_flow_input_history_by_path_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_folder_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_folder_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_folder_response_200_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/get_folder_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_folder_usage_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_folder_usage_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_granular_acls_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_granular_acls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_group_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_group_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_group_response_200_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/get_group_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_app_by_id_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_app_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_app_by_id_response_200_app.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_app_by_id_response_200_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_hub_script_by_path_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_hub_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_input_history_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/get_input_history_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_input_history_response_200_item_args.py` & `windmill_api-1.97.0/windmill_api/models/get_input_history_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_job_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_job_updates_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_job_updates_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_premium_info_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_premium_info_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_public_app_by_secret_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_public_app_by_secret_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_public_app_by_secret_response_200_policy.py` & `windmill_api-1.97.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py` & `windmill_api-1.97.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.97.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_resource_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_resource_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_resource_response_200_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/get_resource_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_resource_type_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_resource_type_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_resume_urls_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_resume_urls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_schedule_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_schedule_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_schedule_response_200_args.py` & `windmill_api-1.97.0/windmill_api/models/get_schedule_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_schedule_response_200_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/get_schedule_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_script_by_hash_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_script_by_hash_response_200_schema.py` & `windmill_api-1.97.0/windmill_api/models/get_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_script_by_path_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_script_by_path_response_200_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_script_by_path_response_200_schema.py` & `windmill_api-1.97.0/windmill_api/models/get_script_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_script_by_path_with_draft_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_script_by_path_with_draft_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py` & `windmill_api-1.97.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py` & `windmill_api-1.97.0/windmill_api/models/get_script_by_path_with_draft_response_200_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py` & `windmill_api-1.97.0/windmill_api/models/get_script_by_path_with_draft_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_script_deployment_status_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_script_deployment_status_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_settings_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_suspended_job_flow_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_suspended_job_flow_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_suspended_job_flow_response_200_job.py` & `windmill_api-1.97.0/windmill_api/models/get_suspended_job_flow_response_200_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_variable_response_200.py` & `windmill_api-1.97.0/windmill_api/models/get_variable_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/get_variable_response_200_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/get_variable_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/global_user_info.py` & `windmill_api-1.97.0/windmill_api/models/global_user_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/global_user_update_json_body.py` & `windmill_api-1.97.0/windmill_api/models/global_user_update_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/global_whoami_response_200.py` & `windmill_api-1.97.0/windmill_api/models/global_whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200.py` & `windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item.py` & `windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.97.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/group.py` & `windmill_api-1.97.0/windmill_api/models/group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/group_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/group_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/identity.py` & `windmill_api-1.97.0/windmill_api/models/identity.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/input_.py` & `windmill_api-1.97.0/windmill_api/models/input_.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/input_args.py` & `windmill_api-1.97.0/windmill_api/models/input_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/input_transform_type_0.py` & `windmill_api-1.97.0/windmill_api/models/input_transform_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/input_transform_type_1.py` & `windmill_api-1.97.0/windmill_api/models/input_transform_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/invite_user_json_body.py` & `windmill_api-1.97.0/windmill_api/models/invite_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/javascript_transform.py` & `windmill_api-1.97.0/windmill_api/models/javascript_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/job.py` & `windmill_api-1.97.0/windmill_api/models/job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_apps_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_apps_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_apps_response_200_item_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/list_apps_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_audit_logs_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_audit_logs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_audit_logs_response_200_item_operation.py` & `windmill_api-1.97.0/windmill_api/models/list_audit_logs_response_200_item_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_audit_logs_response_200_item_parameters.py` & `windmill_api-1.97.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_args.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_contextual_variables_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_contextual_variables_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_flows_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_flows_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_folders_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_folders_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_folders_response_200_item_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/list_folders_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_groups_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_groups_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_groups_response_200_item_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/list_groups_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_hub_apps_response_200.py` & `windmill_api-1.97.0/windmill_api/models/list_hub_apps_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_hub_apps_response_200_apps_item.py` & `windmill_api-1.97.0/windmill_api/models/list_hub_apps_response_200_apps_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_hub_flows_response_200.py` & `windmill_api-1.97.0/windmill_api/models/list_hub_flows_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_hub_flows_response_200_flows_item.py` & `windmill_api-1.97.0/windmill_api/models/list_hub_flows_response_200_flows_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_hub_scripts_response_200.py` & `windmill_api-1.97.0/windmill_api/models/list_hub_scripts_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_hub_scripts_response_200_asks_item.py` & `windmill_api-1.97.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_inputs_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_inputs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_inputs_response_200_item_args.py` & `windmill_api-1.97.0/windmill_api/models/list_inputs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_jobs_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_pending_invites_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_pending_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_args.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_flow_status_retry.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_raw_apps_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_raw_apps_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_raw_apps_response_200_item_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/list_raw_apps_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_resource_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_resource_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_resource_response_200_item_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/list_resource_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_resource_type_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_resource_type_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_schedules_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_schedules_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_schedules_response_200_item_args.py` & `windmill_api-1.97.0/windmill_api/models/list_schedules_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_schedules_response_200_item_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_scripts_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_scripts_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_scripts_response_200_item_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_scripts_response_200_item_schema.py` & `windmill_api-1.97.0/windmill_api/models/list_scripts_response_200_item_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_tokens_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_tokens_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_user_workspaces_response_200.py` & `windmill_api-1.97.0/windmill_api/models/list_user_workspaces_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py` & `windmill_api-1.97.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_users_as_super_admin_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_users_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_users_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_users_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_users_response_200_item_usage.py` & `windmill_api-1.97.0/windmill_api/models/list_users_response_200_item_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_variable_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_variable_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_variable_response_200_item_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/list_variable_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_workers_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_workers_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_workspace_invites_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_workspace_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/list_workspaces_response_200_item.py` & `windmill_api-1.97.0/windmill_api/models/list_workspaces_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/listable_app.py` & `windmill_api-1.97.0/windmill_api/models/listable_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/listable_app_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/listable_app_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/listable_raw_app.py` & `windmill_api-1.97.0/windmill_api/models/listable_raw_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/listable_raw_app_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/listable_raw_app_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/listable_resource.py` & `windmill_api-1.97.0/windmill_api/models/listable_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/listable_resource_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/listable_resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/listable_variable.py` & `windmill_api-1.97.0/windmill_api/models/listable_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/listable_variable_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/listable_variable_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/login.py` & `windmill_api-1.97.0/windmill_api/models/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/login_json_body.py` & `windmill_api-1.97.0/windmill_api/models/login_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/login_with_oauth_json_body.py` & `windmill_api-1.97.0/windmill_api/models/login_with_oauth_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/main_arg_signature.py` & `windmill_api-1.97.0/windmill_api/models/main_arg_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item.py` & `windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_1.py` & `windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_2.py` & `windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_3.py` & `windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py` & `windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_4.py` & `windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.97.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/new_schedule.py` & `windmill_api-1.97.0/windmill_api/models/new_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/new_schedule_args.py` & `windmill_api-1.97.0/windmill_api/models/new_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/new_script.py` & `windmill_api-1.97.0/windmill_api/models/new_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/new_script_schema.py` & `windmill_api-1.97.0/windmill_api/models/new_script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/new_script_with_draft.py` & `windmill_api-1.97.0/windmill_api/models/new_script_with_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/new_script_with_draft_draft.py` & `windmill_api-1.97.0/windmill_api/models/new_script_with_draft_draft.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/new_script_with_draft_draft_schema.py` & `windmill_api-1.97.0/windmill_api/models/new_script_with_draft_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/new_script_with_draft_schema.py` & `windmill_api-1.97.0/windmill_api/models/new_script_with_draft_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/new_token.py` & `windmill_api-1.97.0/windmill_api/models/new_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/new_token_impersonate.py` & `windmill_api-1.97.0/windmill_api/models/new_token_impersonate.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/new_user.py` & `windmill_api-1.97.0/windmill_api/models/new_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow.py` & `windmill_api-1.97.0/windmill_api/models/open_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_schema.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_failure_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_value_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_schema.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/path_flow.py` & `windmill_api-1.97.0/windmill_api/models/path_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/path_flow_input_transforms.py` & `windmill_api-1.97.0/windmill_api/models/path_flow_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py` & `windmill_api-1.97.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py` & `windmill_api-1.97.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/path_script.py` & `windmill_api-1.97.0/windmill_api/models/path_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/path_script_input_transforms.py` & `windmill_api-1.97.0/windmill_api/models/path_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/path_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.97.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/path_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.97.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/policy.py` & `windmill_api-1.97.0/windmill_api/models/policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/policy_triggerables.py` & `windmill_api-1.97.0/windmill_api/models/policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/policy_triggerables_additional_property.py` & `windmill_api-1.97.0/windmill_api/models/policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/preview.py` & `windmill_api-1.97.0/windmill_api/models/preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/preview_args.py` & `windmill_api-1.97.0/windmill_api/models/preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/preview_schedule_json_body.py` & `windmill_api-1.97.0/windmill_api/models/preview_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200.py` & `windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item.py` & `windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.97.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job.py` & `windmill_api-1.97.0/windmill_api/models/queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_args.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_flow_status.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_failure_module_branchall.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_failure_module_iterator.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_modules_item_branchall.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_modules_item_iterator.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_flow_status_retry.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/raw_script.py` & `windmill_api-1.97.0/windmill_api/models/raw_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/raw_script_input_transforms.py` & `windmill_api-1.97.0/windmill_api/models/raw_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.97.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.97.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/refresh_token_json_body.py` & `windmill_api-1.97.0/windmill_api/models/refresh_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/remove_granular_acls_json_body.py` & `windmill_api-1.97.0/windmill_api/models/remove_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/remove_owner_to_folder_json_body.py` & `windmill_api-1.97.0/windmill_api/models/remove_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/remove_user_to_group_json_body.py` & `windmill_api-1.97.0/windmill_api/models/remove_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/resource.py` & `windmill_api-1.97.0/windmill_api/models/resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/resource_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/resource_type.py` & `windmill_api-1.97.0/windmill_api/models/resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/resume_suspended_flow_as_owner_json_body.py` & `windmill_api-1.97.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/resume_suspended_job_post_json_body.py` & `windmill_api-1.97.0/windmill_api/models/resume_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/retry.py` & `windmill_api-1.97.0/windmill_api/models/retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_by_path_json_body.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_args.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_script_by_hash_json_body.py` & `windmill_api-1.97.0/windmill_api/models/run_script_by_hash_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_script_by_path_json_body.py` & `windmill_api-1.97.0/windmill_api/models/run_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_script_preview_json_body.py` & `windmill_api-1.97.0/windmill_api/models/run_script_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_script_preview_json_body_args.py` & `windmill_api-1.97.0/windmill_api/models/run_script_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_wait_result_flow_by_path_json_body.py` & `windmill_api-1.97.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/run_wait_result_script_by_path_json_body.py` & `windmill_api-1.97.0/windmill_api/models/run_wait_result_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/schedule.py` & `windmill_api-1.97.0/windmill_api/models/schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/schedule_args.py` & `windmill_api-1.97.0/windmill_api/models/schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/schedule_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/schedule_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/script.py` & `windmill_api-1.97.0/windmill_api/models/script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/script_args.py` & `windmill_api-1.97.0/windmill_api/models/script_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/script_extra_perms.py` & `windmill_api-1.97.0/windmill_api/models/script_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/script_schema.py` & `windmill_api-1.97.0/windmill_api/models/script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/set_password_json_body.py` & `windmill_api-1.97.0/windmill_api/models/set_password_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/set_schedule_enabled_json_body.py` & `windmill_api-1.97.0/windmill_api/models/set_schedule_enabled_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/slack_token.py` & `windmill_api-1.97.0/windmill_api/models/slack_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/slack_token_bot.py` & `windmill_api-1.97.0/windmill_api/models/slack_token_bot.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/star_json_body.py` & `windmill_api-1.97.0/windmill_api/models/star_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/static_transform.py` & `windmill_api-1.97.0/windmill_api/models/static_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/token_response.py` & `windmill_api-1.97.0/windmill_api/models/token_response.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/truncated_token.py` & `windmill_api-1.97.0/windmill_api/models/truncated_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/unstar_json_body.py` & `windmill_api-1.97.0/windmill_api/models/unstar_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_app_json_body.py` & `windmill_api-1.97.0/windmill_api/models/update_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_app_json_body_policy.py` & `windmill_api-1.97.0/windmill_api/models/update_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_app_json_body_policy_triggerables.py` & `windmill_api-1.97.0/windmill_api/models/update_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.97.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_schema.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_retry.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py` & `windmill_api-1.97.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_folder_json_body.py` & `windmill_api-1.97.0/windmill_api/models/update_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_group_json_body.py` & `windmill_api-1.97.0/windmill_api/models/update_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_input.py` & `windmill_api-1.97.0/windmill_api/models/update_input.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_input_json_body.py` & `windmill_api-1.97.0/windmill_api/models/update_input_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_raw_app_json_body.py` & `windmill_api-1.97.0/windmill_api/models/update_raw_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_resource_json_body.py` & `windmill_api-1.97.0/windmill_api/models/update_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_resource_type_json_body.py` & `windmill_api-1.97.0/windmill_api/models/update_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_resource_value_json_body.py` & `windmill_api-1.97.0/windmill_api/models/update_resource_value_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_schedule_json_body.py` & `windmill_api-1.97.0/windmill_api/models/update_schedule_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_schedule_json_body_args.py` & `windmill_api-1.97.0/windmill_api/models/update_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_user_json_body.py` & `windmill_api-1.97.0/windmill_api/models/update_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/update_variable_json_body.py` & `windmill_api-1.97.0/windmill_api/models/update_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/usage.py` & `windmill_api-1.97.0/windmill_api/models/usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/user.py` & `windmill_api-1.97.0/windmill_api/models/user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/user_usage.py` & `windmill_api-1.97.0/windmill_api/models/user_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/user_workspace_list.py` & `windmill_api-1.97.0/windmill_api/models/user_workspace_list.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/user_workspace_list_workspaces_item.py` & `windmill_api-1.97.0/windmill_api/models/user_workspace_list_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/whoami_response_200.py` & `windmill_api-1.97.0/windmill_api/models/whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/whoami_response_200_usage.py` & `windmill_api-1.97.0/windmill_api/models/whoami_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/whois_response_200.py` & `windmill_api-1.97.0/windmill_api/models/whois_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/whois_response_200_usage.py` & `windmill_api-1.97.0/windmill_api/models/whois_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/worker_ping.py` & `windmill_api-1.97.0/windmill_api/models/worker_ping.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/workspace.py` & `windmill_api-1.97.0/windmill_api/models/workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/models/workspace_invite.py` & `windmill_api-1.97.0/windmill_api/models/workspace_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/windmill_api/types.py` & `windmill_api-1.97.0/windmill_api/types.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.96.3/setup.py` & `windmill_api-1.97.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=21.3.0', 'httpx>=0.15.4,<0.24.0', 'python-dateutil>=2.8.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'windmill-api',
-    'version': '1.96.3',
+    'version': '1.97.0',
     'description': 'A client library for accessing Windmill API',
     'long_description': '# Autogenerated Windmill OpenApi Client\nThis is the raw autogenerated api client. You are most likely more interested in [wmill](https://pypi.org/project/wmill/) which leverages this client to offer an user friendly experience. We use [this openapi python client generator](https://github.com/openapi-generators/openapi-python-client/)\n\n# windmill-api\nA client library for accessing Windmill API\n\n## Usage\nFirst, create a client:\n\n```python\nfrom windmill_api import Client\n\nclient = Client(base_url="https://api.example.com")\n```\n\nIf the endpoints you\'re going to hit require authentication, use `AuthenticatedClient` instead:\n\n```python\nfrom windmill_api import AuthenticatedClient\n\nclient = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = get_my_data_model.sync(client=client)\n# or if you need more info (e.g. status_code)\nresponse: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)\n```\n\nOr do the same thing with an async version:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = await get_my_data_model.asyncio(client=client)\nresponse: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)\n```\n\nBy default, when you\'re calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken",\n    verify_ssl="/path/to/certificate_bundle.pem",\n)\n```\n\nYou can also disable certificate validation altogether, but beware that **this is a security risk**.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken", \n    verify_ssl=False\n)\n```\n\nThings to know:\n1. Every path/method combo becomes a Python module with four functions:\n    1. `sync`: Blocking request that returns parsed data (if successful) or `None`\n    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.\n    1. `asyncio`: Like `sync` but async instead of blocking\n    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking\n\n1. All path/query params, and bodies become method arguments.\n1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)\n1. Any endpoint which did not have a tag will be in `windmill_api.api.default`\n\n',
     'author': 'Ruben Fiszel',
     'author_email': 'ruben@windmill.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `windmill_api-1.96.3/PKG-INFO` & `windmill_api-1.97.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windmill-api
-Version: 1.96.3
+Version: 1.97.0
 Summary: A client library for accessing Windmill API
 License: Apache-2.0
 Author: Ruben Fiszel
 Author-email: ruben@windmill.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

