# Comparing `tmp/pop-create-idem-3.4.0.tar.gz` & `tmp/pop-create-idem-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop-create-idem-3.4.0.tar", last modified: Fri May  5 13:31:18 2023, max compression
+gzip compressed data, was "pop-create-idem-3.4.1.tar", last modified: Tue May  9 14:57:04 2023, max compression
```

## Comparing `pop-create-idem-3.4.0.tar` & `pop-create-idem-3.4.1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.816471 pop-create-idem-3.4.0/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       61 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8796 2023-05-05 13:31:18.816471 pop-create-idem-3.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7947 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.809137 pop-create-idem-3.4.0/cloudspec/
--rw-r--r--   0 root         (0) root         (0)     8546 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/cloudspec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      729 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/cloudspec/conf.py
--rw-r--r--   0 root         (0) root         (0)      149 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/cloudspec/scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.809137 pop-create-idem-3.4.0/pop_create_idem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810054 pop-create-idem-3.4.0/pop_create_idem/cloudspec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810054 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/
--rw-r--r--   0 root         (0) root         (0)     3158 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/auto_state.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810970 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/contracts/
--rw-r--r--   0 root         (0) root         (0)       78 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/docs.py
--rw-r--r--   0 root         (0) root         (0)     2780 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/exec_modules.py
--rw-r--r--   0 root         (0) root         (0)     3241 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/state_modules.py
--rw-r--r--   0 root         (0) root         (0)      270 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/templates.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/tests.py
--rw-r--r--   0 root         (0) root         (0)     3080 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/tool.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810970 pop-create-idem-3.4.0/pop_create_idem/cloudspec/parse/
--rw-r--r--   0 root         (0) root         (0)     2154 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/parse/function.py
--rw-r--r--   0 root         (0) root         (0)     5802 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/parse/param.py
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/parse/plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810970 pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/
--rw-r--r--   0 root         (0) root         (0)     3477 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/auto_state.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/exec.py
--rw-r--r--   0 root         (0) root         (0)      822 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/state.py
--rw-r--r--   0 root         (0) root         (0)      209 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/tool.py
--rw-r--r--   0 root         (0) root         (0)     2075 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810970 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810970 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/hooks/
--rw-r--r--   0 root         (0) root         (0)     1764 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
--rw-r--r--   0 root         (0) root         (0)     2509 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
--rw-r--r--   0 root         (0) root         (0)      173 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     2633 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
--rw-r--r--   0 root         (0) root         (0)      626 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      960 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)      282 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/sample.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      763 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)      891 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.812804 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.813721 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      917 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.813721 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)      196 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
--rw-r--r--   0 root         (0) root         (0)     3854 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.813721 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1548 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.813721 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/
--rw-r--r--   0 root         (0) root         (0)     3840 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.813721 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/hooks/
--rw-r--r--   0 root         (0) root         (0)     1302 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
--rw-r--r--   0 root         (0) root         (0)     5076 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/init.py
--rw-r--r--   0 root         (0) root         (0)     4964 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/params.py
--rw-r--r--   0 root         (0) root         (0)     6475 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/parse.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.807304 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.814637 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     1740 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.814637 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/
--rw-r--r--   0 root         (0) root         (0)      969 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2
--rw-r--r--   0 root         (0) root         (0)      700 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2
--rw-r--r--   0 root         (0) root         (0)     1885 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2
--rw-r--r--   0 root         (0) root         (0)     1539 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2
--rw-r--r--   0 root         (0) root         (0)     1425 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.814637 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/
--rw-r--r--   0 root         (0) root         (0)     1903 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2
--rw-r--r--   0 root         (0) root         (0)      941 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2
--rw-r--r--   0 root         (0) root         (0)     4298 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.814637 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/
--rw-r--r--   0 root         (0) root         (0)     1411 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.815554 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
--rw-r--r--   0 root         (0) root         (0)     2649 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.815554 pop-create-idem-3.4.0/pop_create_idem/pop_create/rest/
--rw-r--r--   0 root         (0) root         (0)      133 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/rest/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.815554 pop-create-idem-3.4.0/pop_create_idem/pop_create/swagger/
--rw-r--r--   0 root         (0) root         (0)      708 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/swagger/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.808220 pop-create-idem-3.4.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.815554 pop-create-idem-3.4.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.815554 pop-create-idem-3.4.0/pop_create_idem/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.815554 pop-create-idem-3.4.0/pop_create_idem/tool/format/
--rw-r--r--   0 root         (0) root         (0)     1048 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/tool/format/case.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/tool/format/html.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/tool/format/inflect.py
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/tool/format/keyword.py
--rw-r--r--   0 root         (0) root         (0)      211 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/tool/format/wrap.py
--rw-r--r--   0 root         (0) root         (0)      878 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/tool/gradle.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/pop_create_idem/tool/jinja.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-05 13:31:18.000000 pop-create-idem-3.4.0/pop_create_idem/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:31:18.810054 pop-create-idem-3.4.0/pop_create_idem.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8796 2023-05-05 13:31:18.000000 pop-create-idem-3.4.0/pop_create_idem.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5938 2023-05-05 13:31:18.000000 pop-create-idem-3.4.0/pop_create_idem.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 13:31:18.000000 pop-create-idem-3.4.0/pop_create_idem.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-05 13:31:18.000000 pop-create-idem-3.4.0/pop_create_idem.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-05 13:31:18.000000 pop-create-idem-3.4.0/pop_create_idem.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-05 13:31:18.000000 pop-create-idem-3.4.0/pop_create_idem.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-05 13:31:18.816471 pop-create-idem-3.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3004 2023-05-05 13:31:01.000000 pop-create-idem-3.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.413895 pop-create-idem-3.4.1/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-05-09 14:57:04.413895 pop-create-idem-3.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7947 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.408395 pop-create-idem-3.4.1/cloudspec/
+-rw-r--r--   0 root         (0) root         (0)     8546 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/cloudspec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      729 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/cloudspec/conf.py
+-rw-r--r--   0 root         (0) root         (0)      149 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/cloudspec/scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.408395 pop-create-idem-3.4.1/pop_create_idem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.408395 pop-create-idem-3.4.1/pop_create_idem/cloudspec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.409312 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/
+-rw-r--r--   0 root         (0) root         (0)     3158 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/auto_state.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.409312 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/contracts/
+-rw-r--r--   0 root         (0) root         (0)       78 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/docs.py
+-rw-r--r--   0 root         (0) root         (0)     2780 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/exec_modules.py
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/state_modules.py
+-rw-r--r--   0 root         (0) root         (0)      270 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/templates.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/tests.py
+-rw-r--r--   0 root         (0) root         (0)     3080 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/tool.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.409312 pop-create-idem-3.4.1/pop_create_idem/cloudspec/parse/
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/parse/function.py
+-rw-r--r--   0 root         (0) root         (0)     5802 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/parse/param.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/parse/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.410228 pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/
+-rw-r--r--   0 root         (0) root         (0)     3477 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/auto_state.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/exec.py
+-rw-r--r--   0 root         (0) root         (0)      822 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/state.py
+-rw-r--r--   0 root         (0) root         (0)      209 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/tool.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.406561 pop-create-idem-3.4.1/pop_create_idem/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.410228 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.410228 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/hooks/
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.410228 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst
+-rw-r--r--   0 root         (0) root         (0)      173 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/build.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.410228 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/requirements/base.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.404728 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.410228 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.404728 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)      282 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/default_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.404728 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.404728 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/sample.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      763 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)      891 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)      917 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/init.py
+-rw-r--r--   0 root         (0) root         (0)     3854 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.411145 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412062 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/
+-rw-r--r--   0 root         (0) root         (0)     3899 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412062 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/hooks/
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py
+-rw-r--r--   0 root         (0) root         (0)     5076 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/init.py
+-rw-r--r--   0 root         (0) root         (0)     4784 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/params.py
+-rw-r--r--   0 root         (0) root         (0)     6475 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/parse.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.406561 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412062 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.405645 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412979 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2
+-rw-r--r--   0 root         (0) root         (0)      700 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412979 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/
+-rw-r--r--   0 root         (0) root         (0)     1903 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2
+-rw-r--r--   0 root         (0) root         (0)      941 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2
+-rw-r--r--   0 root         (0) root         (0)     4298 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412979 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.406561 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412979 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412979 pop-create-idem-3.4.1/pop_create_idem/pop_create/rest/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/rest/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412979 pop-create-idem-3.4.1/pop_create_idem/pop_create/swagger/
+-rw-r--r--   0 root         (0) root         (0)      708 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/swagger/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.406561 pop-create-idem-3.4.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.412979 pop-create-idem-3.4.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/pop_create/swagger/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.413895 pop-create-idem-3.4.1/pop_create_idem/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.413895 pop-create-idem-3.4.1/pop_create_idem/tool/format/
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/tool/format/case.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/tool/format/html.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/tool/format/inflect.py
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/tool/format/keyword.py
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/tool/format/wrap.py
+-rw-r--r--   0 root         (0) root         (0)      878 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/tool/gradle.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/pop_create_idem/tool/jinja.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-09 14:57:03.000000 pop-create-idem-3.4.1/pop_create_idem/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 14:57:04.408395 pop-create-idem-3.4.1/pop_create_idem.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-05-09 14:57:04.000000 pop-create-idem-3.4.1/pop_create_idem.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5938 2023-05-09 14:57:04.000000 pop-create-idem-3.4.1/pop_create_idem.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 14:57:04.000000 pop-create-idem-3.4.1/pop_create_idem.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-09 14:57:04.000000 pop-create-idem-3.4.1/pop_create_idem.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-09 14:57:04.000000 pop-create-idem-3.4.1/pop_create_idem.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-09 14:57:04.000000 pop-create-idem-3.4.1/pop_create_idem.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-09 14:57:04.414812 pop-create-idem-3.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3004 2023-05-09 14:56:47.000000 pop-create-idem-3.4.1/setup.py
```

### Comparing `pop-create-idem-3.4.0/LICENSE` & `pop-create-idem-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/PKG-INFO` & `pop-create-idem-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 3.4.0
+Version: 3.4.1
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-3.4.0/README.rst` & `pop-create-idem-3.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/cloudspec/__init__.py` & `pop-create-idem-3.4.1/cloudspec/__init__.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/cloudspec/conf.py` & `pop-create-idem-3.4.1/cloudspec/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/auto_state.py` & `pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/auto_state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/exec_modules.py` & `pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/exec_modules.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/state_modules.py` & `pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/state_modules.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/tests.py` & `pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/tests.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/cloudspec/create/tool.py` & `pop-create-idem-3.4.1/pop_create_idem/cloudspec/create/tool.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/cloudspec/init.py` & `pop-create-idem-3.4.1/pop_create_idem/cloudspec/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/cloudspec/parse/function.py` & `pop-create-idem-3.4.1/pop_create_idem/cloudspec/parse/function.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/cloudspec/parse/param.py` & `pop-create-idem-3.4.1/pop_create_idem/cloudspec/parse/param.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/cloudspec/parse/plugin.py` & `pop-create-idem-3.4.1/pop_create_idem/cloudspec/parse/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/auto_state.py` & `pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/auto_state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/exec.py` & `pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/exec.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/plugin.py` & `pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/plugin.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/cloudspec/template/state.py` & `pop-create-idem-3.4.1/pop_create_idem/cloudspec/template/state.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/conf.py` & `pop-create-idem-3.4.1/pop_create_idem/conf.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/hooks/pre_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/init.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/README.rst`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/exec/{{cookiecutter.service_name}}/{{cookiecutter.clean_api_version}}/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/states/{{cookiecutter.service_name}}/sample.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/idem_cloud/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/function.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     params.update(request_body_params)
 
     if "name" in params:
         # The template already adds name by default
         params.pop("name")
 
     deprecated_text = "\nDEPRECATED" if func.deprecated else ""
+
     return {
         "doc": f"{func.summary}\n    {func.description}    {deprecated_text}".strip(),
         "params": params,
         "hardcoded": {
             "method": request_type,
             "path": path.split(" ")[0],
             "service_name": ctx.service_name,
@@ -73,16 +74,18 @@
                 schema = list(request_body.content.raw_element.values()).pop()
 
             schema_ref = schema.get("schema", {}).get("$ref")
             hub.pop_create.openapi3.params.parse_schema_members(
                 request_body_params, schema_ref, all_schemas
             )
 
-            request_mappings = hub.pop_create.openapi3.params.parse_request_mappings(
-                schema_ref, all_schemas
+            request_mappings = (
+                hub.pop_create.openapi3.params.parse_resource_to_request_input_mappings(
+                    schema_ref, all_schemas
+                )
             )
     except Exception as e:
         hub.log.debug(f"Failed to parse request body: {e.__class__.__name__}: {e}")
 
     return request_body_params, request_mappings
```

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/init.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/params.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/params.py`

 * *Files 15% similar despite different names*

```diff
@@ -73,47 +73,33 @@
             if isinstance(parameter.schema, openapi3.schemas.Schema)
             else None
         ),
         "doc": parameter.description,
     }
 
 
