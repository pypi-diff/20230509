# Comparing `tmp/scargo-1.3.1.tar.gz` & `tmp/scargo-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scargo-1.3.1.tar", last modified: Thu Apr 27 13:01:13 2023, max compression
+gzip compressed data, was "scargo-1.4.0.tar", last modified: Tue May  9 10:25:23 2023, max compression
```

## Comparing `scargo-1.3.1.tar` & `scargo-1.4.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0     4508 2023-04-27 13:01:06.154297 scargo-1.3.1/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     1066 2023-04-27 13:01:06.154297 scargo-1.3.1/LICENSE
--rw-r--r--   0        0        0     2488 2023-04-27 13:01:06.154297 scargo-1.3.1/README.md
--rw-r--r--   0        0        0     2748 2023-04-27 13:01:06.294298 scargo-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      108 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/__init__.py
--rwxr-xr-x   0        0        0    19839 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/certs/certGen.sh
--rwxr-xr-x   0        0        0     4914 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/certs/generateAllCertificates.sh
--rw-r--r--   0        0        0     3967 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/certs/openssl_device_intermediate_ca.cnf
--rw-r--r--   0        0        0     3957 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/certs/openssl_root_ca.cnf
--rw-r--r--   0        0        0      698 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/clang_utils.py
--rw-r--r--   0        0        0    12631 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/cli.py
--rw-r--r--   0        0        0       86 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/__init__.py
--rw-r--r--   0        0        0     1596 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/build.py
--rw-r--r--   0        0        0    12127 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/check.py
--rw-r--r--   0        0        0     1142 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/clean.py
--rw-r--r--   0        0        0     4205 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/debug.py
--rw-r--r--   0        0        0     3402 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/doc.py
--rw-r--r--   0        0        0     3382 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/docker.py
--rw-r--r--   0        0        0     1124 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/fix.py
--rw-r--r--   0        0        0     3226 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/flash.py
--rw-r--r--   0        0        0     6677 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/gen.py
--rw-r--r--   0        0        0     3319 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/new.py
--rw-r--r--   0        0        0     3405 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/publish.py
--rw-r--r--   0        0        0     1688 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/run.py
--rw-r--r--   0        0        0     3347 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/test.py
--rw-r--r--   0        0        0     4432 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/update.py
--rw-r--r--   0        0        0      228 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/commands/version.py
--rw-r--r--   0        0        0     6578 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/config.py
--rw-r--r--   0        0        0     2127 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/config_utils.py
--rw-r--r--   0        0        0     2174 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/docker_utils.py
--rw-r--r--   0        0        0       86 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/file_generators/__init__.py
--rw-r--r--   0        0        0     1658 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/file_generators/base_gen.py
--rw-r--r--   0        0        0      441 2023-04-27 13:01:06.294298 scargo-1.3.1/scargo/file_generators/cicd_gen.py
--rw-r--r--   0        0        0       86 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/clang_parser/__init__.py
--rw-r--r--   0        0        0     2251 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/clang_parser/data_classes.py
--rw-r--r--   0        0        0     1197 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/clang_parser/header_parser.py
--rw-r--r--   0        0        0     2133 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/clang_parser/params_extractor.py
--rw-r--r--   0        0        0      395 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/cmake_gen.py
--rw-r--r--   0        0        0      569 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/conan_gen.py
--rw-r--r--   0        0        0     2468 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/cpp_gen.py
--rw-r--r--   0        0        0     3186 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/docker_gen.py
--rw-r--r--   0        0        0     1115 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/env_gen.py
--rwxr-xr-x   0        0        0     1607 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/mock_gen.py
--rw-r--r--   0        0        0      454 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/readme_gen.py
--rw-r--r--   0        0        0     4834 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/.gitlab-ci.yml.j2
--rw-r--r--   0        0        0     1580 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/CMakeLists.txt.j2
--rw-r--r--   0        0        0     4275 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/README.md.j2
--rw-r--r--   0        0        0     1693 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/conan/conanfile.py.j2
--rw-r--r--   0        0        0     1464 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/conan/conanfiletest.j2
--rw-r--r--   0        0        0      150 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
--rw-r--r--   0        0        0     2423 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
--rw-r--r--   0        0        0      886 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/cpp/cmake-src-x86.j2
--rw-r--r--   0        0        0      181 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/cpp/lib.cpp.j2
--rw-r--r--   0        0        0      213 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/cpp/lib.h.j2
--rw-r--r--   0        0        0      715 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/cpp/main.cpp.j2
--rw-r--r--   0        0        0      159 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/docker/Dockerfile-custom.j2
--rw-r--r--   0        0        0     2067 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
--rw-r--r--   0        0        0      754 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/docker/Dockerfile-stm32.j2
--rw-r--r--   0        0        0       49 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/docker/Dockerfile-x86.j2
--rw-r--r--   0        0        0     2359 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/docker/Dockerfile.j2
--rw-r--r--   0        0        0      158 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/docker/devcontainer.json.j2
--rw-r--r--   0        0        0     1000 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/docker/docker-compose.yaml.j2
--rw-r--r--   0        0        0      287 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/docker/env.txt.j2
--rw-r--r--   0        0        0       22 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/docker/stm32.cfg.j2
--rw-r--r--   0        0        0      294 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/esp32.cmake.j2
--rw-r--r--   0        0        0       39 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/mock/.clang-format
--rw-r--r--   0        0        0      475 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/mock/CMakeLists.txt
--rw-r--r--   0        0        0      594 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/mock/class_interface.h.j2
--rw-r--r--   0        0        0      835 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/mock/class_mock.cpp.j2
--rw-r--r--   0        0        0      697 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/mock/class_mock.h.j2
--rw-r--r--   0        0        0      510 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/project.cmake.j2
--rw-r--r--   0        0        0     2194 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/scargo.toml.j2
--rw-r--r--   0        0        0      802 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/stm32.cmake.j2
--rw-r--r--   0        0        0       91 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
--rw-r--r--   0        0        0      100 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
--rw-r--r--   0        0        0     1079 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
--rw-r--r--   0        0        0       84 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
--rw-r--r--   0        0        0      326 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
--rw-r--r--   0        0        0     1046 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/tests/static_mock/static_mock.h
--rw-r--r--   0        0        0       39 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/ut/.clang-format
--rw-r--r--   0        0        0      575 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/ut/CMakeLists.txt.j2
--rw-r--r--   0        0        0      719 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/ut/ut.cpp.j2
--rw-r--r--   0        0        0      213 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/templates/x86.cmake.j2
--rw-r--r--   0        0        0     1597 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/tests_gen.py
--rw-r--r--   0        0        0      560 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/toml_gen.py
--rw-r--r--   0        0        0     5357 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/file_generators/ut_gen.py
--rw-r--r--   0        0        0      629 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/global_values.py
--rw-r--r--   0        0        0     2044 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/logger.py
--rw-r--r--   0        0        0     1137 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/path_utils.py
--rw-r--r--   0        0        0     2953 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/templates/.clang-format
--rw-r--r--   0        0        0     8780 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/templates/.clang-tidy
--rw-r--r--   0        0        0     2361 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/templates/.gitignore
--rw-r--r--   0        0        0     1066 2023-04-27 13:01:06.298298 scargo-1.3.1/scargo/templates/LICENSE
--rw-r--r--   0        0        0      519 2023-04-27 13:01:06.298298 scargo-1.3.1/setup.cfg
--rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 scargo-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     4508 2023-05-09 10:25:17.600083 scargo-1.4.0/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     1066 2023-05-09 10:25:17.600083 scargo-1.4.0/LICENSE
+-rw-r--r--   0        0        0     2488 2023-05-09 10:25:17.600083 scargo-1.4.0/README.md
+-rw-r--r--   0        0        0     2748 2023-05-09 10:25:17.720082 scargo-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-05-09 10:25:17.720082 scargo-1.4.0/scargo/__init__.py
+-rwxr-xr-x   0        0        0    19839 2023-05-09 10:25:17.720082 scargo-1.4.0/scargo/certs/certGen.sh
+-rwxr-xr-x   0        0        0     4914 2023-05-09 10:25:17.720082 scargo-1.4.0/scargo/certs/generateAllCertificates.sh
+-rw-r--r--   0        0        0     3967 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/certs/openssl_device_intermediate_ca.cnf
+-rw-r--r--   0        0        0     3957 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/certs/openssl_root_ca.cnf
+-rw-r--r--   0        0        0      698 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/clang_utils.py
+-rw-r--r--   0        0        0    12706 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/cli.py
+-rw-r--r--   0        0        0       86 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/build.py
+-rw-r--r--   0        0        0    12212 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/check.py
+-rw-r--r--   0        0        0     1142 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/clean.py
+-rw-r--r--   0        0        0     4343 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/debug.py
+-rw-r--r--   0        0        0     3402 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/doc.py
+-rw-r--r--   0        0        0     3369 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/docker.py
+-rw-r--r--   0        0        0     1124 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/fix.py
+-rw-r--r--   0        0        0     3927 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/flash.py
+-rw-r--r--   0        0        0     6677 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/gen.py
+-rw-r--r--   0        0        0     2857 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/new.py
+-rw-r--r--   0        0        0     3405 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/publish.py
+-rw-r--r--   0        0        0     1688 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/run.py
+-rw-r--r--   0        0        0     3347 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/test.py
+-rw-r--r--   0        0        0     4419 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/update.py
+-rw-r--r--   0        0        0      228 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/commands/version.py
+-rw-r--r--   0        0        0     6707 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/config.py
+-rw-r--r--   0        0        0     2255 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/config_utils.py
+-rw-r--r--   0        0        0     2174 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/docker_utils.py
+-rw-r--r--   0        0        0       86 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/__init__.py
+-rw-r--r--   0        0        0     1658 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/base_gen.py
+-rw-r--r--   0        0        0      441 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/cicd_gen.py
+-rw-r--r--   0        0        0       86 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/clang_parser/__init__.py
+-rw-r--r--   0        0        0     2251 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/clang_parser/data_classes.py
+-rw-r--r--   0        0        0     1197 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/clang_parser/header_parser.py
+-rw-r--r--   0        0        0     2348 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/clang_parser/params_extractor.py
+-rw-r--r--   0        0        0      395 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/cmake_gen.py
+-rw-r--r--   0        0        0      569 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/conan_gen.py
+-rw-r--r--   0        0        0     2468 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/cpp_gen.py
+-rw-r--r--   0        0        0     3186 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/docker_gen.py
+-rw-r--r--   0        0        0     1115 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/env_gen.py
+-rwxr-xr-x   0        0        0     1607 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/mock_gen.py
+-rw-r--r--   0        0        0      454 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/readme_gen.py
+-rw-r--r--   0        0        0     4834 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/.gitlab-ci.yml.j2
+-rw-r--r--   0        0        0     1580 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/CMakeLists.txt.j2
+-rw-r--r--   0        0        0     4275 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/README.md.j2
+-rw-r--r--   0        0        0     1693 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/conan/conanfile.py.j2
+-rw-r--r--   0        0        0     1464 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/conan/conanfiletest.j2
+-rw-r--r--   0        0        0      150 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
+-rw-r--r--   0        0        0     2423 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
+-rw-r--r--   0        0        0      886 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2
+-rw-r--r--   0        0        0      181 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/cpp/lib.cpp.j2
+-rw-r--r--   0        0        0      213 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/cpp/lib.h.j2
+-rw-r--r--   0        0        0      715 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/cpp/main.cpp.j2
+-rw-r--r--   0        0        0      159 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile-custom.j2
+-rw-r--r--   0        0        0     2067 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
+-rw-r--r--   0        0        0      754 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2
+-rw-r--r--   0        0        0       49 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile-x86.j2
+-rw-r--r--   0        0        0     2359 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile.j2
+-rw-r--r--   0        0        0      158 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/devcontainer.json.j2
+-rw-r--r--   0        0        0     1000 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2
+-rw-r--r--   0        0        0      287 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/env.txt.j2
+-rw-r--r--   0        0        0       22 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/docker/stm32.cfg.j2
+-rw-r--r--   0        0        0      294 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/esp32.cmake.j2
+-rw-r--r--   0        0        0       39 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/mock/.clang-format
+-rw-r--r--   0        0        0      475 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/mock/CMakeLists.txt
+-rw-r--r--   0        0        0      594 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/mock/class_interface.h.j2
+-rw-r--r--   0        0        0      835 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/mock/class_mock.cpp.j2
+-rw-r--r--   0        0        0      697 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/mock/class_mock.h.j2
+-rw-r--r--   0        0        0      510 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/project.cmake.j2
+-rw-r--r--   0        0        0     2228 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/scargo.toml.j2
+-rw-r--r--   0        0        0      802 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/stm32.cmake.j2
+-rw-r--r--   0        0        0       91 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
+-rw-r--r--   0        0        0      100 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
+-rw-r--r--   0        0        0     1079 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
+-rw-r--r--   0        0        0       84 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
+-rw-r--r--   0        0        0      326 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
+-rw-r--r--   0        0        0     1046 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/tests/static_mock/static_mock.h
+-rw-r--r--   0        0        0       39 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/ut/.clang-format
+-rw-r--r--   0        0        0      575 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2
+-rw-r--r--   0        0        0      719 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/ut/ut.cpp.j2
+-rw-r--r--   0        0        0      213 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/templates/x86.cmake.j2
+-rw-r--r--   0        0        0     1597 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/tests_gen.py
+-rw-r--r--   0        0        0      550 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/toml_gen.py
+-rw-r--r--   0        0        0     5357 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/file_generators/ut_gen.py
+-rw-r--r--   0        0        0      629 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/global_values.py
+-rw-r--r--   0        0        0     2044 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/logger.py
+-rw-r--r--   0        0        0     1137 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/path_utils.py
+-rw-r--r--   0        0        0     2953 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/templates/.clang-format
+-rw-r--r--   0        0        0     8780 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/templates/.clang-tidy
+-rw-r--r--   0        0        0     2361 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/templates/.gitignore
+-rw-r--r--   0        0        0     1066 2023-05-09 10:25:17.724082 scargo-1.4.0/scargo/templates/LICENSE
+-rw-r--r--   0        0        0      519 2023-05-09 10:25:17.724082 scargo-1.4.0/setup.cfg
+-rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 scargo-1.4.0/PKG-INFO
```

### Comparing `scargo-1.3.1/CODE-OF-CONDUCT.md` & `scargo-1.4.0/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/LICENSE` & `scargo-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/README.md` & `scargo-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/pyproject.toml` & `scargo-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/certs/certGen.sh` & `scargo-1.4.0/scargo/certs/certGen.sh`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/certs/generateAllCertificates.sh` & `scargo-1.4.0/scargo/certs/generateAllCertificates.sh`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/certs/openssl_device_intermediate_ca.cnf` & `scargo-1.4.0/scargo/certs/openssl_device_intermediate_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/certs/openssl_root_ca.cnf` & `scargo-1.4.0/scargo/certs/openssl_root_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/clang_utils.py` & `scargo-1.4.0/scargo/clang_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/cli.py` & `scargo-1.4.0/scargo/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,22 +220,23 @@
     app: bool = Option(False, "--app", help="Flash app only"),
     file_system: bool = Option(False, "--fs", help="Flash filesystem only"),
     flash_profile: str = Option(
         "Debug", "--profile", help="Flash base on previously built profile"
     ),
     port: Optional[str] = Option(
         None,
-        help="port where the target device of the command is connected to, e.g. /dev/ttyUSB0",
+        help="(esp32 only) port where the target device of the command is connected to, e.g. /dev/ttyUSB0",
     ),
