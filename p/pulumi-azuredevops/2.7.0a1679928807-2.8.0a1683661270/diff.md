# Comparing `tmp/pulumi_azuredevops-2.7.0a1679928807.tar.gz` & `tmp/pulumi_azuredevops-2.8.0a1683661270.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_azuredevops-2.7.0a1679928807.tar", last modified: Mon Mar 27 14:59:53 2023, max compression
+gzip compressed data, was "pulumi_azuredevops-2.8.0a1683661270.tar", last modified: Tue May  9 19:47:38 2023, max compression
```

## Comparing `pulumi_azuredevops-2.7.0a1679928807.tar` & `pulumi_azuredevops-2.8.0a1683661270.tar`

### file list

```diff
@@ -1,169 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:59:53.942332 pulumi_azuredevops-2.7.0a1679928807/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-03-27 14:59:53.938332 pulumi_azuredevops-2.7.0a1679928807/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:59:53.930332 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/
--rw-r--r--   0 runner    (1001) docker     (123)    23248 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   142668 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:59:53.930332 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/agent/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/agent/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/agent/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/agent/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/agent/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/agent/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    17119 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/area_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/branch_policy_auto_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/branch_policy_build_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16901 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/branch_policy_comment_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)    16839 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/branch_policy_merge_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/branch_policy_min_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/branch_policy_status_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/branch_policy_work_item_linking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:59:53.930332 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48005 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38702 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build/build_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    44955 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38457 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    19191 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build_definition_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build_folder_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    32736 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/check_branch_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    52960 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/check_business_hours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:59:53.934332 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:59:53.934332 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/core/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/core/get_client_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/core/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/core/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/core/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21750 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/core/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/core/project_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:59:53.934332 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/entitlement/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/entitlement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/entitlement/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_agent_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_area.py
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_build_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_client_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_git_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_service_endpoint_azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_service_endpoint_github.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_variable_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    22657 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    29029 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/git_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/git_repository_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/git_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    29921 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/group_membership.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:59:53.934332 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/identities/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/identities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/identities/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/identities/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    30141 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/identities/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/identities/group_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/identities/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/iterative_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)   188231 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:59:53.934332 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/pipeline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/pipeline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24757 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/pipeline/variable_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:59:53.938332 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19196 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/policy/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/policy/branch_policy_build_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17760 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/policy/branch_policy_min_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/policy/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    21552 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/project_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/project_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20739 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/project_pipeline_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:59:53.938332 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository/get_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    22877 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21646 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository_policy_author_email_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository_policy_case_enforcement.py
--rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository_policy_check_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository_policy_file_path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository_policy_max_file_size.py
--rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository_policy_max_path_length.py
--rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository_policy_reserved_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/resource_authorization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:59:53.938332 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/security/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17543 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/security/resource_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)    22438 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_artifactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    30438 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    22356 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_azure_dev_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    30733 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_azure_ecr.py
--rw-r--r--   0 runner    (1001) docker     (123)    39015 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (123)    18522 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_bit_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    27775 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_docker_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    21448 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    24317 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_generic_git.py
--rw-r--r--   0 runner    (1001) docker     (123)    22104 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_git_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    18919 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (123)    25990 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_npm.py
--rw-r--r--   0 runner    (1001) docker     (123)    19896 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    26154 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_service_fabric.py
--rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_sonar_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_sonar_qube.py
--rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:59:53.938332 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38745 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/bit_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    27750 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/docker_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    21619 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/git_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)    25315 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    14643 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24537 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint_argocd.py
--rw-r--r--   0 runner    (1001) docker     (123)    17775 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint_externaltfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint_incomingwebhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    19961 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint_octopusdeploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19604 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/servicehook_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15665 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/tagging_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17288 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/team_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/team_members.py
--rw-r--r--   0 runner    (1001) docker     (123)    20819 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    24501 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/variable_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    22220 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/work_item_query_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21319 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/workitem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:59:53.930332 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 14:59:53.942332 pulumi_azuredevops-2.7.0a1679928807/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-03-27 14:59:53.000000 pulumi_azuredevops-2.7.0a1679928807/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.406342 pulumi_azuredevops-2.8.0a1683661270/
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-09 19:47:38.402342 pulumi_azuredevops-2.8.0a1683661270/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.398342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/
+-rw-r--r--   0 runner    (1001) docker     (123)    24455 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147060 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.398342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10876 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17119 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/area_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_auto_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_build_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16901 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_comment_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16839 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_merge_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_min_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17269 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_status_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16783 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_work_item_linking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.398342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48005 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38702 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44955 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38457 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19191 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_definition_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10897 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_folder_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32736 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/check_branch_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52960 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/check_business_hours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.398342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.398342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/get_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21750 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/project_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.398342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/entitlement/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/entitlement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/entitlement/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_agent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_git_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_service_endpoint_azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7381 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_service_endpoint_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_variable_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22657 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29029 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git_repository_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29921 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/group_membership.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.402342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30141 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16604 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/iterative_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   189015 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.402342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24694 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/variable_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.402342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19196 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/branch_policy_build_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17760 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/branch_policy_min_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18687 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21552 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10359 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20739 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project_pipeline_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.402342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/get_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22877 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21646 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_author_email_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_case_enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_check_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_file_path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_max_file_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19867 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_max_path_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17657 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_reserved_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17259 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/resource_authorization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.402342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/security/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17543 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/security/resource_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22800 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_artifactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30438 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22356 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_azure_dev_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30733 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_azure_ecr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39015 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18522 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_bit_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27775 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_docker_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21448 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24317 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_generic_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22104 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_git_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18919 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25990 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_npm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19896 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26154 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_service_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_sonar_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_sonar_qube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.402342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38745 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18472 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/bit_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27750 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/docker_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21619 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/git_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25315 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14643 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24537 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_argocd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17775 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_externaltfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_incomingwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25176 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24924 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19961 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_octopusdeploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19604 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15186 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/servicehook_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15665 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/tagging_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17288 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/team_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/team_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20819 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24438 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/variable_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22220 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/work_item_query_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21319 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/workitem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 19:47:38.398342 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 19:47:38.406342 pulumi_azuredevops-2.8.0a1683661270/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-09 19:47:38.000000 pulumi_azuredevops-2.8.0a1683661270/setup.py
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/PKG-INFO` & `pulumi_azuredevops-2.8.0a1683661270/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_azuredevops
-Version: 2.7.0a1679928807
+Version: 2.8.0a1683661270
 Summary: A Pulumi package for creating and managing Azure DevOps.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuredevops
 Keywords: pulumi azuredevops
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-azuredevops/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-azuredevops/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fazuredevops.svg)](https://www.npmjs.com/package/@pulumi/azuredevops)
 [![Python version](https://badge.fury.io/py/pulumi-azuredevops.svg)](https://pypi.org/project/pulumi-azuredevops)
 [![NuGet version](https://badge.fury.io/nu/pulumi.azuredevops.svg)](https://badge.fury.io/nu/pulumi.azuredevops)
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/README.md` & `pulumi_azuredevops-2.8.0a1683661270/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/__init__.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,18 @@
 from .service_endpoint_service_fabric import *
 from .service_endpoint_sonar_cloud import *
 from .service_endpoint_sonar_qube import *
 from .service_endpoint_ssh import *
 from .serviceendpoint_argocd import *
 from .serviceendpoint_externaltfs import *
 from .serviceendpoint_incomingwebhook import *
+from .serviceendpoint_jfrog_artifactory_v2 import *
+from .serviceendpoint_jfrog_distribution_v2 import *
+from .serviceendpoint_jfrog_platform_v2 import *
+from .serviceendpoint_jfrog_xray_v2 import *
 from .serviceendpoint_octopusdeploy import *
 from .serviceendpoint_permissions import *
 from .servicehook_permissions import *
 from .tagging_permissions import *
 from .team import *
 from .team_administrators import *
 from .team_members import *
@@ -734,14 +738,46 @@
   "fqn": "pulumi_azuredevops",
   "classes": {
    "azuredevops:index/serviceendpointIncomingwebhook:ServiceendpointIncomingwebhook": "ServiceendpointIncomingwebhook"
   }
  },
  {
   "pkg": "azuredevops",
+  "mod": "index/serviceendpointJfrogArtifactoryV2",
+  "fqn": "pulumi_azuredevops",
+  "classes": {
+   "azuredevops:index/serviceendpointJfrogArtifactoryV2:ServiceendpointJfrogArtifactoryV2": "ServiceendpointJfrogArtifactoryV2"
+  }
+ },
+ {
+  "pkg": "azuredevops",
+  "mod": "index/serviceendpointJfrogDistributionV2",
+  "fqn": "pulumi_azuredevops",
+  "classes": {
+   "azuredevops:index/serviceendpointJfrogDistributionV2:ServiceendpointJfrogDistributionV2": "ServiceendpointJfrogDistributionV2"
+  }
+ },
+ {
+  "pkg": "azuredevops",
+  "mod": "index/serviceendpointJfrogPlatformV2",
+  "fqn": "pulumi_azuredevops",
+  "classes": {
+   "azuredevops:index/serviceendpointJfrogPlatformV2:ServiceendpointJfrogPlatformV2": "ServiceendpointJfrogPlatformV2"
+  }
+ },
+ {
+  "pkg": "azuredevops",
+  "mod": "index/serviceendpointJfrogXrayV2",
+  "fqn": "pulumi_azuredevops",
+  "classes": {
+   "azuredevops:index/serviceendpointJfrogXrayV2:ServiceendpointJfrogXrayV2": "ServiceendpointJfrogXrayV2"
+  }
+ },
+ {
+  "pkg": "azuredevops",
   "mod": "index/serviceendpointOctopusdeploy",
   "fqn": "pulumi_azuredevops",
   "classes": {
    "azuredevops:index/serviceendpointOctopusdeploy:ServiceendpointOctopusdeploy": "ServiceendpointOctopusdeploy"
   }
  },
  {
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/_inputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,22 @@
     'ServiceEndpointPipelineAuthPersonalArgs',
     'ServiceEndpointServiceFabricAzureActiveDirectoryArgs',
     'ServiceEndpointServiceFabricCertificateArgs',
     'ServiceEndpointServiceFabricNoneArgs',
     'ServiceendpointArgocdAuthenticationBasicArgs',
     'ServiceendpointArgocdAuthenticationTokenArgs',
     'ServiceendpointExternaltfsAuthPersonalArgs',
+    'ServiceendpointJfrogArtifactoryV2AuthenticationBasicArgs',
+    'ServiceendpointJfrogArtifactoryV2AuthenticationTokenArgs',
+    'ServiceendpointJfrogDistributionV2AuthenticationBasicArgs',
+    'ServiceendpointJfrogDistributionV2AuthenticationTokenArgs',
+    'ServiceendpointJfrogPlatformV2AuthenticationBasicArgs',
+    'ServiceendpointJfrogPlatformV2AuthenticationTokenArgs',
+    'ServiceendpointJfrogXrayV2AuthenticationBasicArgs',
+    'ServiceendpointJfrogXrayV2AuthenticationTokenArgs',
     'VariableGroupKeyVaultArgs',
     'VariableGroupVariableArgs',
 ]
 
 @pulumi.input_type
 class BranchPolicyAutoReviewersSettingsArgs:
     def __init__(__self__, *,
@@ -2242,27 +2250,21 @@
         pulumi.set(self, "source_url", value)
 
 
 @pulumi.input_type
 class ServiceEndpointArtifactoryAuthenticationBasicArgs:
     def __init__(__self__, *,
                  password: pulumi.Input[str],
-                 username: pulumi.Input[str],
-                 password_hash: Optional[pulumi.Input[str]] = None,
-                 username_hash: Optional[pulumi.Input[str]] = None):
+                 username: pulumi.Input[str]):
         """
         :param pulumi.Input[str] password: Artifactory Password.
         :param pulumi.Input[str] username: Artifactory Username.
         """
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "username", username)
-        if password_hash is not None:
-            pulumi.set(__self__, "password_hash", password_hash)
-        if username_hash is not None:
-            pulumi.set(__self__, "username_hash", username_hash)
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Input[str]:
         """
         Artifactory Password.
         """
@@ -2280,66 +2282,36 @@
         """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: pulumi.Input[str]):
         pulumi.set(self, "username", value)
 
-    @property
-    @pulumi.getter(name="passwordHash")
-    def password_hash(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "password_hash")
-
-    @password_hash.setter
-    def password_hash(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "password_hash", value)
-
-    @property
-    @pulumi.getter(name="usernameHash")
-    def username_hash(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "username_hash")
-
-    @username_hash.setter
-    def username_hash(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "username_hash", value)
-
 
 @pulumi.input_type
 class ServiceEndpointArtifactoryAuthenticationTokenArgs:
     def __init__(__self__, *,
-                 token: pulumi.Input[str],
-                 token_hash: Optional[pulumi.Input[str]] = None):
+                 token: pulumi.Input[str]):
         """
         :param pulumi.Input[str] token: Authentication Token generated through Artifactory.
         """
         pulumi.set(__self__, "token", token)
-        if token_hash is not None:
-            pulumi.set(__self__, "token_hash", token_hash)
 
     @property
     @pulumi.getter
     def token(self) -> pulumi.Input[str]:
         """
         Authentication Token generated through Artifactory.
         """
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: pulumi.Input[str]):
         pulumi.set(self, "token", value)
 
-    @property
-    @pulumi.getter(name="tokenHash")
-    def token_hash(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "token_hash")
-
-    @token_hash.setter
-    def token_hash(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "token_hash", value)
-
 
 @pulumi.input_type
 class ServiceEndpointAzureRMCredentialsArgs:
     def __init__(__self__, *,
                  serviceprincipalid: pulumi.Input[str],
                  serviceprincipalkey: pulumi.Input[str],
                  serviceprincipalkey_hash: Optional[pulumi.Input[str]] = None):
@@ -2957,27 +2929,21 @@
         pulumi.set(self, "unsecured", value)
 
 
 @pulumi.input_type
 class ServiceendpointArgocdAuthenticationBasicArgs:
     def __init__(__self__, *,
                  password: pulumi.Input[str],
-                 username: pulumi.Input[str],
-                 password_hash: Optional[pulumi.Input[str]] = None,
-                 username_hash: Optional[pulumi.Input[str]] = None):
+                 username: pulumi.Input[str]):
         """
         :param pulumi.Input[str] password: ArgoCD Password.
         :param pulumi.Input[str] username: ArgoCD Username.
         """
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "username", username)
-        if password_hash is not None:
-            pulumi.set(__self__, "password_hash", password_hash)
-        if username_hash is not None:
-            pulumi.set(__self__, "username_hash", username_hash)
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Input[str]:
         """
         ArgoCD Password.
         """
@@ -2995,66 +2961,36 @@
         """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: pulumi.Input[str]):
         pulumi.set(self, "username", value)
 
-    @property
-    @pulumi.getter(name="passwordHash")
-    def password_hash(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "password_hash")
-
-    @password_hash.setter
-    def password_hash(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "password_hash", value)
-
-    @property
-    @pulumi.getter(name="usernameHash")
-    def username_hash(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "username_hash")
-
-    @username_hash.setter
-    def username_hash(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "username_hash", value)
-
 
 @pulumi.input_type
 class ServiceendpointArgocdAuthenticationTokenArgs:
     def __init__(__self__, *,
-                 token: pulumi.Input[str],
-                 token_hash: Optional[pulumi.Input[str]] = None):
+                 token: pulumi.Input[str]):
         """
         :param pulumi.Input[str] token: Authentication Token generated through ArgoCD.
         """
         pulumi.set(__self__, "token", token)
-        if token_hash is not None:
-            pulumi.set(__self__, "token_hash", token_hash)
 
     @property
     @pulumi.getter
     def token(self) -> pulumi.Input[str]:
         """
         Authentication Token generated through ArgoCD.
         """
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: pulumi.Input[str]):
         pulumi.set(self, "token", value)
 