-def parse_request_mappings(hub, schema_ref: str, all_schemas: dict):
-    """
-    Resolve idem_resource to request payload
-    """
+def parse_resource_to_request_input_mappings(hub, schema_ref: str, all_schemas: dict):
+    resource_to_request_input_mapping = {}
     if not schema_ref:
         return "{}"
 
     parameters: list = all_schemas.get(schema_ref)
-    ret = "{"
     if parameters:
-        # e.g. a create pet request would get the following payload
-        # payload = {
-        #     "id": id,
-        #     "category": category,
-        #     "name": name,
-        #     "photoUrls": photo_urls,
-        #     "tags": tags,
-        #     "status": status,
-        # }
-        ret += "\n"
         for p in parameters:
-            if "actual_name" in p and p.get("actual_name"):
-                ret += (
-                    '        "'
-                    + p.get("actual_name")
-                    + '"'
-                    + ": "
-                    + hub.tool.format.keyword.unclash(p.get("idem_name").strip('"'))
-                    + ",\n    "
+            if "idem_name" in p and p.get("idem_name"):
+                resource_to_request_input_mapping[p.get("idem_name")] = p.get(
+                    "actual_name", ""
                 )
 
-    ret += "}"
-    return ret
+    # This is used when mapping idem formatted resource attributes to raw request inputs
+    # resource_to_request_input_mapping = {
+    #     "photo_urls": "photoUrls", -> photoUrls is the attribute on server side but idem name is snaked as photo_urls
+    #     "tags": tags,
+    # }
+    return resource_to_request_input_mapping
 
 
 def parse_response_mappings(hub, schema_ref: str, all_schemas: dict) -> Dict[str, str]:
     """
     Resolve idem_resource to request payload
     """
     response_mapping = {}
```

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/parse.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/parse.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/schemas.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/schemas.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/api_key_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/acct/{{cookiecutter.service_name}}/client_credentials_auth.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/create.jinja2`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 {# templates/create.jinja2 #}
     result = dict(comment=[], ret=[], result=True)
 
+    desired_state = {
+        k: v
+        for k, v in locals().items()
+        if k not in ("hub", "ctx", "kwargs", "result") and v is not None
+    }
+
     # TODO: Change request param mapping as necessary
-    payload = {{ function.hardcoded.request_mappings|default("{}", true) }}
+    resource_to_raw_input_mapping = {{ function.hardcoded.request_mappings|default("{}", true) }}
+
+    payload = {}
+    for key, value in desired_state.items():
+        if key in resource_to_raw_input_mapping.keys() and value is not None:
+            payload[resource_to_raw_input_mapping[key]] = value
 
     create = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
         ctx,
         method="{{ function.hardcoded.method }}",
         path="{{ function.hardcoded.path }}",
         query_params={{ parameter.mapping.query|default({}) }},
         data=payload,
```

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/delete.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/get.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/list.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/exec/update.jinja2`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     # TODO: Change request param mapping as necessary
     resource_to_raw_input_mapping = {{ function.hardcoded.request_mappings|default("{}", true) }}
 
     payload = {}
     for key, value in desired_state.items():
         if key in resource_to_raw_input_mapping.keys() and value is not None:
-            payload[resource_to_raw_input_mapping[key]] = desired_state.get(key)
+            payload[resource_to_raw_input_mapping[key]] = value
 
     if payload:
         update = await hub.tool.{{ function.hardcoded.service_name }}.session.request(
             ctx,
             method="{{ function.hardcoded.method }}",
             path="{{ function.hardcoded.path }}".format(
                 **{{ parameter.mapping.path|default({}) }}
```

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/absent.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/describe.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/state/present.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/autogen/{{cookiecutter.service_name}}/templates/tool/default.jinja2`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/openapi3/{{cookiecutter.root_dir}}/{{cookiecutter.clean_name}}/tool/{{cookiecutter.service_name}}/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,20 +31,21 @@
             headers["content-type"] = "application/json"
             headers["accept"] = "application/json"
 
         if "headers" in ctx.acct:
             # The acct login could set authorization and other headers
             headers.update(ctx.acct.headers)
 
+        query_params_sanitized = {k: v for k, v in query_params.items() if v is not None}
         async with session.request(
             url=url,
             method=method.lower(),
             ssl=False,
             allow_redirects=True,
-            params=query_params,
+            params=query_params_sanitized,
             data=json.dumps(data),
             headers=headers,
         ) as response:
             result["status"] = response.status
             result["result"] = 200 <= response.status <= 204
             result["comment"].append(response.reason)
             result["headers"].update(response.headers)
```

### Comparing `pop-create-idem-3.4.0/pop_create_idem/pop_create/swagger/init.py` & `pop-create-idem-3.4.1/pop_create_idem/pop_create/swagger/init.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/tool/format/case.py` & `pop-create-idem-3.4.1/pop_create_idem/tool/format/case.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/tool/format/inflect.py` & `pop-create-idem-3.4.1/pop_create_idem/tool/format/inflect.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem/tool/gradle.py` & `pop-create-idem-3.4.1/pop_create_idem/tool/gradle.py`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/pop_create_idem.egg-info/PKG-INFO` & `pop-create-idem-3.4.1/pop_create_idem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-create-idem
-Version: 3.4.0
+Version: 3.4.1
 Summary: UNKNOWN
 Home-page: https://gitlab.com/saltstack/pop/pop-create-idem
 Author: Tyler Johnson
 Author-email: tyjohnson@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `pop-create-idem-3.4.0/pop_create_idem.egg-info/SOURCES.txt` & `pop-create-idem-3.4.1/pop_create_idem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pop-create-idem-3.4.0/setup.py` & `pop-create-idem-3.4.1/setup.py`

 * *Files identical despite different names*