+    no_erase: bool = Option(False, help="(stm32 only) Don't erase target memory"),
     base_dir: Optional[Path] = BASE_DIR_OPTION,
 ) -> None:
-    """Flash the target (only available for esp32 for now)."""
+    """Flash the target."""
     if base_dir:
         os.chdir(base_dir)
-    scargo_flash(app, file_system, flash_profile, port)
+    scargo_flash(app, file_system, flash_profile, port, not no_erase)
 
 
 ###############################################################################
 
 
 @cli.command()
 def gen(
```

### Comparing `scargo-1.3.1/scargo/commands/build.py` & `scargo-1.4.0/scargo/commands/build.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,11 +50,14 @@
             ["conan", "install", ".", "-if", build_dir],
             cwd=project_dir,
         )
         subprocess.check_call(
             ["cmake", f"-DCMAKE_BUILD_TYPE={profile}", project_dir],
             cwd=build_dir,
         )
-        subprocess.check_call("cmake --build . --parallel", shell=True, cwd=build_dir)
+        command = ["cmake", "--build", ".", "--parallel"]
+        if config.project.max_build_jobs is not None:
+            command.append(str(config.project.max_build_jobs))
+        subprocess.check_call(command, cwd=build_dir)
     except subprocess.CalledProcessError:
         logger.error("Unable to build exec file")
         sys.exit(1)
