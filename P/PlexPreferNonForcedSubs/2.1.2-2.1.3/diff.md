# Comparing `tmp/PlexPreferNonForcedSubs-2.1.2.tar.gz` & `tmp/PlexPreferNonForcedSubs-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlexPreferNonForcedSubs-2.1.2.tar", last modified: Wed Apr 26 21:00:32 2023, max compression
+gzip compressed data, was "PlexPreferNonForcedSubs-2.1.3.tar", last modified: Tue May  9 14:56:30 2023, max compression
```

## Comparing `PlexPreferNonForcedSubs-2.1.2.tar` & `PlexPreferNonForcedSubs-2.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 21:00:32.266233 PlexPreferNonForcedSubs-2.1.2/
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 PlexPreferNonForcedSubs-2.1.2/LICENSE
--rw-rw-rw-   0        0        0     4581 2023-04-26 21:00:32.265233 PlexPreferNonForcedSubs-2.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-26 21:00:32.234239 PlexPreferNonForcedSubs-2.1.2/PlexPreferNonForcedSubs/
--rw-rw-rw-   0        0        0     6352 2023-04-26 20:55:48.000000 PlexPreferNonForcedSubs-2.1.2/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py
--rw-rw-rw-   0        0        0        0 2023-04-26 17:50:08.000000 PlexPreferNonForcedSubs-2.1.2/PlexPreferNonForcedSubs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 21:00:32.263736 PlexPreferNonForcedSubs-2.1.2/PlexPreferNonForcedSubs.egg-info/
--rw-rw-rw-   0        0        0     4581 2023-04-26 21:00:32.000000 PlexPreferNonForcedSubs-2.1.2/PlexPreferNonForcedSubs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-04-26 21:00:32.000000 PlexPreferNonForcedSubs-2.1.2/PlexPreferNonForcedSubs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 21:00:32.000000 PlexPreferNonForcedSubs-2.1.2/PlexPreferNonForcedSubs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-04-26 21:00:32.000000 PlexPreferNonForcedSubs-2.1.2/PlexPreferNonForcedSubs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-04-26 21:00:32.000000 PlexPreferNonForcedSubs-2.1.2/PlexPreferNonForcedSubs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-26 21:00:32.000000 PlexPreferNonForcedSubs-2.1.2/PlexPreferNonForcedSubs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3945 2023-04-26 20:00:36.000000 PlexPreferNonForcedSubs-2.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-26 21:00:32.266233 PlexPreferNonForcedSubs-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1516 2023-04-26 20:57:23.000000 PlexPreferNonForcedSubs-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:56:30.416304 PlexPreferNonForcedSubs-2.1.3/
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 PlexPreferNonForcedSubs-2.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5436 2023-05-09 14:56:30.415816 PlexPreferNonForcedSubs-2.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-09 14:56:30.386345 PlexPreferNonForcedSubs-2.1.3/PlexPreferNonForcedSubs/
+-rw-rw-rw-   0        0        0     6483 2023-05-09 14:54:51.000000 PlexPreferNonForcedSubs-2.1.3/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:50:08.000000 PlexPreferNonForcedSubs-2.1.3/PlexPreferNonForcedSubs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-09 14:56:30.413818 PlexPreferNonForcedSubs-2.1.3/PlexPreferNonForcedSubs.egg-info/
+-rw-rw-rw-   0        0        0     5436 2023-05-09 14:56:30.000000 PlexPreferNonForcedSubs-2.1.3/PlexPreferNonForcedSubs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-05-09 14:56:30.000000 PlexPreferNonForcedSubs-2.1.3/PlexPreferNonForcedSubs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 14:56:30.000000 PlexPreferNonForcedSubs-2.1.3/PlexPreferNonForcedSubs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-05-09 14:56:30.000000 PlexPreferNonForcedSubs-2.1.3/PlexPreferNonForcedSubs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-05-09 14:56:30.000000 PlexPreferNonForcedSubs-2.1.3/PlexPreferNonForcedSubs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-09 14:56:30.000000 PlexPreferNonForcedSubs-2.1.3/PlexPreferNonForcedSubs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4792 2023-05-09 14:55:37.000000 PlexPreferNonForcedSubs-2.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 14:56:30.416804 PlexPreferNonForcedSubs-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1516 2023-05-09 14:55:59.000000 PlexPreferNonForcedSubs-2.1.3/setup.py
```

### Comparing `PlexPreferNonForcedSubs-2.1.2/LICENSE` & `PlexPreferNonForcedSubs-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PlexPreferNonForcedSubs-2.1.2/PKG-INFO` & `PlexPreferNonForcedSubs-2.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexPreferNonForcedSubs
-Version: 2.1.2
+Version: 2.1.3
 Summary: This script will set all movies and shows in your local Plex library to English non forced subtitles by default.
 Home-page: https://github.com/RileyXX/PlexPreferNonForcedSubs
 Keywords: python,video,plex,subtitles,subs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 License-File: LICENSE
 
 
 # PlexPreferNonForcedSubs
 
 
 ## Short description:
