# Comparing `tmp/stable-ts-2.6.0.tar.gz` & `tmp/stable-ts-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.6.0.tar", last modified: Mon May  8 03:27:48 2023, max compression
+gzip compressed data, was "stable-ts-2.6.1.tar", last modified: Tue May  9 04:05:52 2023, max compression
```

## Comparing `stable-ts-2.6.0.tar` & `stable-ts-2.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 03:27:48.099213 stable-ts-2.6.0/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.6.0/LICENSE
--rw-rw-rw-   0        0        0     6890 2023-05-08 03:27:48.098212 stable-ts-2.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     6594 2023-04-04 01:04:16.000000 stable-ts-2.6.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 03:27:48.099213 stable-ts-2.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 03:27:48.055173 stable-ts-2.6.0/stable_ts.egg-info/
--rw-rw-rw-   0        0        0     6890 2023-05-08 03:27:47.000000 stable-ts-2.6.0/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-05-08 03:27:47.000000 stable-ts-2.6.0/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 03:27:47.000000 stable-ts-2.6.0/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-05-08 03:27:47.000000 stable-ts-2.6.0/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-05-08 03:27:47.000000 stable-ts-2.6.0/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-08 03:27:47.000000 stable-ts-2.6.0/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 03:27:48.096219 stable-ts-2.6.0/stable_whisper/
--rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.6.0/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.6.0/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-05-07 23:07:54.000000 stable-ts-2.6.0/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     7619 2023-04-28 17:05:35.000000 stable-ts-2.6.0/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.6.0/stable_whisper/decode.py
--rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.6.0/stable_whisper/enhancement.py
--rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.6.0/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    34883 2023-05-06 20:00:11.000000 stable-ts-2.6.0/stable_whisper/result.py
--rw-rw-rw-   0        0        0    13549 2023-05-07 22:50:34.000000 stable-ts-2.6.0/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.6.0/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.6.0/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.6.0/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    52677 2023-05-08 03:08:18.000000 stable-ts-2.6.0/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-05-09 04:05:52.441967 stable-ts-2.6.1/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.6.1/LICENSE
+-rw-rw-rw-   0        0        0    11221 2023-05-09 04:05:52.441967 stable-ts-2.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10925 2023-05-09 03:44:10.000000 stable-ts-2.6.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 04:05:52.442968 stable-ts-2.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 04:05:52.383279 stable-ts-2.6.1/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0    11221 2023-05-09 04:05:52.000000 stable-ts-2.6.1/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-09 04:05:52.000000 stable-ts-2.6.1/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 04:05:52.000000 stable-ts-2.6.1/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-05-09 04:05:52.000000 stable-ts-2.6.1/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-05-09 04:05:52.000000 stable-ts-2.6.1/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-09 04:05:52.000000 stable-ts-2.6.1/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 04:05:52.439965 stable-ts-2.6.1/stable_whisper/
+-rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.6.1/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.6.1/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-05-09 03:45:55.000000 stable-ts-2.6.1/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     7619 2023-04-28 17:05:35.000000 stable-ts-2.6.1/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.6.1/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.6.1/stable_whisper/enhancement.py
+-rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.6.1/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    37293 2023-05-09 01:32:32.000000 stable-ts-2.6.1/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    13549 2023-05-07 22:50:34.000000 stable-ts-2.6.1/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.6.1/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.6.1/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.6.1/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    52980 2023-05-09 03:55:07.000000 stable-ts-2.6.1/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.6.0/LICENSE` & `stable-ts-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.0/setup.py` & `stable-ts-2.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.0/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.6.1/stable_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.0/stable_whisper/audio.py` & `stable-ts-2.6.1/stable_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.0/stable_whisper/decode.py` & `stable-ts-2.6.1/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.0/stable_whisper/enhancement.py` & `stable-ts-2.6.1/stable_whisper/enhancement.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.0/stable_whisper/quantization.py` & `stable-ts-2.6.1/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.0/stable_whisper/result.py` & `stable-ts-2.6.1/stable_whisper/result.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,38 @@
 from .stabilization import suppress_silence
 from .text_output import *
 
 
 __all__ = ['WhisperResult', 'Segment']
 
 