-    @property
-    @pulumi.getter(name="tokenHash")
-    def token_hash(self) -> Optional[pulumi.Input[str]]:
-        return pulumi.get(self, "token_hash")
-
-    @token_hash.setter
-    def token_hash(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "token_hash", value)
-
 
 @pulumi.input_type
 class ServiceendpointExternaltfsAuthPersonalArgs:
     def __init__(__self__, *,
                  personal_access_token: pulumi.Input[str]):
         """
         :param pulumi.Input[str] personal_access_token: The Personal Access Token for Azure DevOps Organization.
@@ -3071,14 +3007,250 @@
 
     @personal_access_token.setter
     def personal_access_token(self, value: pulumi.Input[str]):
         pulumi.set(self, "personal_access_token", value)
 
 
 @pulumi.input_type
+class ServiceendpointJfrogArtifactoryV2AuthenticationBasicArgs:
+    def __init__(__self__, *,
+                 password: pulumi.Input[str],
+                 username: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] password: Artifactory Password.
+        :param pulumi.Input[str] username: Artifactory Username.
+        """
+        pulumi.set(__self__, "password", password)
+        pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def password(self) -> pulumi.Input[str]:
+        """
+        Artifactory Password.
+        """
+        return pulumi.get(self, "password")
+
+    @password.setter
+    def password(self, value: pulumi.Input[str]):
+        pulumi.set(self, "password", value)
+
+    @property
+    @pulumi.getter
+    def username(self) -> pulumi.Input[str]:
+        """
+        Artifactory Username.
+        """
+        return pulumi.get(self, "username")
+
+    @username.setter
+    def username(self, value: pulumi.Input[str]):
+        pulumi.set(self, "username", value)
+
+
+@pulumi.input_type
+class ServiceendpointJfrogArtifactoryV2AuthenticationTokenArgs:
+    def __init__(__self__, *,
+                 token: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] token: Authentication Token generated through Artifactory.
+        """
+        pulumi.set(__self__, "token", token)
+
+    @property
+    @pulumi.getter
+    def token(self) -> pulumi.Input[str]:
+        """
+        Authentication Token generated through Artifactory.
+        """
+        return pulumi.get(self, "token")
+
+    @token.setter
+    def token(self, value: pulumi.Input[str]):
+        pulumi.set(self, "token", value)
+
+
+@pulumi.input_type
+class ServiceendpointJfrogDistributionV2AuthenticationBasicArgs:
+    def __init__(__self__, *,
+                 password: pulumi.Input[str],
+                 username: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] password: Artifactory Password.
+        :param pulumi.Input[str] username: Artifactory Username.
+        """
+        pulumi.set(__self__, "password", password)
+        pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def password(self) -> pulumi.Input[str]:
+        """
+        Artifactory Password.
+        """
+        return pulumi.get(self, "password")
+
+    @password.setter
+    def password(self, value: pulumi.Input[str]):
+        pulumi.set(self, "password", value)
+
+    @property
+    @pulumi.getter
+    def username(self) -> pulumi.Input[str]:
+        """
+        Artifactory Username.
+        """
+        return pulumi.get(self, "username")
+
+    @username.setter
+    def username(self, value: pulumi.Input[str]):
+        pulumi.set(self, "username", value)
+
+
+@pulumi.input_type
+class ServiceendpointJfrogDistributionV2AuthenticationTokenArgs:
+    def __init__(__self__, *,
+                 token: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] token: Authentication Token generated through Artifactory.
+        """
+        pulumi.set(__self__, "token", token)
+
+    @property
+    @pulumi.getter
+    def token(self) -> pulumi.Input[str]:
+        """
+        Authentication Token generated through Artifactory.
+        """
+        return pulumi.get(self, "token")
+
+    @token.setter
+    def token(self, value: pulumi.Input[str]):
+        pulumi.set(self, "token", value)
+
+
+@pulumi.input_type
+class ServiceendpointJfrogPlatformV2AuthenticationBasicArgs:
+    def __init__(__self__, *,
+                 password: pulumi.Input[str],
+                 username: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] password: Artifactory Password.
+        :param pulumi.Input[str] username: Artifactory Username.
+        """
+        pulumi.set(__self__, "password", password)
+        pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def password(self) -> pulumi.Input[str]:
+        """
+        Artifactory Password.
+        """
+        return pulumi.get(self, "password")
+
+    @password.setter
+    def password(self, value: pulumi.Input[str]):
+        pulumi.set(self, "password", value)
+
+    @property
+    @pulumi.getter
+    def username(self) -> pulumi.Input[str]:
+        """
+        Artifactory Username.
+        """
+        return pulumi.get(self, "username")
+
+    @username.setter
+    def username(self, value: pulumi.Input[str]):
+        pulumi.set(self, "username", value)
+
+
+@pulumi.input_type
+class ServiceendpointJfrogPlatformV2AuthenticationTokenArgs:
+    def __init__(__self__, *,
+                 token: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] token: Authentication Token generated through Artifactory.
+        """
+        pulumi.set(__self__, "token", token)
+
+    @property
+    @pulumi.getter
+    def token(self) -> pulumi.Input[str]:
+        """
+        Authentication Token generated through Artifactory.
+        """
+        return pulumi.get(self, "token")
+
+    @token.setter
+    def token(self, value: pulumi.Input[str]):
+        pulumi.set(self, "token", value)
+
+
+@pulumi.input_type
+class ServiceendpointJfrogXrayV2AuthenticationBasicArgs:
+    def __init__(__self__, *,
+                 password: pulumi.Input[str],
+                 username: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] password: Artifactory Password.
+        :param pulumi.Input[str] username: Artifactory Username.
+        """
+        pulumi.set(__self__, "password", password)
+        pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def password(self) -> pulumi.Input[str]:
+        """
+        Artifactory Password.
+        """
+        return pulumi.get(self, "password")
+
+    @password.setter
+    def password(self, value: pulumi.Input[str]):
+        pulumi.set(self, "password", value)
+
+    @property
+    @pulumi.getter
+    def username(self) -> pulumi.Input[str]:
+        """
+        Artifactory Username.
+        """
+        return pulumi.get(self, "username")
+
+    @username.setter
+    def username(self, value: pulumi.Input[str]):
+        pulumi.set(self, "username", value)
+
+
+@pulumi.input_type
+class ServiceendpointJfrogXrayV2AuthenticationTokenArgs:
+    def __init__(__self__, *,
+                 token: pulumi.Input[str]):
+        """
+        :param pulumi.Input[str] token: Authentication Token generated through Artifactory.
+        """
+        pulumi.set(__self__, "token", token)
+
+    @property
+    @pulumi.getter
+    def token(self) -> pulumi.Input[str]:
+        """
+        Authentication Token generated through Artifactory.
+        """
+        return pulumi.get(self, "token")
+
+    @token.setter
+    def token(self, value: pulumi.Input[str]):
+        pulumi.set(self, "token", value)
+
+
+@pulumi.input_type
 class VariableGroupKeyVaultArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  service_endpoint_id: pulumi.Input[str],
                  search_depth: Optional[pulumi.Input[int]] = None):
         """
         :param pulumi.Input[str] name: The name of the Azure key vault to link secrets from as variables.
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/_utilities.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/agent/get_pool.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/agent/get_pools.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/get_pools.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,18 +65,18 @@
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_pools()
-    pulumi.export("agentPoolName", [__item.name for __item in [example.agent_pools]])
-    pulumi.export("autoProvision", [__item.auto_provision for __item in [example.agent_pools]])
-    pulumi.export("autoUpdate", [__item.auto_update for __item in [example.agent_pools]])
-    pulumi.export("poolType", [__item.pool_type for __item in [example.agent_pools]])
+    pulumi.export("agentPoolName", [__item.name for __item in example.agent_pools])
+    pulumi.export("autoProvision", [__item.auto_provision for __item in example.agent_pools])
+    pulumi.export("autoUpdate", [__item.auto_update for __item in example.agent_pools])
+    pulumi.export("poolType", [__item.pool_type for __item in example.agent_pools])
     ```
     ## Relevant Links
 
     - [Azure DevOps Service REST API 6.0 - Agent Pools - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/pools/get?view=azure-devops-rest-6.0)
     """
     pulumi.log.warn("""get_pools is deprecated: azuredevops.agent.getPools has been deprecated in favor of azuredevops.getPools""")
     __args__ = dict()
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/agent/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/agent/pool.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/agent/queue.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/agent/queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/area_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/area_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/branch_policy_auto_reviewers.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_auto_reviewers.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/branch_policy_build_validation.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_build_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/branch_policy_comment_resolution.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_comment_resolution.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/branch_policy_merge_types.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_merge_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/branch_policy_min_reviewers.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_min_reviewers.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/branch_policy_status_check.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_status_check.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/branch_policy_work_item_linking.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/branch_policy_work_item_linking.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build/_inputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build/build_definition.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/build_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build_definition.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build_definition_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_definition_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build_folder.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/build_folder_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/build_folder_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/check_branch_control.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/check_branch_control.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/check_business_hours.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/check_business_hours.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/config/vars.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/core/get_client_config.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/get_client_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/core/get_project.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/core/get_projects.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/get_projects.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
-        Project name.
+        The name of the Project.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def projects(self) -> Sequence['outputs.GetProjectsProjectResult']:
         """
@@ -93,18 +93,18 @@
 
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_projects(name="Example Project",
         state="wellFormed")
-    pulumi.export("projectId", [__item.project_id for __item in [example.projects]])
-    pulumi.export("name", [__item.name for __item in [example.projects]])
-    pulumi.export("projectUrl", [__item.project_url for __item in [example.projects]])
-    pulumi.export("state", [__item.state for __item in [example.projects]])
+    pulumi.export("projectId", [__item.project_id for __item in example.projects])
+    pulumi.export("name", [__item.name for __item in example.projects])
+    pulumi.export("projectUrl", [__item.project_url for __item in example.projects])
+    pulumi.export("state", [__item.state for __item in example.projects])
     ```
     ## Relevant Links
 
     - [Azure DevOps Service REST API 6.0 - Projects - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/projects/get?view=azure-devops-rest-6.0)
 
 
     :param str name: Name of the Project, if not specified all projects will be returned.
@@ -135,18 +135,18 @@
 
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_projects(name="Example Project",
         state="wellFormed")
-    pulumi.export("projectId", [__item.project_id for __item in [example.projects]])
-    pulumi.export("name", [__item.name for __item in [example.projects]])
-    pulumi.export("projectUrl", [__item.project_url for __item in [example.projects]])
-    pulumi.export("state", [__item.state for __item in [example.projects]])
+    pulumi.export("projectId", [__item.project_id for __item in example.projects])
+    pulumi.export("name", [__item.name for __item in example.projects])
+    pulumi.export("projectUrl", [__item.project_url for __item in example.projects])
+    pulumi.export("state", [__item.state for __item in example.projects])
     ```
     ## Relevant Links
 
     - [Azure DevOps Service REST API 6.0 - Projects - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/projects/get?view=azure-devops-rest-6.0)
 
 
     :param str name: Name of the Project, if not specified all projects will be returned.
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/core/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/outputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def __init__(__self__, *,
                  name: str,
                  project_id: str,
                  project_url: str,
                  state: str):
         """
         :param str name: Name of the Project, if not specified all projects will be returned.
