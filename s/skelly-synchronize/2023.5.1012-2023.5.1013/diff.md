# Comparing `tmp/skelly_synchronize-2023.5.1012.tar.gz` & `tmp/skelly_synchronize-2023.5.1013.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skelly_synchronize-2023.5.1012.tar", last modified: Mon May  8 17:01:08 2023, max compression
+gzip compressed data, was "skelly_synchronize-2023.5.1013.tar", last modified: Tue May  9 20:19:47 2023, max compression
```

## Comparing `skelly_synchronize-2023.5.1012.tar` & `skelly_synchronize-2023.5.1013.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0       65 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/.gitattributes
--rw-r--r--   0        0        0      146 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/.github/workflows/lint-with-black.yml
--rw-r--r--   0        0        0     1087 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     1025 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/.github/workflows/python-testing.yml
--rw-r--r--   0        0        0     2783 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/.gitignore
--rw-r--r--   0        0        0    34523 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/LICENSE
--rw-r--r--   0        0        0     3030 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/README.md
--rw-r--r--   0        0        0     1608 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/pyproject.toml
--rw-r--r--   0        0        0      123 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/requirements.txt
--rw-r--r--   0        0        0       50 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/setup.py
--rw-r--r--   0        0        0     1056 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/__init__.py
--rw-r--r--   0        0        0      333 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/__main__.py
--rw-r--r--   0        0        0     1965 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/core_processes/audio_utilities.py
--rw-r--r--   0        0        0     2758 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/core_processes/correlation_functions.py
--rw-r--r--   0        0        0      821 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/core_processes/debug_output.py
--rw-r--r--   0        0        0     1557 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
--rw-r--r--   0        0        0     2699 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
--rw-r--r--   0        0        0     4510 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/core_processes/video_functions/video_utilities.py
--rw-r--r--   0        0        0     1821 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/gui/skelly_synchronize_gui.py
--rw-r--r--   0        0        0      420 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/gui/widgets/run_button_widget.py
--rw-r--r--   0        0        0     4763 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/skelly_synchronize.py
--rw-r--r--   0        0        0        0 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/system/__init__.py
--rw-r--r--   0        0        0     1479 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/system/default_paths.py
--rw-r--r--   0        0        0     1402 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/system/logging_configuration.py
--rw-r--r--   0        0        0      323 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/system/paths_and_file_names.py
--rw-r--r--   0        0        0     1085 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/tests/conftest.py
--rw-r--r--   0        0        0      656 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/tests/test_normalize_lag_dict.py
--rw-r--r--   0        0        0      847 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/tests/test_trim_single_video_deffcode.py
--rw-r--r--   0        0        0      577 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
--rw-r--r--   0        0        0      262 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
--rw-r--r--   0        0        0     1263 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
--rw-r--r--   0        0        0     1061 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/tests/utilities/load_sample_data.py
--rw-r--r--   0        0        0     2048 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
--rw-r--r--   0        0        0     1340 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/utils/get_video_files.py
--rw-r--r--   0        0        0     1569 2023-05-08 17:01:02.667818 skelly_synchronize-2023.5.1012/skelly_synchronize/utils/path_handling_utilities.py
--rw-r--r--   0        0        0     3917 1970-01-01 00:00:00.000000 skelly_synchronize-2023.5.1012/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-05-09 20:19:40.841418 skelly_synchronize-2023.5.1013/.gitattributes
+-rw-r--r--   0        0        0      146 2023-05-09 20:19:40.841418 skelly_synchronize-2023.5.1013/.github/workflows/lint-with-black.yml
+-rw-r--r--   0        0        0     1087 2023-05-09 20:19:40.841418 skelly_synchronize-2023.5.1013/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     1025 2023-05-09 20:19:40.841418 skelly_synchronize-2023.5.1013/.github/workflows/python-testing.yml
+-rw-r--r--   0        0        0     2783 2023-05-09 20:19:40.841418 skelly_synchronize-2023.5.1013/.gitignore
+-rw-r--r--   0        0        0    34523 2023-05-09 20:19:40.841418 skelly_synchronize-2023.5.1013/LICENSE
+-rw-r--r--   0        0        0     3030 2023-05-09 20:19:40.841418 skelly_synchronize-2023.5.1013/README.md
+-rw-r--r--   0        0        0     1608 2023-05-09 20:19:40.841418 skelly_synchronize-2023.5.1013/pyproject.toml
+-rw-r--r--   0        0        0      123 2023-05-09 20:19:40.841418 skelly_synchronize-2023.5.1013/requirements.txt
+-rw-r--r--   0        0        0       50 2023-05-09 20:19:40.841418 skelly_synchronize-2023.5.1013/setup.py
+-rw-r--r--   0        0        0     1056 2023-05-09 20:19:40.841418 skelly_synchronize-2023.5.1013/skelly_synchronize/__init__.py
+-rw-r--r--   0        0        0      333 2023-05-09 20:19:40.841418 skelly_synchronize-2023.5.1013/skelly_synchronize/__main__.py
+-rw-r--r--   0        0        0     2192 2023-05-09 20:19:40.841418 skelly_synchronize-2023.5.1013/skelly_synchronize/core_processes/audio_utilities.py
+-rw-r--r--   0        0        0     2758 2023-05-09 20:19:40.841418 skelly_synchronize-2023.5.1013/skelly_synchronize/core_processes/correlation_functions.py
+-rw-r--r--   0        0        0      821 2023-05-09 20:19:40.841418 skelly_synchronize-2023.5.1013/skelly_synchronize/core_processes/debug_output.py
+-rw-r--r--   0        0        0     1557 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
+-rw-r--r--   0        0        0     2699 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
+-rw-r--r--   0        0        0     4510 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/core_processes/video_functions/video_utilities.py
+-rw-r--r--   0        0        0     1821 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/gui/skelly_synchronize_gui.py
+-rw-r--r--   0        0        0      420 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/gui/widgets/run_button_widget.py
+-rw-r--r--   0        0        0     4763 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/skelly_synchronize.py
+-rw-r--r--   0        0        0        0 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/system/__init__.py
+-rw-r--r--   0        0        0     1479 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/system/default_paths.py
+-rw-r--r--   0        0        0     1402 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/system/logging_configuration.py
+-rw-r--r--   0        0        0      323 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/system/paths_and_file_names.py
+-rw-r--r--   0        0        0     1085 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/tests/conftest.py
+-rw-r--r--   0        0        0      656 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/tests/test_normalize_lag_dict.py
+-rw-r--r--   0        0        0      847 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/tests/test_trim_single_video_deffcode.py
+-rw-r--r--   0        0        0      577 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
+-rw-r--r--   0        0        0      262 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
+-rw-r--r--   0        0        0     1263 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0     1061 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/tests/utilities/load_sample_data.py
+-rw-r--r--   0        0        0     2048 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
+-rw-r--r--   0        0        0     1340 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/utils/get_video_files.py
+-rw-r--r--   0        0        0     1569 2023-05-09 20:19:40.845419 skelly_synchronize-2023.5.1013/skelly_synchronize/utils/path_handling_utilities.py
+-rw-r--r--   0        0        0     3917 1970-01-01 00:00:00.000000 skelly_synchronize-2023.5.1013/PKG-INFO
```

### Comparing `skelly_synchronize-2023.5.1012/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skelly_synchronize-2023.5.1013/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/.github/workflows/python-testing.yml` & `skelly_synchronize-2023.5.1013/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/.gitignore` & `skelly_synchronize-2023.5.1013/.gitignore`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/LICENSE` & `skelly_synchronize-2023.5.1013/LICENSE`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/README.md` & `skelly_synchronize-2023.5.1013/README.md`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/pyproject.toml` & `skelly_synchronize-2023.5.1013/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver] #bump the version by entering `bumpver update` in the terminal
-current_version = "v2023.05.1012"
+current_version = "v2023.05.1013"
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/__init__.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for basic_template_repo."""
 
 __package_name__ = "skelly_synchronize"
-__version__ = "v2023.05.1012"
+__version__ = "v2023.05.1013"
 
 __author__ = """Philip Queen"""
 __email__ = "info@freemocap.org"
 __repo_owner_github_user_name__ = "freemocap"
 __repo_url__ = (
     f"https://github.com/{__repo_owner_github_user_name__}/{__package_name__}/"
 )
```

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/core_processes/audio_utilities.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/core_processes/audio_utilities.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,18 +34,21 @@
             file_pathstring=video_dict["video pathstring"],
             file_name=video_dict["camera name"],
             output_folder_path=audio_folder_path,
             output_extension=audio_extension,
         )
 
         audio_name = video_dict["camera name"] + "." + audio_extension