+def _combine_attr(obj: object, other_obj: object, attr: str):
+    if (val := getattr(obj, attr)) is not None:
+        other_val = getattr(other_obj, attr)
+        if isinstance(val, list):
+            if other_val is None:
+                setattr(obj, attr, None)
+            else:
+                val.extend(other_val)
+        else:
+            new_val = None if other_val is None else ((val + other_val) / 2)
+            setattr(obj, attr, new_val)
+
+
+def _increment_attr(obj: object, attr: str, val: Union[int, float]):
+    if (curr_val := getattr(obj, attr, None)) is not None:
+        setattr(obj, attr, curr_val + val)
+
+
 @dataclass
 class WordTiming:
     word: str
     start: float
     end: float
-    probability: float
+    probability: float = None
     tokens: List[int] = None
     left_locked: bool = False
     right_locked: bool = False
 
     def __len__(self):
         return len(self.word)
 
@@ -30,18 +48,18 @@
         assert self.start <= other.start or self.end <= other.end
 
         self_copy = deepcopy(self)
 
         self_copy.start = min(self_copy.start, other.start)
         self_copy.end = max(other.end, self_copy.end)
         self_copy.word += other.word
-        self_copy.probability = (other.probability + self_copy.probability) / 2
-        self_copy.tokens.extend(other.tokens)
         self_copy.left_locked = self_copy.left_locked or other.left_locked
         self_copy.right_locked = self_copy.right_locked or other.right_locked
+        _combine_attr(self_copy, other, 'probability')
+        _combine_attr(self_copy, other, 'tokens')
 
         return self_copy
 
     @property
     def duration(self):
         return self.end - self.start
 
@@ -79,38 +97,39 @@
     def rescale_time(self, scale_factor: float):
         self.start = round(self.start * scale_factor, 3)
         self.end = round(self.end * scale_factor, 3)
 
 
 @dataclass
 class Segment:
-    seek: float
     start: float
     end: float
     text: str
-    tokens: List[int]
-    temperature: float
-    avg_logprob: float
-    compression_ratio: float
-    no_speech_prob: float
-    id: int = None
+    seek: float = None
+    tokens: List[int] = None
+    temperature: float = None
+    avg_logprob: float = None
+    compression_ratio: float = None
+    no_speech_prob: float = None
     words: Union[List[WordTiming], List[dict]] = None
     ori_has_words: bool = None
+    id: int = None
 
     @property
     def has_words(self):
         return bool(self.words)
 
     @property
     def duration(self):
         return self.end - self.start
 
     def word_count(self):
         if self.has_words:
             return len(self.words)
+        return -1
 
     def char_count(self):
         if self.has_words:
             return sum(len(w) for w in self.words)
         return len(self.text)
 
     def __post_init__(self):
@@ -124,48 +143,54 @@
         assert self.start <= other.start or self.end <= other.end
 
         self_copy = deepcopy(self)
 
         self_copy.start = min(self_copy.start, other.start)
         self_copy.end = max(other.end, self_copy.end)
         self_copy.text += other.text
-        self_copy.tokens.extend(other.tokens)
-        if self_copy.has_words:
-            self_copy.words.extend(other.words)
 
-        self_copy.temperature = (other.temperature + self_copy.temperature) / 2
-        self_copy.avg_logprob = (other.avg_logprob + self_copy.avg_logprob) / 2
-        self_copy.compression_ratio = (other.compression_ratio + self_copy.compression_ratio) / 2
-        self_copy.no_speech_prob = (other.no_speech_prob + self_copy.no_speech_prob) / 2
+        _combine_attr(self_copy, other, 'tokens')
+        _combine_attr(self_copy, other, 'temperature')
+        _combine_attr(self_copy, other, 'avg_logprob')
+        _combine_attr(self_copy, other, 'compression_ratio')
+        _combine_attr(self_copy, other, 'no_speech_prob')
+        if self_copy.has_words:
+            if other.has_words:
+                self_copy.words.extend(other.words)
+            else:
+                self_copy.words = None
 
         return self_copy
 