-        :param str project_id: Project identifier.
+        :param str project_id: The ID of the Project.
         :param str project_url: Url to the full version of the object.
         :param str state: State of the Project, if not specified all projects will be returned. Valid values are `all`, `deleting`, `new`, `wellFormed`, `createPending`, `unchanged`,`deleted`.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "project_id", project_id)
         pulumi.set(__self__, "project_url", project_url)
         pulumi.set(__self__, "state", state)
@@ -39,15 +39,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> str:
         """
-        Project identifier.
+        The ID of the Project.
         """
         return pulumi.get(self, "project_id")
 
     @property
     @pulumi.getter(name="projectUrl")
     def project_url(self) -> str:
         """
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/core/project.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/core/project_features.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/core/project_features.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/entitlement/user.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/entitlement/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/environment.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_agent_queue.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_agent_queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_area.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_area.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_build_definition.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_build_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_client_config.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_client_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_git_repository.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_git_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
 
 def get_git_repository(name: Optional[str] = None,
                        project_id: Optional[str] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetGitRepositoryResult:
     """
     Use this data source to access information about a **single** (existing) Git Repository within Azure DevOps.
-    To read information about **multiple** Git Repositories use the data source _get_repositories_
+    To read information about **multiple** Git Repositories use the data source `get_repositories`
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
@@ -195,15 +195,15 @@
 
 @_utilities.lift_output_func(get_git_repository)
 def get_git_repository_output(name: Optional[pulumi.Input[str]] = None,
                               project_id: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGitRepositoryResult]:
     """
     Use this data source to access information about a **single** (existing) Git Repository within Azure DevOps.
-    To read information about **multiple** Git Repositories use the data source _get_repositories_
+    To read information about **multiple** Git Repositories use the data source `get_repositories`
 
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_group.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_groups.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_iteration.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_iteration.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_pool.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_pools.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_pools.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,18 +63,18 @@
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_pools()
-    pulumi.export("agentPoolName", [__item.name for __item in [example.agent_pools]])
-    pulumi.export("autoProvision", [__item.auto_provision for __item in [example.agent_pools]])
-    pulumi.export("autoUpdate", [__item.auto_update for __item in [example.agent_pools]])
-    pulumi.export("poolType", [__item.pool_type for __item in [example.agent_pools]])
+    pulumi.export("agentPoolName", [__item.name for __item in example.agent_pools])
+    pulumi.export("autoProvision", [__item.auto_provision for __item in example.agent_pools])
+    pulumi.export("autoUpdate", [__item.auto_update for __item in example.agent_pools])
+    pulumi.export("poolType", [__item.pool_type for __item in example.agent_pools])
     ```
     ## Relevant Links
 
     - [Azure DevOps Service REST API 6.0 - Agent Pools - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/distributedtask/pools/get?view=azure-devops-rest-6.0)
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_project.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_projects.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_projects.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
-        Project name.
+        The name of the Project.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def projects(self) -> Sequence['outputs.GetProjectsProjectResult']:
         """
