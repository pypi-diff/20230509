# Comparing `tmp/dnstwist-20230413.tar.gz` & `tmp/dnstwist-20230509.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnstwist-20230413.tar", last modified: Thu Apr 13 07:31:33 2023, max compression
+gzip compressed data, was "dnstwist-20230509.tar", last modified: Tue May  9 16:44:57 2023, max compression
```

## Comparing `dnstwist-20230413.tar` & `dnstwist-20230509.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 mulikowski  (1000) mulikowski  (1000)        0 2023-04-13 07:31:33.392742 dnstwist-20230413/
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)      561 2023-04-13 07:31:33.392742 dnstwist-20230413/PKG-INFO
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)     9422 2023-04-02 12:37:37.000000 dnstwist-20230413/README.md
-drwxrwxr-x   0 mulikowski  (1000) mulikowski  (1000)        0 2023-04-13 07:31:33.392742 dnstwist-20230413/dnstwist.egg-info/
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)      561 2023-04-13 07:31:32.000000 dnstwist-20230413/dnstwist.egg-info/PKG-INFO
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)      224 2023-04-13 07:31:32.000000 dnstwist-20230413/dnstwist.egg-info/SOURCES.txt
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)        1 2023-04-13 07:31:32.000000 dnstwist-20230413/dnstwist.egg-info/dependency_links.txt
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)       43 2023-04-13 07:31:32.000000 dnstwist-20230413/dnstwist.egg-info/entry_points.txt
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)      104 2023-04-13 07:31:32.000000 dnstwist-20230413/dnstwist.egg-info/requires.txt
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)        9 2023-04-13 07:31:32.000000 dnstwist-20230413/dnstwist.egg-info/top_level.txt
--rwxrwxr-x   0 mulikowski  (1000) mulikowski  (1000)    43475 2023-04-13 07:31:22.000000 dnstwist-20230413/dnstwist.py
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)       38 2023-04-13 07:31:33.392742 dnstwist-20230413/setup.cfg
--rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)     1163 2023-03-02 11:24:31.000000 dnstwist-20230413/setup.py
+drwxrwxr-x   0 mulikowski  (1000) mulikowski  (1000)        0 2023-05-09 16:44:57.429918 dnstwist-20230509/
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)      561 2023-05-09 16:44:57.429918 dnstwist-20230509/PKG-INFO
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)     9572 2023-05-09 16:19:09.000000 dnstwist-20230509/README.md
+drwxrwxr-x   0 mulikowski  (1000) mulikowski  (1000)        0 2023-05-09 16:44:57.429918 dnstwist-20230509/dnstwist.egg-info/
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)      561 2023-05-09 16:44:57.000000 dnstwist-20230509/dnstwist.egg-info/PKG-INFO
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)      224 2023-05-09 16:44:57.000000 dnstwist-20230509/dnstwist.egg-info/SOURCES.txt
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)        1 2023-05-09 16:44:57.000000 dnstwist-20230509/dnstwist.egg-info/dependency_links.txt
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)       43 2023-05-09 16:44:57.000000 dnstwist-20230509/dnstwist.egg-info/entry_points.txt
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)      104 2023-05-09 16:44:57.000000 dnstwist-20230509/dnstwist.egg-info/requires.txt
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)        9 2023-05-09 16:44:57.000000 dnstwist-20230509/dnstwist.egg-info/top_level.txt
+-rwxrwxr-x   0 mulikowski  (1000) mulikowski  (1000)    46264 2023-05-09 16:36:51.000000 dnstwist-20230509/dnstwist.py
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)       38 2023-05-09 16:44:57.429918 dnstwist-20230509/setup.cfg
+-rw-rw-r--   0 mulikowski  (1000) mulikowski  (1000)     1163 2023-03-02 11:24:31.000000 dnstwist-20230509/setup.py
```

### Comparing `dnstwist-20230413/PKG-INFO` & `dnstwist-20230509/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnstwist
-Version: 20230413
+Version: 20230509
 Summary: Domain name permutation engine for detecting homograph phishing attacks, typo squatting, and brand impersonation
 Home-page: https://github.com/elceef/dnstwist
 Author: Marcin Ulikowski
 Author-email: marcin@ulikowski.pl
 License: ASL 2.0
 Description: Project website: https://github.com/elceef/dnstwist
 Platform: UNKNOWN