-This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices.
+This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices. This script should work on any OS where Python is installed (Windows, MacOS and Linux etc).
 
 ## Long description:
 This script was created with the help of [ChatGPT Open AI](https://chat.openai.com/chat) and further edited and completed by me. It uses [Plex Python Api](https://python-plexapi.readthedocs.io/en/latest/). It will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices. Assuming your Plex subtitles settings are setup in your server settings Plex will default to Forced Subtitles by default when they are available for a given item. Plex will not allow you to prefer non forced subtitles natively hence why this script was created.
 
 This script is confirmed tested and working. Feel free to use this code for your own purposes. I will be running this code periodically on my home server along with some of my other neat little plex scripts like [Plex Auto Delete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py). Thanks to [all](https://stackoverflow.com/questions/75027919/python-script-to-set-all-subtitles-for-movies-shows-in-plex-to-english-non-for) who helped! If you use this script and run into any bugs feel free to open an issue. Cheers!
 
 ## What are "non-forced" subtitles?
@@ -31,41 +31,49 @@
 
 
 ## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/).
 2. Run `python -m pip install PlexPreferNonForcedSubs` in command line.
 3. Make sure Plex media server is running then run the script using `PlexPreferNonForcedSubs` in command line.
 4. On first run the script will ask you to fill in your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). Your token will be saved locally in the same folder as token.txt.
-5. Done
+5. Done.
 
-_Note: This script should work on any OS where Python is installed (Windows, MacOS and Linux etc)._
+_See [below](https://github.com/RileyXX/PlexPreferNonForcedSubs#run) for details on how to run, update and uninstall._
 
 ### Run:
 `PlexPreferNonForcedSubs` in command line.
 
 ### Update:
 `python -m pip install PlexPreferNonForcedSubs --upgrade` in command line.
 ### Uninstall:
 `python -m pip uninstall PlexPreferNonForcedSubs` in command line.
 
+## Alternative manual no install method:
+1. Download the latest .py script from the [releases page](https://github.com/RileyXX/PlexPreferNonForcedSubs/releases) and move it to the file directory of your choice.
+2. Run the script by running `PlexPreferNonForcedSubs.py` OR open terminal and navigate to folder where `PlexPreferNonForcedSubs.py` is located. Run `PlexPreferNonForcedSubs.py` in terminal. 
+4. On first run the script will ask you to fill in your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). Your token will be saved locally in the same folder as token.txt.
+3. Done.
+
+_See [above](https://github.com/RileyXX/PlexPreferNonForcedSubs#run) for details on how to run, update and uninstall._
+
 ## Known issues/future outlook:
 * Several lines of redundant code can be shortened and/or removed
 
 ## Also posted on:
 * [Stackoverflow](https://stackoverflow.com/q/75027919/9196825)
 * [Reddit](https://www.reddit.com/r/PleX/comments/105gdh7/python_code_to_set_all_movies_and_shows_in_plex/)
 * [Plex Forums](https://forums.plex.tv/t/python-script-to-set-all-movies-and-shows-in-plex-to-use-english-non-forced-subtitles/825871)
 
 ## Screenshots:
 ##### Plex subtitle dropdown after script is done running:
 ![Plex Subtitle Dropdown](https://i.imgur.com/BNOlwtL.png)
 ##### PlexPreferNonForcedSubs.py script in action:
 ![PlexPreferNonForcedSubs.py Script in Action](https://github.com/RileyXX/PlexPreferNonForcedSubs/raw/main/demo.gif)
 
-## Donations, Sponsorships and Custom Projects:
+## Sponsorships, Donations and Custom Projects:
 Like my scripts? Become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! See below for other donation options. Need help with a project? Open an issue and I will try my best to help! For other inquiries and custom projects contact me on [Twitter](https://twitter.com/RileyxBell).
 
 #### More donation options:
 - Cashapp: `$rileyxx`
 - Venmo: `@rileyxx`
 - Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
```

### Comparing `PlexPreferNonForcedSubs-2.1.2/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py` & `PlexPreferNonForcedSubs-2.1.3/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 from plexapi.server import PlexServer
-from plexapi.media import SubtitleStream
 import os
 
 def main():
-    
     # Connect to Plex Media Server. Replace PLEX_TOKEN below with your Plex token. How to get token: https://www.plexopedia.com/plex-media-server/general/plex-token/
     baseurl = 'http://localhost:32400'
     token = 'PLEX_TOKEN'
-    
+
     script_dir = os.path.dirname(os.path.abspath(__file__))
     token_file = os.path.join(script_dir, 'token.txt')
-    
+
     try:
         with open(token_file, 'r') as f:
             token = f.read().strip()
     except FileNotFoundError:
         pass
 
     if token == 'PLEX_TOKEN':
         print(f'\nHow to get your Plex token: https://www.plexopedia.com/plex-media-server/general/plex-token/\n')
         token = input("Enter your Plex token: ")
         with open(token_file, 'w') as f:
             f.write(token)
 
     plex = PlexServer(baseurl, token)
 
+    # Movies
     table_headers = ['Title', 'Year', 'Status', 'Changes']
     title_width = 70
     year_width = 5
     status_width = 20
     changes_width = 8
 
     print("\n" + "-" * 114 + "\nMovies\n" + "-" * 114)
     print(f'\033[1m\033[96m{" | ".join([h.ljust(title_width if i == 0 else year_width if i == 1 else status_width if i == 2 else changes_width) for i, h in enumerate(table_headers)])}\033[0m')
 
     for section in plex.library.sections():
         if section.type == 'movie':
             for movie in section.all():
-                movie.reload()
-                english_subs = [stream for stream in movie.subtitleStreams() if stream.languageCode == 'eng']
-                non_forced_english_subs = [stream for stream in english_subs if not stream.forced or (hasattr(stream, 'title') and stream.title is not None and 'forced' not in stream.title.lower())]
-                forced_english_subs = [stream for stream in english_subs if stream.forced or (hasattr(stream, 'title') and stream.title is not None and 'forced' in stream.title.lower())]
-                part = movie.media[0].parts[0]
-                partsid = part.id
-                if forced_english_subs and non_forced_english_subs:
-                    non_forced_english_subs[0].setDefault()
-                    print(f'\033[92m{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"English (Non-Forced)".ljust(status_width)} | {"Y".ljust(changes_width)}\033[0m')
-                elif non_forced_english_subs and not forced_english_subs:
-                    print(f'{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"English".ljust(status_width)} | {"N".ljust(changes_width)}')
-                elif not non_forced_english_subs and not forced_english_subs:
-                    print(f'\033[91m{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"No Subtitles Found".ljust(status_width)} | {"N".ljust(changes_width)}\033[0m')
-                else:
-                    print(f'\033[91m{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"English (Forced)".ljust(status_width)} | {"N (Error)".ljust(changes_width)}\033[0m')
-
+                english_subs = movie.subtitleStreams()
+                if english_subs is not None:
+                    english_subs = [stream for stream in english_subs if stream is not None and stream.languageCode == 'eng']
+                    non_forced_english_subs = [stream for stream in english_subs if stream is not None and (not stream.forced or ('forced' not in getattr(stream, 'title', '').lower()))]
+                    forced_english_subs = [stream for stream in english_subs if stream is not None and (hasattr(stream, 'title') and stream.title is not None and 'forced' in stream.title.lower())]
+                    part = movie.media[0].parts[0]
+                    partsid = part.id
+                    if forced_english_subs and non_forced_english_subs:
+                        non_forced_english_subs[0].setDefault()
+                        print(f'\033[92m{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"English (Non-Forced)".ljust(status_width)} | {"Y".ljust(changes_width)}\033[0m')
+                    elif non_forced_english_subs and not forced_english_subs:
+                        print(f'{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"English".ljust(status_width)} | {"N".ljust(changes_width)}')
+                    elif not non_forced_english_subs and not forced_english_subs:
+                        print(f'\033[91m{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"No Subtitles Found".ljust(status_width)} | {"N".ljust(changes_width)}\033[0m')
+                    else:
+                        print(f'\033[91m{movie.title[:title_width].ljust(title_width)} | {str(movie.year).ljust(year_width)} | {"English (Forced)".ljust(status_width)} | {"N (Error)".ljust(changes_width)}\033[0m')
 
+    # Shows
     table_headers = ['Title', 'Year', 'Season #', 'Episode #', 'Status', 'Changes']
     title_width = 42
     year_width = 5
     season_width = 11
     episode_width = 11
     status_width = 20
     changes_width = 8
@@ -66,29 +66,27 @@
 
     print("\n" + "-" * 114 + "\nShows\n" + "-" * 114)
     print(f'\033[1m\033[96m{" | ".join([h.ljust(title_width if i == 0 else year_width if i == 1 else season_width if i == 2 else episode_width if i == 3 else status_width if i == 4 else changes_width) for i, h in enumerate(table_headers)])}\033[0m')
 
     for section in plex.library.sections():
         if section.type == 'show':
             for show in section.all():
-                show.reload()
                 for episode in show.episodes():
-                    show.reload()
-                    episode.reload()
-                    english_subs = [stream for stream in episode.subtitleStreams() if stream.languageCode == 'eng']
-                    non_forced_english_subs = [stream for stream in english_subs if not stream.forced or (hasattr(stream, 'title') and stream.title is not None and 'forced' not in stream.title.lower())]
-                    forced_english_subs = [stream for stream in english_subs if stream.forced or (hasattr(stream, 'title') and stream.title is not None and 'forced' in stream.title.lower())]
-                    part = episode.media[0].parts[0]
-                    partsid = part.id
-                    if forced_english_subs and non_forced_english_subs:
-                        non_forced_english_subs[0].setDefault()
-                        print(f'\033[92m{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"English (Non-Forced)".ljust(status_width)} | {"Y".ljust(changes_width)}\033[0m')
-                    elif non_forced_english_subs and not forced_english_subs:
-                        print(f'{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"English".ljust(status_width)} | {"N".ljust(changes_width)}')
-                    elif not non_forced_english_subs and not forced_english_subs and not forced_english_subs:
-                        print(f'\033[91m{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"No Subtitles Found".ljust(status_width)} | {"N".ljust(changes_width)}\033[0m')
-                    else:
-                        print(f'\033[91m{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"English (Forced)".ljust(status_width)} | {"N (Error)".ljust(changes_width)}\033[0m')
-
+                    english_subs = episode.subtitleStreams()
+                    if english_subs is not None:
+                        english_subs = [stream for stream in english_subs if stream is not None and stream.languageCode == 'eng']
+                        non_forced_english_subs = [stream for stream in english_subs if stream is not None and (not stream.forced or ('forced' not in getattr(stream, 'title', '').lower()))]
+                        forced_english_subs = [stream for stream in english_subs if stream is not None and (hasattr(stream, 'title') and stream.title is not None and 'forced' in stream.title.lower())]
+                        part = episode.media[0].parts[0]
+                        partsid = part.id
+                        if forced_english_subs and non_forced_english_subs:
+                            non_forced_english_subs[0].setDefault()
+                            print(f'\033[92m{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"English (Non-Forced)".ljust(status_width)} | {"Y".ljust(changes_width)}\033[0m')
+                        elif non_forced_english_subs and not forced_english_subs:
+                            print(f'{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"English".ljust(status_width)} | {"N".ljust(changes_width)}')
+                        elif not non_forced_english_subs and not forced_english_subs:
+                            print(f'\033[91m{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"No Subtitles Found".ljust(status_width)} | {"N".ljust(changes_width)}\033[0m')
+                        else:
+                            print(f'\033[91m{show.title[:title_width].ljust(title_width)} | {str(show.year).ljust(year_width)} | {"Season " + str(episode.seasonNumber).ljust(season_row_width)} | {"Episode " + str(episode.index).ljust(episode_row_width)} | {"English (Forced)".ljust(status_width)} | {"N (Error)".ljust(changes_width)}\033[0m')
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `PlexPreferNonForcedSubs-2.1.2/PlexPreferNonForcedSubs.egg-info/PKG-INFO` & `PlexPreferNonForcedSubs-2.1.3/PlexPreferNonForcedSubs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexPreferNonForcedSubs
-Version: 2.1.2
+Version: 2.1.3
 Summary: This script will set all movies and shows in your local Plex library to English non forced subtitles by default.
 Home-page: https://github.com/RileyXX/PlexPreferNonForcedSubs
 Keywords: python,video,plex,subtitles,subs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 License-File: LICENSE
 
 
 # PlexPreferNonForcedSubs
 
 
 ## Short description:
-This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices.
+This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices. This script should work on any OS where Python is installed (Windows, MacOS and Linux etc).
 
 ## Long description:
 This script was created with the help of [ChatGPT Open AI](https://chat.openai.com/chat) and further edited and completed by me. It uses [Plex Python Api](https://python-plexapi.readthedocs.io/en/latest/). It will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices. Assuming your Plex subtitles settings are setup in your server settings Plex will default to Forced Subtitles by default when they are available for a given item. Plex will not allow you to prefer non forced subtitles natively hence why this script was created.
 
 This script is confirmed tested and working. Feel free to use this code for your own purposes. I will be running this code periodically on my home server along with some of my other neat little plex scripts like [Plex Auto Delete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py). Thanks to [all](https://stackoverflow.com/questions/75027919/python-script-to-set-all-subtitles-for-movies-shows-in-plex-to-english-non-for) who helped! If you use this script and run into any bugs feel free to open an issue. Cheers!
 
 ## What are "non-forced" subtitles?
@@ -31,41 +31,49 @@
 
 
 ## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/).
 2. Run `python -m pip install PlexPreferNonForcedSubs` in command line.
 3. Make sure Plex media server is running then run the script using `PlexPreferNonForcedSubs` in command line.
 4. On first run the script will ask you to fill in your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). Your token will be saved locally in the same folder as token.txt.
-5. Done
+5. Done.
 
-_Note: This script should work on any OS where Python is installed (Windows, MacOS and Linux etc)._
+_See [below](https://github.com/RileyXX/PlexPreferNonForcedSubs#run) for details on how to run, update and uninstall._
 
 ### Run:
 `PlexPreferNonForcedSubs` in command line.
 
 ### Update:
 `python -m pip install PlexPreferNonForcedSubs --upgrade` in command line.
 ### Uninstall:
 `python -m pip uninstall PlexPreferNonForcedSubs` in command line.
 
+## Alternative manual no install method:
+1. Download the latest .py script from the [releases page](https://github.com/RileyXX/PlexPreferNonForcedSubs/releases) and move it to the file directory of your choice.
+2. Run the script by running `PlexPreferNonForcedSubs.py` OR open terminal and navigate to folder where `PlexPreferNonForcedSubs.py` is located. Run `PlexPreferNonForcedSubs.py` in terminal. 
+4. On first run the script will ask you to fill in your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). Your token will be saved locally in the same folder as token.txt.
+3. Done.
+
+_See [above](https://github.com/RileyXX/PlexPreferNonForcedSubs#run) for details on how to run, update and uninstall._
+
 ## Known issues/future outlook:
 * Several lines of redundant code can be shortened and/or removed
 
 ## Also posted on:
 * [Stackoverflow](https://stackoverflow.com/q/75027919/9196825)
 * [Reddit](https://www.reddit.com/r/PleX/comments/105gdh7/python_code_to_set_all_movies_and_shows_in_plex/)
 * [Plex Forums](https://forums.plex.tv/t/python-script-to-set-all-movies-and-shows-in-plex-to-use-english-non-forced-subtitles/825871)
 
 ## Screenshots:
 ##### Plex subtitle dropdown after script is done running:
 ![Plex Subtitle Dropdown](https://i.imgur.com/BNOlwtL.png)
 ##### PlexPreferNonForcedSubs.py script in action:
 ![PlexPreferNonForcedSubs.py Script in Action](https://github.com/RileyXX/PlexPreferNonForcedSubs/raw/main/demo.gif)
 
-## Donations, Sponsorships and Custom Projects:
+## Sponsorships, Donations and Custom Projects:
 Like my scripts? Become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! See below for other donation options. Need help with a project? Open an issue and I will try my best to help! For other inquiries and custom projects contact me on [Twitter](https://twitter.com/RileyxBell).
 
 #### More donation options:
 - Cashapp: `$rileyxx`
 - Venmo: `@rileyxx`
 - Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
```

### Comparing `PlexPreferNonForcedSubs-2.1.2/README.md` & `PlexPreferNonForcedSubs-2.1.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PlexPreferNonForcedSubs
 
 
 ## Short description:
-This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices.
+This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices. This script should work on any OS where Python is installed (Windows, MacOS and Linux etc).
 
 ## Long description:
 This script was created with the help of [ChatGPT Open AI](https://chat.openai.com/chat) and further edited and completed by me. It uses [Plex Python Api](https://python-plexapi.readthedocs.io/en/latest/). It will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices. Assuming your Plex subtitles settings are setup in your server settings Plex will default to Forced Subtitles by default when they are available for a given item. Plex will not allow you to prefer non forced subtitles natively hence why this script was created.
 
 This script is confirmed tested and working. Feel free to use this code for your own purposes. I will be running this code periodically on my home server along with some of my other neat little plex scripts like [Plex Auto Delete](https://github.com/Casvt/Plex-scripts/blob/main/changing_settings/plex_auto_delete.py). Thanks to [all](https://stackoverflow.com/questions/75027919/python-script-to-set-all-subtitles-for-movies-shows-in-plex-to-english-non-for) who helped! If you use this script and run into any bugs feel free to open an issue. Cheers!
 
 ## What are "non-forced" subtitles?
@@ -17,41 +17,49 @@
 
 
 ## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/).
 2. Run `python -m pip install PlexPreferNonForcedSubs` in command line.
 3. Make sure Plex media server is running then run the script using `PlexPreferNonForcedSubs` in command line.
 4. On first run the script will ask you to fill in your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). Your token will be saved locally in the same folder as token.txt.
-5. Done
+5. Done.
 
-_Note: This script should work on any OS where Python is installed (Windows, MacOS and Linux etc)._
+_See [below](https://github.com/RileyXX/PlexPreferNonForcedSubs#run) for details on how to run, update and uninstall._
 
 ### Run:
 `PlexPreferNonForcedSubs` in command line.
 
 ### Update:
 `python -m pip install PlexPreferNonForcedSubs --upgrade` in command line.
 ### Uninstall:
 `python -m pip uninstall PlexPreferNonForcedSubs` in command line.
 
+## Alternative manual no install method:
+1. Download the latest .py script from the [releases page](https://github.com/RileyXX/PlexPreferNonForcedSubs/releases) and move it to the file directory of your choice.
+2. Run the script by running `PlexPreferNonForcedSubs.py` OR open terminal and navigate to folder where `PlexPreferNonForcedSubs.py` is located. Run `PlexPreferNonForcedSubs.py` in terminal. 
+4. On first run the script will ask you to fill in your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). Your token will be saved locally in the same folder as token.txt.
+3. Done.
+
+_See [above](https://github.com/RileyXX/PlexPreferNonForcedSubs#run) for details on how to run, update and uninstall._
+
 ## Known issues/future outlook:
 * Several lines of redundant code can be shortened and/or removed
 
 ## Also posted on:
 * [Stackoverflow](https://stackoverflow.com/q/75027919/9196825)
 * [Reddit](https://www.reddit.com/r/PleX/comments/105gdh7/python_code_to_set_all_movies_and_shows_in_plex/)
 * [Plex Forums](https://forums.plex.tv/t/python-script-to-set-all-movies-and-shows-in-plex-to-use-english-non-forced-subtitles/825871)
 
 ## Screenshots:
 ##### Plex subtitle dropdown after script is done running:
 ![Plex Subtitle Dropdown](https://i.imgur.com/BNOlwtL.png)
 ##### PlexPreferNonForcedSubs.py script in action:
 ![PlexPreferNonForcedSubs.py Script in Action](https://github.com/RileyXX/PlexPreferNonForcedSubs/raw/main/demo.gif)
 
-## Donations, Sponsorships and Custom Projects:
+## Sponsorships, Donations and Custom Projects:
 Like my scripts? Become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! See below for other donation options. Need help with a project? Open an issue and I will try my best to help! For other inquiries and custom projects contact me on [Twitter](https://twitter.com/RileyxBell).
 
 #### More donation options:
 - Cashapp: `$rileyxx`
 - Venmo: `@rileyxx`
 - Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
```

### Comparing `PlexPreferNonForcedSubs-2.1.2/setup.py` & `PlexPreferNonForcedSubs-2.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '2.1.2'
+VERSION = '2.1.3'
 DESCRIPTION = 'This script will set all movies and shows in your local Plex library to English non forced subtitles by default.'
 LONG_DESCRIPTION = 'This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices.'
 
 # Setting up
 setup(
     name="PlexPreferNonForcedSubs",
     version=VERSION,
```