@@ -91,18 +91,18 @@
 
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_projects(name="Example Project",
         state="wellFormed")
-    pulumi.export("projectId", [__item.project_id for __item in [example.projects]])
-    pulumi.export("name", [__item.name for __item in [example.projects]])
-    pulumi.export("projectUrl", [__item.project_url for __item in [example.projects]])
-    pulumi.export("state", [__item.state for __item in [example.projects]])
+    pulumi.export("projectId", [__item.project_id for __item in example.projects])
+    pulumi.export("name", [__item.name for __item in example.projects])
+    pulumi.export("projectUrl", [__item.project_url for __item in example.projects])
+    pulumi.export("state", [__item.state for __item in example.projects])
     ```
     ## Relevant Links
 
     - [Azure DevOps Service REST API 6.0 - Projects - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/projects/get?view=azure-devops-rest-6.0)
 
 
     :param str name: Name of the Project, if not specified all projects will be returned.
@@ -132,18 +132,18 @@
 
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_projects(name="Example Project",
         state="wellFormed")
-    pulumi.export("projectId", [__item.project_id for __item in [example.projects]])
-    pulumi.export("name", [__item.name for __item in [example.projects]])
-    pulumi.export("projectUrl", [__item.project_url for __item in [example.projects]])
-    pulumi.export("state", [__item.state for __item in [example.projects]])
+    pulumi.export("projectId", [__item.project_id for __item in example.projects])
+    pulumi.export("name", [__item.name for __item in example.projects])
+    pulumi.export("projectUrl", [__item.project_url for __item in example.projects])
+    pulumi.export("state", [__item.state for __item in example.projects])
     ```
     ## Relevant Links
 
     - [Azure DevOps Service REST API 6.0 - Projects - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/projects/get?view=azure-devops-rest-6.0)
 
 
     :param str name: Name of the Project, if not specified all projects will be returned.
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_repositories.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_service_endpoint_azure_rm.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_service_endpoint_azure_rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_service_endpoint_github.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_service_endpoint_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_team.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_team.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,21 +17,24 @@
 ]
 
 @pulumi.output_type
 class GetTeamResult:
     """
     A collection of values returned by getTeam.
     """