```

### Comparing `dnstwist-20230413/README.md` & `dnstwist-20230509/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 See what sort of trouble users can get in trying to type your domain name.
 Find lookalike domains that adversaries can use to attack you. Can detect
 typosquatters, phishing attacks, fraud, and brand impersonation. Useful as an
 additional source of targeted threat intelligence.
 
 ![Demo](/docs/demo.gif)
 
-DNS fuzzing is an automated workflow for discovering potentially malicious
-domains targeting your organisation. This tool works by generating a large list
-of permutations based on a domain name you provide and then checking if any of
-those permutations are in use.
-Additionally, it can generate fuzzy hashes of the web pages to see if they are
-part of an ongoing phishing attack or brand impersonation, and much more!
+DNS fuzzing is an automated workflow that aims to uncover potentially malicious
+domains that target your organization. This tool generates a comprehensive list
+of permutations based on a provided domain name, and subsequently verifies
+whether any of these permutations are in use.
+Additionally, it can generate fuzzy hashes of web pages to detect ongoing
+phishing attacks or brand impersonation, and much more!
 
 In a hurry? Try it in your web browser: [dnstwist.it](https://dnstwist.it)
 
 
 Key features
 ------------
 
@@ -182,15 +182,15 @@
 
 **Fuzzy hashing**
 
 The unique feature of detecting similar HTML source code can be enabled with
 `--lsh` argument. For each generated domain, `dnstwist` will fetch content
 from responding HTTP server (following possible redirects), normalize HTML code
 and compare its fuzzy hash with the one for the original (initial) domain. The
-level of similarity is be expressed as a percentage.
+level of similarity is expressed as a percentage.
 
 In cases when the effective URL is the same as for the original domain, the
 fuzzy hash is not calculated at all in order to reject false positive
 indications.
 
 Note: Keep in mind it's rather unlikely to get 100% match, even for MITM attack
 frameworks, and that a phishing site can have a completely different HTML
@@ -215,37 +215,39 @@
 
 ```
 $ dnstwist --lsh tlsh domain.name
 ```
 
 **Perceptual hashing**
 
-If Chromium browser is installed, `dnstwist` can run it in so called headless
-mode (without GUI) to render web pages, take their screenshots and calculate
-pHash to evaluate visual similarity.
+If Chromium browser is installed, `dnstwist` can utilize its headless mode,
+which operates without a graphical user interface, to capture web page
+screenshots, render them, and calculate pHash values. These pHash values are
+then compared to evaluate the visual similarity, expressed as a percentage.
 
 ```
 $ dnstwist --phash domain.name
 ```
 
-Additionally, screenshots in PNG format can be saved to selected location:
+Moreover, it is possible to save the captured screenshots in the PNG format to
+a location of choice:
 
 ```
 $ dnstwist --phash --screenshots /tmp/domain domain.name
 ```
 
 Note: Due to the multi-threaded use of a fully functional web browser,
 an appropriate amount of free resources (mainly memory) should be provided.
 
 
 API
 ---
 
 In case you need to consume the data produced by the tool within your code,
-probably the most convenient and fast way is to pass the input as follows.
+the most convenient and efficient way is to pass the input as follows.
 
 ```
 >>> import dnstwist
 >>> data = dnstwist.run(domain='domain.name', registered=True, format='null')
 ```
 
 The arguments for `dnstwist.run()` are translated internally, so the usage is
@@ -253,26 +255,25 @@
 easy-to-process list of dictionaries. Keep in mind that `dnstwist.run()` spawns
 a number of daemon threads.
 
 
 Notes on coverage
 -----------------
 
-Along with the length of the domain, the number of variants generated by the
-algorithms increases considerably, and therefore the time and resources needed
-to verify them. It's mathematically impossible to check all domain
-permutations - especially for longer input domains which would require millions
-of DNS lookups.
-For this reason, this tool generates and checks domains very close to the
-original one. Theoretically, these are the most attractive domains from the
-attacker's point of view. However, be aware that the imagination of the
-aggressors is unlimited.
+As the length of the input domain increases, the number of variants generated
+by the algorithms increases significantly, resulting in a substantial increase
+in the time and resources required to verify them. Checking every possible
+domain permutation is impractical, especially for longer input domains, which
+would require millions of DNS lookups. Thus, this tool generates and checks
+domains that are very similar to the original one. Theoretically, these domains
+are the most appealing from an attacker's point of view. However, it's
+essential to note that attackers' imagination is unlimited.
 
-Unicode tables consist of thousands of characters with many of them visually
-similar to each other. However, despite the fact certain characters are
+Unicode tables comprise thousands of characters with many of them visually
+similar to one another. However, despite the fact certain characters are
 encodable using punycode, most TLD authorities will reject them during domain
 registration process. In general, TLD authorities disallow mixing of characters
 coming from different Unicode scripts or maintain their own sets of acceptable
 characters. With that being said, the homoglyph fuzzer was build on top of
 carefully researched range of Unicode characters (homoglyphs) to ensure that
 generated domains can be registered in practice.
```

### Comparing `dnstwist-20230413/dnstwist.egg-info/PKG-INFO` & `dnstwist-20230509/dnstwist.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnstwist
-Version: 20230413
+Version: 20230509
 Summary: Domain name permutation engine for detecting homograph phishing attacks, typo squatting, and brand impersonation
 Home-page: https://github.com/elceef/dnstwist
 Author: Marcin Ulikowski
 Author-email: marcin@ulikowski.pl
 License: ASL 2.0
 Description: Project website: https://github.com/elceef/dnstwist
 Platform: UNKNOWN
```

### Comparing `dnstwist-20230413/dnstwist.py` & `dnstwist-20230509/dnstwist.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 '''
 
 __author__ = 'Marcin Ulikowski'
-__version__ = '20230413'
+__version__ = '20230509'
 __email__ = 'marcin@ulikowski.pl'
 
 import re
 import sys
 import socket
-socket.setdefaulttimeout(10.0)
+socket.setdefaulttimeout(12.0)
 import signal
 import time
 import argparse
 import threading
 import os
 import smtplib
 import json
@@ -322,15 +322,15 @@
 		return '{:x}'.format(int(self.hash, base=2))
 
 	def __int__(self):
 		return int(self.hash, base=2)
 
 
 class HeadlessBrowser():
-	WEBDRIVER_TIMEOUT = 10
+	WEBDRIVER_TIMEOUT = 12
 	WEBDRIVER_ARGUMENTS = (
 		'--disable-dev-shm-usage',
 		'--ignore-certificate-errors',
 		'--headless',
 		'--incognito',
 		'--no-sandbox',
 		'--disable-gpu',
@@ -394,80 +394,197 @@
 			pass
 
 	def __del__(self):
 		self.stop()
 
 
 class Fuzzer():
+	glyphs_idn_by_tld = {
+		**dict.fromkeys(['cz', 'sk', 'uk', 'co.uk', 'nl', 'edu'], {
+			# IDN not suported by the corresponding registry
+		}),
+		**dict.fromkeys(['br'], {
+			'a': ('à', 'á', 'â', 'ã'),
+			'c': ('ç',),
+			'e': ('é', 'ê'),
+			'i': ('í',),
+			'o': ('ó', 'ô', 'õ'),
+			'u': ('ú', 'ü'),
+			'y': ('ý', 'ÿ'),
+		}),
+		**dict.fromkeys(['dk'], {
+			'a': ('ä', 'å'),
+			'e': ('é',),
+			'o': ('ö', 'ø'),
+			'u': ('ü',),
+			'ae': ('æ',),
+		}),
+		**dict.fromkeys(['eu', 'de', 'pl'], {
+			'a': ('á', 'à', 'ă', 'â', 'å', 'ä', 'ã', 'ą', 'ā'),
+			'c': ('ć', 'ĉ', 'č', 'ċ', 'ç'),
+			'd': ('ď', 'đ'),
+			'e': ('é', 'è', 'ĕ', 'ê', 'ě', 'ë', 'ė', 'ę', 'ē'),
+			'g': ('ğ', 'ĝ', 'ġ', 'ģ'),
+			'h': ('ĥ', 'ħ'),
+			'i': ('í', 'ì', 'ĭ', 'î', 'ï', 'ĩ', 'į', 'ī'),
+			'j': ('ĵ',),
+			'k': ('ķ', 'ĸ'),
+			'l': ('ĺ', 'ľ', 'ļ', 'ł'),
+			'n': ('ń', 'ň', 'ñ', 'ņ'),
+			'o': ('ó', 'ò', 'ŏ', 'ô', 'ö', 'ő', 'õ', 'ø', 'ō'),
+			'r': ('ŕ', 'ř', 'ŗ'),
+			's': ('ś', 'ŝ', 'š', 'ş'),
+			't': ('ť', 'ţ', 'ŧ'),
+			'u': ('ú', 'ù', 'ŭ', 'û', 'ů', 'ü', 'ű', 'ũ', 'ų', 'ū'),
+			'w': ('ŵ',),
+			'y': ('ý', 'ŷ', 'ÿ'),
+			'z': ('ź', 'ž', 'ż'),
+			'ae': ('æ',),
+			'oe': ('œ',),
+		}),
+		**dict.fromkeys(['fi'], {
+			'3': ('ʒ',),
+			'a': ('á', 'ä', 'å', 'â'),
+			'c': ('č',),
+			'd': ('đ',),
+			'g': ('ǧ', 'ǥ'),
+			'k': ('ǩ',),
+			'n': ('ŋ',),
+			'o': ('õ', 'ö'),
+			's': ('š',),
+			't': ('ŧ',),
+			'z': ('ž',),
+		}),
+		**dict.fromkeys(['no'], {
+			'a': ('á', 'à', 'ä', 'å'),
+			'c': ('č', 'ç'),
+			'e': ('é', 'è', 'ê'),
+			'i': ('ï',),
+			'n': ('ŋ', 'ń', 'ñ'),
+			'o': ('ó', 'ò', 'ô', 'ö', 'ø'),
+			's': ('š',),
+			't': ('ŧ',),
+			'u': ('ü',),
+			'z': ('ž',),
+			'ae': ('æ',),
+		}),
+		**dict.fromkeys(['be', 'fr', 're', 'yt', 'pm', 'wf', 'tf', 'ch', 'li'], {
+			'a': ('à', 'á', 'â', 'ã', 'ä', 'å'),
+			'c': ('ç',),
+			'e': ('è', 'é', 'ê', 'ë'),
+			'i': ('ì', 'í', 'î', 'ï'),
+			'n': ('ñ',),
+			'o': ('ò', 'ó', 'ô', 'õ', 'ö'),
+			'u': ('ù', 'ú', 'û', 'ü'),
+			'y': ('ý', 'ÿ'),
+			'ae': ('æ',),
+			'oe': ('œ',),
+		}),
+		**dict.fromkeys(['ca'], {
+			'a': ('à', 'â'),
+			'c': ('ç',),
+			'e': ('è', 'é', 'ê', 'ë'),
+			'i': ('î', 'ï'),
+			'o': ('ô',),
+			'u': ('ù', 'û', 'ü'),
+			'y': ('ÿ',),
+			'ae': ('æ',),
+			'oe': ('œ',),
+		}),
+	}
+
+	glyphs_unicode = {
+		'2': ('ƻ',),
+		'3': ('ʒ',),
+		'5': ('ƽ',),
+		'a': ('ạ', 'ă', 'ȧ', 'ɑ', 'å', 'ą', 'â', 'ǎ', 'á', 'ə', 'ä', 'ã', 'ā', 'à'),
+		'b': ('ḃ', 'ḅ', 'ƅ', 'ʙ', 'ḇ', 'ɓ'),
+		'c': ('č', 'ᴄ', 'ċ', 'ç', 'ć', 'ĉ', 'ƈ'),
+		'd': ('ď', 'ḍ', 'ḋ', 'ɖ', 'ḏ', 'ɗ', 'ḓ', 'ḑ', 'đ'),
+		'e': ('ê', 'ẹ', 'ę', 'è', 'ḛ', 'ě', 'ɇ', 'ė', 'ĕ', 'é', 'ë', 'ē', 'ȩ'),
+		'f': ('ḟ', 'ƒ'),
+		'g': ('ǧ', 'ġ', 'ǵ', 'ğ', 'ɡ', 'ǥ', 'ĝ', 'ģ', 'ɢ'),
+		'h': ('ȟ', 'ḫ', 'ḩ', 'ḣ', 'ɦ', 'ḥ', 'ḧ', 'ħ', 'ẖ', 'ⱨ', 'ĥ'),
+		'i': ('ɩ', 'ǐ', 'í', 'ɪ', 'ỉ', 'ȋ', 'ɨ', 'ï', 'ī', 'ĩ', 'ị', 'î', 'ı', 'ĭ', 'į', 'ì'),
+		'j': ('ǰ', 'ĵ', 'ʝ', 'ɉ'),
+		'k': ('ĸ', 'ǩ', 'ⱪ', 'ḵ', 'ķ', 'ᴋ', 'ḳ'),
+		'l': ('ĺ', 'ł', 'ɫ', 'ļ', 'ľ'),
+		'm': ('ᴍ', 'ṁ', 'ḿ', 'ṃ', 'ɱ'),
+		'n': ('ņ', 'ǹ', 'ń', 'ň', 'ṅ', 'ṉ', 'ṇ', 'ꞑ', 'ñ', 'ŋ'),
+		'o': ('ö', 'ó', 'ȯ', 'ỏ', 'ô', 'ᴏ', 'ō', 'ò', 'ŏ', 'ơ', 'ő', 'õ', 'ọ', 'ø'),
+		'p': ('ṗ', 'ƿ', 'ƥ', 'ṕ'),
+		'q': ('ʠ',),
+		'r': ('ʀ', 'ȓ', 'ɍ', 'ɾ', 'ř', 'ṛ', 'ɽ', 'ȑ', 'ṙ', 'ŗ', 'ŕ', 'ɼ', 'ṟ'),
+		's': ('ṡ', 'ș', 'ŝ', 'ꜱ', 'ʂ', 'š', 'ś', 'ṣ', 'ş'),
+		't': ('ť', 'ƫ', 'ţ', 'ṭ', 'ṫ', 'ț', 'ŧ'),
+		'u': ('ᴜ', 'ų', 'ŭ', 'ū', 'ű', 'ǔ', 'ȕ', 'ư', 'ù', 'ů', 'ʉ', 'ú', 'ȗ', 'ü', 'û', 'ũ', 'ụ'),
+		'v': ('ᶌ', 'ṿ', 'ᴠ', 'ⱴ', 'ⱱ', 'ṽ'),
+		'w': ('ᴡ', 'ẇ', 'ẅ', 'ẃ', 'ẘ', 'ẉ', 'ⱳ', 'ŵ', 'ẁ'),
+		'x': ('ẋ', 'ẍ'),
+		'y': ('ŷ', 'ÿ', 'ʏ', 'ẏ', 'ɏ', 'ƴ', 'ȳ', 'ý', 'ỿ', 'ỵ'),
+		'z': ('ž', 'ƶ', 'ẓ', 'ẕ', 'ⱬ', 'ᴢ', 'ż', 'ź', 'ʐ'),
+		'ae': ('æ',),
+		'oe': ('œ',),
+	}
+
+	glyphs_ascii = {
+		'0': ('o',),
+		'1': ('l', 'i'),
+		'3': ('8',),
+		'6': ('9',),
+		'8': ('3',),
+		'9': ('6',),
+		'b': ('d', 'lb'),
+		'c': ('e',),
+		'd': ('b', 'cl', 'dl'),
+		'e': ('c',),
+		'g': ('q',),
+		'h': ('lh'),
+		'i': ('1', 'l'),
+		'k': ('lc'),
+		'l': ('1', 'i'),
+		'm': ('n', 'nn', 'rn', 'rr'),
+		'n': ('m', 'r'),
+		'o': ('0',),
+		'q': ('g',),
+		'w': ('vv',),
+	}
+
+	latin_to_cyrillic = {
+		'a': 'а', 'b': 'ь', 'c': 'с', 'd': 'ԁ', 'e': 'е', 'g': 'ԍ', 'h': 'һ',
+		'i': 'і', 'j': 'ј', 'k': 'к', 'l': 'ӏ', 'm': 'м', 'o': 'о', 'p': 'р',
+		'q': 'ԛ', 's': 'ѕ', 't': 'т', 'v': 'ѵ', 'w': 'ԝ', 'x': 'х', 'y': 'у',
+	}
+
+	qwerty = {
+		'1': '2q', '2': '3wq1', '3': '4ew2', '4': '5re3', '5': '6tr4', '6': '7yt5', '7': '8uy6', '8': '9iu7', '9': '0oi8', '0': 'po9',
+		'q': '12wa', 'w': '3esaq2', 'e': '4rdsw3', 'r': '5tfde4', 't': '6ygfr5', 'y': '7uhgt6', 'u': '8ijhy7', 'i': '9okju8', 'o': '0plki9', 'p': 'lo0',
+		'a': 'qwsz', 's': 'edxzaw', 'd': 'rfcxse', 'f': 'tgvcdr', 'g': 'yhbvft', 'h': 'ujnbgy', 'j': 'ikmnhu', 'k': 'olmji', 'l': 'kop',
+		'z': 'asx', 'x': 'zsdc', 'c': 'xdfv', 'v': 'cfgb', 'b': 'vghn', 'n': 'bhjm', 'm': 'njk'
+	}
+	qwertz = {
+		'1': '2q', '2': '3wq1', '3': '4ew2', '4': '5re3', '5': '6tr4', '6': '7zt5', '7': '8uz6', '8': '9iu7', '9': '0oi8', '0': 'po9',
+		'q': '12wa', 'w': '3esaq2', 'e': '4rdsw3', 'r': '5tfde4', 't': '6zgfr5', 'z': '7uhgt6', 'u': '8ijhz7', 'i': '9okju8', 'o': '0plki9', 'p': 'lo0',
+		'a': 'qwsy', 's': 'edxyaw', 'd': 'rfcxse', 'f': 'tgvcdr', 'g': 'zhbvft', 'h': 'ujnbgz', 'j': 'ikmnhu', 'k': 'olmji', 'l': 'kop',
+		'y': 'asx', 'x': 'ysdc', 'c': 'xdfv', 'v': 'cfgb', 'b': 'vghn', 'n': 'bhjm', 'm': 'njk'
+	}
+	azerty = {
+		'1': '2a', '2': '3za1', '3': '4ez2', '4': '5re3', '5': '6tr4', '6': '7yt5', '7': '8uy6', '8': '9iu7', '9': '0oi8', '0': 'po9',
+		'a': '2zq1', 'z': '3esqa2', 'e': '4rdsz3', 'r': '5tfde4', 't': '6ygfr5', 'y': '7uhgt6', 'u': '8ijhy7', 'i': '9okju8', 'o': '0plki9', 'p': 'lo0m',
+		'q': 'zswa', 's': 'edxwqz', 'd': 'rfcxse', 'f': 'tgvcdr', 'g': 'yhbvft', 'h': 'ujnbgy', 'j': 'iknhu', 'k': 'olji', 'l': 'kopm', 'm': 'lp',
+		'w': 'sxq', 'x': 'wsdc', 'c': 'xdfv', 'v': 'cfgb', 'b': 'vghn', 'n': 'bhj'
+	}
+	keyboards = [qwerty, qwertz, azerty]
+
 	def __init__(self, domain, dictionary=[], tld_dictionary=[]):
 		self.subdomain, self.domain, self.tld = domain_tld(domain)
 		self.domain = idna.decode(self.domain)
 		self.dictionary = list(dictionary)
 		self.tld_dictionary = list(tld_dictionary)
 		self.domains = set()
-		self.qwerty = {
-			'1': '2q', '2': '3wq1', '3': '4ew2', '4': '5re3', '5': '6tr4', '6': '7yt5', '7': '8uy6', '8': '9iu7', '9': '0oi8', '0': 'po9',
-			'q': '12wa', 'w': '3esaq2', 'e': '4rdsw3', 'r': '5tfde4', 't': '6ygfr5', 'y': '7uhgt6', 'u': '8ijhy7', 'i': '9okju8', 'o': '0plki9', 'p': 'lo0',
-			'a': 'qwsz', 's': 'edxzaw', 'd': 'rfcxse', 'f': 'tgvcdr', 'g': 'yhbvft', 'h': 'ujnbgy', 'j': 'ikmnhu', 'k': 'olmji', 'l': 'kop',
-			'z': 'asx', 'x': 'zsdc', 'c': 'xdfv', 'v': 'cfgb', 'b': 'vghn', 'n': 'bhjm', 'm': 'njk'
-			}
-		self.qwertz = {
-			'1': '2q', '2': '3wq1', '3': '4ew2', '4': '5re3', '5': '6tr4', '6': '7zt5', '7': '8uz6', '8': '9iu7', '9': '0oi8', '0': 'po9',
-			'q': '12wa', 'w': '3esaq2', 'e': '4rdsw3', 'r': '5tfde4', 't': '6zgfr5', 'z': '7uhgt6', 'u': '8ijhz7', 'i': '9okju8', 'o': '0plki9', 'p': 'lo0',
-			'a': 'qwsy', 's': 'edxyaw', 'd': 'rfcxse', 'f': 'tgvcdr', 'g': 'zhbvft', 'h': 'ujnbgz', 'j': 'ikmnhu', 'k': 'olmji', 'l': 'kop',
-			'y': 'asx', 'x': 'ysdc', 'c': 'xdfv', 'v': 'cfgb', 'b': 'vghn', 'n': 'bhjm', 'm': 'njk'
-			}
-		self.azerty = {
-			'1': '2a', '2': '3za1', '3': '4ez2', '4': '5re3', '5': '6tr4', '6': '7yt5', '7': '8uy6', '8': '9iu7', '9': '0oi8', '0': 'po9',
-			'a': '2zq1', 'z': '3esqa2', 'e': '4rdsz3', 'r': '5tfde4', 't': '6ygfr5', 'y': '7uhgt6', 'u': '8ijhy7', 'i': '9okju8', 'o': '0plki9', 'p': 'lo0m',
-			'q': 'zswa', 's': 'edxwqz', 'd': 'rfcxse', 'f': 'tgvcdr', 'g': 'yhbvft', 'h': 'ujnbgy', 'j': 'iknhu', 'k': 'olji', 'l': 'kopm', 'm': 'lp',
-			'w': 'sxq', 'x': 'wsdc', 'c': 'xdfv', 'v': 'cfgb', 'b': 'vghn', 'n': 'bhj'
-			}
-		self.keyboards = [self.qwerty, self.qwertz, self.azerty]
-		self.glyphs = {
-			'0': ['o'],
-			'1': ['l', 'i'],
-			'2': ['ƻ'],
-			'3': ['8'],
-			'5': ['ƽ'],
-			'6': ['9'],
-			'8': ['3'],
-			'9': ['6'],
-			'a': ['à', 'á', 'à', 'â', 'ã', 'ä', 'å', 'ɑ', 'ạ', 'ǎ', 'ă', 'ȧ', 'ą', 'ə'],
-			'b': ['d', 'lb', 'ʙ', 'ɓ', 'ḃ', 'ḅ', 'ḇ', 'ƅ'],
-			'c': ['e', 'ƈ', 'ċ', 'ć', 'ç', 'č', 'ĉ', 'ᴄ'],
-			'd': ['b', 'cl', 'dl', 'ɗ', 'đ', 'ď', 'ɖ', 'ḑ', 'ḋ', 'ḍ', 'ḏ', 'ḓ'],
-			'e': ['c', 'é', 'è', 'ê', 'ë', 'ē', 'ĕ', 'ě', 'ė', 'ẹ', 'ę', 'ȩ', 'ɇ', 'ḛ'],
-			'f': ['ƒ', 'ḟ'],
-			'g': ['q', 'ɢ', 'ɡ', 'ġ', 'ğ', 'ǵ', 'ģ', 'ĝ', 'ǧ', 'ǥ'],
-			'h': ['lh', 'ĥ', 'ȟ', 'ħ', 'ɦ', 'ḧ', 'ḩ', 'ⱨ', 'ḣ', 'ḥ', 'ḫ', 'ẖ'],
-			'i': ['1', 'l', 'í', 'ì', 'ï', 'ı', 'ɩ', 'ǐ', 'ĭ', 'ỉ', 'ị', 'ɨ', 'ȋ', 'ī', 'ɪ'],
-			'j': ['ʝ', 'ǰ', 'ɉ', 'ĵ'],
-			'k': ['lk', 'ik', 'lc', 'ḳ', 'ḵ', 'ⱪ', 'ķ', 'ᴋ'],
-			'l': ['1', 'i', 'ɫ', 'ł'],
-			'm': ['n', 'nn', 'rn', 'rr', 'ṁ', 'ṃ', 'ᴍ', 'ɱ', 'ḿ'],
-			'n': ['m', 'r', 'ń', 'ṅ', 'ṇ', 'ṉ', 'ñ', 'ņ', 'ǹ', 'ň', 'ꞑ'],
-			'o': ['0', 'ȯ', 'ọ', 'ỏ', 'ơ', 'ó', 'ö', 'ᴏ'],
-			'p': ['ƿ', 'ƥ', 'ṕ', 'ṗ'],
-			'q': ['g', 'ʠ'],
-			'r': ['ʀ', 'ɼ', 'ɽ', 'ŕ', 'ŗ', 'ř', 'ɍ', 'ɾ', 'ȓ', 'ȑ', 'ṙ', 'ṛ', 'ṟ'],
-			's': ['ʂ', 'ś', 'ṣ', 'ṡ', 'ș', 'ŝ', 'š', 'ꜱ'],
-			't': ['ţ', 'ŧ', 'ṫ', 'ṭ', 'ț', 'ƫ'],
-			'u': ['ᴜ', 'ǔ', 'ŭ', 'ü', 'ʉ', 'ù', 'ú', 'û', 'ũ', 'ū', 'ų', 'ư', 'ů', 'ű', 'ȕ', 'ȗ', 'ụ'],
-			'v': ['ṿ', 'ⱱ', 'ᶌ', 'ṽ', 'ⱴ', 'ᴠ'],
-			'w': ['vv', 'ŵ', 'ẁ', 'ẃ', 'ẅ', 'ⱳ', 'ẇ', 'ẉ', 'ẘ', 'ᴡ'],
-			'x': ['ẋ', 'ẍ'],
-			'y': ['ʏ', 'ý', 'ÿ', 'ŷ', 'ƴ', 'ȳ', 'ɏ', 'ỿ', 'ẏ', 'ỵ'],
-			'z': ['ʐ', 'ż', 'ź', 'ᴢ', 'ƶ', 'ẓ', 'ẕ', 'ⱬ']
-			}
-		self.latin_to_cyrillic = {
-			'a': 'а', 'b': 'ь', 'c': 'с', 'd': 'ԁ', 'e': 'е', 'g': 'ԍ', 'h': 'һ',
-			'i': 'і', 'j': 'ј', 'k': 'к', 'l': 'ӏ', 'm': 'м', 'o': 'о', 'p': 'р',
-			'q': 'ԛ', 's': 'ѕ', 't': 'т', 'v': 'ѵ', 'w': 'ԝ', 'x': 'х', 'y': 'у',
-			}
 
 	def _bitsquatting(self):
 		masks = [1, 2, 4, 8, 16, 32, 64, 128]
 		chars = set('abcdefghijklmnopqrstuvwxyz0123456789-')
 		for i, c in enumerate(self.domain):
 			for mask in masks:
 				b = chr(ord(c) ^ mask)
@@ -480,22 +597,23 @@
 			cdomain = cdomain.replace(l, c)
 		for c, l in zip(cdomain, self.domain):
 			if c == l:
 				return []
 		return [cdomain]
 
 	def _homoglyph(self):
+		md = lambda a, b: {k: set(a.get(k, [])) | set(b.get(k, [])) for k in set(a.keys()) | set(b.keys())}
+		glyphs = md(self.glyphs_ascii, self.glyphs_idn_by_tld.get(self.tld, self.glyphs_unicode))
 		def mix(domain):
-			glyphs = self.glyphs
 			for w in range(1, len(domain)):
 				for i in range(len(domain)-w+1):
 					pre = domain[:i]
 					win = domain[i:i+w]
 					suf = domain[i+w:]
-					for c in set(win):
+					for c in (set(win) | {win[:2]}):
 						for g in glyphs.get(c, []):
 							yield pre + win.replace(c, g) + suf
 		result1 = set(mix(self.domain))
 		result2 = set()
 		for r in result1:
 			result2.update(set(mix(r)))
 		return result1 | result2
```

### Comparing `dnstwist-20230413/setup.py` & `dnstwist-20230509/setup.py`

 * *Files identical despite different names*

