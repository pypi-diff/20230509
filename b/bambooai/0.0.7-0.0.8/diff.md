# Comparing `tmp/bambooai-0.0.7.tar.gz` & `tmp/bambooai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambooai-0.0.7.tar", last modified: Sun May  7 09:22:31 2023, max compression
+gzip compressed data, was "bambooai-0.0.8.tar", last modified: Tue May  9 08:40:23 2023, max compression
```

## Comparing `bambooai-0.0.7.tar` & `bambooai-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 09:22:31.065001 bambooai-0.0.7/
--rw-rw-rw-   0        0        0      369 2023-05-07 09:22:31.064477 bambooai-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-07 09:22:31.036997 bambooai-0.0.7/bambooai/
--rw-rw-rw-   0        0        0       30 2023-05-07 07:18:22.000000 bambooai-0.0.7/bambooai/__init__.py
--rw-rw-rw-   0        0        0     7040 2023-05-07 09:08:21.000000 bambooai-0.0.7/bambooai/bambooai.py
-drwxrwxrwx   0        0        0        0 2023-05-07 09:22:31.062367 bambooai-0.0.7/bambooai.egg-info/
--rw-rw-rw-   0        0        0      369 2023-05-07 09:22:30.000000 bambooai-0.0.7/bambooai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-07 09:22:30.000000 bambooai-0.0.7/bambooai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 09:22:30.000000 bambooai-0.0.7/bambooai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-07 09:22:30.000000 bambooai-0.0.7/bambooai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-07 09:22:30.000000 bambooai-0.0.7/bambooai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 09:22:31.065873 bambooai-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      501 2023-05-07 09:09:39.000000 bambooai-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:40:23.542205 bambooai-0.0.8/
+-rw-rw-rw-   0        0        0     5507 2023-05-09 08:40:23.541569 bambooai-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5015 2023-05-09 08:27:19.000000 bambooai-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-09 08:40:23.501510 bambooai-0.0.8/bambooai/
+-rw-rw-rw-   0        0        0       30 2023-05-07 07:18:22.000000 bambooai-0.0.8/bambooai/__init__.py
+-rw-rw-rw-   0        0        0     8005 2023-05-09 08:12:22.000000 bambooai-0.0.8/bambooai/bambooai.py
+drwxrwxrwx   0        0        0        0 2023-05-09 08:40:23.539068 bambooai-0.0.8/bambooai.egg-info/
+-rw-rw-rw-   0        0        0     5507 2023-05-09 08:40:23.000000 bambooai-0.0.8/bambooai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-09 08:40:23.000000 bambooai-0.0.8/bambooai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 08:40:23.000000 bambooai-0.0.8/bambooai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-09 08:40:23.000000 bambooai-0.0.8/bambooai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 08:40:23.000000 bambooai-0.0.8/bambooai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 08:40:23.542706 bambooai-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      676 2023-05-09 08:27:58.000000 bambooai-0.0.8/setup.py
```

### Comparing `bambooai-0.0.7/bambooai/bambooai.py` & `bambooai-0.0.8/bambooai/bambooai.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,39 +52,55 @@
             max_tokens=max_tokens,
         )
 
         content = response.choices[0].message.content.strip()
         tokens_used = response.usage.total_tokens
 
         return content, tokens_used
-
+    
+    # Function to sanitize the output from the LLM
     def _extract_code(self, response: str, separator: str = "```") -> str:
+
+        # Define a blacklist of Python keywords and functions that are not allowed
+        blacklist = ['os','subprocess','sys','eval','exec','file','open','socket','urllib']
+
         # Set the initial value of code to the response
         code = response
 
         # If the response contains the separator, extract the code block between the separators
         if len(response.split(separator)) > 1:
             code = response.split(separator)[1]
 
         # Search for a pattern between <code> and </code> in the extracted code
         match = re.search(r"<code>(.*)</code>", code, re.DOTALL)
         if match:
             # If a match is found, extract the code between <code> and </code>
             code = match.group(1)
-
             # Remove the "python" or "py" prefix if present
             if re.match(r"^(python|py)", code):
                 code = re.sub(r"^(python|py)", "", code)
 
         # If the code is between single backticks, extract the code between them
         if re.match(r"^`.*`$", code):
             code = re.sub(r"^`(.*)`$", r"\1", code)
 
         # Remove any instances of "df = pd.read_csv('filename.csv')" from the code
         code = re.sub(r"df\s*=\s*pd\.read_csv\('.*?'\)", "", code)
+        
+        # Remove any occurrences of df = pd.DataFrame() with any number of characters inside the parentheses.
+        code = re.sub(r"df\s*=\s*pd\.DataFrame\(.*?\)", "", code)
+
+        # Define the regular expression pattern to match the blacklist items
+        pattern = r"\b(" + "|".join(blacklist) + r")\b"
+
+        # Replace the blacklist items with comments
+        code = re.sub(pattern, r"# \1 not allowed", code)
+
+        # Remove any import statements that were turned into comments
+        code = re.sub(r"^\s*#\s*import\s.*?$", "", code, flags=re.MULTILINE)
 
         # Return the cleaned and extracted code
         return code.strip()
 
     def pd_agent_converse(self, question=None):
         # Initialize the messages list with a system message containing the task prompt
         messages = [{"role": "system", "content": self.task.format(self.df_head, "")}]
@@ -175,8 +191,14 @@
         # Print the total tokens used
         print(colored("\nTotal tokens used:{}".format(total_tokens_used_sum), "yellow"))
 
         # Get the output from the executed code
         answer = output.getvalue()
 
         return answer
+    
+# Test the BambooAI class
+
+df = pd.read_csv('./Next_Seq_Nr/Timeseries_DJI.csv')
+bamboo = BambooAI(df)
+bamboo.pd_agent_converse()
```