-    def __init__(__self__, administrators=None, description=None, id=None, members=None, name=None, project_id=None):
+    def __init__(__self__, administrators=None, description=None, descriptor=None, id=None, members=None, name=None, project_id=None):
         if administrators and not isinstance(administrators, list):
             raise TypeError("Expected argument 'administrators' to be a list")
         pulumi.set(__self__, "administrators", administrators)
         if description and not isinstance(description, str):
             raise TypeError("Expected argument 'description' to be a str")
         pulumi.set(__self__, "description", description)
+        if descriptor and not isinstance(descriptor, str):
+            raise TypeError("Expected argument 'descriptor' to be a str")
+        pulumi.set(__self__, "descriptor", descriptor)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if members and not isinstance(members, list):
             raise TypeError("Expected argument 'members' to be a list")
         pulumi.set(__self__, "members", members)
         if name and not isinstance(name, str):
@@ -55,14 +58,22 @@
         """
         Team description.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
+    def descriptor(self) -> str:
+        """
+        The descriptor of the Team.
+        """
+        return pulumi.get(self, "descriptor")
+
+    @property
+    @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
@@ -88,14 +99,15 @@
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetTeamResult(
             administrators=self.administrators,
             description=self.description,
+            descriptor=self.descriptor,
             id=self.id,
             members=self.members,
             name=self.name,
             project_id=self.project_id)
 
 
 def get_team(name: Optional[str] = None,
@@ -135,14 +147,15 @@
     __args__['projectId'] = project_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('azuredevops:index/getTeam:getTeam', __args__, opts=opts, typ=GetTeamResult).value
 
     return AwaitableGetTeamResult(
         administrators=__ret__.administrators,
         description=__ret__.description,
+        descriptor=__ret__.descriptor,
         id=__ret__.id,
         members=__ret__.members,
         name=__ret__.name,
         project_id=__ret__.project_id)
 
 
 @_utilities.lift_output_func(get_team)
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_teams.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_teams.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,18 +78,18 @@
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_teams()
-    pulumi.export("projectId", [__item.project_id for __item in [example.teams]])
-    pulumi.export("name", [__item.name for __item in [example.teams]])
-    pulumi.export("alladministrators", [__item.administrators for __item in [example.teams]])
-    pulumi.export("administrators", [__item.members for __item in [example.teams]])
+    pulumi.export("projectId", [__item.project_id for __item in example.teams])
+    pulumi.export("name", [__item.name for __item in example.teams])
+    pulumi.export("alladministrators", [__item.administrators for __item in example.teams])
+    pulumi.export("administrators", [__item.members for __item in example.teams])
     ```
     ## Relevant Links
 
     - [Azure DevOps Service REST API 6.0 - Teams - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get?view=azure-devops-rest-6.0)
 
     ## PAT Permissions Required
 
@@ -118,18 +118,18 @@
     ## Example Usage
 
     ```python
     import pulumi
     import pulumi_azuredevops as azuredevops
 
     example = azuredevops.get_teams()
-    pulumi.export("projectId", [__item.project_id for __item in [example.teams]])
-    pulumi.export("name", [__item.name for __item in [example.teams]])
-    pulumi.export("alladministrators", [__item.administrators for __item in [example.teams]])
-    pulumi.export("administrators", [__item.members for __item in [example.teams]])
+    pulumi.export("projectId", [__item.project_id for __item in example.teams])
+    pulumi.export("name", [__item.name for __item in example.teams])
+    pulumi.export("alladministrators", [__item.administrators for __item in example.teams])
+    pulumi.export("administrators", [__item.members for __item in example.teams])
     ```
     ## Relevant Links
 
     - [Azure DevOps Service REST API 6.0 - Teams - Get](https://docs.microsoft.com/en-us/rest/api/azure/devops/core/teams/get?view=azure-devops-rest-6.0)
 
     ## PAT Permissions Required
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_users.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/get_variable_group.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/get_variable_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/git.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/git_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/git_repository_branch.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git_repository_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/git_repository_file.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/git_repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/group.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/group_membership.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/identities/get_group.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/identities/get_users.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/identities/group.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/identities/group_membership.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/identities/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/identities/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/iterative_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/iterative_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,22 @@
     'ServiceEndpointPipelineAuthPersonal',
     'ServiceEndpointServiceFabricAzureActiveDirectory',
     'ServiceEndpointServiceFabricCertificate',
     'ServiceEndpointServiceFabricNone',
     'ServiceendpointArgocdAuthenticationBasic',
     'ServiceendpointArgocdAuthenticationToken',
     'ServiceendpointExternaltfsAuthPersonal',
+    'ServiceendpointJfrogArtifactoryV2AuthenticationBasic',
+    'ServiceendpointJfrogArtifactoryV2AuthenticationToken',
+    'ServiceendpointJfrogDistributionV2AuthenticationBasic',
+    'ServiceendpointJfrogDistributionV2AuthenticationToken',
+    'ServiceendpointJfrogPlatformV2AuthenticationBasic',
+    'ServiceendpointJfrogPlatformV2AuthenticationToken',
+    'ServiceendpointJfrogXrayV2AuthenticationBasic',
+    'ServiceendpointJfrogXrayV2AuthenticationToken',
     'VariableGroupKeyVault',
     'VariableGroupVariable',
     'GetAreaChildrenResult',
     'GetBuildDefinitionCiTriggerResult',
     'GetBuildDefinitionCiTriggerOverrideResult',
     'GetBuildDefinitionCiTriggerOverrideBranchFilterResult',
     'GetBuildDefinitionCiTriggerOverridePathFilterResult',
@@ -2307,48 +2315,23 @@
         The URL of the source repository. Used if the `init_type` is `Import`.
         """
         return pulumi.get(self, "source_url")
 
 
 @pulumi.output_type
 class ServiceEndpointArtifactoryAuthenticationBasic(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "passwordHash":
-            suggest = "password_hash"
-        elif key == "usernameHash":
-            suggest = "username_hash"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in ServiceEndpointArtifactoryAuthenticationBasic. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        ServiceEndpointArtifactoryAuthenticationBasic.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        ServiceEndpointArtifactoryAuthenticationBasic.__key_warning(key)
-        return super().get(key, default)
-
     def __init__(__self__, *,
                  password: str,
-                 username: str,
-                 password_hash: Optional[str] = None,
-                 username_hash: Optional[str] = None):
+                 username: str):
         """
         :param str password: Artifactory Password.
         :param str username: Artifactory Username.
         """
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "username", username)
-        if password_hash is not None:
-            pulumi.set(__self__, "password_hash", password_hash)
-        if username_hash is not None:
-            pulumi.set(__self__, "username_hash", username_hash)
 
     @property
     @pulumi.getter
     def password(self) -> str:
         """
         Artifactory Password.
         """
@@ -2358,67 +2341,32 @@
     @pulumi.getter
     def username(self) -> str:
         """
         Artifactory Username.
         """
         return pulumi.get(self, "username")
 
