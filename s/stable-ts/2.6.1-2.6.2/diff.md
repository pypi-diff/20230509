# Comparing `tmp/stable-ts-2.6.1.tar.gz` & `tmp/stable-ts-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.6.1.tar", last modified: Tue May  9 04:05:52 2023, max compression
+gzip compressed data, was "stable-ts-2.6.2.tar", last modified: Tue May  9 17:17:28 2023, max compression
```

## Comparing `stable-ts-2.6.1.tar` & `stable-ts-2.6.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 04:05:52.441967 stable-ts-2.6.1/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.6.1/LICENSE
--rw-rw-rw-   0        0        0    11221 2023-05-09 04:05:52.441967 stable-ts-2.6.1/PKG-INFO
--rw-rw-rw-   0        0        0    10925 2023-05-09 03:44:10.000000 stable-ts-2.6.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-09 04:05:52.442968 stable-ts-2.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-09 04:05:52.383279 stable-ts-2.6.1/stable_ts.egg-info/
--rw-rw-rw-   0        0        0    11221 2023-05-09 04:05:52.000000 stable-ts-2.6.1/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-05-09 04:05:52.000000 stable-ts-2.6.1/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 04:05:52.000000 stable-ts-2.6.1/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-05-09 04:05:52.000000 stable-ts-2.6.1/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-05-09 04:05:52.000000 stable-ts-2.6.1/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-09 04:05:52.000000 stable-ts-2.6.1/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-09 04:05:52.439965 stable-ts-2.6.1/stable_whisper/
--rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.6.1/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.6.1/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-05-09 03:45:55.000000 stable-ts-2.6.1/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     7619 2023-04-28 17:05:35.000000 stable-ts-2.6.1/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.6.1/stable_whisper/decode.py
--rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.6.1/stable_whisper/enhancement.py
--rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.6.1/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    37293 2023-05-09 01:32:32.000000 stable-ts-2.6.1/stable_whisper/result.py
--rw-rw-rw-   0        0        0    13549 2023-05-07 22:50:34.000000 stable-ts-2.6.1/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.6.1/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.6.1/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.6.1/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    52980 2023-05-09 03:55:07.000000 stable-ts-2.6.1/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:17:28.511973 stable-ts-2.6.2/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.6.2/LICENSE
+-rw-rw-rw-   0        0        0    11221 2023-05-09 17:17:28.510972 stable-ts-2.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10925 2023-05-09 03:44:10.000000 stable-ts-2.6.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 17:17:28.511973 stable-ts-2.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 17:17:28.454921 stable-ts-2.6.2/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0    11221 2023-05-09 17:17:28.000000 stable-ts-2.6.2/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-09 17:17:28.000000 stable-ts-2.6.2/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 17:17:28.000000 stable-ts-2.6.2/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-05-09 17:17:28.000000 stable-ts-2.6.2/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-05-09 17:17:28.000000 stable-ts-2.6.2/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-09 17:17:28.000000 stable-ts-2.6.2/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 17:17:28.508971 stable-ts-2.6.2/stable_whisper/
+-rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.6.2/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.6.2/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-05-09 17:08:07.000000 stable-ts-2.6.2/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     7619 2023-04-28 17:05:35.000000 stable-ts-2.6.2/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.6.2/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.6.2/stable_whisper/enhancement.py
+-rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.6.2/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    37293 2023-05-09 01:32:32.000000 stable-ts-2.6.2/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    13540 2023-05-09 17:04:10.000000 stable-ts-2.6.2/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.6.2/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.6.2/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.6.2/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    53068 2023-05-09 17:03:34.000000 stable-ts-2.6.2/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.6.1/LICENSE` & `stable-ts-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.1/PKG-INFO` & `stable-ts-2.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.6.1
+Version: 2.6.2
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.6.1/README.md` & `stable-ts-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.1/setup.py` & `stable-ts-2.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.1/stable_ts.egg-info/PKG-INFO` & `stable-ts-2.6.2/stable_ts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.6.1
+Version: 2.6.2
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.6.1/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.6.2/stable_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.1/stable_whisper/audio.py` & `stable-ts-2.6.2/stable_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.1/stable_whisper/decode.py` & `stable-ts-2.6.2/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.1/stable_whisper/enhancement.py` & `stable-ts-2.6.2/stable_whisper/enhancement.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.1/stable_whisper/quantization.py` & `stable-ts-2.6.2/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.1/stable_whisper/result.py` & `stable-ts-2.6.2/stable_whisper/result.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.1/stable_whisper/stabilization.py` & `stable-ts-2.6.2/stable_whisper/stabilization.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         top_values, _ = torch.topk(audio_tensor, k)
         threshold = top_values[-1]
     else:
         threshold = audio_tensor.quantile(0.999, dim=-1)
     if (token_count := round(audio_tensor.shape[-1] / N_SAMPLES_PER_TOKEN)+1) > 2:
         if threshold < 1e-5:
             return torch.zeros(token_count, dtype=audio_tensor.dtype, device=audio_tensor.device)