+    def _word_operations(self, operation: str, *args, **kwargs):
+        if self.has_words:
+            for w in self.words:
+                getattr(w, operation)(*args, **kwargs)
+
     def offset_time(self, offset_seconds: float):
-        self.seek = self.seek + offset_seconds
         self.start = self.start + offset_seconds
         self.end = self.end + offset_seconds
-        if self.has_words:
-            for w in self.words:
-                w.offset_time(offset_seconds)
+        _increment_attr(self, 'seek', offset_seconds)
+        self._word_operations('offset_time', offset_seconds)
 
     def add_words(self, index0: int, index1: int, inplace: bool = False):
-        new_word = self.words[index0] + self.words[index1]
-        if inplace:
-            i0, i1 = sorted([index0, index1])
-            self.words[i0] = new_word
-            del self.words[i1]
-        return new_word
+        if self.has_words:
+            new_word = self.words[index0] + self.words[index1]
+            if inplace:
+                i0, i1 = sorted([index0, index1])
+                self.words[i0] = new_word
+                del self.words[i1]
+            return new_word
 
     def rescale_time(self, scale_factor: float):
-        self.seek = round(self.seek * scale_factor, 3)
         self.start = round(self.start * scale_factor, 3)
         self.end = round(self.end * scale_factor, 3)
-        if self.has_words:
-            for w in self.words:
-                w.rescale_time(scale_factor)
+        if self.seek is not None:
+            self.seek = round(self.seek * scale_factor, 3)
+        self._word_operations('rescale_time', scale_factor)
         self.update_seg_with_words()
 
     def apply_min_dur(self, min_dur: float, inplace: bool = False):
         """
         Any duration is less than [min_dur] will be merged with adjacent word.
         """
         segment = self if inplace else deepcopy(self)
@@ -284,25 +309,26 @@
             self.words[-1].lock_right()
 
     def lock_both(self):
         self.lock_left()
         self.lock_right()
 
     def unlock_all_words(self):
-        if self.has_words:
-            for w in self.words:
-                w.unlock_both()
+        self._word_operations('unlock_both')
 
     def update_seg_with_words(self):
         if self.has_words:
             self.start = self.words[0].start
             self.end = self.words[-1].end
-            if self.words[0].tokens:
-                self.tokens = [t for w in self.words for t in w.tokens]
             self.text = ''.join(w.word for w in self.words)
+            self.tokens = (
+                None
+                if any(w.tokens is None for w in self.words) else
+                [t for w in self.words for t in w.tokens]
+            )
 
     def suppress_silence(self,
                          silent_starts: np.ndarray,
                          silent_ends: np.ndarray,
                          min_word_dur: float = 0.1,
                          word_level: bool = True):
         if self.has_words:
@@ -397,23 +423,54 @@
             seg_copies.append(c)
             prev_i = i
         return seg_copies
 
 
 class WhisperResult:
 
-    def __init__(self, result: (str, dict)):
-        if isinstance(result, str):
-            self.path = result
-            result = load_result(self.path)
+    def __init__(self, result: Union[str, dict, list]):
+        result, self.path = self._standardize_result(result)
         self.ori_dict = result.get('ori_dict') or result
         self.language = self.ori_dict.get('language')
-        segments = self.ori_dict.get('segments')
+        segments = deepcopy(result.get('segments', self.ori_dict.get('segments')))
         self.segments: List[Segment] = [Segment(**s) for s in segments] if segments else []
         self.remove_no_word_segments()
+        self.update_all_segs_with_words()
+
+    @staticmethod
+    def _standardize_result(result: Union[str, dict, list]):
+        path = None
+        if isinstance(result, str):
+            path = result
+            result = load_result(path)
+        if isinstance(result, list):
+            if isinstance(result[0], list):
+                if not isinstance(result[0][0], dict):
+                    raise NotImplementedError(f'Got list of list of {type(result[0])} but expects list of list of dict')
+                result = dict(
+                    segments=[
+                        dict(
+                            start=words[0]['start'],
+                            end=words[-1]['end'],
+                            text=''.join(w['word'] for w in words),
+                            words=words
+                        )
+                        for words in result
+                    ]
+                )
+
+            elif isinstance(result[0], dict):
+                result = dict(segments=result)
+            else:
+                raise NotImplementedError(f'Got list of {type(result[0])} but expects list of list/dict')
+        return result, path
+
+    def update_all_segs_with_words(self):
+        for seg in self.segments:
+            seg.update_seg_with_words()
 
     def add_segments(self, index0: int, index1: int, inplace: bool = False, lock: bool = False):
         new_seg = self.segments[index0] + self.segments[index1]
         new_seg.update_seg_with_words()
         if lock and self.segments[index0].has_words:
             lock_idx = len(self.segments[index0].words)
             new_seg.words[lock_idx - 1].lock_right()