-    @property
-    @pulumi.getter(name="passwordHash")
-    def password_hash(self) -> Optional[str]:
-        return pulumi.get(self, "password_hash")
-
-    @property
-    @pulumi.getter(name="usernameHash")
-    def username_hash(self) -> Optional[str]:
-        return pulumi.get(self, "username_hash")
-
 
 @pulumi.output_type
 class ServiceEndpointArtifactoryAuthenticationToken(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "tokenHash":
-            suggest = "token_hash"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in ServiceEndpointArtifactoryAuthenticationToken. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        ServiceEndpointArtifactoryAuthenticationToken.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        ServiceEndpointArtifactoryAuthenticationToken.__key_warning(key)
-        return super().get(key, default)
-
     def __init__(__self__, *,
-                 token: str,
-                 token_hash: Optional[str] = None):
+                 token: str):
         """
         :param str token: Authentication Token generated through Artifactory.
         """
         pulumi.set(__self__, "token", token)
-        if token_hash is not None:
-            pulumi.set(__self__, "token_hash", token_hash)
 
     @property
     @pulumi.getter
     def token(self) -> str:
         """
         Authentication Token generated through Artifactory.
         """
         return pulumi.get(self, "token")
 
-    @property
-    @pulumi.getter(name="tokenHash")
-    def token_hash(self) -> Optional[str]:
-        return pulumi.get(self, "token_hash")
-
 
 @pulumi.output_type
 class ServiceEndpointAzureRMCredentials(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "serviceprincipalkeyHash":
@@ -3111,48 +3059,23 @@
         Skip using windows security for authentication.
         """
         return pulumi.get(self, "unsecured")
 
 
 @pulumi.output_type
 class ServiceendpointArgocdAuthenticationBasic(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "passwordHash":
-            suggest = "password_hash"
-        elif key == "usernameHash":
-            suggest = "username_hash"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in ServiceendpointArgocdAuthenticationBasic. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        ServiceendpointArgocdAuthenticationBasic.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        ServiceendpointArgocdAuthenticationBasic.__key_warning(key)
-        return super().get(key, default)
-
     def __init__(__self__, *,
                  password: str,
-                 username: str,
-                 password_hash: Optional[str] = None,
-                 username_hash: Optional[str] = None):
+                 username: str):
         """
         :param str password: ArgoCD Password.
         :param str username: ArgoCD Username.
         """
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "username", username)
-        if password_hash is not None:
-            pulumi.set(__self__, "password_hash", password_hash)
-        if username_hash is not None:
-            pulumi.set(__self__, "username_hash", username_hash)
 
     @property
     @pulumi.getter
     def password(self) -> str:
         """
         ArgoCD Password.
         """
@@ -3162,67 +3085,32 @@
     @pulumi.getter
     def username(self) -> str:
         """
         ArgoCD Username.
         """
         return pulumi.get(self, "username")
 
-    @property
-    @pulumi.getter(name="passwordHash")
-    def password_hash(self) -> Optional[str]:
-        return pulumi.get(self, "password_hash")
-
-    @property
-    @pulumi.getter(name="usernameHash")
-    def username_hash(self) -> Optional[str]:
-        return pulumi.get(self, "username_hash")
-
 
 @pulumi.output_type
 class ServiceendpointArgocdAuthenticationToken(dict):
-    @staticmethod
-    def __key_warning(key: str):
-        suggest = None
-        if key == "tokenHash":
-            suggest = "token_hash"
-
-        if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in ServiceendpointArgocdAuthenticationToken. Access the value via the '{suggest}' property getter instead.")
-
-    def __getitem__(self, key: str) -> Any:
-        ServiceendpointArgocdAuthenticationToken.__key_warning(key)
-        return super().__getitem__(key)
-
-    def get(self, key: str, default = None) -> Any:
-        ServiceendpointArgocdAuthenticationToken.__key_warning(key)
-        return super().get(key, default)
-
     def __init__(__self__, *,
-                 token: str,
-                 token_hash: Optional[str] = None):
+                 token: str):
         """
         :param str token: Authentication Token generated through ArgoCD.
         """
         pulumi.set(__self__, "token", token)
-        if token_hash is not None:
-            pulumi.set(__self__, "token_hash", token_hash)
 
     @property
     @pulumi.getter
     def token(self) -> str:
         """
         Authentication Token generated through ArgoCD.
         """
         return pulumi.get(self, "token")
 
-    @property
-    @pulumi.getter(name="tokenHash")
-    def token_hash(self) -> Optional[str]:
-        return pulumi.get(self, "token_hash")
-
 
 @pulumi.output_type
 class ServiceendpointExternaltfsAuthPersonal(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "personalAccessToken":
@@ -3252,14 +3140,202 @@
         """
         The Personal Access Token for Azure DevOps Organization.
         """
         return pulumi.get(self, "personal_access_token")
 
 
 @pulumi.output_type
+class ServiceendpointJfrogArtifactoryV2AuthenticationBasic(dict):
+    def __init__(__self__, *,
+                 password: str,
+                 username: str):
+        """
+        :param str password: Artifactory Password.
+        :param str username: Artifactory Username.
+        """
+        pulumi.set(__self__, "password", password)
+        pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def password(self) -> str:
+        """
+        Artifactory Password.
+        """
+        return pulumi.get(self, "password")
+
+    @property
+    @pulumi.getter
+    def username(self) -> str:
+        """
+        Artifactory Username.
+        """
+        return pulumi.get(self, "username")
+
+
+@pulumi.output_type
+class ServiceendpointJfrogArtifactoryV2AuthenticationToken(dict):
+    def __init__(__self__, *,
+                 token: str):
+        """
+        :param str token: Authentication Token generated through Artifactory.
+        """
+        pulumi.set(__self__, "token", token)
+
+    @property
+    @pulumi.getter
+    def token(self) -> str:
+        """
+        Authentication Token generated through Artifactory.
+        """
+        return pulumi.get(self, "token")
+
+
+@pulumi.output_type
+class ServiceendpointJfrogDistributionV2AuthenticationBasic(dict):
+    def __init__(__self__, *,
+                 password: str,
+                 username: str):
+        """
+        :param str password: Artifactory Password.
+        :param str username: Artifactory Username.
+        """
+        pulumi.set(__self__, "password", password)
+        pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def password(self) -> str:
+        """
+        Artifactory Password.
+        """
+        return pulumi.get(self, "password")
+
+    @property
+    @pulumi.getter
+    def username(self) -> str:
+        """
+        Artifactory Username.
+        """
+        return pulumi.get(self, "username")
+
+
+@pulumi.output_type
+class ServiceendpointJfrogDistributionV2AuthenticationToken(dict):
+    def __init__(__self__, *,
+                 token: str):
+        """
+        :param str token: Authentication Token generated through Artifactory.
+        """
+        pulumi.set(__self__, "token", token)
+
+    @property
+    @pulumi.getter
+    def token(self) -> str:
+        """
+        Authentication Token generated through Artifactory.
+        """
+        return pulumi.get(self, "token")
+
+
+@pulumi.output_type
+class ServiceendpointJfrogPlatformV2AuthenticationBasic(dict):
+    def __init__(__self__, *,
+                 password: str,
+                 username: str):
+        """
+        :param str password: Artifactory Password.
+        :param str username: Artifactory Username.
+        """
+        pulumi.set(__self__, "password", password)
+        pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def password(self) -> str:
+        """
+        Artifactory Password.
+        """
+        return pulumi.get(self, "password")
+
+    @property
+    @pulumi.getter
+    def username(self) -> str:
+        """
+        Artifactory Username.
+        """
+        return pulumi.get(self, "username")
+
+
+@pulumi.output_type
+class ServiceendpointJfrogPlatformV2AuthenticationToken(dict):
+    def __init__(__self__, *,
+                 token: str):
+        """
+        :param str token: Authentication Token generated through Artifactory.
+        """
+        pulumi.set(__self__, "token", token)
+
+    @property
+    @pulumi.getter
+    def token(self) -> str:
+        """
+        Authentication Token generated through Artifactory.
+        """
+        return pulumi.get(self, "token")
+
+
+@pulumi.output_type
+class ServiceendpointJfrogXrayV2AuthenticationBasic(dict):
+    def __init__(__self__, *,
+                 password: str,
+                 username: str):
+        """
+        :param str password: Artifactory Password.
+        :param str username: Artifactory Username.
+        """
+        pulumi.set(__self__, "password", password)
+        pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def password(self) -> str:
+        """
+        Artifactory Password.
+        """
+        return pulumi.get(self, "password")
+
+    @property
+    @pulumi.getter
+    def username(self) -> str:
+        """
+        Artifactory Username.
+        """
+        return pulumi.get(self, "username")
+
+
+@pulumi.output_type
+class ServiceendpointJfrogXrayV2AuthenticationToken(dict):
+    def __init__(__self__, *,
+                 token: str):
+        """
+        :param str token: Authentication Token generated through Artifactory.
+        """
+        pulumi.set(__self__, "token", token)
+
+    @property
+    @pulumi.getter
+    def token(self) -> str:
+        """
+        Authentication Token generated through Artifactory.
+        """
+        return pulumi.get(self, "token")
+
+
+@pulumi.output_type
 class VariableGroupKeyVault(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "serviceEndpointId":
             suggest = "service_endpoint_id"
         elif key == "searchDepth":
@@ -4319,15 +4395,15 @@
     def __init__(__self__, *,
                  name: str,
                  project_id: str,
                  project_url: str,
                  state: str):
         """
         :param str name: Name of the Project, if not specified all projects will be returned.
-        :param str project_id: Project identifier.
+        :param str project_id: The ID of the Project.
         :param str project_url: Url to the full version of the object.
         :param str state: State of the Project, if not specified all projects will be returned. Valid values are `all`, `deleting`, `new`, `wellFormed`, `createPending`, `unchanged`,`deleted`.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "project_id", project_id)
         pulumi.set(__self__, "project_url", project_url)
         pulumi.set(__self__, "state", state)