-        audio_tensor = audio_tensor / min(1., max(threshold * 1.75, .3))
+        audio_tensor = audio_tensor / min(1., threshold * 1.75)
         audio_tensor = F.interpolate(
             audio_tensor[None, None],
             size=token_count,
             mode='linear',
             align_corners=False
         )[0, 0]
         return audio_tensor
```

### Comparing `stable-ts-2.6.1/stable_whisper/text_output.py` & `stable-ts-2.6.2/stable_whisper/text_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.1/stable_whisper/timing.py` & `stable-ts-2.6.2/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.1/stable_whisper/video_output.py` & `stable-ts-2.6.2/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.1/stable_whisper/whisper_word_level.py` & `stable-ts-2.6.2/stable_whisper/whisper_word_level.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,14 +253,15 @@
             audio = resample(audio, input_sr, curr_sr, resampling_method="kaiser_window")
     if only_voice_freq:
         from .audio import voice_freq_filter
         audio = voice_freq_filter(audio, curr_sr)
     sample_padding = int(N_FFT // 2) + 1
     whole_mel = log_mel_spectrogram(audio, padding=sample_padding) if mel_first else None
     tokenizer = None
+    language = None
     initial_prompt_tokens = []
     task = decode_options.get("task", "transcribe")
 
     def detect_language():
         nonlocal tokenizer
         if tokenizer is None:
             if decode_options.get("language", None) is None and model:
@@ -297,14 +298,15 @@
                     if verbose is not None:
                         detected_msg = f"Detected language: {LANGUAGES[decode_options['language']]}"
                         if tqdm_pbar.disable:
                             print(detected_msg)
                         else:
                             tqdm_pbar.write(detected_msg)
 
+            nonlocal language
             language = decode_options["language"]
             tokenizer = get_tokenizer(model.is_multilingual, language=language, task=task)
 
             if word_timestamps and task == "translate":
                 warnings.warn("Word-level timestamps on translations may not be reliable.")
 
             if initial_prompt is not None:
@@ -595,17 +597,18 @@
 
         # final update
         update_pbar()
 
     if model.device != torch.device('cpu'):
         torch.cuda.empty_cache()
 
-    final_result = WhisperResult(dict(text=tokenizer.decode(all_tokens[len(initial_prompt_tokens):]),
+    text = '' if tokenizer is None else tokenizer.decode(all_tokens[len(initial_prompt_tokens):])
+    final_result = WhisperResult(dict(text=text,
                                       segments=all_segments,
-                                      language=tokenizer.language,
+                                      language=language,
                                       time_scale=time_scale))
     if word_timestamps and regroup:
         final_result.regroup()
 
     if time_scale is not None:
         final_result.rescale_time(1 / time_scale)
```