@@ -787,14 +844,18 @@
 
     def unlock_all_segments(self):
         for s in self.segments:
             s.unlock_all_words()
         return self
 
     def reset(self):
+        """
+        Restore all values to that in `ori_dict` which is the state at initialization
+        or the state store in the `ori_dict` key of the dictionary that initialized this instance.
+        """
         self.language = self.ori_dict.get('language')
         segments = self.ori_dict.get('segments')
         self.segments: List[Segment] = [Segment(**s) for s in segments] if segments else []
 
     to_srt_vtt = result_to_srt_vtt
     to_ass = result_to_ass
     to_tsv = result_to_tsv
```

### Comparing `stable-ts-2.6.0/stable_whisper/stabilization.py` & `stable-ts-2.6.1/stable_whisper/stabilization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.0/stable_whisper/text_output.py` & `stable-ts-2.6.1/stable_whisper/text_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.0/stable_whisper/timing.py` & `stable-ts-2.6.1/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.0/stable_whisper/video_output.py` & `stable-ts-2.6.1/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.6.0/stable_whisper/whisper_word_level.py` & `stable-ts-2.6.1/stable_whisper/whisper_word_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -824,14 +824,16 @@
                         help="whether to reverse the order of words for each segment of text output")
 
     # ass output
     parser.add_argument('--font', type=str, default='Arial',
                         help="word font for ASS output(s)")
     parser.add_argument('--font_size', type=int, default=48,
                         help="word font size for ASS output(s)")
+    parser.add_argument('--karaoke', type=str2bool, default=False,
+                        help="whether to use progressive filling highlights for karaoke effect (only for ASS outputs)")
 
     parser.add_argument("--temperature", type=float, default=0,
                         help="temperature to use for sampling")
     parser.add_argument("--best_of", type=optional_int,
                         help="number of candidates when sampling with non-zero temperature")
     parser.add_argument("--beam_size", type=optional_int,
                         help="number of beams in beam search, only applicable when temperature is zero")
@@ -910,14 +912,15 @@
                                   f'Got {len(demucs_outputs)} and {len(inputs)}')
 
     strip: bool = args.pop('strip')
 
     segment_level: bool = args.pop('segment_level')
     word_level: bool = args.pop('word_level')
     tag: List[str] = args.pop('tag')
+    karaoke: bool = args.pop('karaoke')
     if tag:
         assert len(tag) == 2, f'[tag] must be a pair of str but got {tag}'
 
     font: str = args.pop('font')
     font_size: int = args.pop('font_size')
 
     def make_parent(filepath: str):
@@ -999,14 +1002,15 @@
             print(f'{k}: {v}')
         print(f'use_demucs: {use_demucs}')
         print(f'\nArguments for Output(s)',
               f'\noverwrite: {overwrite}\n'
               f'segment_level: {segment_level}\n'
               f'word_level: {word_level}\n'
               f'tag: {tag}\n'
+              f'karaoke: {karaoke}\n'
               f'strip: {strip}\n'
               f'regroup: {regroup}\n'
               f'max_chars: {max_chars}\n'
               f'max_words: {max_words}\n'
               f'reverse_text: {reverse_text}\n'
               f'\nArguments for ASS Output',
               f'\nfont: {font}\n'
@@ -1099,14 +1103,15 @@
             )
         else:
             result.to_ass(
                 filepath=output_path,
                 segment_level=segment_level,
                 word_level=word_level,
                 tag=tag,
+                karaoke=karaoke,
                 font=font,
                 font_size=font_size,
                 strip=strip,
                 reverse_text=reverse_text
             )
```