@@ -4340,15 +4416,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> str:
         """
-        Project identifier.
+        The ID of the Project.
         """
         return pulumi.get(self, "project_id")
 
     @property
     @pulumi.getter(name="projectUrl")
     def project_url(self) -> str:
         """
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/pipeline/_inputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/pipeline/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/pipeline/variable_group.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pipeline/variable_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                  variables: pulumi.Input[Sequence[pulumi.Input['VariableGroupVariableArgs']]],
                  allow_access: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  key_vault: Optional[pulumi.Input['VariableGroupKeyVaultArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a VariableGroup resource.
-        :param pulumi.Input[str] project_id: The project ID or project name.
+        :param pulumi.Input[str] project_id: The ID of the project.
         :param pulumi.Input[Sequence[pulumi.Input['VariableGroupVariableArgs']]] variables: One or more `variable` blocks as documented below.
         :param pulumi.Input[bool] allow_access: Boolean that indicate if this variable group is shared by all pipelines of this project.
         :param pulumi.Input[str] description: The description of the Variable Group.
         :param pulumi.Input['VariableGroupKeyVaultArgs'] key_vault: A list of `key_vault` blocks as documented below.
         :param pulumi.Input[str] name: The name of the Variable Group.
         """
         pulumi.set(__self__, "project_id", project_id)
@@ -42,15 +42,15 @@
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> pulumi.Input[str]:
         """
-        The project ID or project name.
+        The ID of the project.
         """
         return pulumi.get(self, "project_id")
 
     @project_id.setter
     def project_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "project_id", value)
 
@@ -126,15 +126,15 @@
                  variables: Optional[pulumi.Input[Sequence[pulumi.Input['VariableGroupVariableArgs']]]] = None):
         """
         Input properties used for looking up and filtering VariableGroup resources.
         :param pulumi.Input[bool] allow_access: Boolean that indicate if this variable group is shared by all pipelines of this project.
         :param pulumi.Input[str] description: The description of the Variable Group.
         :param pulumi.Input['VariableGroupKeyVaultArgs'] key_vault: A list of `key_vault` blocks as documented below.
         :param pulumi.Input[str] name: The name of the Variable Group.
-        :param pulumi.Input[str] project_id: The project ID or project name.
+        :param pulumi.Input[str] project_id: The ID of the project.
         :param pulumi.Input[Sequence[pulumi.Input['VariableGroupVariableArgs']]] variables: One or more `variable` blocks as documented below.
         """
         if allow_access is not None:
             pulumi.set(__self__, "allow_access", allow_access)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if key_vault is not None:
@@ -194,15 +194,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The project ID or project name.
+        The ID of the project.
         """
         return pulumi.get(self, "project_id")
 
     @project_id.setter
     def project_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "project_id", value)
 
@@ -335,15 +335,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] allow_access: Boolean that indicate if this variable group is shared by all pipelines of this project.
         :param pulumi.Input[str] description: The description of the Variable Group.
         :param pulumi.Input[pulumi.InputType['VariableGroupKeyVaultArgs']] key_vault: A list of `key_vault` blocks as documented below.
         :param pulumi.Input[str] name: The name of the Variable Group.
-        :param pulumi.Input[str] project_id: The project ID or project name.
+        :param pulumi.Input[str] project_id: The ID of the project.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VariableGroupVariableArgs']]]] variables: One or more `variable` blocks as documented below.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: VariableGroupArgs,
@@ -509,15 +509,15 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] allow_access: Boolean that indicate if this variable group is shared by all pipelines of this project.
         :param pulumi.Input[str] description: The description of the Variable Group.
         :param pulumi.Input[pulumi.InputType['VariableGroupKeyVaultArgs']] key_vault: A list of `key_vault` blocks as documented below.
         :param pulumi.Input[str] name: The name of the Variable Group.
-        :param pulumi.Input[str] project_id: The project ID or project name.
+        :param pulumi.Input[str] project_id: The ID of the project.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VariableGroupVariableArgs']]]] variables: One or more `variable` blocks as documented below.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _VariableGroupState.__new__(_VariableGroupState)
 
         __props__.__dict__["allow_access"] = allow_access
@@ -560,15 +560,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> pulumi.Output[str]:
         """