```

### Comparing `scargo-1.3.1/scargo/commands/check.py` & `scargo-1.4.0/scargo/commands/check.py`

 * *Files 4% similar despite different names*

```diff
@@ -266,43 +266,50 @@
 
 
 class ClangFormatChecker(CheckerFixer):
     check_name = "clang-format"
     can_fix = True
 
     def check_file(self, file_path: Path) -> CheckResult:
-        cmd = ["clang-format", "--style=file", "--dry-run", "-Werror", str(file_path)]
+        cmd = [
+            "/usr/bin/clang-format",
+            "--style=file",
+            "--dry-run",
+            "-Werror",
+            str(file_path),
+        ]
         try:
             subprocess.check_output(cmd)
         except subprocess.CalledProcessError as e:
             if self._verbose:
                 logger.info(e.output.decode())
             else:
                 logger.warning("clang-format found error in file %s", file_path)
             return CheckResult(1)
         return CheckResult(0)
 
     def fix_file(self, file_path: Path) -> None:
-        subprocess.check_call(["clang-format", "-style=file", "-i", str(file_path)])
+        subprocess.check_call(
+            ["/usr/bin/clang-format", "-style=file", "-i", str(file_path)]
+        )
 
 
 class ClangTidyChecker(CheckerFixer):
     check_name = "clang-tidy"
     build_path = Path("./build/")
 
     def check_file(self, file_path: Path) -> CheckResult:
         cmd = ["clang-tidy", str(file_path)]
         if self._config.project.target.family == "esp32":
             cmd.extend(["-p", str(self.build_path)])
             if not Path(self.build_path, "compile_commands.json").exists():
                 # creates compilation database and runs run-clang-tidy.py on the whole project
                 # (the latter is not needed, but there's no option to suppress it)