+        audio_file_path = audio_folder_path / audio_name
 
-        audio_signal, sample_rate = librosa.load(
-            path=audio_folder_path / audio_name, sr=None
-        )
+        if not audio_file_path.is_file():
+            logging.error("Error loading audio file, verify video has audio track")
+            raise FileNotFoundError(f"Audio file not found: {audio_file_path}")
+
+        audio_signal, sample_rate = librosa.load(path=audio_file_path, sr=None)
 
         audio_duration = librosa.get_duration(y=audio_signal, sr=sample_rate)
         logging.info(f"audio file {audio_name} is {audio_duration} seconds long")
         audio_signal_dict[audio_name] = {
             "audio file": audio_signal,
             "sample rate": sample_rate,
             "camera name": video_dict["camera name"],
```

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/core_processes/correlation_functions.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/core_processes/correlation_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/core_processes/debug_output.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/core_processes/debug_output.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/core_processes/video_functions/deffcode_functions.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/core_processes/video_functions/deffcode_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/core_processes/video_functions/video_utilities.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/core_processes/video_functions/video_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/gui/skelly_synchronize_gui.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/gui/skelly_synchronize_gui.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/skelly_synchronize.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/skelly_synchronize.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/system/default_paths.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/system/default_paths.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/system/logging_configuration.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/system/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/tests/conftest.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/tests/test_normalize_lag_dict.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/tests/test_normalize_lag_dict.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/tests/test_trim_single_video_deffcode.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/tests/test_trim_single_video_deffcode.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/tests/utilities/check_list_values_are_equal.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/tests/utilities/check_list_values_are_equal.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/tests/utilities/load_sample_data.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/tests/utilities/load_sample_data.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/utils/get_video_files.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/utils/get_video_files.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/skelly_synchronize/utils/path_handling_utilities.py` & `skelly_synchronize-2023.5.1013/skelly_synchronize/utils/path_handling_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1012/PKG-INFO` & `skelly_synchronize-2023.5.1013/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skelly_synchronize
-Version: 2023.5.1012
+Version: 2023.5.1013
 Summary: Basic template of a python repository
 Keywords: basic,template,python,repository
 Author-email: skelly_synchronize <info@freemocap.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
```