-        The project ID or project name.
+        The ID of the project.
         """
         return pulumi.get(self, "project_id")
 
     @property
     @pulumi.getter
     def variables(self) -> pulumi.Output[Sequence['outputs.VariableGroupVariable']]:
         """
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/policy/_inputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/policy/branch_policy_build_validation.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/branch_policy_build_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/policy/branch_policy_min_reviewers.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/branch_policy_min_reviewers.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/policy/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/policy/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/pool.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/project.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/project_features.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project_features.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/project_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/project_pipeline_settings.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/project_pipeline_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/provider.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/queue.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository/_inputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository/get_repositories.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/get_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository/git.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/git.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository_policy_author_email_pattern.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_author_email_pattern.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository_policy_case_enforcement.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_case_enforcement.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository_policy_check_credentials.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_check_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository_policy_file_path_pattern.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_file_path_pattern.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository_policy_max_file_size.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_max_file_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository_policy_max_path_length.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_max_path_length.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/repository_policy_reserved_names.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/repository_policy_reserved_names.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/resource_authorization.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/resource_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/security/resource_authorization.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/security/resource_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_artifactory.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_artifactory.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                  authorization: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  service_endpoint_name: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Manages an Artifactory server endpoint within an Azure DevOps organization.
+        Manages an Artifactory server endpoint within an Azure DevOps organization. Using this service endpoint requires you to first install [JFrog Artifactory Extension](https://marketplace.visualstudio.com/items?itemName=JFrog.jfrog-artifactory-vsts-extension).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
 
@@ -306,15 +306,15 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ServiceEndpointArtifactoryArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Manages an Artifactory server endpoint within an Azure DevOps organization.
+        Manages an Artifactory server endpoint within an Azure DevOps organization. Using this service endpoint requires you to first install [JFrog Artifactory Extension](https://marketplace.visualstudio.com/items?itemName=JFrog.jfrog-artifactory-vsts-extension).
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_azuredevops as azuredevops
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_aws.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_aws.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_azure_dev_ops.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_azure_dev_ops.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_azure_ecr.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_azure_ecr.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_azure_rm.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_azure_rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_bit_bucket.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_bit_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_docker_registry.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_docker_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_generic.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_generic.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_generic_git.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_generic_git.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_git_hub.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_git_hub.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_kubernetes.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_kubernetes.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_npm.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_npm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_pipeline.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_service_fabric.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_service_fabric.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_sonar_cloud.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_sonar_cloud.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_sonar_qube.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_sonar_qube.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/service_endpoint_ssh.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/service_endpoint_ssh.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/_inputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/azure_rm.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/azure_rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/bit_bucket.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/bit_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/docker_registry.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/docker_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/git_hub.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/git_hub.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/kubernetes.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/kubernetes.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint/outputs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint_argocd.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_argocd.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint_externaltfs.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_externaltfs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint_incomingwebhook.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_incomingwebhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint_octopusdeploy.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_octopusdeploy.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/serviceendpoint_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/serviceendpoint_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/servicehook_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/servicehook_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/tagging_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/tagging_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/team.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/team_administrators.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/team_administrators.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/team_members.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/team_members.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/user.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/variable_group.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/variable_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                  variables: pulumi.Input[Sequence[pulumi.Input['VariableGroupVariableArgs']]],
                  allow_access: Optional[pulumi.Input[bool]] = None,
                  description: Optional[pulumi.Input[str]] = None,
                  key_vault: Optional[pulumi.Input['VariableGroupKeyVaultArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a VariableGroup resource.
-        :param pulumi.Input[str] project_id: The project ID or project name.
+        :param pulumi.Input[str] project_id: The ID of the project.
         :param pulumi.Input[Sequence[pulumi.Input['VariableGroupVariableArgs']]] variables: One or more `variable` blocks as documented below.
         :param pulumi.Input[bool] allow_access: Boolean that indicate if this variable group is shared by all pipelines of this project.
         :param pulumi.Input[str] description: The description of the Variable Group.
         :param pulumi.Input['VariableGroupKeyVaultArgs'] key_vault: A list of `key_vault` blocks as documented below.
         :param pulumi.Input[str] name: The name of the Variable Group.
         """
         pulumi.set(__self__, "project_id", project_id)
@@ -42,15 +42,15 @@
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> pulumi.Input[str]:
         """
-        The project ID or project name.
+        The ID of the project.
         """
         return pulumi.get(self, "project_id")
 
     @project_id.setter
     def project_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "project_id", value)
 
@@ -126,15 +126,15 @@
                  variables: Optional[pulumi.Input[Sequence[pulumi.Input['VariableGroupVariableArgs']]]] = None):
         """
         Input properties used for looking up and filtering VariableGroup resources.
         :param pulumi.Input[bool] allow_access: Boolean that indicate if this variable group is shared by all pipelines of this project.
         :param pulumi.Input[str] description: The description of the Variable Group.
         :param pulumi.Input['VariableGroupKeyVaultArgs'] key_vault: A list of `key_vault` blocks as documented below.
         :param pulumi.Input[str] name: The name of the Variable Group.
-        :param pulumi.Input[str] project_id: The project ID or project name.
+        :param pulumi.Input[str] project_id: The ID of the project.
         :param pulumi.Input[Sequence[pulumi.Input['VariableGroupVariableArgs']]] variables: One or more `variable` blocks as documented below.
         """
         if allow_access is not None:
             pulumi.set(__self__, "allow_access", allow_access)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if key_vault is not None:
@@ -194,15 +194,15 @@
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The project ID or project name.
+        The ID of the project.
         """
         return pulumi.get(self, "project_id")
 
     @project_id.setter
     def project_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "project_id", value)
 
@@ -330,15 +330,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] allow_access: Boolean that indicate if this variable group is shared by all pipelines of this project.
         :param pulumi.Input[str] description: The description of the Variable Group.
         :param pulumi.Input[pulumi.InputType['VariableGroupKeyVaultArgs']] key_vault: A list of `key_vault` blocks as documented below.
         :param pulumi.Input[str] name: The name of the Variable Group.
-        :param pulumi.Input[str] project_id: The project ID or project name.
+        :param pulumi.Input[str] project_id: The ID of the project.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VariableGroupVariableArgs']]]] variables: One or more `variable` blocks as documented below.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: VariableGroupArgs,
@@ -505,15 +505,15 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] allow_access: Boolean that indicate if this variable group is shared by all pipelines of this project.
         :param pulumi.Input[str] description: The description of the Variable Group.
         :param pulumi.Input[pulumi.InputType['VariableGroupKeyVaultArgs']] key_vault: A list of `key_vault` blocks as documented below.
         :param pulumi.Input[str] name: The name of the Variable Group.
-        :param pulumi.Input[str] project_id: The project ID or project name.
+        :param pulumi.Input[str] project_id: The ID of the project.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VariableGroupVariableArgs']]]] variables: One or more `variable` blocks as documented below.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _VariableGroupState.__new__(_VariableGroupState)
 
         __props__.__dict__["allow_access"] = allow_access
@@ -556,15 +556,15 @@
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> pulumi.Output[str]:
         """
-        The project ID or project name.
+        The ID of the project.
         """
         return pulumi.get(self, "project_id")
 
     @property
     @pulumi.getter
     def variables(self) -> pulumi.Output[Sequence['outputs.VariableGroupVariable']]:
         """
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/work_item_query_permissions.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/work_item_query_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops/workitem.py` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops/workitem.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops.egg-info/PKG-INFO` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-azuredevops
-Version: 2.7.0a1679928807
+Version: 2.8.0a1683661270
 Summary: A Pulumi package for creating and managing Azure DevOps.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuredevops
 Keywords: pulumi azuredevops
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-azuredevops/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-azuredevops/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fazuredevops.svg)](https://www.npmjs.com/package/@pulumi/azuredevops)
 [![Python version](https://badge.fury.io/py/pulumi-azuredevops.svg)](https://pypi.org/project/pulumi-azuredevops)
 [![NuGet version](https://badge.fury.io/nu/pulumi.azuredevops.svg)](https://badge.fury.io/nu/pulumi.azuredevops)
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/pulumi_azuredevops.egg-info/SOURCES.txt` & `pulumi_azuredevops-2.8.0a1683661270/pulumi_azuredevops.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,18 @@
 pulumi_azuredevops/service_endpoint_service_fabric.py
 pulumi_azuredevops/service_endpoint_sonar_cloud.py
 pulumi_azuredevops/service_endpoint_sonar_qube.py
 pulumi_azuredevops/service_endpoint_ssh.py
 pulumi_azuredevops/serviceendpoint_argocd.py
 pulumi_azuredevops/serviceendpoint_externaltfs.py
 pulumi_azuredevops/serviceendpoint_incomingwebhook.py
+pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py
+pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py
+pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py
+pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py
 pulumi_azuredevops/serviceendpoint_octopusdeploy.py
 pulumi_azuredevops/serviceendpoint_permissions.py
 pulumi_azuredevops/servicehook_permissions.py
 pulumi_azuredevops/tagging_permissions.py
 pulumi_azuredevops/team.py
 pulumi_azuredevops/team_administrators.py
 pulumi_azuredevops/team_members.py
```

### Comparing `pulumi_azuredevops-2.7.0a1679928807/setup.py` & `pulumi_azuredevops-2.8.0a1683661270/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.7.0a1679928807"
-PLUGIN_VERSION = "2.7.0-alpha.1679928807+409dde1c"
+VERSION = "2.8.0a1683661270"
+PLUGIN_VERSION = "2.8.0-alpha.1683661270+aa6c7d3b"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'azuredevops', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "azuredevops Pulumi Package - Development Version"
 
 
 setup(name='pulumi_azuredevops',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing Azure DevOps.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