-                cmd = ["idf.py", "clang-check"]
                 subprocess.run(
-                    cmd,
+                    ["idf.py", "clang-check"],
                     stdout=subprocess.DEVNULL,
                     stderr=subprocess.DEVNULL,
                     check=False,
                 )
         if file_path.suffix == ".h":
             cmd.extend(["--", "-x", "c++"])
         try:
```

### Comparing `scargo-1.3.1/scargo/commands/clean.py` & `scargo-1.4.0/scargo/commands/clean.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/commands/debug.py` & `scargo-1.4.0/scargo/commands/debug.py`

 * *Files 13% similar despite different names*

```diff
@@ -81,14 +81,16 @@
                 check=True,
             )
         finally:
             openocd.terminate()
 
     def _debug_stm32(self) -> None:
         chip_script = f"target/{self._chip[:7].lower()}x.cfg"
+        if not Path("/usr/share/openocd/scripts", chip_script).exists():
+            chip_script = f"target/{self._chip[:7].lower()}.cfg"
         openocd_args = [
             "-f",
             "interface/stlink-v2-1.cfg",
             "-f",
             chip_script,
             "-f",
             ".devcontainer/stm32.cfg",
```

### Comparing `scargo-1.3.1/scargo/commands/doc.py` & `scargo-1.4.0/scargo/commands/doc.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/commands/docker.py` & `scargo-1.4.0/scargo/commands/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,11 +109,11 @@
     except subprocess.CalledProcessError:
         logger.error("Exec docker fail.")
         sys.exit(1)
 
 
 def _get_docker_path(project_path: Path) -> Path:
     # do not rebuild dockers in the docker
-    if Path(project_path, ".dockerenv").exists():
+    if Path("/.dockerenv").exists():
         logger.error("Cannot used docker command inside the docker container.")
         sys.exit(1)
     return Path(project_path, ".devcontainer")
```

### Comparing `scargo-1.3.1/scargo/commands/fix.py` & `scargo-1.4.0/scargo/commands/fix.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/commands/flash.py` & `scargo-1.4.0/scargo/commands/flash.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,26 +10,33 @@
 from scargo.config_utils import prepare_config
 from scargo.logger import get_logger
 
 logger = get_logger()
 
 
 def scargo_flash(
-    app: bool, fs: bool, flash_profile: str, port: Optional[str] = None
+    app: bool,
+    fs: bool,
+    flash_profile: str,
+    port: Optional[str] = None,
+    erase_memory: bool = True,
 ) -> None:
     config = prepare_config()
     target = config.project.target
 
-    if port and target.family != "esp32":
-        logger.error("--port option is only supported for esp32 projects.")
+    if port and (target.family != "esp32" and target.family != "stm32"):
+        logger.error("--port option is only supported for esp32 and stm32 projects.")
+        sys.exit(1)
+    if not erase_memory and target.family != "stm32":
+        logger.error("--no-erase option is only supported for stm32 projects.")
         sys.exit(1)
     if target.family == "esp32":
         flash_esp32(config, app=app, fs=fs, flash_profile=flash_profile, port=port)
     elif target.family == "stm32":
-        flash_stm32(config, flash_profile)
+        flash_stm32(config, flash_profile, erase_memory, port=port)
     else:
         logger.error("Flash command not supported for this target yet.")
 
 
 def flash_esp32(
     config: Config,
     app: bool,
@@ -41,44 +48,54 @@
     out_dir = project_path / "build" / flash_profile
     target = config.project.target
     command = []
     try:
         if app:
             app_name = config.project.name
             app_path = out_dir / f"{app_name}.bin"
-            command = [
-                "parttool.py",
-                "write_partition",
-                "--partition-name=ota_0",
-                f"--input={app_path}",
-            ]
+            command = ["parttool.py"]
             if port:
                 command.append(f"--port={port}")
-            subprocess.check_call(command, cwd=project_path)
+            command.extend(
+                [
+                    "write_partition",
+                    "--partition-name=ota_0",
+                    f"--input={app_path}",
+                ]
+            )
+            subprocess.check_call(command)
         elif fs:
             fs_path = config.project_root / "build" / "spiffs.bin"
-            command = [
-                "parttool.py",
-                "write_partition",
-                "--partition-name=spiffs",
-                f"--input={fs_path}",
-            ]
+            command = ["parttool.py"]
             if port:
                 command.append(f"--port={port}")
-            subprocess.check_call(command, cwd=project_path)
+            command.extend(
+                [
+                    "write_partition",
+                    "--partition-name=spiffs",
+                    f"--input={fs_path}",
+                ]
+            )
+            subprocess.check_call(command)
         else:
-            command = ["esptool.py", "--chip", target.id, "write_flash", "@flash_args"]
+            command = ["esptool.py"]
             if port:
                 command.append(f"--port={port}")
+            command.extend(["--chip", target.id, "write_flash", "@flash_args"])
             subprocess.check_call(command, cwd=out_dir)
     except subprocess.CalledProcessError:
         logger.error("%s fail", command)
 
 
-def flash_stm32(config: Config, flash_profile: str = "Debug") -> None:
+def flash_stm32(
+    config: Config,
+    flash_profile: str = "Debug",
+    erase_memory: bool = True,
+    port: Optional[str] = None,
+) -> None:
     project_path = config.project_root
     bin_name = config.project.bin_name
     if not bin_name:
         logger.error("No bin_name in config!")
         sys.exit(1)
     bin_name = bin_name.lower()
     bin_path = project_path / "build" / flash_profile / "bin" / f"{bin_name}.bin"
@@ -88,11 +105,19 @@
     if not bin_path.exists():
         logger.error("%s does not exist", bin_path)
         logger.info("Did you run scargo build --profile %s", flash_profile)
     elif not flash_start:
         logger.error("Flash start address not found in lock file")
         logger.info("Define flash-start in scargo.toml under stm32 section")
     else:
-        subprocess.check_call(["st-flash", "erase"])
-        subprocess.check_call(
-            ["st-flash", "--reset", "write", str(bin_path), flash_start]
-        )
+        if erase_memory:
+            command = ["st-flash"]
+            if port:
+                command.append(f"--serial={port}")
+            command.append("erase")
+            subprocess.check_call(command)
+
+        command = ["st-flash", "--reset"]
+        if port:
+            command.append(f"--serial={port}")
+        command.extend(["write", str(bin_path), flash_start])
+        subprocess.check_call(command)
```

### Comparing `scargo-1.3.1/scargo/commands/gen.py` & `scargo-1.4.0/scargo/commands/gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/commands/new.py` & `scargo-1.4.0/scargo/commands/new.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # #
 
 """Create new project"""
 import re
 import subprocess
 import sys
 from pathlib import Path
-from typing import Optional, Tuple
+from typing import Optional
 
 from scargo import __version__
 from scargo.config import Target
 from scargo.config_utils import get_scargo_config_or_exit
 from scargo.file_generators.cpp_gen import generate_cpp
 from scargo.file_generators.toml_gen import generate_toml
 from scargo.global_values import SCARGO_DEFAULT_CONFIG_FILE, SCARGO_DOCKER_ENV
@@ -57,25 +57,22 @@
         project_dir.mkdir()
     except FileExistsError:
         logger.error("Provided project name: %s already exist.", name)
         sys.exit(1)
 
     build_env = get_build_env(create_docker)
 
-    cc, cflags, cxx, cxxflags = get_cc_config(target)
     toml_path = project_dir / SCARGO_DEFAULT_CONFIG_FILE
     generate_toml(
         toml_path,
         project_name=name,
         target=target,
         build_env=build_env,
-        cc=cc,
-        cxx=cxx,
-        cflags=cflags,
-        cxxflags=cxxflags,
+        cflags="-Wall -Wextra",
+        cxxflags="-Wall -Wextra",
         version=__version__,
         docker_image_tag=f"{name.lower()}-dev:1.0",
         lib_name=lib_name,
         bin_name=bin_name,
     )
 
     config = get_scargo_config_or_exit(toml_path)
@@ -87,29 +84,14 @@
     Path(test_dir, "it").mkdir(parents=True)
 
     if git:
         subprocess.check_call("git init -q", shell=True, cwd=project_dir)
         logger.info("Initialized git repo")
 
 
-def get_cc_config(target: Target) -> Tuple[str, str, str, str]:
-    """
-    Get c configuration base on architecture
-
-    :param target: project architecture
-    :return: tuple of string
-    :raises Exception: if architecture not allowed
-    """
-    cflags = "-Wall -Wextra"
-    cxxflags = "-Wall -Wextra"
-    cc = target.cc
-    cxx = target.cxx
-    return cc, cflags, cxx, cxxflags
-
-
 def get_build_env(create_docker: bool) -> str:
     """
     Get build env
     :param bool create_docker: if create docker
     :return: build env
     """
     if create_docker:
```

### Comparing `scargo-1.3.1/scargo/commands/publish.py` & `scargo-1.4.0/scargo/commands/publish.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/commands/run.py` & `scargo-1.4.0/scargo/commands/run.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/commands/test.py` & `scargo-1.4.0/scargo/commands/test.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/commands/update.py` & `scargo-1.4.0/scargo/commands/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     if (
         target.family == "stm32"
         and not Path(config.project_root, "third-party/stm32-cmake").is_dir()
     ):
         subprocess.run("conan source .", shell=True, cwd=project_path, check=True)
 
     if project_config.build_env == SCARGO_DOCKER_ENV:
-        if not Path(project_path, ".dockerenv").exists():
+        if not Path("/.dockerenv").exists():
             if not pull_docker_image(docker_path):
                 scargo_docker_build([], config.project_root)
         else:
             logger.warning("Cannot run docker inside docker")
 
 
 def pull_docker_image(docker_path: Path) -> bool:
```

### Comparing `scargo-1.3.1/scargo/config.py` & `scargo-1.4.0/scargo/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,19 +50,20 @@
             raise ConfigError("No [esp32] section in config")
         return self.esp32
 
     @root_validator
     def validate_special_configs(  # pylint: disable=no-self-argument
         cls, values: Dict[str, Any]
     ) -> Dict[str, Any]:
-        target_id = values["project"].target_id
-        if target_id == "stm32" and not values["stm32"]:
-            raise ConfigError("No [stm32] section in config")
-        if target_id == "esp32" and not values["esp32"]:
-            raise ConfigError("No [esp32] section in config")
+        if "project" in values:
+            target_id = values["project"].target_id
+            if target_id == "stm32" and not values["stm32"]:
+                raise ConfigError("No [stm32] section in config")
+            if target_id == "esp32" and not values["esp32"]:
+                raise ConfigError("No [esp32] section in config")
         return values
 
 
 class ProjectConfig(BaseModel):
     name: str
     version: str
     description: Optional[str]
@@ -72,65 +73,57 @@
     lib_name: Optional[str]
     target_id: str = Field(..., alias="target")
     build_env: str = Field(SCARGO_DEFAULT_BUILD_ENV, alias="build-env")
     docker_file: Path = Field(..., alias="docker-file")
     docker_image_tag: str = Field(..., alias="docker-image-tag")
     in_repo_conan_cache: bool = Field(..., alias="in-repo-conan-cache")
 
-    cc: str
-    cxx: str
+    cc: Optional[str] = None
+    cxx: Optional[str] = None
     cxxstandard: str
 
     cflags: str
     cxxflags: str
 
+    max_build_jobs: Optional[int] = Field(None, alias="max-build-jobs")
+
     cmake_variables: Dict[str, str] = Field(
         default_factory=dict, alias="cmake-variables"
     )
 
     @property
     def target(self) -> "Target":
         return Target.get_target_by_id(self.target_id)
 
+    def get_compiler_warning(self) -> Optional[str]:
+        if (self.cc and not self.target.cc) or (self.cxx and not self.target.cxx):
+            return "Compiler settings are ignored for this target"
+        return None
+
 
 class Target(BaseModel):
     id: str
     family: str
     source_dir: str
-    cc: str
-    cxx: str
+    cc: Optional[str] = None
+    cxx: Optional[str] = None
 
     @classmethod
     def get_target_by_id(cls, target_id: str) -> "Target":
         return TARGETS[target_id]
 
 
-ARM_CC = "arm-none-eabi-gcc"
-ARM_CXX = "arm-none-eabi-g++"
-
 TARGETS = {
     "x86": Target(id="x86", family="x86", source_dir="src", cc="gcc", cxx="g++"),
-    "stm32": Target(
-        id="stm32", family="stm32", source_dir="src", cc=ARM_CC, cxx=ARM_CXX
-    ),
-    "esp32": Target(
-        id="esp32", family="esp32", source_dir="main", cc=ARM_CC, cxx=ARM_CXX
-    ),
-    "esp32s2": Target(
-        id="esp32s2", family="esp32", source_dir="main", cc=ARM_CC, cxx=ARM_CXX
-    ),
-    "esp32s3": Target(
-        id="esp32s3", family="esp32", source_dir="main", cc=ARM_CC, cxx=ARM_CXX
-    ),
-    "esp32c2": Target(
-        id="esp32c2", family="esp32", source_dir="main", cc=ARM_CC, cxx=ARM_CXX
-    ),
-    "esp32c3": Target(
-        id="esp32c3", family="esp32", source_dir="main", cc=ARM_CC, cxx=ARM_CXX
-    ),
+    "stm32": Target(id="stm32", family="stm32", source_dir="src"),
+    "esp32": Target(id="esp32", family="esp32", source_dir="main"),
+    "esp32s2": Target(id="esp32s2", family="esp32", source_dir="main"),
+    "esp32s3": Target(id="esp32s3", family="esp32", source_dir="main"),
+    "esp32c2": Target(id="esp32c2", family="esp32", source_dir="main"),
+    "esp32c3": Target(id="esp32c3", family="esp32", source_dir="main"),
 }
 
 
 # for typer
 ScargoTargets = Enum(  # type: ignore[misc]
     "ScargoTargets", {target.id: target.id for target in TARGETS.values()}
 )
```

### Comparing `scargo-1.3.1/scargo/config_utils.py` & `scargo-1.4.0/scargo/config_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,19 +25,23 @@
         config_file_path = get_config_file_path(SCARGO_LOCK_FILE)
     if config_file_path is None or not config_file_path.exists():
         logger.error("File `%s` does not exist.", SCARGO_LOCK_FILE)
         logger.info("Did you run `scargo update`?")
         sys.exit(1)
 
     try:
-        return parse_config(config_file_path)
+        config = parse_config(config_file_path)
     except ConfigError as e:
         logger.error(e.args[0])
         sys.exit(1)
 
+    if compiler_warning := config.project.get_compiler_warning():
+        logger.warning(compiler_warning)
+    return config
+
 
 def prepare_config(run_in_docker: bool = True) -> Config:
     """
     Prepare configuration file
 
     :return: project configuration
     """
```

### Comparing `scargo-1.3.1/scargo/docker_utils.py` & `scargo-1.4.0/scargo/docker_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/base_gen.py` & `scargo-1.4.0/scargo/file_generators/base_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/clang_parser/data_classes.py` & `scargo-1.4.0/scargo/file_generators/clang_parser/data_classes.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/clang_parser/header_parser.py` & `scargo-1.4.0/scargo/file_generators/clang_parser/header_parser.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/clang_parser/params_extractor.py` & `scargo-1.4.0/scargo/file_generators/clang_parser/params_extractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,35 +12,37 @@
 
 
 def extract_namespaces(cursor: Cursor, filename: str) -> List[NamespaceDescriptor]:
     return [
         NamespaceDescriptor(descendant.spelling)
         for descendant in cursor.walk_preorder()
         if descendant.kind == CursorKind.NAMESPACE
-        and descendant.location.file == filename
+        # remove type ignore after fix is relased:
+        # https://github.com/tgockel/types-clang/issues/10
+        and descendant.location.file.name == filename  # type: ignore[attr-defined]
     ]
 
 
 def extract_classes(cursor: Cursor, filename: str) -> List[ClassDescriptor]:
     return [
         ClassDescriptor(
             cursor.spelling, f"Mock{cursor.spelling}", _extract_cxx_methods(cursor)
         )
         for descendant in cursor.walk_preorder()
         if descendant.kind == CursorKind.CLASS_DECL
-        and descendant.location.file == filename
+        and descendant.location.file.name == filename  # type: ignore[attr-defined]
     ]
 
 
 def extract_includes(cursor: Cursor, filename: str) -> List[IncludeDescriptor]:
     return [
         IncludeDescriptor(descendant.displayname)
         for descendant in cursor.walk_preorder()
         if descendant.kind == CursorKind.INCLUSION_DIRECTIVE
-        and descendant.location.file == filename
+        and descendant.location.file.name == filename  # type: ignore[attr-defined]
     ]
 
 
 def _extract_cxx_methods(cursor: Cursor) -> List[FunctionDescriptor]:
     return [
         _extract_method_params(descendant)
         for descendant in cursor.walk_preorder()
```

### Comparing `scargo-1.3.1/scargo/file_generators/conan_gen.py` & `scargo-1.4.0/scargo/file_generators/conan_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/cpp_gen.py` & `scargo-1.4.0/scargo/file_generators/cpp_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/docker_gen.py` & `scargo-1.4.0/scargo/file_generators/docker_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/env_gen.py` & `scargo-1.4.0/scargo/file_generators/env_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/mock_gen.py` & `scargo-1.4.0/scargo/file_generators/mock_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/.gitlab-ci.yml.j2` & `scargo-1.4.0/scargo/file_generators/templates/.gitlab-ci.yml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/CMakeLists.txt.j2` & `scargo-1.4.0/scargo/file_generators/templates/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/README.md.j2` & `scargo-1.4.0/scargo/file_generators/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/conan/conanfile.py.j2` & `scargo-1.4.0/scargo/file_generators/templates/conan/conanfile.py.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/conan/conanfiletest.j2` & `scargo-1.4.0/scargo/file_generators/templates/conan/conanfiletest.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/cpp/cmake-src-stm32.j2` & `scargo-1.4.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/cpp/cmake-src-x86.j2` & `scargo-1.4.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/cpp/main.cpp.j2` & `scargo-1.4.0/scargo/file_generators/templates/cpp/main.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/docker/Dockerfile-esp32.j2` & `scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/docker/Dockerfile-stm32.j2` & `scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/docker/Dockerfile.j2` & `scargo-1.4.0/scargo/file_generators/templates/docker/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/docker/docker-compose.yaml.j2` & `scargo-1.4.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/mock/class_interface.h.j2` & `scargo-1.4.0/scargo/file_generators/templates/mock/class_interface.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/mock/class_mock.cpp.j2` & `scargo-1.4.0/scargo/file_generators/templates/mock/class_mock.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/mock/class_mock.h.j2` & `scargo-1.4.0/scargo/file_generators/templates/mock/class_mock.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/scargo.toml.j2` & `scargo-1.4.0/scargo/file_generators/templates/scargo.toml.j2`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 [project]
-name = "{{ data.project_name }}"
+name = "{{ project_name }}"
 version = "0.1.0"
 description = "Project description."
 homepage-url = "www.hello-world.com"
 
-{% if data.bin_name %}
-bin_name = "{{ data.bin_name }}"
+{% if bin_name %}
+bin_name = "{{ bin_name }}"
 {% endif %}
-{% if data.lib_name %}
-lib_name = "{{ data.lib_name }}"
+{% if lib_name %}
+lib_name = "{{ lib_name }}"
 {% endif %}
-target = "{{ data.target.id }}"
-build-env = "{{ data.build_env }}"
+target = "{{ target.id }}"
+build-env = "{{ build_env }}"
 docker-file = ".devcontainer/Dockerfile-custom"
-docker-image-tag = "{{ data.docker_image_tag }}"
+docker-image-tag = "{{ docker_image_tag }}"
 
-cc  = "{{ data.cc }}"
-cxx = "{{ data.cxx }}"
+{% if target.cc %}
+cc  = "{{ target.cc }}"
+{% endif %}
+{% if target.cxx %}
+cxx = "{{ target.cxx }}"
+{% endif %}
 cxxstandard = "17"
 
-cflags   = "{{ data.cflags }}"
-cxxflags = "{{ data.cxxflags }}"
+cflags   = "{{ cflags }}"
+cxxflags = "{{ cxxflags }}"
 
 in-repo-conan-cache = false
 
 [profile.Debug]
 cflags   = "-g"
 cxxflags = "-g"
 
@@ -83,30 +87,31 @@
 test = [
     "gtest/cci.20210126"
 ]
 
 [conan.repo]
 # conancenter = "https://center.conan.io"
 
-{% if data.target.family == "esp32" %}
+{% if target.family == "esp32" %}
 [esp32]
 extra_component_dirs=[]
 partitions = [
     "nvs,      data, nvs,     0x9000,  0x4000,",
     "otadata,  data, ota,     0xd000,  0x2000,",
     "phy_init, data, phy,     0xf000,  0x1000,",
     "ota_0,    app,  ota_0,   0x10000, 0x180000,",
     "ota_1,    app,  ota_1,   0x190000,0x180000,",
     "spiffs,   data, spiffs,  0x310000,0x6000,"
 ]
-{% elif data.target.family == "stm32" %}
+{% elif target.family == "stm32" %}
 [stm32]
 chip = "STM32L496AG"
 flash-start = 0x08000000
 {% endif %}
 
 [scargo]
 console-log-level = "INFO"
 file-log-level = "WARNING"
-update-exclude = [
+update-exclude = []
 
-]
+[docker-compose]
+ports = []
```

### Comparing `scargo-1.3.1/scargo/file_generators/templates/stm32.cmake.j2` & `scargo-1.4.0/scargo/file_generators/templates/stm32.cmake.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2` & `scargo-1.4.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/tests/static_mock/static_mock.h` & `scargo-1.4.0/scargo/file_generators/templates/tests/static_mock/static_mock.h`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/ut/CMakeLists.txt.j2` & `scargo-1.4.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/templates/ut/ut.cpp.j2` & `scargo-1.4.0/scargo/file_generators/templates/ut/ut.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/tests_gen.py` & `scargo-1.4.0/scargo/file_generators/tests_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/file_generators/toml_gen.py` & `scargo-1.4.0/scargo/file_generators/toml_gen.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 def generate_toml(output_file_path: Path, **values: Any) -> None:
     """_summary_
 
     Args:
         output_file_path (String): path to the output .env file
         **values (Dict): dict contains all necessary values for toml
     """
-    write_template(output_file_path, "scargo.toml.j2", template_params={"data": values})
+    write_template(output_file_path, "scargo.toml.j2", template_params=values)
```

### Comparing `scargo-1.3.1/scargo/file_generators/ut_gen.py` & `scargo-1.4.0/scargo/file_generators/ut_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/global_values.py` & `scargo-1.4.0/scargo/global_values.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/logger.py` & `scargo-1.4.0/scargo/logger.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/path_utils.py` & `scargo-1.4.0/scargo/path_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/templates/.clang-format` & `scargo-1.4.0/scargo/templates/.clang-format`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/templates/.clang-tidy` & `scargo-1.4.0/scargo/templates/.clang-tidy`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/templates/.gitignore` & `scargo-1.4.0/scargo/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/scargo/templates/LICENSE` & `scargo-1.4.0/scargo/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/setup.cfg` & `scargo-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `scargo-1.3.1/PKG-INFO` & `scargo-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scargo
-Version: 1.3.1
+Version: 1.4.0
 Summary: C/C++ package and software development life cycle manager inspired by RUST cargo idea.
 Keywords: scargo,Package manager,C++
 Author-email: "Spyrosoft Solutions S.A." <aak@spyro-soft.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

