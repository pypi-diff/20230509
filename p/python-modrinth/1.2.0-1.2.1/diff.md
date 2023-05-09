# Comparing `tmp/python-modrinth-1.2.0.tar.gz` & `tmp/python-modrinth-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-modrinth-1.2.0.tar", last modified: Sun Apr 30 22:10:50 2023, max compression
+gzip compressed data, was "python-modrinth-1.2.1.tar", last modified: Tue May  9 21:24:47 2023, max compression
```

## Comparing `python-modrinth-1.2.0.tar` & `python-modrinth-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:10:50.672475 python-modrinth-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-30 22:10:50.672475 python-modrinth-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-30 22:10:50.672475 python-modrinth-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:10:50.668475 python-modrinth-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:10:50.672475 python-modrinth-1.2.0/src/pyrinth/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/modrinth.py
--rw-r--r--   0 runner    (1001) docker     (123)    50360 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/teams.py
--rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-30 22:10:32.000000 python-modrinth-1.2.0/src/pyrinth/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 22:10:50.672475 python-modrinth-1.2.0/src/python_modrinth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-30 22:10:50.000000 python-modrinth-1.2.0/src/python_modrinth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-30 22:10:50.000000 python-modrinth-1.2.0/src/python_modrinth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 22:10:50.000000 python-modrinth-1.2.0/src/python_modrinth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-30 22:10:50.000000 python-modrinth-1.2.0/src/python_modrinth.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 21:24:47.617307 python-modrinth-1.2.1/
+-rw-rw-rw-   0        0        0     1095 2023-05-09 21:21:44.000000 python-modrinth-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     6430 2023-05-09 21:24:47.617307 python-modrinth-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5866 2023-05-09 21:21:44.000000 python-modrinth-1.2.1/README.md
+-rw-rw-rw-   0        0        0      277 2023-05-09 21:21:44.000000 python-modrinth-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      703 2023-05-09 21:24:47.618307 python-modrinth-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-09 21:24:47.602178 python-modrinth-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-09 21:24:47.613179 python-modrinth-1.2.1/src/pyrinth/
+-rw-rw-rw-   0        0        0      214 2023-05-09 21:21:44.000000 python-modrinth-1.2.1/src/pyrinth/__init__.py
+-rw-rw-rw-   0        0        0      709 2023-05-09 21:21:44.000000 python-modrinth-1.2.1/src/pyrinth/exceptions.py
+-rw-rw-rw-   0        0        0     1053 2023-05-09 21:21:44.000000 python-modrinth-1.2.1/src/pyrinth/literals.py
+-rw-rw-rw-   0        0        0    18572 2023-05-09 21:21:44.000000 python-modrinth-1.2.1/src/pyrinth/models.py
+-rw-rw-rw-   0        0        0     2569 2023-05-09 21:21:44.000000 python-modrinth-1.2.1/src/pyrinth/modrinth.py
+-rw-rw-rw-   0        0        0    51777 2023-05-09 21:21:44.000000 python-modrinth-1.2.1/src/pyrinth/projects.py
+-rw-rw-rw-   0        0        0     8678 2023-05-09 21:21:44.000000 python-modrinth-1.2.1/src/pyrinth/tags.py
+-rw-rw-rw-   0        0        0     2868 2023-05-09 21:21:44.000000 python-modrinth-1.2.1/src/pyrinth/teams.py
+-rw-rw-rw-   0        0        0    13518 2023-05-09 21:21:44.000000 python-modrinth-1.2.1/src/pyrinth/users.py
+-rw-rw-rw-   0        0        0     1503 2023-05-09 21:21:44.000000 python-modrinth-1.2.1/src/pyrinth/util.py
+drwxrwxrwx   0        0        0        0 2023-05-09 21:24:47.616307 python-modrinth-1.2.1/src/python_modrinth.egg-info/
+-rw-rw-rw-   0        0        0     6430 2023-05-09 21:24:47.000000 python-modrinth-1.2.1/src/python_modrinth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-05-09 21:24:47.000000 python-modrinth-1.2.1/src/python_modrinth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 21:24:47.000000 python-modrinth-1.2.1/src/python_modrinth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-09 21:24:47.000000 python-modrinth-1.2.1/src/python_modrinth.egg-info/top_level.txt
```

### Comparing `python-modrinth-1.2.0/LICENSE` & `python-modrinth-1.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Revolving Madness
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Revolving Madness
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `python-modrinth-1.2.0/PKG-INFO` & `python-modrinth-1.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,185 +1,170 @@
-Metadata-Version: 2.1
-Name: python-modrinth
-Version: 1.2.0
-Summary: A Python library that interacts with the Modrinth API
-Home-page: https://github.com/RevolvingMadness/Pyrinth
-Author: RevolvingMadness
-Author-email: revolvingmad@gmail.com
-Project-URL: Bug Tracker, https://github.com/RevolvingMadness/Pyrinth/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<div align="center">
-
-<div id="user-content-toc">
-  <ul>
-    <img src="pyrinth.png" width="64" height="64"/>
-    <summary><h1>Pyrinth</h1></summary>
-  </ul>
-</div>
-
-  <p>
-    Interacts with the Modrinth API
-    <br />
-    <a href="https://github.com/RevolvingMadness/Pyrinth"><strong>Explore the docs »</strong></a>
-    <br />
-    <br />
-    <a href="https://github.com/RevolvingMadness/Pyrinth/issues">Report Bug</a>
-    ·
-    <a href="https://github.com/RevolvingMadness/Pyrinth/issues">Request Feature</a>
-  </p>
-
-[![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
-[![Apache License][license-shield]][license-url]
-</div>
-<br />
-
-
-## Getting Started
-
-### Prerequisites
-
-To use Pyrinth you need the following:
-- [Python](https://www.python.org/downloads)
-- pip (Comes with Python)
-
-### Installation
-
-#### Automatic Installation
-
-To automatically install the latest version of Pyrinth, run this command in the terminal:
-```sh
-pip install python-modrinth
-```
----
-
-#### Manual Installation
-If you want to get the latest beta or pre-releases, follow the steps below:
-1. Go to the [releases page](https://github.com/RevolvingMadness/Pyrinth/releases/) and download one of the `.whl` files.
-2. Open a terminal and go to the downloads directory.
-3. Type this: `pip install pyrinth`, then press tab and it should autocomplete.
-
-## Issues
-
-If you find a bug, please check if the issue already exists, otherwise open an issue through [this](https://github.com/RevolvingMadness/Pyrinth/issues) link.
-
-
-
-## Contributing
-
-### Creating A Fork And Pull Request
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
-
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".  
-Don't forget to give the project a star! Thanks again!
-
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
-
-## Using Pyrinth Source Code
-When you're using the Pyrinth source code, navigate to the `src` directory and create your main Python file.
-
-
-
-
-
-## License
-
-This project is distributed under the MIT License. See `LICENSE` for more information.
-
-## Contact
-
-Project Link: https://github.com/RevolvingMadness/Pyrinth 
-Discord Server: Coming Soon!
-
-## To-Do
-- Projects
-  - [x] Search Projects
-  - [x] Get a project
-  - [x] Modify a project
-  - [x] Delete a project
-  - [x] Get multiple projects
-  - [x] Edit multiple projects
-  - [x] Get a list of random projects
-  - [x] Create a project
-  - [x] Change project's icon
-  - [x] Delete projcet's icon
-  - [x] Check project slug/ID validity
-  - [x] Add a gallery image
-  - [x] Modify a gallery image
-  - [x] Delete a gallery image
-  - [x] Get all of a project's dependencies
-  - [x] Follow a project
-  - [x] Unfollow a project
-  - [ ] Schedule a project
-- Versions
-  - [x] List project's versions
-  - [x] Get a version
-  - [x] Modify a version
-  - [x] Delete a version
-  - [x] Create a version
-  - [ ] Schedule a version
-  - [x] Get multipe versions
-  - [ ] Add files to version
-- Version Files
-  - [x] Get version from hash
-  - [x] Delete a file from its hash
-  - [ ] Latest version of a project from a has, loader(s), and game version(s)
-  - [ ] Get versions from hashes
-  - [ ] Latest versions multiple project from hashes, loader(s), and game version(s)
-- Users - Complete
-  - [x] Get a user
-  - [x] Modify a user
-  - [x] Delete a user
-  - [x] Get user from authorization header
-  - [x] Get multiple users
-  - [x] Change user's avatar
-  - [x] Get user's projects
-  - [x] Get user's notifications
-  - [x] Get user's followed projects
-  - [x] Get user's payout history
-  - [x] Withdraw payout balance to PayPal or Venmo
-- Teams
-  - [x] Get a project's team members
-  - [x] Get a team's members
-  - [ ] Add a user to a team
-  - [x] Get the members of multiple teams
-  - [ ] Join a team
-  - [ ] Modify a team member's information
-  - [ ] Remove a team member from a team
-  - [ ] Transfer team's ownership to another user
-- Tags - Complete
-  - [x] Get a list of categories
-  - [x] Get a list of loaders
-  - [x] Get a list of game versions
-  - [x] Get a list of licenses
-  - [x] Get a list of donation platforms
-  - [x] Get a list of report types
-- Miscellaneous
-  - [ ] Report a project, user, or version
-  - [x] Various statistics about this Modrinth instance
-
-## Documentation
-You can find the documentation [here](https://revolvingmadness.github.io/Pyrinth)
-
-
-[contributors-shield]: https://img.shields.io/github/contributors/RevolvingMadness/Pyrinth.svg?style=for-the-badge
-[contributors-url]: https://github.com/RevolvingMadness/Pyrinth/graphs/contributors
-[forks-shield]: https://img.shields.io/github/forks/RevolvingMadness/Pyrinth.svg?style=for-the-badge
-[forks-url]: https://github.com/RevolvingMadness/Pyrinth/network/members
-[stars-shield]: https://img.shields.io/github/stars/RevolvingMadness/Pyrinth.svg?style=for-the-badge
-[stars-url]: https://github.com/RevolvingMadness/Pyrinth/stargazers
-[issues-shield]: https://img.shields.io/github/issues/RevolvingMadness/Pyrinth.svg?style=for-the-badge
-[issues-url]: https://github.com/RevolvingMadness/Pyrinth/issues
-[license-shield]: https://img.shields.io/github/license/RevolvingMadness/Pyrinth.svg?style=for-the-badge
-[license-url]: https://github.com/RevolvingMadness/Pyrinth/LICENSE.txt
+<div align="center">
+
+<div id="user-content-toc">
+  <ul>
+    <img src="pyrinth.png" width="64" height="64"/>
+    <summary><h1>Pyrinth</h1></summary>
+  </ul>
+</div>
+
+  <p>
+    Interacts with the Modrinth API
+    <br />
+    <a href="https://github.com/RevolvingMadness/Pyrinth"><strong>Explore the docs »</strong></a>
+    <br />
+    <br />
+    <a href="https://github.com/RevolvingMadness/Pyrinth/issues">Report Bug</a>
+    ·
+    <a href="https://github.com/RevolvingMadness/Pyrinth/issues">Request Feature</a>
+  </p>
+
+[![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
+[![Apache License][license-shield]][license-url]
+</div>
+<br />
+
+
+## Getting Started
+
+### Prerequisites
+
+To use Pyrinth you need the following:
+- [Python](https://www.python.org/downloads)
+- pip (Comes with Python)
+
+### Installation
+
+#### Automatic Installation
+
+To automatically install the latest version of Pyrinth, run this command in the terminal:
+```sh
+pip install python-modrinth
+```
+---
+
+#### Manual Installation
+If you want to get the latest beta or pre-releases, follow the steps below:
+1. Go to the [releases page](https://github.com/RevolvingMadness/Pyrinth/releases/) and download one of the `.whl` files.
+2. Open a terminal and go to the downloads directory.
+3. Type this: `pip install pyrinth`, then press tab and it should autocomplete.
+
+## Issues
+
+If you find a bug, please check if the issue already exists, otherwise open an issue through [this](https://github.com/RevolvingMadness/Pyrinth/issues) link.
+
+
+
+## Contributing
+
+### Creating A Fork And Pull Request
+Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".  
+Don't forget to give the project a star! Thanks again!
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+## Using Pyrinth Source Code
+When you're using the Pyrinth source code, navigate to the `src` directory and create your main Python file.
+
+
+
+
+
+## License
+
+This project is distributed under the MIT License. See `LICENSE` for more information.
+
+## Contact
+
+Project Link: https://github.com/RevolvingMadness/Pyrinth 
+Discord Server: Coming Soon!
+
+## To-Do
+- Projects
+  - [x] Search Projects
+  - [x] Get a project
+  - [x] Modify a project
+  - [x] Delete a project
+  - [x] Get multiple projects
+  - [x] Edit multiple projects
+  - [x] Get a list of random projects
+  - [x] Create a project
+  - [x] Change project's icon
+  - [x] Delete projcet's icon
+  - [x] Check project slug/ID validity
+  - [x] Add a gallery image
+  - [x] Modify a gallery image
+  - [x] Delete a gallery image
+  - [x] Get all of a project's dependencies
+  - [x] Follow a project
+  - [x] Unfollow a project
+  - [ ] Schedule a project
+- Versions
+  - [x] List project's versions
+  - [x] Get a version
+  - [x] Modify a version
+  - [x] Delete a version
+  - [x] Create a version
+  - [ ] Schedule a version
+  - [x] Get multipe versions
+  - [ ] Add files to version
+- Version Files
+  - [x] Get version from hash
+  - [x] Delete a file from its hash
+  - [ ] Latest version of a project from a has, loader(s), and game version(s)
+  - [ ] Get versions from hashes
+  - [ ] Latest versions multiple project from hashes, loader(s), and game version(s)
+- Users - Complete
+  - [x] Get a user
+  - [x] Modify a user
+  - [x] Delete a user
+  - [x] Get user from authorization header
+  - [x] Get multiple users
+  - [x] Change user's avatar
+  - [x] Get user's projects
+  - [x] Get user's notifications
+  - [x] Get user's followed projects
+  - [x] Get user's payout history
+  - [x] Withdraw payout balance to PayPal or Venmo
+- Teams
+  - [x] Get a project's team members
+  - [x] Get a team's members
+  - [ ] Add a user to a team
+  - [x] Get the members of multiple teams
+  - [ ] Join a team
+  - [ ] Modify a team member's information
+  - [ ] Remove a team member from a team
+  - [ ] Transfer team's ownership to another user
+- Tags - Complete
+  - [x] Get a list of categories
+  - [x] Get a list of loaders
+  - [x] Get a list of game versions
+  - [x] Get a list of licenses
+  - [x] Get a list of donation platforms
+  - [x] Get a list of report types
+- Miscellaneous
+  - [ ] Report a project, user, or version
+  - [x] Various statistics about this Modrinth instance
+
+## Documentation
+You can find the documentation [here](https://revolvingmadness.github.io/Pyrinth)
+
+
+[contributors-shield]: https://img.shields.io/github/contributors/RevolvingMadness/Pyrinth.svg?style=for-the-badge
+[contributors-url]: https://github.com/RevolvingMadness/Pyrinth/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/RevolvingMadness/Pyrinth.svg?style=for-the-badge
+[forks-url]: https://github.com/RevolvingMadness/Pyrinth/network/members
+[stars-shield]: https://img.shields.io/github/stars/RevolvingMadness/Pyrinth.svg?style=for-the-badge
+[stars-url]: https://github.com/RevolvingMadness/Pyrinth/stargazers
+[issues-shield]: https://img.shields.io/github/issues/RevolvingMadness/Pyrinth.svg?style=for-the-badge
+[issues-url]: https://github.com/RevolvingMadness/Pyrinth/issues
+[license-shield]: https://img.shields.io/github/license/RevolvingMadness/Pyrinth.svg?style=for-the-badge
+[license-url]: https://github.com/RevolvingMadness/Pyrinth/LICENSE.txt
```

#### html2text {}

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1 Name: python-modrinth Version: 1.2.0 Summary: A Python
-library that interacts with the Modrinth API Home-page: https://github.com/
-RevolvingMadness/Pyrinth Author: RevolvingMadness Author-email:
-revolvingmad@gmail.com Project-URL: Bug Tracker, https://github.com/
-RevolvingMadness/Pyrinth/issues Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.11 Description-Content-Type: text/
-markdown License-File: LICENSE
     * [pyrinth.png]
                              ****** Pyrinth ******
 Interacts with the Modrinth API
 Explore_the_docs_Â»
 
 Report_Bug Â· Request_Feature
 [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
```

### Comparing `python-modrinth-1.2.0/README.md` & `python-modrinth-1.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,170 +1,185 @@
-<div align="center">
-
-<div id="user-content-toc">
-  <ul>
-    <img src="pyrinth.png" width="64" height="64"/>
-    <summary><h1>Pyrinth</h1></summary>
-  </ul>
-</div>
-
-  <p>
-    Interacts with the Modrinth API
-    <br />
-    <a href="https://github.com/RevolvingMadness/Pyrinth"><strong>Explore the docs »</strong></a>
-    <br />
-    <br />
-    <a href="https://github.com/RevolvingMadness/Pyrinth/issues">Report Bug</a>
-    ·
-    <a href="https://github.com/RevolvingMadness/Pyrinth/issues">Request Feature</a>
-  </p>
-
-[![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
-[![Apache License][license-shield]][license-url]
-</div>
-<br />
-
-
-## Getting Started
-
-### Prerequisites
-
-To use Pyrinth you need the following:
-- [Python](https://www.python.org/downloads)
-- pip (Comes with Python)
-
-### Installation
-
-#### Automatic Installation
-
-To automatically install the latest version of Pyrinth, run this command in the terminal:
-```sh
-pip install python-modrinth
-```
----
-
-#### Manual Installation
-If you want to get the latest beta or pre-releases, follow the steps below:
-1. Go to the [releases page](https://github.com/RevolvingMadness/Pyrinth/releases/) and download one of the `.whl` files.
-2. Open a terminal and go to the downloads directory.
-3. Type this: `pip install pyrinth`, then press tab and it should autocomplete.
-
-## Issues
-
-If you find a bug, please check if the issue already exists, otherwise open an issue through [this](https://github.com/RevolvingMadness/Pyrinth/issues) link.
-
-
-
-## Contributing
-
-### Creating A Fork And Pull Request
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
-
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".  
-Don't forget to give the project a star! Thanks again!
-
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
-
-## Using Pyrinth Source Code
-When you're using the Pyrinth source code, navigate to the `src` directory and create your main Python file.
-
-
-
-
-
-## License
-
-This project is distributed under the MIT License. See `LICENSE` for more information.
-
-## Contact
-
-Project Link: https://github.com/RevolvingMadness/Pyrinth 
-Discord Server: Coming Soon!
-
-## To-Do
-- Projects
-  - [x] Search Projects
-  - [x] Get a project
-  - [x] Modify a project
-  - [x] Delete a project
-  - [x] Get multiple projects
-  - [x] Edit multiple projects
-  - [x] Get a list of random projects
-  - [x] Create a project
-  - [x] Change project's icon
-  - [x] Delete projcet's icon
-  - [x] Check project slug/ID validity
-  - [x] Add a gallery image
-  - [x] Modify a gallery image
-  - [x] Delete a gallery image
-  - [x] Get all of a project's dependencies
-  - [x] Follow a project
-  - [x] Unfollow a project
-  - [ ] Schedule a project
-- Versions
-  - [x] List project's versions
-  - [x] Get a version
-  - [x] Modify a version
-  - [x] Delete a version
-  - [x] Create a version
-  - [ ] Schedule a version
-  - [x] Get multipe versions
-  - [ ] Add files to version
-- Version Files
-  - [x] Get version from hash
-  - [x] Delete a file from its hash
-  - [ ] Latest version of a project from a has, loader(s), and game version(s)
-  - [ ] Get versions from hashes
-  - [ ] Latest versions multiple project from hashes, loader(s), and game version(s)
-- Users - Complete
-  - [x] Get a user
-  - [x] Modify a user
-  - [x] Delete a user
-  - [x] Get user from authorization header
-  - [x] Get multiple users
-  - [x] Change user's avatar
-  - [x] Get user's projects
-  - [x] Get user's notifications
-  - [x] Get user's followed projects
-  - [x] Get user's payout history
-  - [x] Withdraw payout balance to PayPal or Venmo
-- Teams
-  - [x] Get a project's team members
-  - [x] Get a team's members
-  - [ ] Add a user to a team
-  - [x] Get the members of multiple teams
-  - [ ] Join a team
-  - [ ] Modify a team member's information
-  - [ ] Remove a team member from a team
-  - [ ] Transfer team's ownership to another user
-- Tags - Complete
-  - [x] Get a list of categories
-  - [x] Get a list of loaders
-  - [x] Get a list of game versions
-  - [x] Get a list of licenses
-  - [x] Get a list of donation platforms
-  - [x] Get a list of report types
-- Miscellaneous
-  - [ ] Report a project, user, or version
-  - [x] Various statistics about this Modrinth instance
-
-## Documentation
-You can find the documentation [here](https://revolvingmadness.github.io/Pyrinth)
-
-
-[contributors-shield]: https://img.shields.io/github/contributors/RevolvingMadness/Pyrinth.svg?style=for-the-badge
-[contributors-url]: https://github.com/RevolvingMadness/Pyrinth/graphs/contributors
-[forks-shield]: https://img.shields.io/github/forks/RevolvingMadness/Pyrinth.svg?style=for-the-badge
-[forks-url]: https://github.com/RevolvingMadness/Pyrinth/network/members
-[stars-shield]: https://img.shields.io/github/stars/RevolvingMadness/Pyrinth.svg?style=for-the-badge
-[stars-url]: https://github.com/RevolvingMadness/Pyrinth/stargazers
-[issues-shield]: https://img.shields.io/github/issues/RevolvingMadness/Pyrinth.svg?style=for-the-badge
-[issues-url]: https://github.com/RevolvingMadness/Pyrinth/issues
-[license-shield]: https://img.shields.io/github/license/RevolvingMadness/Pyrinth.svg?style=for-the-badge
-[license-url]: https://github.com/RevolvingMadness/Pyrinth/LICENSE.txt
+Metadata-Version: 2.1
+Name: python-modrinth
+Version: 1.2.1
+Summary: A Python library that interacts with the Modrinth API
+Home-page: https://github.com/RevolvingMadness/Pyrinth
+Author: RevolvingMadness
+Author-email: revolvingmad@gmail.com
+Project-URL: Bug Tracker, https://github.com/RevolvingMadness/Pyrinth/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+
+<div id="user-content-toc">
+  <ul>
+    <img src="pyrinth.png" width="64" height="64"/>
+    <summary><h1>Pyrinth</h1></summary>
+  </ul>
+</div>
+
+  <p>
+    Interacts with the Modrinth API
+    <br />
+    <a href="https://github.com/RevolvingMadness/Pyrinth"><strong>Explore the docs »</strong></a>
+    <br />
+    <br />
+    <a href="https://github.com/RevolvingMadness/Pyrinth/issues">Report Bug</a>
+    ·
+    <a href="https://github.com/RevolvingMadness/Pyrinth/issues">Request Feature</a>
+  </p>
+
+[![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
+[![Apache License][license-shield]][license-url]
+</div>
+<br />
+
+
+## Getting Started
+
+### Prerequisites
+
+To use Pyrinth you need the following:
+- [Python](https://www.python.org/downloads)
+- pip (Comes with Python)
+
+### Installation
+
+#### Automatic Installation
+
+To automatically install the latest version of Pyrinth, run this command in the terminal:
+```sh
+pip install python-modrinth
+```
+---
+
+#### Manual Installation
+If you want to get the latest beta or pre-releases, follow the steps below:
+1. Go to the [releases page](https://github.com/RevolvingMadness/Pyrinth/releases/) and download one of the `.whl` files.
+2. Open a terminal and go to the downloads directory.
+3. Type this: `pip install pyrinth`, then press tab and it should autocomplete.
+
+## Issues
+
+If you find a bug, please check if the issue already exists, otherwise open an issue through [this](https://github.com/RevolvingMadness/Pyrinth/issues) link.
+
+
+
+## Contributing
+
+### Creating A Fork And Pull Request
+Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".  
+Don't forget to give the project a star! Thanks again!
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+## Using Pyrinth Source Code
+When you're using the Pyrinth source code, navigate to the `src` directory and create your main Python file.
+
+
+
+
+
+## License
+
+This project is distributed under the MIT License. See `LICENSE` for more information.
+
+## Contact
+
+Project Link: https://github.com/RevolvingMadness/Pyrinth 
+Discord Server: Coming Soon!
+
+## To-Do
+- Projects
+  - [x] Search Projects
+  - [x] Get a project
+  - [x] Modify a project
+  - [x] Delete a project
+  - [x] Get multiple projects
+  - [x] Edit multiple projects
+  - [x] Get a list of random projects
+  - [x] Create a project
+  - [x] Change project's icon
+  - [x] Delete projcet's icon
+  - [x] Check project slug/ID validity
+  - [x] Add a gallery image
+  - [x] Modify a gallery image
+  - [x] Delete a gallery image
+  - [x] Get all of a project's dependencies
+  - [x] Follow a project
+  - [x] Unfollow a project
+  - [ ] Schedule a project
+- Versions
+  - [x] List project's versions
+  - [x] Get a version
+  - [x] Modify a version
+  - [x] Delete a version
+  - [x] Create a version
+  - [ ] Schedule a version
+  - [x] Get multipe versions
+  - [ ] Add files to version
+- Version Files
+  - [x] Get version from hash
+  - [x] Delete a file from its hash
+  - [ ] Latest version of a project from a has, loader(s), and game version(s)
+  - [ ] Get versions from hashes
+  - [ ] Latest versions multiple project from hashes, loader(s), and game version(s)
+- Users - Complete
+  - [x] Get a user
+  - [x] Modify a user
+  - [x] Delete a user
+  - [x] Get user from authorization header
+  - [x] Get multiple users
+  - [x] Change user's avatar
+  - [x] Get user's projects
+  - [x] Get user's notifications
+  - [x] Get user's followed projects
+  - [x] Get user's payout history
+  - [x] Withdraw payout balance to PayPal or Venmo
+- Teams
+  - [x] Get a project's team members
+  - [x] Get a team's members
+  - [ ] Add a user to a team
+  - [x] Get the members of multiple teams
+  - [ ] Join a team
+  - [ ] Modify a team member's information
+  - [ ] Remove a team member from a team
+  - [ ] Transfer team's ownership to another user
+- Tags - Complete
+  - [x] Get a list of categories
+  - [x] Get a list of loaders
+  - [x] Get a list of game versions
+  - [x] Get a list of licenses
+  - [x] Get a list of donation platforms
+  - [x] Get a list of report types
+- Miscellaneous
+  - [ ] Report a project, user, or version
+  - [x] Various statistics about this Modrinth instance
+
+## Documentation
+You can find the documentation [here](https://revolvingmadness.github.io/Pyrinth)
+
+
+[contributors-shield]: https://img.shields.io/github/contributors/RevolvingMadness/Pyrinth.svg?style=for-the-badge
+[contributors-url]: https://github.com/RevolvingMadness/Pyrinth/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/RevolvingMadness/Pyrinth.svg?style=for-the-badge
+[forks-url]: https://github.com/RevolvingMadness/Pyrinth/network/members
+[stars-shield]: https://img.shields.io/github/stars/RevolvingMadness/Pyrinth.svg?style=for-the-badge
+[stars-url]: https://github.com/RevolvingMadness/Pyrinth/stargazers
+[issues-shield]: https://img.shields.io/github/issues/RevolvingMadness/Pyrinth.svg?style=for-the-badge
+[issues-url]: https://github.com/RevolvingMadness/Pyrinth/issues
+[license-shield]: https://img.shields.io/github/license/RevolvingMadness/Pyrinth.svg?style=for-the-badge
+[license-url]: https://github.com/RevolvingMadness/Pyrinth/LICENSE.txt
```

#### html2text {}

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1 Name: python-modrinth Version: 1.2.1 Summary: A Python
+library that interacts with the Modrinth API Home-page: https://github.com/
+RevolvingMadness/Pyrinth Author: RevolvingMadness Author-email:
+revolvingmad@gmail.com Project-URL: Bug Tracker, https://github.com/
+RevolvingMadness/Pyrinth/issues Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.11 Description-Content-Type: text/
+markdown License-File: LICENSE
     * [pyrinth.png]
                              ****** Pyrinth ******
 Interacts with the Modrinth API
 Explore_the_docs_Â»
 
 Report_Bug Â· Request_Feature
 [![Contributors][contributors-shield]][contributors-url] [![Forks][forks-
```

### Comparing `python-modrinth-1.2.0/src/pyrinth/models.py` & `python-modrinth-1.2.1/src/pyrinth/models.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,400 +1,400 @@
-"""Contains all models used in Pyrinth."""
-
-import json
-
-import pyrinth.literals as literals
-import pyrinth.projects as projects
-import pyrinth.util as util
-
-
-class ProjectModel:
-    """The model used for the Project class
-
-    Attributes:
-        slug (str): The slug of the project, used for vanity URLs. Regex: ^[\\w!@$()`.+,"\\-']{3,64}$
-        title (str): The title or name of the project
-        description (str): A short description of the project
-        categories (list[str]): A list of categories that the project has
-        client_side (str): The client side support of the project
-        server_side (str): The server side support of the project
-        body (str): A long form description of the project
-        additional_categories (list[str]): A list of categories which are searchable but non-primary
-        issues_url (str): An optional link to where to submit bugs or issues with the project
-        source_url (str): An optional link to the source code of the project
-        wiki_url (str): An optional link to the project's wiki page or other relevant information
-        discord_url (str): An optional invite link to the project's discord
-        donation_urls (list[dict]): A list of donations for the project
-        project_type (str): The project type
-        downloads (int): The total number of downloads of the project
-        icon_url (str): The URL of the project's icon
-        color (str): The RGB color of the project, automatically generated from the project icon
-        id (str): The ID of the project, encoded as a base62 string
-        team (str): The ID of the team that has ownership of this project
-        moderator_message: A message that a moderator sent regarding the project
-        published (str): The date the project was published
-        updated (str): The date the project was last updated
-        approved (str): The date of the project's status was set to approved or unlisted
-        followers (int): The total number of users following the project
-        status (str): The status of the project
-        license (dict): The license of the project
-        version_ids (list[str]): A list of version IDs of the project (will never be empty unless draft status)
-        game_versions (list[str]): A list of all the game versions supported by the project
-        loaders (list[str]): A list of all the loaders supported by the project
-        gallery (list[dict]): A list of images that have been uploaded to the project's gallery
-        auth (str): The project's authorization token
-    """
-
-    def __init__(
-        self,
-        slug: str,
-        title: str,
-        description: str,
-        categories: list[str],
-        client_side: str,
-        server_side: str,
-        body: str,
-        license_: "projects.Project.License",
-        project_type: str,
-        additional_categories: list[str] | None = None,
-        issues_url: str | None = None,
-        source_url: str | None = None,
-        wiki_url: str | None = None,
-        discord_url: str | None = None,
-        auth: str | None = None,
-    ) -> None:
-        """Initializes a new instance of ProjectModel
-
-        Args:
-            slug (str): The slug of the project, used for vanity URLs. Regex: ^[\\w!@$()`.+,"\\-']{3,64}$
-            title (str): The title or name of the project
-            description (str): A short description of the project
-            categories (list[str]): A list of categories that the project has
-            client_side (str): The client side support of the project
-            server_side (str): The server side support of the project
-            body (str): A long form description of the project
-            license_ (Project.License): The license of the project
-            project_type (str): The project type
-            additional_categories (list[str], optional): A list of categories which are searchable but non-primary
-            issues_url (str, optional): An optional link to where to submit bugs or issues with the project
-            source_url (str, optional): An optional link to the source code of the project
-            wiki_url (str, optional): An optional link to the project's wiki page or other relevant information
-            discord_url (str, optional): An optional invite link to the project's discord
-            auth (str, optional): Authentication token for the project
-        """
-        self.slug = slug
-        self.title = title
-        self.description = description
-        self.categories = categories
-        self.client_side = client_side
-        self.server_side = server_side
-        self.body = body
-        self.license = license_._to_json()
-        self.project_type = project_type
-        self.additional_categories = additional_categories
-        self.issues_url = issues_url
-        self.source_url = source_url
-        self.wiki_url = wiki_url
-        self.discord_url = discord_url
-        self.donation_urls: list[dict] | None = None
-        self.auth = auth
-        self.id: str | None = None
-        self.downloads: int | None = None
-        self.icon_url: str | None = None
-        self.color: str | None = None
-        self.team: str | None = None
-        self.moderator_message = None
-        self.published: str | None = None
-        self.updated: str | None = None
-        self.approved: str | None = None
-        self.followers: int | None = None
-        self.status: str | None = None
-        self.version_ids: list[str] | None = None
-        self.game_versions: list[str] | None = None
-        self.loaders: list[str] | None = None
-        self.gallery: list[dict] | None = None
-
-    @staticmethod
-    def _from_json(json_: dict) -> "ProjectModel":
-        license_ = projects.Project.License._from_json(json_.get("license"))  # type: ignore
-
-        result = ProjectModel(
-            json_.get("slug"),  # type: ignore
-            json_.get("title"),  # type: ignore
-            json_.get("description"),  # type: ignore
-            json_.get("categories"),  # type: ignore
-            json_.get("client_side"),  # type: ignore
-            json_.get("server_side"),  # type: ignore
-            json_.get("body"),  # type: ignore
-            license_,
-            json_.get("project_type"),  # type: ignore
-            json_.get("additional_categories"),  # type: ignore
-            json_.get("issues_url"),  # type: ignore
-            json_.get("source_url"),  # type: ignore
-            json_.get("wiki_url"),  # type: ignore
-            json_.get("discord_url"),  # type: ignore
-            json_.get("authorization"),
-        )
-        result.id = json_.get("id")
-        result.downloads = json_.get("downloads")
-        result.donation_urls = json_.get("donation_urls")
-        result.icon_url = json_.get("icon_url")
-        result.color = json_.get("color")
-        result.team = json_.get("team")
-        result.moderator_message = json_.get("moderator_message")
-        result.published = json_.get("published")
-        result.updated = json_.get("updated")
-        result.approved = json_.get("approved")
-        result.followers = json_.get("followers")
-        result.status = json_.get("status")
-        result.version_ids = json_.get("versions")
-        result.game_versions = json_.get("game_versions")
-        result.loaders = json_.get("loaders")
-        result.gallery = json_.get("gallery")
-        return result
-
-    def _to_json(self) -> dict:
-        return util.remove_null_values(self.__dict__)
-
-    def _to_bytes(self) -> bytes:
-        return json.dumps(self._to_json()).encode()
-
-
-class SearchResultModel:
-    """The model used for the SearchResult class
-
-    Attributes:
-        slug (str): The slug of a project, used for vanity URLs. Regex: ^[\\w!@$()`.+,"\\-']{3,64}$
-        title (str): The title or name of the project
-        description (str): A short description of the project
-        client_side (str): The client side support of the project
-        server_side (str): The server side support of the project
-        project_type (str): The project type
-        downloads (int): The total number of downloads of the project
-        project_id (str): The ID of the project
-        author (str): The username of the project's author
-        versions (list[str]): A list of the minecraft versions supported by the project
-        follows (int): The total number of users following the project
-        date_created (str): The date the project was added to search
-        date_modified (str): The date the project was last modified
-        license (str): The SPDX license ID of the project
-        categories (list[str]): A list of categories that the project has
-        icon_url (str): The URL of the project's icon
-        color (str): The RGB color of the project, automatically generated from the project icon
-        display_categories (list[str]): A list of categories that the project has which are not secondary
-        latest_version (str): The latest version of minecraft that this project supports
-        gallery (list[str]): All gallery images attached to the project
-        featured_gallery (list[str]): The featured gallery image of the project
-
-    """
-
-    def __init__(self) -> None:
-        self.slug: str | None = None
-        self.title: str | None = None
-        self.description: str | None = None
-        self.client_side: str | None = None
-        self.server_side: str | None = None
-        self.project_type: str | None = None
-        self.downloads: int | None = None
-        self.project_id: str | None = None
-        self.author: str | None = None
-        self.versions: list[str] | None = None
-        self.follows: int | None = None
-        self.date_created = None
-        self.date_modified = None
-        self.license: str | None = None
-        self.categories: list[str] | None = None
-        self.icon_url: str | None = None
-        self.color: str | None = None
-        self.display_categories: list[str] | None = None
-        self.latest_version: list[str] | None = None
-        self.gallery: list[str] | None = None
-        self.featured_gallery: list[str] | None = None
-
-    @staticmethod
-    def _from_json(json_: dict) -> "SearchResultModel":
-        result = SearchResultModel()
-        result.slug = json_.get("slug")
-        result.title = json_.get("title")
-        result.description = json_.get("description")
-        result.client_side = json_.get("client_side")
-        result.server_side = json_.get("server_side")
-        result.project_type = json_.get("project_type")
-        result.downloads = json_.get("downloads")
-        result.project_id = json_.get("project_id")
-        result.author = json_.get("author")
-        result.versions = json_.get("versions")
-        result.follows = json_.get("follows")
-        result.date_created = json_.get("date_created")
-        result.date_modified = json_.get("date_modified")
-        result.license = json_.get("license")
-        result.categories = json_.get("categories")
-        result.icon_url = json_.get("icon_url")
-        result.color = json_.get("color")
-        result.display_categories = json_.get("display_categories")
-        result.latest_version = json_.get("latest_version")
-        result.gallery = json_.get("gallery")
-        result.featured_gallery = json_.get("featured_gallery")
-
-        return result
-
-    def _to_json(self) -> dict:
-        return util.remove_null_values(self.__dict__)
-
-    def _to_bytes(self) -> bytes:
-        return json.dumps(self._to_json()).encode()
-
-
-class VersionModel:
-    """The model used for the Version class
-
-    Attributes:
-        name (str): The name of this version
-        version_number (str): The version number. Ideally will follow semantic versioning
-        changelog (str): The changelog for this version
-        dependencies (list[dict]): A list of specific versions of projects that this version depends on
-        game_versions (list[str]): A list of versions of Minecraft that this version supports
-        version_type (str): The release channel for this version
-        loaders (list[str]): The mod loaders that this version supports
-        featured (bool): Whether the version is featured or not
-        status (str): The version's status
-        requested_status (str): The version's requested status
-        files (list[dict]): A list of files avaliable for download for this version
-        project_id (str): The ID of the project this version is for
-        id (str): The ID of the version, encoded as base62 string
-        author_id (str): The ID of the author who published this version
-        date_published (str): When the version was published
-        downloads (int): The number of times this version has been downloaded
-
-    """
-
-    def __init__(
-        self,
-        name: str,
-        version_number: str,
-        dependencies: list["projects.Project.Dependency"],
-        game_versions: list[str],
-        version_type: literals.version_type_literal,
-        loaders: list[str],
-        featured: bool,
-        file_parts: list[str],
-        changelog: str | None = None,
-        status: literals.version_status_literal | None = None,
-        requested_status: literals.requested_version_status_literal | None = None,
-    ) -> None:
-        """
-        Initializes a new instance of VersionModel
-
-        Args:
-            name (str): The name of this version
-            version_number (str): The version number. Ideally will follow semantic versioning
-            dependencies (list[Project.Dependency]): A list of specific versions of projects that this version depends on
-            game_versions (list[str]): A list of versions of Minecraft that this version supports
-            version_type (Literal["release", "beta", "alpha"]): The release channel for this version
-            loaders (list[str]): The mod loaders that this version supports
-            featured (bool): Whether the version is featured or not
-            file_parts (list[str]): A list of files avaliable for download for this version
-            changelog (str, optional): The changelog for this version
-            status (Literal["listed", "archived", "draft", "unlisted", "scheduled", "unknown"], optional): The version's status
-            requested_status (Literal["listed", "archived", "draft", "unlisted"], optional): The version's requested status
-        """
-        self.name = name
-        self.version_number = version_number
-        self.changelog = changelog
-        self.dependencies = util.list_to_json(dependencies)
-        self.game_versions = game_versions
-        self.version_type = version_type
-        self.loaders = loaders
-        self.featured = featured
-        self.status = status
-        self.requested_status = requested_status
-        self.files = file_parts
-        self.project_id = None
-        self.id = None
-        self.author_id = None
-        self.date_published = None
-        self.downloads = None
-
-    @staticmethod
-    def _from_json(json_: dict) -> "VersionModel":
-        result = VersionModel(
-            json_.get("name"),  # type: ignore
-            json_.get("version_number"),  # type: ignore
-            json_.get("dependencies"),  # type: ignore
-            json_.get("game_versions"),  # type: ignore
-            json_.get("version_type"),  # type: ignore
-            json_.get("loaders"),  # type: ignore
-            json_.get("featured"),  # type: ignore
-            json_.get("files"),  # type: ignore
-            json_.get("changelog"),  # type: ignore
-            json_.get("status"),  # type: ignore
-            json_.get("requested_status"),  # type: ignore
-        )
-        result.project_id = json_.get("project_id")
-        result.id = json_.get("id")
-        result.author_id = json_.get("author_id")
-        result.date_published = json_.get("date_published")
-        result.downloads = json_.get("downloads")
-        return result
-
-    def _to_json(self) -> dict:
-        return util.remove_null_values(self.__dict__)
-
-    def _to_bytes(self) -> bytes:
-        return json.dumps(self._to_json()).encode()
-
-
-class UserModel:
-    """The model used for the User class
-
-    Attributes:
-        username (str): The user's username
-        id (str): The user's ID
-        avatar_url (str): The user's avatar URL
-        created (str): The time at which the user was created
-        role (str): The user's role
-        name (str): The user's display name
-        email (str): The user's email (only when your own is ever displayed)
-        bio (str): A description of the user
-        payout_data (, optional): Various data relating to the user's payouts status (you can only see your own)
-        github_id (int): The user's GitHub ID
-        badges (list[str]): Any badges applicable to this user. These are currently unused and undisplayed, and as such are subject to change
-        auth (str): Authentication token for the user
-    """
-
-    def __init__(self) -> None:
-        self.username: str | None = None
-        self.id: str | None = None
-        self.avatar_url: str | None = None
-        self.created: str | None = None
-        self.role: str | None = None
-        self.name: str | None = None
-        self.email: str | None = None
-        self.bio: str | None = None
-        self.payout_data = None
-        self.github_id: int | None = None
-        self.badges: list[str] | None = None
-        self.auth: str | None = None
-
-    @staticmethod
-    def _from_json(json_: dict) -> "UserModel":
-        result = UserModel()
-        result.username = json_.get("username")
-        result.id = json_.get("id")
-        result.avatar_url = json_.get("avatar_url")
-        result.created = json_.get("created")
-        result.role = json_.get("role")
-        result.name = json_.get("name")
-        result.email = json_.get("email")
-        result.bio = json_.get("bio")
-        result.payout_data = json_.get("payout_data")
-        result.github_id = json_.get("github_id")
-        result.badges = json_.get("badges")
-        result.auth = json_.get("authorization", "")
-
-        return result
-
-    def _to_json(self) -> dict:
-        return util.remove_null_values(self.__dict__)
-
-    def _to_bytes(self) -> bytes:
-        return json.dumps(self._to_json()).encode()
+"""Contains all models used in Pyrinth."""
+
+import json
+
+import pyrinth.literals as literals
+import pyrinth.projects as projects
+import pyrinth.util as util
+
+
+class ProjectModel:
+    """The model used for the Project class
+
+    Attributes:
+        slug (str): The slug of the project, used for vanity URLs. Regex: ^[\\w!@$()`.+,"\\-']{3,64}$
+        title (str): The title or name of the project
+        description (str): A short description of the project
+        categories (list[str]): A list of categories that the project has
+        client_side (str): The client side support of the project
+        server_side (str): The server side support of the project
+        body (str): A long form description of the project
+        additional_categories (list[str]): A list of categories which are searchable but non-primary
+        issues_url (str): An optional link to where to submit bugs or issues with the project
+        source_url (str): An optional link to the source code of the project
+        wiki_url (str): An optional link to the project's wiki page or other relevant information
+        discord_url (str): An optional invite link to the project's discord
+        donation_urls (list[dict]): A list of donations for the project
+        project_type (str): The project type
+        downloads (int): The total number of downloads of the project
+        icon_url (str): The URL of the project's icon
+        color (str): The RGB color of the project, automatically generated from the project icon
+        id (str): The ID of the project, encoded as a base62 string
+        team (str): The ID of the team that has ownership of this project
+        moderator_message: A message that a moderator sent regarding the project
+        published (str): The date the project was published
+        updated (str): The date the project was last updated
+        approved (str): The date of the project's status was set to approved or unlisted
+        followers (int): The total number of users following the project
+        status (str): The status of the project
+        license (dict): The license of the project
+        version_ids (list[str]): A list of version IDs of the project (will never be empty unless draft status)
+        game_versions (list[str]): A list of all the game versions supported by the project
+        loaders (list[str]): A list of all the loaders supported by the project
+        gallery (list[dict]): A list of images that have been uploaded to the project's gallery
+        auth (str): The project's authorization token
+    """
+
+    def __init__(
+        self,
+        slug: str,
+        title: str,
+        description: str,
+        categories: list[str],
+        client_side: str,
+        server_side: str,
+        body: str,
+        license_: "projects.Project.License",
+        project_type: str,
+        additional_categories: list[str] | None = None,
+        issues_url: str | None = None,
+        source_url: str | None = None,
+        wiki_url: str | None = None,
+        discord_url: str | None = None,
+        auth: str | None = None,
+    ) -> None:
+        """Initializes a new instance of ProjectModel
+
+        Args:
+            slug (str): The slug of the project, used for vanity URLs. Regex: ^[\\w!@$()`.+,"\\-']{3,64}$
+            title (str): The title or name of the project
+            description (str): A short description of the project
+            categories (list[str]): A list of categories that the project has
+            client_side (str): The client side support of the project
+            server_side (str): The server side support of the project
+            body (str): A long form description of the project
+            license_ (Project.License): The license of the project
+            project_type (str): The project type
+            additional_categories (list[str], optional): A list of categories which are searchable but non-primary
+            issues_url (str, optional): An optional link to where to submit bugs or issues with the project
+            source_url (str, optional): An optional link to the source code of the project
+            wiki_url (str, optional): An optional link to the project's wiki page or other relevant information
+            discord_url (str, optional): An optional invite link to the project's discord
+            auth (str, optional): Authentication token for the project
+        """
+        self.slug = slug
+        self.title = title
+        self.description = description
+        self.categories = categories
+        self.client_side = client_side
+        self.server_side = server_side
+        self.body = body
+        self.license = license_._to_json()
+        self.project_type = project_type
+        self.additional_categories = additional_categories
+        self.issues_url = issues_url
+        self.source_url = source_url
+        self.wiki_url = wiki_url
+        self.discord_url = discord_url
+        self.donation_urls: list[dict] | None = None
+        self.auth = auth
+        self.id: str | None = None
+        self.downloads: int | None = None
+        self.icon_url: str | None = None
+        self.color: str | None = None
+        self.team: str | None = None
+        self.moderator_message = None
+        self.published: str | None = None
+        self.updated: str | None = None
+        self.approved: str | None = None
+        self.followers: int | None = None
+        self.status: str | None = None
+        self.version_ids: list[str] | None = None
+        self.game_versions: list[str] | None = None
+        self.loaders: list[str] | None = None
+        self.gallery: list[dict] | None = None
+
+    @staticmethod
+    def _from_json(json_: dict) -> "ProjectModel":
+        license_ = projects.Project.License._from_json(json_.get("license"))  # type: ignore
+
+        result = ProjectModel(
+            json_.get("slug"),  # type: ignore
+            json_.get("title"),  # type: ignore
+            json_.get("description"),  # type: ignore
+            json_.get("categories"),  # type: ignore
+            json_.get("client_side"),  # type: ignore
+            json_.get("server_side"),  # type: ignore
+            json_.get("body"),  # type: ignore
+            license_,
+            json_.get("project_type"),  # type: ignore
+            json_.get("additional_categories"),  # type: ignore
+            json_.get("issues_url"),  # type: ignore
+            json_.get("source_url"),  # type: ignore
+            json_.get("wiki_url"),  # type: ignore
+            json_.get("discord_url"),  # type: ignore
+            json_.get("authorization"),
+        )
+        result.id = json_.get("id")
+        result.downloads = json_.get("downloads")
+        result.donation_urls = json_.get("donation_urls")
+        result.icon_url = json_.get("icon_url")
+        result.color = json_.get("color")
+        result.team = json_.get("team")
+        result.moderator_message = json_.get("moderator_message")
+        result.published = json_.get("published")
+        result.updated = json_.get("updated")
+        result.approved = json_.get("approved")
+        result.followers = json_.get("followers")
+        result.status = json_.get("status")
+        result.version_ids = json_.get("versions")
+        result.game_versions = json_.get("game_versions")
+        result.loaders = json_.get("loaders")
+        result.gallery = json_.get("gallery")
+        return result
+
+    def _to_json(self) -> dict:
+        return util.remove_null_values(self.__dict__)
+
+    def _to_bytes(self) -> bytes:
+        return json.dumps(self._to_json()).encode()
+
+
+class SearchResultModel:
+    """The model used for the SearchResult class
+
+    Attributes:
+        slug (str): The slug of a project, used for vanity URLs. Regex: ^[\\w!@$()`.+,"\\-']{3,64}$
+        title (str): The title or name of the project
+        description (str): A short description of the project
+        client_side (str): The client side support of the project
+        server_side (str): The server side support of the project
+        project_type (str): The project type
+        downloads (int): The total number of downloads of the project
+        project_id (str): The ID of the project
+        author (str): The username of the project's author
+        versions (list[str]): A list of the minecraft versions supported by the project
+        follows (int): The total number of users following the project
+        date_created (str): The date the project was added to search
+        date_modified (str): The date the project was last modified
+        license (str): The SPDX license ID of the project
+        categories (list[str]): A list of categories that the project has
+        icon_url (str): The URL of the project's icon
+        color (str): The RGB color of the project, automatically generated from the project icon
+        display_categories (list[str]): A list of categories that the project has which are not secondary
+        latest_version (str): The latest version of minecraft that this project supports
+        gallery (list[str]): All gallery images attached to the project
+        featured_gallery (list[str]): The featured gallery image of the project
+
+    """
+
+    def __init__(self) -> None:
+        self.slug: str | None = None
+        self.title: str | None = None
+        self.description: str | None = None
+        self.client_side: str | None = None
+        self.server_side: str | None = None
+        self.project_type: str | None = None
+        self.downloads: int | None = None
+        self.project_id: str | None = None
+        self.author: str | None = None
+        self.versions: list[str] | None = None
+        self.follows: int | None = None
+        self.date_created = None
+        self.date_modified = None
+        self.license: str | None = None
+        self.categories: list[str] | None = None
+        self.icon_url: str | None = None
+        self.color: str | None = None
+        self.display_categories: list[str] | None = None
+        self.latest_version: list[str] | None = None
+        self.gallery: list[str] | None = None
+        self.featured_gallery: list[str] | None = None
+
+    @staticmethod
+    def _from_json(json_: dict) -> "SearchResultModel":
+        result = SearchResultModel()
+        result.slug = json_.get("slug")
+        result.title = json_.get("title")
+        result.description = json_.get("description")
+        result.client_side = json_.get("client_side")
+        result.server_side = json_.get("server_side")
+        result.project_type = json_.get("project_type")
+        result.downloads = json_.get("downloads")
+        result.project_id = json_.get("project_id")
+        result.author = json_.get("author")
+        result.versions = json_.get("versions")
+        result.follows = json_.get("follows")
+        result.date_created = json_.get("date_created")
+        result.date_modified = json_.get("date_modified")
+        result.license = json_.get("license")
+        result.categories = json_.get("categories")
+        result.icon_url = json_.get("icon_url")
+        result.color = json_.get("color")
+        result.display_categories = json_.get("display_categories")
+        result.latest_version = json_.get("latest_version")
+        result.gallery = json_.get("gallery")
+        result.featured_gallery = json_.get("featured_gallery")
+
+        return result
+
+    def _to_json(self) -> dict:
+        return util.remove_null_values(self.__dict__)
+
+    def _to_bytes(self) -> bytes:
+        return json.dumps(self._to_json()).encode()
+
+
+class VersionModel:
+    """The model used for the Version class
+
+    Attributes:
+        name (str): The name of this version
+        version_number (str): The version number. Ideally will follow semantic versioning
+        changelog (str): The changelog for this version
+        dependencies (list[dict]): A list of specific versions of projects that this version depends on
+        game_versions (list[str]): A list of versions of Minecraft that this version supports
+        version_type (str): The release channel for this version
+        loaders (list[str]): The mod loaders that this version supports
+        featured (bool): Whether the version is featured or not
+        status (str): The version's status
+        requested_status (str): The version's requested status
+        files (list[dict]): A list of files avaliable for download for this version
+        project_id (str): The ID of the project this version is for
+        id (str): The ID of the version, encoded as base62 string
+        author_id (str): The ID of the author who published this version
+        date_published (str): When the version was published
+        downloads (int): The number of times this version has been downloaded
+
+    """
+
+    def __init__(
+        self,
+        name: str,
+        version_number: str,
+        dependencies: list["projects.Project.Dependency"],
+        game_versions: list[str],
+        version_type: literals.version_type_literal,
+        loaders: list[str],
+        featured: bool,
+        file_parts: list[str],
+        changelog: str | None = None,
+        status: literals.version_status_literal | None = None,
+        requested_status: literals.requested_version_status_literal | None = None,
+    ) -> None:
+        """
+        Initializes a new instance of VersionModel
+
+        Args:
+            name (str): The name of this version
+            version_number (str): The version number. Ideally will follow semantic versioning
+            dependencies (list[Project.Dependency]): A list of specific versions of projects that this version depends on
+            game_versions (list[str]): A list of versions of Minecraft that this version supports
+            version_type (Literal["release", "beta", "alpha"]): The release channel for this version
+            loaders (list[str]): The mod loaders that this version supports
+            featured (bool): Whether the version is featured or not
+            file_parts (list[str]): A list of files avaliable for download for this version
+            changelog (str, optional): The changelog for this version
+            status (Literal["listed", "archived", "draft", "unlisted", "scheduled", "unknown"], optional): The version's status
+            requested_status (Literal["listed", "archived", "draft", "unlisted"], optional): The version's requested status
+        """
+        self.name = name
+        self.version_number = version_number
+        self.changelog = changelog
+        self.dependencies = util.list_to_json(dependencies)
+        self.game_versions = game_versions
+        self.version_type = version_type
+        self.loaders = loaders
+        self.featured = featured
+        self.status = status
+        self.requested_status = requested_status
+        self.files = file_parts
+        self.project_id = None
+        self.id = None
+        self.author_id = None
+        self.date_published = None
+        self.downloads = None
+
+    @staticmethod
+    def _from_json(json_: dict) -> "VersionModel":
+        result = VersionModel(
+            json_.get("name"),  # type: ignore
+            json_.get("version_number"),  # type: ignore
+            json_.get("dependencies"),  # type: ignore
+            json_.get("game_versions"),  # type: ignore
+            json_.get("version_type"),  # type: ignore
+            json_.get("loaders"),  # type: ignore
+            json_.get("featured"),  # type: ignore
+            json_.get("files"),  # type: ignore
+            json_.get("changelog"),  # type: ignore
+            json_.get("status"),  # type: ignore
+            json_.get("requested_status"),  # type: ignore
+        )
+        result.project_id = json_.get("project_id")
+        result.id = json_.get("id")
+        result.author_id = json_.get("author_id")
+        result.date_published = json_.get("date_published")
+        result.downloads = json_.get("downloads")
+        return result
+
+    def _to_json(self) -> dict:
+        return util.remove_null_values(self.__dict__)
+
+    def _to_bytes(self) -> bytes:
+        return json.dumps(self._to_json()).encode()
+
+
+class UserModel:
+    """The model used for the User class
+
+    Attributes:
+        username (str): The user's username
+        id (str): The user's ID
+        avatar_url (str): The user's avatar URL
+        created (str): The time at which the user was created
+        role (str): The user's role
+        name (str): The user's display name
+        email (str): The user's email (only when your own is ever displayed)
+        bio (str): A description of the user
+        payout_data (, optional): Various data relating to the user's payouts status (you can only see your own)
+        github_id (int): The user's GitHub ID
+        badges (list[str]): Any badges applicable to this user. These are currently unused and undisplayed, and as such are subject to change
+        auth (str): Authentication token for the user
+    """
+
+    def __init__(self) -> None:
+        self.username: str | None = None
+        self.id: str | None = None
+        self.avatar_url: str | None = None
+        self.created: str | None = None
+        self.role: str | None = None
+        self.name: str | None = None
+        self.email: str | None = None
+        self.bio: str | None = None
+        self.payout_data = None
+        self.github_id: int | None = None
+        self.badges: list[str] | None = None
+        self.auth: str | None = None
+
+    @staticmethod
+    def _from_json(json_: dict) -> "UserModel":
+        result = UserModel()
+        result.username = json_.get("username")
+        result.id = json_.get("id")
+        result.avatar_url = json_.get("avatar_url")
+        result.created = json_.get("created")
+        result.role = json_.get("role")
+        result.name = json_.get("name")
+        result.email = json_.get("email")
+        result.bio = json_.get("bio")
+        result.payout_data = json_.get("payout_data")
+        result.github_id = json_.get("github_id")
+        result.badges = json_.get("badges")
+        result.auth = json_.get("authorization", "")
+
+        return result
+
+    def _to_json(self) -> dict:
+        return util.remove_null_values(self.__dict__)
+
+    def _to_bytes(self) -> bytes:
+        return json.dumps(self._to_json()).encode()
```

### Comparing `python-modrinth-1.2.0/src/pyrinth/projects.py` & `python-modrinth-1.2.1/src/pyrinth/projects.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,1417 +1,1417 @@
-"""Projects can be mods or modpacks and are created by users"""
-
-import datetime as dt
-import json
-import typing
-
-import requests as r
-
-import pyrinth.exceptions as exceptions
-import pyrinth.literals as literals
-import pyrinth.models as models
-import pyrinth.modrinth as modrinth
-import pyrinth.users as users
-import pyrinth.util as util
-import pyrinth.teams as teams
-
-
-class Project:
-    """Projects can be mods or modpacks and are created by users
-
-    Attributes:
-        model (ProjectModel): The project's model
-    """
-
-    def __init__(self, project_model: "models.ProjectModel") -> None:
-        """
-        Args:
-            project_model (ProjectModel): The project's model
-        """
-        if isinstance(project_model, dict):
-            project_model = models.ProjectModel._from_json(project_model)
-        self.model = project_model
-
-    def get_donations(self) -> list["Project.Donation"]:
-        """Gets the project's donations
-
-        Returns:
-            (list[Donation]): The project's donations
-        """
-        return util.list_to_object(Project.Donation, self.model.donation_urls)
-
-    def _get_auth(self, auth: str | None) -> str:
-        if auth:
-            return auth
-        return self.model.auth  # type: ignore
-
-    @staticmethod
-    def get(id_: str, auth: object = None) -> "Project":
-        """Gets a project based on an ID
-
-        Args:
-            id_ (str): The ID or slug of the project
-            auth (str, optional): An optional authorization token when getting the project
-
-        Raises:
-            NotFoundError: The requested project wasn't found or no authorization to see this project
-            InvalidRequestError: Invalid request
-
-        Returns:
-            (Project): The project that was found
-        """
-        raw_response = r.get(
-            f"https://api.modrinth.com/v2/project/{id_}",
-            headers={"authorization": auth},  # type: ignore
-            timeout=60,
-        )
-        match raw_response.status_code:
-            case 404:
-                raise exceptions.NotFoundError(
-                    "The requested project wasn't found or no authorization to see this project"
-                )
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-        response = raw_response.json()
-        response.update({"authorization": auth})
-        return Project(response)
-
-    @staticmethod
-    def get_multiple(ids: list[str]) -> list["Project"]:
-        """Gets multiple projects
-
-        Args:
-            ids (list[str]): The IDs of the projects
-
-        Raises:
-            InvalidRequestError: Invalid request
-
-        Returns:
-            (list[Project]): The projects that were found
-        """
-        raw_response = r.get(
-            "https://api.modrinth.com/v2/projects",
-            params={"ids": json.dumps(ids)},
-            timeout=60,
-        )
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-        response = raw_response.json()
-        return [Project(project) for project in response]
-
-    def get_latest_version(
-        self,
-        loaders: list[str] | None = None,
-        game_versions: list[str] | None = None,
-        featured: bool | None = None,
-        types: literals.version_type_literal | None = None,
-        auth: str | None = None,
-    ) -> "Project.Version":
-        """Gets this project's latest version
-
-        Args:
-            loaders (list[str], optional): The loaders filter. Defaults to None
-            game_versions (list[str], optional): The game versions filter. Defaults to None
-            featured (bool, optional): The is featured filter. Defaults to None
-            types (Literal["release", "beta", "alpha"], optional): The types filter. Defaults to None
-            auth (str, optional): The authorization token. Defaults to None
-
-        Returns:
-            (Project.Version): The project's latest version
-        """
-        versions = self.get_versions(loaders, game_versions, featured, types, auth)
-
-        return versions[0]
-
-    def get_gallery(self) -> list["Project.GalleryImage"]:
-        """Gets the project's gallery
-
-        Returns:
-            (list[Project.GalleryImage]): The project's gallery images
-        """
-        result = util.list_to_object(Project.GalleryImage, self.model.gallery)
-
-        return result
-
-    def is_client_side(self) -> bool:
-        """Checks if this project is client side
-
-        Returns:
-            (bool): Whether this project is client side
-        """
-        return True if self.model.client_side == "required" else False
-
-    def is_server_side(self) -> bool:
-        """Checks if this project is server side
-
-        Returns:
-            (bool): Whether this project is server side
-        """
-        return True if self.model.server_side == "required" else False
-
-    def get_downloads(self) -> int:
-        """Gets the number of downloads this project has
-
-        Returns:
-            (int): The number of downloads for this project
-        """
-        return self.model.downloads  # type: ignore
-
-    def get_categories(self) -> list[str]:
-        """Gets this projects categories
-
-        Returns:
-            (list[str]): The categories associated with this project
-        """
-        return self.model.categories
-
-    def get_additional_categories(self) -> list[str]:
-        """Gets this projects additional categories
-
-        Returns:
-            (list[str]): The additional categories associated with this project
-        """
-        return self.model.additional_categories  # type: ignore
-
-    def get_all_categories(self) -> list[str]:
-        """Gets this projects categories and additional categories
-
-        Returns:
-            (list[str]): The categories and additional categories associated with this project
-        """
-        return self.get_categories() + self.get_additional_categories()
-
-    def get_license(self) -> "Project.License":
-        """Gets this project license
-
-        Returns:
-            (Project.License): The license associated with this project
-        """
-        return Project.License._from_json(self.model.license)
-
-    def get_specific_version(
-        self, semantic_version: str
-    ) -> typing.Optional["Project.Version"]:
-        """Gets a specific version based on the semantic version
-
-        Args:
-            semantic_version (str): The semantic version to search for
-
-        Returns:
-            (Project.Version): The version that was found using the semantic version
-            (None): No version was found with that semantic version
-        """
-        versions = self.get_versions()
-        if versions:
-            for version in versions:
-                if version.model.version_number == semantic_version:
-                    return version
-
-        return None
-
-    def download(self, recursive: bool = False) -> None:
-        """Downloads this project
-
-        Args:
-            recursive (bool): Whether to download dependencies. Defaults to False
-        """
-        latest = self.get_latest_version()
-        files = latest.get_files()
-        for file in files:
-            file_content = r.get(file.url).content
-            open(file.name, "wb").write(file_content)
-
-        if recursive:
-            dependencies = latest.get_dependencies()
-            for dep in dependencies:
-                files = dep.get_version().get_files()
-                for file in files:
-                    file_content = r.get(file.url).content
-                    open(file.name, "wb").write(file_content)
-
-    def get_versions(
-        self,
-        loaders: list[str] | None = None,
-        game_versions: list[str] | None = None,
-        featured: bool | None = None,
-        types: literals.version_type_literal | None = None,
-        auth: str | None = None,
-    ) -> list["Project.Version"]:
-        """Gets project versions based on filters
-
-        Args:
-            loaders (list[str], optional): The types of loaders to filter for
-            game_versions (list[str], optional): The game versions to filter for
-            featured (bool, optional): Allows to filter for featured or non-featured versions only
-            types (Literal["release", "beta", "alpha"], optional): The release type of version
-            auth (str, optional): An optional authorization token to use when getting the project versions
-
-        Raises:
-            NotFoundError: The requested project wasn't found or no authorization to see this project
-            InvalidRequestError: Invalid request
-
-        Returns:
-            (list[Project.Version]): The versions that were found
-        """
-        filters = {
-            "loaders": loaders,
-            "game_versions": game_versions,
-            "featured": featured,
-        }
-
-        filters = util.remove_null_values(filters)
-        raw_response = r.get(
-            f"https://api.modrinth.com/v2/project/{self.model.slug}/version",
-            params=util.json_to_query_params(filters),
-            headers={"authorization": self._get_auth(auth)},
-            timeout=60,
-        )
-
-        match raw_response.status_code:
-            case 404:
-                raise exceptions.NotFoundError(
-                    "The requested project wasn't found or no authorization to see this project"
-                )
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        response = raw_response.json()
-
-        versions = [
-            self.Version(models.VersionModel._from_json(version))
-            for version in response
-        ]
-
-        if not types:
-            return versions
-
-        result = []
-        for version in versions:
-            if version.model.version_type in types:
-                result.append(version)
-
-        return result
-
-    def get_oldest_version(
-        self,
-        loaders: list[str] | None = None,
-        game_versions: list[str] | None = None,
-        featured: bool | None = None,
-        types: literals.version_type_literal | None = None,
-        auth: str | None = None,
-    ) -> "Project.Version":
-        """Gets the oldest project version
-
-        Args:
-            loaders (list[str], optional): The types of loaders to filter for
-            game_versions (list[str], optional): The game versions to filter for
-            featured (bool, optional): Allows to filter for featured or non-featured versions only
-            types (Literal["release", "beta", "alpha"], optional): The type of version
-            auth (str, optional): An optional authorization token to use when getting the project versions
-
-        Returns:
-            (Project.Version): The version that was found
-        """
-        versions = self.get_versions(loaders, game_versions, featured, types, auth)
-
-        return versions[-1]
-
-    def get_id(self) -> str:
-        """Gets the ID of the project
-
-        Returns:
-            (str): The ID of the project
-        """
-        return self.model.id  # type: ignore
-
-    def get_slug(self) -> str:
-        """Gets the slug of the project
-
-        Returns:
-            (str): The slug of the project
-        """
-        return self.model.slug
-
-    def get_name(self) -> str:
-        """Gets the name of the project
-
-        Returns:
-            (str): The name of the project
-        """
-        return self.model.title
-
-    @staticmethod
-    def get_version(id_: str) -> "Project.Version":
-        """Gets a version by ID
-
-        Args:
-            id_ (str): The ID of the version
-
-        Raises:
-            NotFoundError: The requested version wasn't found or no authorization to see this version
-            InvalidRequestError: Invalid request
-
-        Returns:
-            (Project.Version): The version that was found
-        """
-        raw_response = r.get(f"https://api.modrinth.com/v2/version/{id_}", timeout=60)
-
-        match raw_response.status_code:
-            case 404:
-                raise exceptions.NotFoundError(
-                    "The requested version wasn't found or no authorization to see this version"
-                )
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        response = raw_response.json()
-        return Project.Version(models.VersionModel._from_json(response))
-
-    def create_version(self, version_model, auth: str | None = None) -> int:
-        """Creates a new version on the project
-
-        Args:
-            auth (str, optional): The authorization token to use when creating the version
-            version_model (VersionModel): The model to use when creating the version
-
-        Raises:
-            NoAuthorizationError: No authorization to create this version
-            InvalidRequestError: Invalid request
-
-        Returns:
-            (int): Whether creating the version was successful
-        """
-        version_model.project_id = self.model.id
-
-        files = {"data": version_model.to_bytes()}
-
-        for file in version_model.files:
-            files.update({util.remove_file_path(file): open(file, "rb").read()})
-
-        raw_response = r.post(
-            "https://api.modrinth.com/v2/version",
-            headers={"authorization": self._get_auth(auth)},
-            files=files,
-            timeout=60,
-        )
-
-        match raw_response.status_code:
-            case 401:
-                raise exceptions.NoAuthorizationError(
-                    "No authorization to create this version"
-                )
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        return True
-
-    def change_icon(self, file_path: str, auth: str | None = None) -> bool:
-        """Changes the project icon
-
-        Args:
-            file_path (str): The file path of the image to use for the new project icon
-            auth (str, optional): The authorization token to use when changing the project icon
-
-        Raises:
-            InvalidParamError: Invalid input for new icon
-            InvalidRequestError: Invalid request
-
-        Returns:
-            (bool): Whether the project icon change was successful
-        """
-        raw_response = r.patch(
-            f"https://api.modrinth.com/v2/project/{self.model.slug}/icon",
-            params={"ext": file_path.split(".")[-1]},
-            headers={"authorization": self._get_auth(auth)},
-            data=open(file_path, "rb"),
-            timeout=60,
-        )
-
-        match raw_response.status_code:
-            case 400:
-                raise exceptions.InvalidParamError("Invalid input for new icon")
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        return True
-
-    def delete_icon(self, auth: str | None = None) -> bool:
-        """Deletes the project icon
-
-        Args:
-            auth (str, optional): The authorization token to use when deleting the project icon
-
-        Raises:
-            InvalidParamError: Invalid input
-            NoAuthorizationError: No authorization to edit this project
-            InvalidRequestError: Invalid request
-
-        Returns:
-            (bool): Whether the project icon deletion was successful
-        """
-        raw_response = r.delete(
-            f"https://api.modrinth.com/v2/project/{self.model.slug}/icon",
-            headers={"authorization": self._get_auth(auth)},
-            timeout=60,
-        )
-
-        match raw_response.status_code:
-            case 400:
-                raise exceptions.InvalidParamError("Invalid input")
-
-            case 401:
-                raise exceptions.NoAuthorizationError(
-                    "No authorization to edit this project"
-                )
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        return True
-
-    def add_gallery_image(
-        self, image: "Project.GalleryImage", auth: str | None = None
-    ) -> bool:
-        """Adds a gallery image to the project
-
-        Args:
-            image (Project.GalleryImage): The gallery image to add
-            auth (str, optional): The authorization token to use when adding the gallery image
-
-        Raises:
-            NoAuthorizationError: No authorization to create a gallery image
-            NotFoundError: The requested project wasn't found or no authorization to see this project
-            InvalidRequestError: Invalid request
-
-        Returns:
-            (bool): If the gallery image addition was successful
-        """
-        raw_response = r.post(
-            f"https://api.modrinth.com/v2/project/{self.model.slug}/gallery",
-            headers={"authorization": self._get_auth(auth)},
-            params=image._to_json(),
-            data=open(image.file_path, "rb"),
-            timeout=60,
-        )
-
-        match raw_response.status_code:
-            case 401:
-                raise exceptions.NoAuthorizationError(
-                    "No authorization to create a gallery image"
-                )
-
-            case 404:
-                raise exceptions.NotFoundError(
-                    "The requested project wasn't found or no authorization to see this project"
-                )
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        return True
-
-    def modify_gallery_image(
-        self,
-        url: str,
-        featured: bool | None = None,
-        title: str | None = None,
-        description: str | None = None,
-        ordering: int | None = None,
-        auth: str | None = None,
-    ) -> bool:
-        """Modifies a gallery image
-
-        Args:
-            url (str): URL link of the image to modify
-            featured (bool, optional): Whether the image is featured
-            title (str, optional): New title of the image
-            description (str, optional): New description of the image
-            ordering (int, optional): New ordering of the image
-            auth (str, optional): Authentication token when modifying the gallery image
-
-        Raises:
-            NoAuthorizationError: No authorization to edit this gallery image
-            NotFoundError: The requested project wasn't found or no authorization to see this project
-            InvalidRequestError: Invalid request
-
-        Returns:
-            (bool): Whether the gallery image modification was successful
-        """
-        modified_json = {
-            "url": url,
-            "featured": featured,
-            "title": title,
-            "description": description,
-            "ordering": ordering,
-        }
-
-        modified_json = util.remove_null_values(modified_json)
-
-        raw_response = r.patch(
-            f"https://api.modrinth.com/v2/project/{self.model.slug}/gallery",
-            params=modified_json,
-            headers={"authorization": self._get_auth(auth)},
-            timeout=60,
-        )
-
-        match raw_response.status_code:
-            case 401:
-                raise exceptions.NoAuthorizationError(
-                    "No authorization to edit this gallery image"
-                )
-
-            case 404:
-                raise exceptions.NotFoundError(
-                    "The requested project wasn't found or no authorization to see this project"
-                )
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        return True
-
-    def delete_gallery_image(self, url: str, auth: str | None = None) -> bool:
-        """Deletes a gallery image
-
-        Args:
-            url (str): URL link of the image to delete
-            auth (str, optional): Authentication token to use when deleting the gallery image
-
-        Raises:
-            InvalidParamError: Invalid URL or project specified
-            NoAuthorizationError: No authorization to delete this gallery image
-            InvalidRequestError: Invalid request
-
-        Returns:
-            (bool): Whether the gallery image deletion was successful
-        """
-        if "-raw" in url:
-            raise exceptions.InvalidParamError(
-                "Please use cdn.modrinth.com instead of cdn-raw.modrinth.com"
-            )
-
-        raw_response = r.delete(
-            f"https://api.modrinth.com/v2/project/{self.model.slug}/gallery",
-            headers={"authorization": self._get_auth(auth)},
-            params={"url": url},
-            timeout=60,
-        )
-
-        match raw_response.status_code:
-            case 400:
-                raise exceptions.InvalidParamError("Invalid URL or project specified")
-
-            case 401:
-                raise exceptions.NoAuthorizationError(
-                    "No authorization to delete this gallery image"
-                )
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        return True
-
-    def modify(
-        self,
-        slug: str | None = None,
-        title: str | None = None,
-        description: str | None = None,
-        categories: list[str] | None = None,
-        client_side: str | None = None,
-        server_side: str | None = None,
-        body: str | None = None,
-        additional_categories: list[str] | None = None,
-        issues_url: str | None = None,
-        source_url: str | None = None,
-        wiki_url: str | None = None,
-        discord_url: str | None = None,
-        license_id: str | None = None,
-        license_url: str | None = None,
-        status: literals.project_status_literal | None = None,
-        requested_status: literals.requested_project_status_literal | None = None,
-        moderation_message: str | None = None,
-        moderation_message_body: str | None = None,
-        auth: str | None = None,
-    ) -> bool:
-        """Modifies the project
-
-        Args:
-            slug (str, optional): The slug of a project, used for vanity URLs. Regex: ^[\\w!@$()`.+,"\\-']{3,64}$
-            title (str, optional): The title or name of the project
-            description (str, optional): A short description of the project
-            categories (list[str], optional): A list of categories that the project has
-            client_side (str, optional): The client side support of the project
-            server_side (str, optional): The server side support of the project
-            body (str, optional): A long form description of the project
-            additional_categories (list[str], optional): A list of categories which are searchable but non-primary
-            issues_url (str, optional): An optional link to where to submit bugs or issues with the project
-            source_url (str, optional): An optional link to the source code of the project
-            wiki_url (str, optional): An optional link to the project's wiki page or other relevant information
-            discord_url (str, optional): An optional invite link to the project's discord
-            license_id (str, optional): The SPDX license ID of a project
-            license_url (str, optional): The URL to this license
-            status (Literal["approved", "archived", "rejected", "draft", "unlisted", "processing", "withheld", "scheduled", "private", "unknown"], optional): The status of the project
-            requested_status (Literal["approved", "archived", "unlisted", "private", "draft"], optional): The requested status when submitting for review or scheduling the project for release
-            moderation_message (str, optional): The title of the moderators' message for the project
-            moderation_message_body (str, optional): The body of the moderators' message for the project
-            auth (str, optional): Authentication token to use when modifying the project
-
-        Raises:
-            InvalidParamError: Please specify at least 1 optional argument
-            NoAuthorizationError: No authorization to modify this project
-            NotFoundError: The requested project wasn't found or no authorization to see this project
-            InvalidRequestError: Invalid request
-
-        Returns:
-            (bool): Whether the project modification was successful
-        """
-        modified_json = {
-            "slug": slug,
-            "title": title,
-            "description": description,
-            "categories": categories,
-            "client_side": client_side,
-            "server_side": server_side,
-            "body": body,
-            "additional_categories": additional_categories,
-            "issues_url": issues_url,
-            "source_url": source_url,
-            "wiki_url": wiki_url,
-            "discord_url": discord_url,
-            "license_id": license_id,
-            "license_url": license_url,
-            "status": status,
-            "requested_status": requested_status,
-            "moderation_message": moderation_message,
-            "moderation_message_body": moderation_message_body,
-        }
-
-        modified_json = util.remove_null_values(modified_json)
-
-        if not modified_json:
-            raise exceptions.InvalidParamError(
-                "Please specify at least 1 optional argument"
-            )
-
-        raw_response = r.patch(
-            f"https://api.modrinth.com/v2/project/{self.model.slug}",
-            data=json.dumps(modified_json),
-            headers={
-                "Content-Type": "application/json",
-                "authorization": self._get_auth(auth),
-            },
-            timeout=60,
-        )
-
-        match raw_response.status_code:
-            case 401:
-                raise exceptions.NoAuthorizationError(
-                    "No authorization to edit this project"
-                )
-
-            case 404:
-                raise exceptions.NotFoundError(
-                    "The requested project wasn't found or no authorization to see this project"
-                )
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        return True
-
-    def delete(self, auth: str | None = None) -> typing.Literal[True]:
-        """Deletes the project
-
-        Args:
-            auth (str, optional): Authentication token to use when deleting the project
-
-        Raises:
-            NotFoundError: The requested project wasn't found
-            NoAuthorizationError: No authorization to delete this project
-            InvalidRequestError: Invalid request
-
-        Returns:
-            (bool): Whether the project deletion was successful
-        """
-        raw_response = r.delete(
-            f"https://api.modrinth.com/v2/project/{self.model.slug}",
-            headers={"authorization": self._get_auth(auth)},
-            timeout=60,
-        )
-
-        match raw_response.status_code:
-            case 400:
-                raise exceptions.NotFoundError("The requested project was not found")
-
-            case 401:
-                raise exceptions.NoAuthorizationError(
-                    "No authorization to delete this project"
-                )
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        return True
-
-    def get_dependencies(self) -> list["Project"]:
-        """Gets the dependencies of the project
-
-        Raises:
-            NotFoundError: The requested project wasn't found or no authorization to see this project
-            InvalidRequestError: Invalid request
-
-        Returns:
-            (list[Project]): The dependencies of the project
-        """
-        raw_response = r.get(
-            f"https://api.modrinth.com/v2/project/{self.model.slug}/dependencies",
-            timeout=60,
-        )
-
-        match raw_response.status_code:
-            case 404:
-                raise exceptions.NotFoundError(
-                    "The requested project wasn't found or no authorization to see this project"
-                )
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        response = raw_response.json()
-        return [Project(dependency) for dependency in response.get("projects")]
-
-    @staticmethod
-    def search(
-        query: str = "",
-        facets: list[list[str]] | None = None,
-        index: literals.index_literal = "relevance",
-        offset: int = 0,
-        limit: int = 10,
-        filters: list[str] | None = None,
-    ) -> list["Project.SearchResult"]:
-        """Searches for projects
-
-        Args:
-            query (str, optional): The query to search for
-            facets (list[list[str]], optional): The recommended way of filtering search results. [Learn more about using facets](https://docs.modrinth.com/docs/tutorials/api_search)
-            index (Literal["relevance", "downloads", "follows", "newest", "updated"], optional): The sorting method used for sorting search results
-            offset (int, optional): The offset into the search. Skip this number of results
-            limit (int, optional): The number of results returned by the search
-            filters (list[str], optional): A list of filters relating to the properties of a project. Use filters when there isn't an available facet for your needs. [More information](https://docs.meilisearch.com/reference/features/filtering.html)
-
-        Raises:
-            NotFoundError: The requested project wasn't found or no authorization to see this project
-            InvalidRequestError: Invalid request
-
-        Returns:
-            (list[Project.SearchResult]): The project search results
-        """
-        params = {}
-        if query != "":
-            params.update({"query": query})
-        if facets:
-            params.update({"facets": json.dumps(facets)})
-        if index != "relevance":
-            params.update({"index": index})
-        if offset != 0:
-            params.update({"offset": str(offset)})
-        if limit != 10:
-            params.update({"limit": str(limit)})
-        if filters:
-            params.update({"filters": json.dumps(filters)})
-        raw_response = r.get(
-            "https://api.modrinth.com/v2/search", params=params, timeout=60
-        )
-        response = raw_response.json()
-        return [
-            Project.SearchResult(models.SearchResultModel._from_json(project))
-            for project in response.get("hits")
-        ]
-
-    def get_team_members(self) -> "list[teams.Team.TeamMember]":
-        """Gets the team members of the project
-
-        Returns:
-            (list[Project.TeamMember)]: The team members of the project
-        """
-        raw_response = r.get(
-            f"https://api.modrinth.com/v2/project/{self.model.id}/members", timeout=60
-        )
-
-        match raw_response.status_code:
-            case 404:
-                raise exceptions.NotFoundError(
-                    "The requested project wasn't found or no authorization to see this project"
-                )
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        response = raw_response.json()
-
-        return [
-            teams.Team.TeamMember._from_json(team_member) for team_member in response
-        ]
-
-    def get_team(self) -> "teams.Team":
-        """Gets the project's team
-
-        Raises:
-            NotFoundError: The requested project wasn't found or no authorization to see this project
-            InvalidRequestError: Invalid request
-
-        Returns:
-            (Team): The project's team
-        """
-        raw_response = r.get(
-            f"https://api.modrinth.com/v2/project/{self.model.id}/members", timeout=60
-        )
-
-        match raw_response.status_code:
-            case 404:
-                raise exceptions.NotFoundError(
-                    "The requested project wasn't found or no authorization to see this project"
-                )
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        response = raw_response.json()
-
-        return teams.Team._from_json(response)
-
-    def __repr__(self) -> str:
-        """Returns a string representation of the Project instance
-
-        Returns:
-            (str): A string representation of the Project instance
-        """
-        return f"Project: {self.model.title}"
-
-    class Version:
-        """Versions contain download links to files with additional metadata
-
-        Attributes:
-            model (VersionModel): The version model associated with the version
-
-        """
-
-        def __init__(self, version_model: "models.VersionModel") -> None:
-            """
-            Args:
-                version_model (VersionModel): The version model to associate with the Version object
-            """
-            self.model = version_model
-
-        def get_type(self) -> str:
-            """Gets the type of the version
-
-            Returns:
-                (str): The type of the version
-            """
-            return self.model.version_type
-
-        def get_dependencies(self) -> list["Project.Dependency"]:
-            """Gets the dependencies of the version
-
-            Returns:
-                (list[Project.Dependency]): The dependencies of the version
-            """
-            result = []
-            for dependency in self.model.dependencies:
-                result.append(Project.Dependency._from_json(dependency))
-            return result
-
-        @staticmethod
-        def get(id_: str) -> "Project.Version":
-            """Gets a version by ID
-
-            Args:
-                id_ (str): The ID of the version
-
-            Raises:
-                NotFoundError: The requested version wasn't found or no authorization to see this version
-                InvalidRequestError: Invalid request
-
-            Returns:
-                (Project.Version): The version that was found
-            """
-            raw_response = r.get(
-                f"https://api.modrinth.com/v2/version/{id_}", timeout=60
-            )
-            match raw_response.status_code:
-                case 404:
-                    raise exceptions.NotFoundError(
-                        "The requested version wasn't found or no authorization to see this version"
-                    )
-            if not raw_response.ok:
-                raise exceptions.InvalidRequestError(raw_response.text)
-            response = raw_response.json()
-            return Project.Version(models.VersionModel._from_json(response))
-
-        @staticmethod
-        def get_from_hash(
-            hash_: str,
-            algorithm: literals.sha_algorithm_literal = "sha1",
-            multiple: bool = False,
-        ) -> typing.Union["Project.Version", list["Project.Version"]]:
-            """Gets a version by hash
-
-            Args:
-                hash_ (str): The hash of the file, considering its byte content, and encoded in hexadecimal
-                algorithm (Literal["sha512", "sha1"]): The algorithm of the hash
-                multiple (bool): Whether to return multiple results when looking for this hash
-
-            Raises:
-                NotFoundError: The requested version file wasn't found or no authorization to see this version
-                InvalidRequestError: Invalid request
-
-            Returns:
-                (Project.Version): The version that was found
-            """
-            raw_response = r.get(
-                f"https://api.modrinth.com/v2/version_file/{hash_}",
-                params={"algorithm": algorithm, "multiple": str(multiple).lower()},
-                timeout=60,
-            )
-            match raw_response.status_code:
-                case 404:
-                    raise exceptions.NotFoundError(
-                        "The requested version file wasn't found or no authorization to see this version"
-                    )
-            if not raw_response.ok:
-                raise exceptions.InvalidRequestError(raw_response.text)
-            response = raw_response.json()
-            if isinstance(response, list):
-                return [
-                    Project.Version(models.VersionModel._from_json(version))
-                    for version in response
-                ]
-            return Project.Version(models.VersionModel._from_json(response))
-
-        @staticmethod
-        def delete_file_from_hash(
-            auth: str,
-            hash_: str,
-            version_id: str,
-            algorithm: literals.sha_algorithm_literal = "sha1",
-        ) -> typing.Literal[True]:
-            """Deletes a file from its hash
-
-            Args:
-                hash_ (str): The hash of the file, considering its byte content, and encoded in hexadecimal
-                algorithm (Literal["sha512", "sha1"]): The algorithm of the hash
-                version_id (bool): Version ID to delete the version from, if multiple files of the same hash exist
-                auth (str): The authorization token to use when deleting the file from its hash
-
-            Raises:
-                NotFoundError: The requested version wasn't found
-                NoAuthorizationError: No authorization to delete this file
-                InvalidRequestError: Invalid request
-
-            Returns:
-                (bool): If the file deletion was successful
-            """
-            raw_response = r.delete(
-                f"https://api.modrinth.com/v2/version_file/{hash_}",
-                params={"algorithm": algorithm, "version_id": version_id},
-                headers={"authorization": auth},
-                timeout=60,
-            )
-            match raw_response.status_code:
-                case 404:
-                    raise exceptions.NotFoundError(
-                        "The requested version was not found"
-                    )
-                case 401:
-                    raise exceptions.NoAuthorizationError(
-                        "No authorization to delete this file"
-                    )
-            if not raw_response.ok:
-                raise exceptions.InvalidRequestError(raw_response.text)
-            return True
-
-        def get_files(self) -> list["Project.File"]:
-            """Gets the files associated with the version
-
-            Returns:
-                (list[Project.File]): The files associated with the version
-            """
-            result = []
-            for file in self.model.files:
-                result.append(Project.File._from_json(file))  # type: ignore
-            return result
-
-        def download(self, recursive: bool = False) -> None:
-            """Downloads the files associated with the version
-
-            Args:
-                recursive (bool, optional): Whether to also download the files of the dependencies
-            """
-            files = self.get_files()
-            for file in files:
-                file_content = r.get(file.url).content
-                open(file.name, "wb").write(file_content)
-
-            if recursive:
-                dependencies = self.get_dependencies()
-                for dep in dependencies:
-                    files = dep.get_version().get_files()
-                    for file in files:
-                        file_content = r.get(file.url).content
-                        open(file.name, "wb").write(file_content)
-
-        def get_project(self) -> "Project":
-            """Gets the project associated with the version
-
-            Returns:
-                (Project): The project associated with the version
-            """
-            return modrinth.Modrinth.get_project(self.model.project_id)  # type: ignore
-
-        def get_primary_files(self) -> list["Project.File"]:
-            """Gets the primary files associated with the version
-
-            Returns:
-                (list[Project.File]): The primary files associated with the version
-            """
-            result = []
-            for file in self.get_files():
-                if file.primary:
-                    result.append(file)
-            return result
-
-        def get_author(self) -> "users.User":
-            """Gets the author of the version
-
-            Returns:
-                (User): The author of the version
-            """
-            user = users.User.get(self.model.author_id)  # type: ignore
-            return user
-
-        def is_featured(self) -> bool:
-            """Checks if the version is featured
-
-            Returns:
-                (bool): Whether the version is featured
-            """
-            return self.model.featured
-
-        def get_date_published(self) -> "dt.datetime":
-            """Gets the date when the version was published
-
-            Returns:
-                (datetime): The date when the version was published
-            """
-            return util.format_time(self.model.date_published)
-
-        def get_downloads(self) -> int:
-            """Gets the number of downloads for the version
-
-            Returns:
-                (int): The number of downloads of the version
-            """
-            return self.model.downloads  # type: ignore
-
-        def get_name(self) -> str:
-            """Gets the name of the version
-
-            Returns:
-                (str): The name of the version
-            """
-            return self.model.name
-
-        def get_version_number(self) -> str:
-            """Gets the version number of the version
-
-            Returns:
-                (str): The version number of the version
-            """
-            return self.model.version_number
-
-        def __repr__(self) -> str:
-            return f"Version: {self.model.name}"
-
-    class GalleryImage:
-        """
-        Represents an image in a gallery
-
-        Attributes:
-            file_path (str): The path to the image
-            ext (str): Image extension
-            featured (str): Whether an image is featured
-            title (str): Title of the image
-            description (str): Description of the image
-            ordering (int): Ordering of the image
-
-        """
-
-        def __init__(
-            self,
-            file_path: str,
-            featured: bool,
-            title: str,
-            description: str,
-            ordering: int = 0,
-        ) -> None:
-            """
-            Initializes a GalleryImage object
-
-            Args:
-                file_path (str): The path to the image
-                featured (str): Whether an image is featured
-                title (str): Title of the image
-                description (str): Description of the image
-                ordering (int): Ordering of the image
-            """
-            self.file_path = file_path
-            self.ext = file_path.split(".")[-1]
-            self.featured = str(featured).lower()
-            self.title = title
-            self.description = description
-            self.ordering = ordering
-
-        @staticmethod
-        def _from_json(json_: dict) -> "Project.GalleryImage":
-            return Project.GalleryImage(
-                json_.get("url"),  # type: ignore
-                json_.get("featured"),  # type: ignore
-                json_.get("title"),  # type: ignore
-                json_.get("description"),  # type: ignore
-                json_.get("ordering"),  # type: ignore
-            )
-
-        def _to_json(self) -> dict:
-            return util.remove_null_values(self.__dict__)
-
-    class File:
-        """
-        Represents a file with various attributes and methods
-
-        Attributes:
-            hashes (dict[str, str]): A dictionary of hash algorithms and their corresponding hash values for the file
-            url (str): The URL where the file can be downloaded
-            name (str): The name of the file
-            primary (str): The primary hash algorithm used to verify the file's integrity
-            size (int): The size of the file in bytes
-            file_type (str): The type of the file
-            extension (str): The file extension
-
-        """
-
-        def __init__(
-            self,
-            hashes: dict[str, str],
-            url: str,
-            filename: str,
-            primary: str,
-            size: int,
-            file_type: str,
-        ) -> None:
-            """
-            Initializes a File object
-
-            Args:
-                hashes (dict[str, str]): A dictionary of hash algorithms and their corresponding hash values for the file
-                url (str): The URL where the file can be downloaded
-                filename (str): The name of the file
-                primary (str): The primary hash algorithm used to verify the file's integrity
-                size (int): The size of the file in bytes
-                file_type (str): The type of the file
-            """
-            self.hashes = hashes
-            self.url = url
-            self.name = filename
-            self.primary = primary
-            self.size = size
-            self.file_type = file_type
-            self.extension = filename.split(".")[-1]
-
-        def is_resourcepack(self) -> bool:
-            """
-            Checks if a file is a resourcepack
-
-            Returns:
-                (bool): If the file is a resourcepack
-            """
-            if self.file_type is None:
-                return False
-            return True
-
-        @staticmethod
-        def _from_json(json_: dict) -> "Project.File":
-            result = Project.File(
-                json_.get("hashes"),  # type: ignore
-                json_.get("url"),  # type: ignore
-                json_.get("filename"),  # type: ignore
-                json_.get("primary"),  # type: ignore
-                json_.get("size"),  # type: ignore
-                json_.get("file_type"),  # type: ignore
-            )
-            return result
-
-        def __repr__(self) -> str:
-            return f"File: {self.name}"
-
-    class License:
-        """
-        Represents a license
-
-        Attributes:
-            id (str): The SPDX license ID of a project
-            name (str): The long name of a license
-            url (str): The URL to this license
-
-        """
-
-        def __init__(self, id_: str, name: str, url: str | None = None) -> None:
-            """
-            Initializes a License object
-
-            Args:
-                id_ (str): The SPDX license ID of a project
-                name (str): The long name of a license
-                url (str): The URL to this license
-            """
-            self.id = id_
-            self.name = name
-            self.url = url
-
-        @staticmethod
-        def _from_json(json_: dict) -> "Project.License":
-            result = Project.License(
-                json_.get("id"),  # type: ignore
-                json_.get("name"),  # type: ignore
-                json_.get("url"),  # type: ignore
-            )
-
-            return result
-
-        def _to_json(self) -> dict:
-            return self.__dict__
-
-        def __repr__(self) -> str:
-            return f"License: {self.name if self.name else self.id}"
-
-    class Donation:
-        """
-        Represents a donation
-
-        Attributes:
-            id (str): The ID of the donation platform
-            platform (str): The donation platform this link is to
-            url (str): The URL of the donation platform and user
-
-        """
-
-        def __init__(self, id_: str, platform: str, url: str) -> None:
-            """
-            Initializes a Donation object
-
-            Args:
-                id_ (str): The ID of the donation
-                platform (str): The platform used for the donation
-                url (str): The URL to the donation page
-            """
-            self.id = id_
-            self.platform = platform
-            self.url = url
-
-        @staticmethod
-        def _from_json(json_: dict) -> "Project.Donation":
-            result = Project.Donation(
-                json_.get("id"),  # type: ignore
-                json_.get("platform"),  # type: ignore
-                json_.get("url"),  # type: ignore
-            )
-
-            return result
-
-        def __repr__(self) -> str:
-            return f"Donation: {self.platform}"
-
-    class Dependency:
-        """
-        Represents a dependency
-
-        Attributes:
-            dependency_type (str): The type of the dependency
-            id (str): The ID of the dependency
-            dependency_option (str): The option for the dependency
-        """
-
-        def __init__(self) -> None:
-            self.dependency_option: str | None = None
-            self.file_name: str | None = None
-            self.version_id: str | None = None
-            self.project_id: str | None = None
-
-        def _to_json(self) -> dict:
-            return self.__dict__
-
-        @staticmethod
-        def _from_json(json_: dict) -> "Project.Dependency":
-            result = Project.Dependency()
-            result.version_id = json_.get("version_id")
-            result.project_id = json_.get("project_id")
-            result.dependency_option = json_.get("dependency_option")
-            result.file_name = json_.get("file_name")
-            return result
-
-        def get_version(self) -> "Project.Version":
-            id_ = self.project_id
-            if self.version_id:
-                id_ = self.version_id
-            return Project.Version.get(id_)  # type: ignore
-
-        def is_required(self) -> bool:
-            """
-            Checks if the dependency is required
-
-            Returns:
-                (bool): True if the dependency is required, False otherwise
-            """
-            return True if self.dependency_option == "required" else False
-
-        def is_optional(self) -> bool:
-            """
-            Checks if the dependency is optional
-
-            Returns:
-                (bool): True if the dependency is optional, False otherwise
-            """
-            return True if self.dependency_option == "optional" else False
-
-        def is_incompatible(self) -> bool:
-            """
-            Checks if the dependency is incompatible
-
-            Returns:
-                (bool): True if the dependency is incompatible, False otherwise
-            """
-            return True if self.dependency_option == "incompatible" else False
-
-    class SearchResult:
-        """
-        Represents a search result
-
-        Attributes:
-            model (SearchResultModel): The search result model
-
-        """
-
-        def __init__(self, search_result_model: "models.SearchResultModel") -> None:
-            """
-            Initializes a SearchResult object
-
-            Args:
-                search_result_model (SearchResultModel): The search result model or a dictionary representing the search result model
-            """
-            self.model = search_result_model
-
-        def __repr__(self) -> str:
-            return f"Search Result: {self.model.title}"
+"""Projects can be mods or modpacks and are created by users"""
+
+import datetime as dt
+import json
+import typing
+
+import requests as r
+
+import pyrinth.exceptions as exceptions
+import pyrinth.literals as literals
+import pyrinth.models as models
+import pyrinth.modrinth as modrinth
+import pyrinth.users as users
+import pyrinth.util as util
+import pyrinth.teams as teams
+
+
+class Project:
+    """Projects can be mods or modpacks and are created by users
+
+    Attributes:
+        model (ProjectModel): The project's model
+    """
+
+    def __init__(self, project_model: "models.ProjectModel") -> None:
+        """
+        Args:
+            project_model (ProjectModel): The project's model
+        """
+        if isinstance(project_model, dict):
+            project_model = models.ProjectModel._from_json(project_model)
+        self.model = project_model
+
+    def get_donations(self) -> list["Project.Donation"]:
+        """Gets the project's donations
+
+        Returns:
+            (list[Donation]): The project's donations
+        """
+        return util.list_to_object(Project.Donation, self.model.donation_urls)
+
+    def _get_auth(self, auth: str | None) -> str:
+        if auth:
+            return auth
+        return self.model.auth  # type: ignore
+
+    @staticmethod
+    def get(id_: str, auth: object = None) -> "Project":
+        """Gets a project based on an ID
+
+        Args:
+            id_ (str): The ID or slug of the project
+            auth (str, optional): An optional authorization token when getting the project
+
+        Raises:
+            NotFoundError: The requested project wasn't found or no authorization to see this project
+            InvalidRequestError: Invalid request
+
+        Returns:
+            (Project): The project that was found
+        """
+        raw_response = r.get(
+            f"https://api.modrinth.com/v2/project/{id_}",
+            headers={"authorization": auth},  # type: ignore
+            timeout=60,
+        )
+        match raw_response.status_code:
+            case 404:
+                raise exceptions.NotFoundError(
+                    "The requested project wasn't found or no authorization to see this project"
+                )
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+        response = raw_response.json()
+        response.update({"authorization": auth})
+        return Project(response)
+
+    @staticmethod
+    def get_multiple(ids: list[str]) -> list["Project"]:
+        """Gets multiple projects
+
+        Args:
+            ids (list[str]): The IDs of the projects
+
+        Raises:
+            InvalidRequestError: Invalid request
+
+        Returns:
+            (list[Project]): The projects that were found
+        """
+        raw_response = r.get(
+            "https://api.modrinth.com/v2/projects",
+            params={"ids": json.dumps(ids)},
+            timeout=60,
+        )
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+        response = raw_response.json()
+        return [Project(project) for project in response]
+
+    def get_latest_version(
+        self,
+        loaders: list[str] | None = None,
+        game_versions: list[str] | None = None,
+        featured: bool | None = None,
+        types: literals.version_type_literal | None = None,
+        auth: str | None = None,
+    ) -> "Project.Version":
+        """Gets this project's latest version
+
+        Args:
+            loaders (list[str], optional): The loaders filter. Defaults to None
+            game_versions (list[str], optional): The game versions filter. Defaults to None
+            featured (bool, optional): The is featured filter. Defaults to None
+            types (Literal["release", "beta", "alpha"], optional): The types filter. Defaults to None
+            auth (str, optional): The authorization token. Defaults to None
+
+        Returns:
+            (Project.Version): The project's latest version
+        """
+        versions = self.get_versions(loaders, game_versions, featured, types, auth)
+
+        return versions[0]
+
+    def get_gallery(self) -> list["Project.GalleryImage"]:
+        """Gets the project's gallery
+
+        Returns:
+            (list[Project.GalleryImage]): The project's gallery images
+        """
+        result = util.list_to_object(Project.GalleryImage, self.model.gallery)
+
+        return result
+
+    def is_client_side(self) -> bool:
+        """Checks if this project is client side
+
+        Returns:
+            (bool): Whether this project is client side
+        """
+        return True if self.model.client_side == "required" else False
+
+    def is_server_side(self) -> bool:
+        """Checks if this project is server side
+
+        Returns:
+            (bool): Whether this project is server side
+        """
+        return True if self.model.server_side == "required" else False
+
+    def get_downloads(self) -> int:
+        """Gets the number of downloads this project has
+
+        Returns:
+            (int): The number of downloads for this project
+        """
+        return self.model.downloads  # type: ignore
+
+    def get_categories(self) -> list[str]:
+        """Gets this projects categories
+
+        Returns:
+            (list[str]): The categories associated with this project
+        """
+        return self.model.categories
+
+    def get_additional_categories(self) -> list[str]:
+        """Gets this projects additional categories
+
+        Returns:
+            (list[str]): The additional categories associated with this project
+        """
+        return self.model.additional_categories  # type: ignore
+
+    def get_all_categories(self) -> list[str]:
+        """Gets this projects categories and additional categories
+
+        Returns:
+            (list[str]): The categories and additional categories associated with this project
+        """
+        return self.get_categories() + self.get_additional_categories()
+
+    def get_license(self) -> "Project.License":
+        """Gets this project license
+
+        Returns:
+            (Project.License): The license associated with this project
+        """
+        return Project.License._from_json(self.model.license)
+
+    def get_specific_version(
+        self, semantic_version: str
+    ) -> typing.Optional["Project.Version"]:
+        """Gets a specific version based on the semantic version
+
+        Args:
+            semantic_version (str): The semantic version to search for
+
+        Returns:
+            (Project.Version): The version that was found using the semantic version
+            (None): No version was found with that semantic version
+        """
+        versions = self.get_versions()
+        if versions:
+            for version in versions:
+                if version.model.version_number == semantic_version:
+                    return version
+
+        return None
+
+    def download(self, recursive: bool = False) -> None:
+        """Downloads this project
+
+        Args:
+            recursive (bool): Whether to download dependencies. Defaults to False
+        """
+        latest = self.get_latest_version()
+        files = latest.get_files()
+        for file in files:
+            file_content = r.get(file.url).content
+            open(file.name, "wb").write(file_content)
+
+        if recursive:
+            dependencies = latest.get_dependencies()
+            for dep in dependencies:
+                files = dep.get_version().get_files()
+                for file in files:
+                    file_content = r.get(file.url).content
+                    open(file.name, "wb").write(file_content)
+
+    def get_versions(
+        self,
+        loaders: list[str] | None = None,
+        game_versions: list[str] | None = None,
+        featured: bool | None = None,
+        types: literals.version_type_literal | None = None,
+        auth: str | None = None,
+    ) -> list["Project.Version"]:
+        """Gets project versions based on filters
+
+        Args:
+            loaders (list[str], optional): The types of loaders to filter for
+            game_versions (list[str], optional): The game versions to filter for
+            featured (bool, optional): Allows to filter for featured or non-featured versions only
+            types (Literal["release", "beta", "alpha"], optional): The release type of version
+            auth (str, optional): An optional authorization token to use when getting the project versions
+
+        Raises:
+            NotFoundError: The requested project wasn't found or no authorization to see this project
+            InvalidRequestError: Invalid request
+
+        Returns:
+            (list[Project.Version]): The versions that were found
+        """
+        filters = {
+            "loaders": loaders,
+            "game_versions": game_versions,
+            "featured": featured,
+        }
+
+        filters = util.remove_null_values(filters)
+        raw_response = r.get(
+            f"https://api.modrinth.com/v2/project/{self.model.slug}/version",
+            params=util.json_to_query_params(filters),
+            headers={"authorization": self._get_auth(auth)},
+            timeout=60,
+        )
+
+        match raw_response.status_code:
+            case 404:
+                raise exceptions.NotFoundError(
+                    "The requested project wasn't found or no authorization to see this project"
+                )
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        response = raw_response.json()
+
+        versions = [
+            self.Version(models.VersionModel._from_json(version))
+            for version in response
+        ]
+
+        if not types:
+            return versions
+
+        result = []
+        for version in versions:
+            if version.model.version_type in types:
+                result.append(version)
+
+        return result
+
+    def get_oldest_version(
+        self,
+        loaders: list[str] | None = None,
+        game_versions: list[str] | None = None,
+        featured: bool | None = None,
+        types: literals.version_type_literal | None = None,
+        auth: str | None = None,
+    ) -> "Project.Version":
+        """Gets the oldest project version
+
+        Args:
+            loaders (list[str], optional): The types of loaders to filter for
+            game_versions (list[str], optional): The game versions to filter for
+            featured (bool, optional): Allows to filter for featured or non-featured versions only
+            types (Literal["release", "beta", "alpha"], optional): The type of version
+            auth (str, optional): An optional authorization token to use when getting the project versions
+
+        Returns:
+            (Project.Version): The version that was found
+        """
+        versions = self.get_versions(loaders, game_versions, featured, types, auth)
+
+        return versions[-1]
+
+    def get_id(self) -> str:
+        """Gets the ID of the project
+
+        Returns:
+            (str): The ID of the project
+        """
+        return self.model.id  # type: ignore
+
+    def get_slug(self) -> str:
+        """Gets the slug of the project
+
+        Returns:
+            (str): The slug of the project
+        """
+        return self.model.slug
+
+    def get_name(self) -> str:
+        """Gets the name of the project
+
+        Returns:
+            (str): The name of the project
+        """
+        return self.model.title
+
+    @staticmethod
+    def get_version(id_: str) -> "Project.Version":
+        """Gets a version by ID
+
+        Args:
+            id_ (str): The ID of the version
+
+        Raises:
+            NotFoundError: The requested version wasn't found or no authorization to see this version
+            InvalidRequestError: Invalid request
+
+        Returns:
+            (Project.Version): The version that was found
+        """
+        raw_response = r.get(f"https://api.modrinth.com/v2/version/{id_}", timeout=60)
+
+        match raw_response.status_code:
+            case 404:
+                raise exceptions.NotFoundError(
+                    "The requested version wasn't found or no authorization to see this version"
+                )
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        response = raw_response.json()
+        return Project.Version(models.VersionModel._from_json(response))
+
+    def create_version(self, version_model, auth: str | None = None) -> int:
+        """Creates a new version on the project
+
+        Args:
+            auth (str, optional): The authorization token to use when creating the version
+            version_model (VersionModel): The model to use when creating the version
+
+        Raises:
+            NoAuthorizationError: No authorization to create this version
+            InvalidRequestError: Invalid request
+
+        Returns:
+            (int): Whether creating the version was successful
+        """
+        version_model.project_id = self.model.id
+
+        files = {"data": version_model.to_bytes()}
+
+        for file in version_model.files:
+            files.update({util.remove_file_path(file): open(file, "rb").read()})
+
+        raw_response = r.post(
+            "https://api.modrinth.com/v2/version",
+            headers={"authorization": self._get_auth(auth)},
+            files=files,
+            timeout=60,
+        )
+
+        match raw_response.status_code:
+            case 401:
+                raise exceptions.NoAuthorizationError(
+                    "No authorization to create this version"
+                )
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        return True
+
+    def change_icon(self, file_path: str, auth: str | None = None) -> bool:
+        """Changes the project icon
+
+        Args:
+            file_path (str): The file path of the image to use for the new project icon
+            auth (str, optional): The authorization token to use when changing the project icon
+
+        Raises:
+            InvalidParamError: Invalid input for new icon
+            InvalidRequestError: Invalid request
+
+        Returns:
+            (bool): Whether the project icon change was successful
+        """
+        raw_response = r.patch(
+            f"https://api.modrinth.com/v2/project/{self.model.slug}/icon",
+            params={"ext": file_path.split(".")[-1]},
+            headers={"authorization": self._get_auth(auth)},
+            data=open(file_path, "rb"),
+            timeout=60,
+        )
+
+        match raw_response.status_code:
+            case 400:
+                raise exceptions.InvalidParamError("Invalid input for new icon")
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        return True
+
+    def delete_icon(self, auth: str | None = None) -> bool:
+        """Deletes the project icon
+
+        Args:
+            auth (str, optional): The authorization token to use when deleting the project icon
+
+        Raises:
+            InvalidParamError: Invalid input
+            NoAuthorizationError: No authorization to edit this project
+            InvalidRequestError: Invalid request
+
+        Returns:
+            (bool): Whether the project icon deletion was successful
+        """
+        raw_response = r.delete(
+            f"https://api.modrinth.com/v2/project/{self.model.slug}/icon",
+            headers={"authorization": self._get_auth(auth)},
+            timeout=60,
+        )
+
+        match raw_response.status_code:
+            case 400:
+                raise exceptions.InvalidParamError("Invalid input")
+
+            case 401:
+                raise exceptions.NoAuthorizationError(
+                    "No authorization to edit this project"
+                )
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        return True
+
+    def add_gallery_image(
+        self, image: "Project.GalleryImage", auth: str | None = None
+    ) -> bool:
+        """Adds a gallery image to the project
+
+        Args:
+            image (Project.GalleryImage): The gallery image to add
+            auth (str, optional): The authorization token to use when adding the gallery image
+
+        Raises:
+            NoAuthorizationError: No authorization to create a gallery image
+            NotFoundError: The requested project wasn't found or no authorization to see this project
+            InvalidRequestError: Invalid request
+
+        Returns:
+            (bool): If the gallery image addition was successful
+        """
+        raw_response = r.post(
+            f"https://api.modrinth.com/v2/project/{self.model.slug}/gallery",
+            headers={"authorization": self._get_auth(auth)},
+            params=image._to_json(),
+            data=open(image.file_path, "rb"),
+            timeout=60,
+        )
+
+        match raw_response.status_code:
+            case 401:
+                raise exceptions.NoAuthorizationError(
+                    "No authorization to create a gallery image"
+                )
+
+            case 404:
+                raise exceptions.NotFoundError(
+                    "The requested project wasn't found or no authorization to see this project"
+                )
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        return True
+
+    def modify_gallery_image(
+        self,
+        url: str,
+        featured: bool | None = None,
+        title: str | None = None,
+        description: str | None = None,
+        ordering: int | None = None,
+        auth: str | None = None,
+    ) -> bool:
+        """Modifies a gallery image
+
+        Args:
+            url (str): URL link of the image to modify
+            featured (bool, optional): Whether the image is featured
+            title (str, optional): New title of the image
+            description (str, optional): New description of the image
+            ordering (int, optional): New ordering of the image
+            auth (str, optional): Authentication token when modifying the gallery image
+
+        Raises:
+            NoAuthorizationError: No authorization to edit this gallery image
+            NotFoundError: The requested project wasn't found or no authorization to see this project
+            InvalidRequestError: Invalid request
+
+        Returns:
+            (bool): Whether the gallery image modification was successful
+        """
+        modified_json = {
+            "url": url,
+            "featured": featured,
+            "title": title,
+            "description": description,
+            "ordering": ordering,
+        }
+
+        modified_json = util.remove_null_values(modified_json)
+
+        raw_response = r.patch(
+            f"https://api.modrinth.com/v2/project/{self.model.slug}/gallery",
+            params=modified_json,
+            headers={"authorization": self._get_auth(auth)},
+            timeout=60,
+        )
+
+        match raw_response.status_code:
+            case 401:
+                raise exceptions.NoAuthorizationError(
+                    "No authorization to edit this gallery image"
+                )
+
+            case 404:
+                raise exceptions.NotFoundError(
+                    "The requested project wasn't found or no authorization to see this project"
+                )
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        return True
+
+    def delete_gallery_image(self, url: str, auth: str | None = None) -> bool:
+        """Deletes a gallery image
+
+        Args:
+            url (str): URL link of the image to delete
+            auth (str, optional): Authentication token to use when deleting the gallery image
+
+        Raises:
+            InvalidParamError: Invalid URL or project specified
+            NoAuthorizationError: No authorization to delete this gallery image
+            InvalidRequestError: Invalid request
+
+        Returns:
+            (bool): Whether the gallery image deletion was successful
+        """
+        if "-raw" in url:
+            raise exceptions.InvalidParamError(
+                "Please use cdn.modrinth.com instead of cdn-raw.modrinth.com"
+            )
+
+        raw_response = r.delete(
+            f"https://api.modrinth.com/v2/project/{self.model.slug}/gallery",
+            headers={"authorization": self._get_auth(auth)},
+            params={"url": url},
+            timeout=60,
+        )
+
+        match raw_response.status_code:
+            case 400:
+                raise exceptions.InvalidParamError("Invalid URL or project specified")
+
+            case 401:
+                raise exceptions.NoAuthorizationError(
+                    "No authorization to delete this gallery image"
+                )
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        return True
+
+    def modify(
+        self,
+        slug: str | None = None,
+        title: str | None = None,
+        description: str | None = None,
+        categories: list[str] | None = None,
+        client_side: str | None = None,
+        server_side: str | None = None,
+        body: str | None = None,
+        additional_categories: list[str] | None = None,
+        issues_url: str | None = None,
+        source_url: str | None = None,
+        wiki_url: str | None = None,
+        discord_url: str | None = None,
+        license_id: str | None = None,
+        license_url: str | None = None,
+        status: literals.project_status_literal | None = None,
+        requested_status: literals.requested_project_status_literal | None = None,
+        moderation_message: str | None = None,
+        moderation_message_body: str | None = None,
+        auth: str | None = None,
+    ) -> bool:
+        """Modifies the project
+
+        Args:
+            slug (str, optional): The slug of a project, used for vanity URLs. Regex: ^[\\w!@$()`.+,"\\-']{3,64}$
+            title (str, optional): The title or name of the project
+            description (str, optional): A short description of the project
+            categories (list[str], optional): A list of categories that the project has
+            client_side (str, optional): The client side support of the project
+            server_side (str, optional): The server side support of the project
+            body (str, optional): A long form description of the project
+            additional_categories (list[str], optional): A list of categories which are searchable but non-primary
+            issues_url (str, optional): An optional link to where to submit bugs or issues with the project
+            source_url (str, optional): An optional link to the source code of the project
+            wiki_url (str, optional): An optional link to the project's wiki page or other relevant information
+            discord_url (str, optional): An optional invite link to the project's discord
+            license_id (str, optional): The SPDX license ID of a project
+            license_url (str, optional): The URL to this license
+            status (Literal["approved", "archived", "rejected", "draft", "unlisted", "processing", "withheld", "scheduled", "private", "unknown"], optional): The status of the project
+            requested_status (Literal["approved", "archived", "unlisted", "private", "draft"], optional): The requested status when submitting for review or scheduling the project for release
+            moderation_message (str, optional): The title of the moderators' message for the project
+            moderation_message_body (str, optional): The body of the moderators' message for the project
+            auth (str, optional): Authentication token to use when modifying the project
+
+        Raises:
+            InvalidParamError: Please specify at least 1 optional argument
+            NoAuthorizationError: No authorization to modify this project
+            NotFoundError: The requested project wasn't found or no authorization to see this project
+            InvalidRequestError: Invalid request
+
+        Returns:
+            (bool): Whether the project modification was successful
+        """
+        modified_json = {
+            "slug": slug,
+            "title": title,
+            "description": description,
+            "categories": categories,
+            "client_side": client_side,
+            "server_side": server_side,
+            "body": body,
+            "additional_categories": additional_categories,
+            "issues_url": issues_url,
+            "source_url": source_url,
+            "wiki_url": wiki_url,
+            "discord_url": discord_url,
+            "license_id": license_id,
+            "license_url": license_url,
+            "status": status,
+            "requested_status": requested_status,
+            "moderation_message": moderation_message,
+            "moderation_message_body": moderation_message_body,
+        }
+
+        modified_json = util.remove_null_values(modified_json)
+
+        if not modified_json:
+            raise exceptions.InvalidParamError(
+                "Please specify at least 1 optional argument"
+            )
+
+        raw_response = r.patch(
+            f"https://api.modrinth.com/v2/project/{self.model.slug}",
+            data=json.dumps(modified_json),
+            headers={
+                "Content-Type": "application/json",
+                "authorization": self._get_auth(auth),
+            },
+            timeout=60,
+        )
+
+        match raw_response.status_code:
+            case 401:
+                raise exceptions.NoAuthorizationError(
+                    "No authorization to edit this project"
+                )
+
+            case 404:
+                raise exceptions.NotFoundError(
+                    "The requested project wasn't found or no authorization to see this project"
+                )
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        return True
+
+    def delete(self, auth: str | None = None) -> typing.Literal[True]:
+        """Deletes the project
+
+        Args:
+            auth (str, optional): Authentication token to use when deleting the project
+
+        Raises:
+            NotFoundError: The requested project wasn't found
+            NoAuthorizationError: No authorization to delete this project
+            InvalidRequestError: Invalid request
+
+        Returns:
+            (bool): Whether the project deletion was successful
+        """
+        raw_response = r.delete(
+            f"https://api.modrinth.com/v2/project/{self.model.slug}",
+            headers={"authorization": self._get_auth(auth)},
+            timeout=60,
+        )
+
+        match raw_response.status_code:
+            case 400:
+                raise exceptions.NotFoundError("The requested project was not found")
+
+            case 401:
+                raise exceptions.NoAuthorizationError(
+                    "No authorization to delete this project"
+                )
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        return True
+
+    def get_dependencies(self) -> list["Project"]:
+        """Gets the dependencies of the project
+
+        Raises:
+            NotFoundError: The requested project wasn't found or no authorization to see this project
+            InvalidRequestError: Invalid request
+
+        Returns:
+            (list[Project]): The dependencies of the project
+        """
+        raw_response = r.get(
+            f"https://api.modrinth.com/v2/project/{self.model.slug}/dependencies",
+            timeout=60,
+        )
+
+        match raw_response.status_code:
+            case 404:
+                raise exceptions.NotFoundError(
+                    "The requested project wasn't found or no authorization to see this project"
+                )
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        response = raw_response.json()
+        return [Project(dependency) for dependency in response.get("projects")]
+
+    @staticmethod
+    def search(
+        query: str = "",
+        facets: list[list[str]] | None = None,
+        index: literals.index_literal = "relevance",
+        offset: int = 0,
+        limit: int = 10,
+        filters: list[str] | None = None,
+    ) -> list["Project.SearchResult"]:
+        """Searches for projects
+
+        Args:
+            query (str, optional): The query to search for
+            facets (list[list[str]], optional): The recommended way of filtering search results. [Learn more about using facets](https://docs.modrinth.com/docs/tutorials/api_search)
+            index (Literal["relevance", "downloads", "follows", "newest", "updated"], optional): The sorting method used for sorting search results
+            offset (int, optional): The offset into the search. Skip this number of results
+            limit (int, optional): The number of results returned by the search
+            filters (list[str], optional): A list of filters relating to the properties of a project. Use filters when there isn't an available facet for your needs. [More information](https://docs.meilisearch.com/reference/features/filtering.html)
+
+        Raises:
+            NotFoundError: The requested project wasn't found or no authorization to see this project
+            InvalidRequestError: Invalid request
+
+        Returns:
+            (list[Project.SearchResult]): The project search results
+        """
+        params = {}
+        if query != "":
+            params.update({"query": query})
+        if facets:
+            params.update({"facets": json.dumps(facets)})
+        if index != "relevance":
+            params.update({"index": index})
+        if offset != 0:
+            params.update({"offset": str(offset)})
+        if limit != 10:
+            params.update({"limit": str(limit)})
+        if filters:
+            params.update({"filters": json.dumps(filters)})
+        raw_response = r.get(
+            "https://api.modrinth.com/v2/search", params=params, timeout=60
+        )
+        response = raw_response.json()
+        return [
+            Project.SearchResult(models.SearchResultModel._from_json(project))
+            for project in response.get("hits")
+        ]
+
+    def get_team_members(self) -> "list[teams.Team.TeamMember]":
+        """Gets the team members of the project
+
+        Returns:
+            (list[Project.TeamMember)]: The team members of the project
+        """
+        raw_response = r.get(
+            f"https://api.modrinth.com/v2/project/{self.model.id}/members", timeout=60
+        )
+
+        match raw_response.status_code:
+            case 404:
+                raise exceptions.NotFoundError(
+                    "The requested project wasn't found or no authorization to see this project"
+                )
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        response = raw_response.json()
+
+        return [
+            teams.Team.TeamMember._from_json(team_member) for team_member in response
+        ]
+
+    def get_team(self) -> "teams.Team":
+        """Gets the project's team
+
+        Raises:
+            NotFoundError: The requested project wasn't found or no authorization to see this project
+            InvalidRequestError: Invalid request
+
+        Returns:
+            (Team): The project's team
+        """
+        raw_response = r.get(
+            f"https://api.modrinth.com/v2/project/{self.model.id}/members", timeout=60
+        )
+
+        match raw_response.status_code:
+            case 404:
+                raise exceptions.NotFoundError(
+                    "The requested project wasn't found or no authorization to see this project"
+                )
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        response = raw_response.json()
+
+        return teams.Team._from_json(response)
+
+    def __repr__(self) -> str:
+        """Returns a string representation of the Project instance
+
+        Returns:
+            (str): A string representation of the Project instance
+        """
+        return f"Project: {self.model.title}"
+
+    class Version:
+        """Versions contain download links to files with additional metadata
+
+        Attributes:
+            model (VersionModel): The version model associated with the version
+
+        """
+
+        def __init__(self, version_model: "models.VersionModel") -> None:
+            """
+            Args:
+                version_model (VersionModel): The version model to associate with the Version object
+            """
+            self.model = version_model
+
+        def get_type(self) -> str:
+            """Gets the type of the version
+
+            Returns:
+                (str): The type of the version
+            """
+            return self.model.version_type
+
+        def get_dependencies(self) -> list["Project.Dependency"]:
+            """Gets the dependencies of the version
+
+            Returns:
+                (list[Project.Dependency]): The dependencies of the version
+            """
+            result = []
+            for dependency in self.model.dependencies:
+                result.append(Project.Dependency._from_json(dependency))
+            return result
+
+        @staticmethod
+        def get(id_: str) -> "Project.Version":
+            """Gets a version by ID
+
+            Args:
+                id_ (str): The ID of the version
+
+            Raises:
+                NotFoundError: The requested version wasn't found or no authorization to see this version
+                InvalidRequestError: Invalid request
+
+            Returns:
+                (Project.Version): The version that was found
+            """
+            raw_response = r.get(
+                f"https://api.modrinth.com/v2/version/{id_}", timeout=60
+            )
+            match raw_response.status_code:
+                case 404:
+                    raise exceptions.NotFoundError(
+                        "The requested version wasn't found or no authorization to see this version"
+                    )
+            if not raw_response.ok:
+                raise exceptions.InvalidRequestError(raw_response.text)
+            response = raw_response.json()
+            return Project.Version(models.VersionModel._from_json(response))
+
+        @staticmethod
+        def get_from_hash(
+            hash_: str,
+            algorithm: literals.sha_algorithm_literal = "sha1",
+            multiple: bool = False,
+        ) -> typing.Union["Project.Version", list["Project.Version"]]:
+            """Gets a version by hash
+
+            Args:
+                hash_ (str): The hash of the file, considering its byte content, and encoded in hexadecimal
+                algorithm (Literal["sha512", "sha1"]): The algorithm of the hash
+                multiple (bool): Whether to return multiple results when looking for this hash
+
+            Raises:
+                NotFoundError: The requested version file wasn't found or no authorization to see this version
+                InvalidRequestError: Invalid request
+
+            Returns:
+                (Project.Version): The version that was found
+            """
+            raw_response = r.get(
+                f"https://api.modrinth.com/v2/version_file/{hash_}",
+                params={"algorithm": algorithm, "multiple": str(multiple).lower()},
+                timeout=60,
+            )
+            match raw_response.status_code:
+                case 404:
+                    raise exceptions.NotFoundError(
+                        "The requested version file wasn't found or no authorization to see this version"
+                    )
+            if not raw_response.ok:
+                raise exceptions.InvalidRequestError(raw_response.text)
+            response = raw_response.json()
+            if isinstance(response, list):
+                return [
+                    Project.Version(models.VersionModel._from_json(version))
+                    for version in response
+                ]
+            return Project.Version(models.VersionModel._from_json(response))
+
+        @staticmethod
+        def delete_file_from_hash(
+            auth: str,
+            hash_: str,
+            version_id: str,
+            algorithm: literals.sha_algorithm_literal = "sha1",
+        ) -> typing.Literal[True]:
+            """Deletes a file from its hash
+
+            Args:
+                hash_ (str): The hash of the file, considering its byte content, and encoded in hexadecimal
+                algorithm (Literal["sha512", "sha1"]): The algorithm of the hash
+                version_id (bool): Version ID to delete the version from, if multiple files of the same hash exist
+                auth (str): The authorization token to use when deleting the file from its hash
+
+            Raises:
+                NotFoundError: The requested version wasn't found
+                NoAuthorizationError: No authorization to delete this file
+                InvalidRequestError: Invalid request
+
+            Returns:
+                (bool): If the file deletion was successful
+            """
+            raw_response = r.delete(
+                f"https://api.modrinth.com/v2/version_file/{hash_}",
+                params={"algorithm": algorithm, "version_id": version_id},
+                headers={"authorization": auth},
+                timeout=60,
+            )
+            match raw_response.status_code:
+                case 404:
+                    raise exceptions.NotFoundError(
+                        "The requested version was not found"
+                    )
+                case 401:
+                    raise exceptions.NoAuthorizationError(
+                        "No authorization to delete this file"
+                    )
+            if not raw_response.ok:
+                raise exceptions.InvalidRequestError(raw_response.text)
+            return True
+
+        def get_files(self) -> list["Project.File"]:
+            """Gets the files associated with the version
+
+            Returns:
+                (list[Project.File]): The files associated with the version
+            """
+            result = []
+            for file in self.model.files:
+                result.append(Project.File._from_json(file))  # type: ignore
+            return result
+
+        def download(self, recursive: bool = False) -> None:
+            """Downloads the files associated with the version
+
+            Args:
+                recursive (bool, optional): Whether to also download the files of the dependencies
+            """
+            files = self.get_files()
+            for file in files:
+                file_content = r.get(file.url).content
+                open(file.name, "wb").write(file_content)
+
+            if recursive:
+                dependencies = self.get_dependencies()
+                for dep in dependencies:
+                    files = dep.get_version().get_files()
+                    for file in files:
+                        file_content = r.get(file.url).content
+                        open(file.name, "wb").write(file_content)
+
+        def get_project(self) -> "Project":
+            """Gets the project associated with the version
+
+            Returns:
+                (Project): The project associated with the version
+            """
+            return modrinth.Modrinth.get_project(self.model.project_id)  # type: ignore
+
+        def get_primary_files(self) -> list["Project.File"]:
+            """Gets the primary files associated with the version
+
+            Returns:
+                (list[Project.File]): The primary files associated with the version
+            """
+            result = []
+            for file in self.get_files():
+                if file.primary:
+                    result.append(file)
+            return result
+
+        def get_author(self) -> "users.User":
+            """Gets the author of the version
+
+            Returns:
+                (User): The author of the version
+            """
+            user = users.User.get(self.model.author_id)  # type: ignore
+            return user
+
+        def is_featured(self) -> bool:
+            """Checks if the version is featured
+
+            Returns:
+                (bool): Whether the version is featured
+            """
+            return self.model.featured
+
+        def get_date_published(self) -> "dt.datetime":
+            """Gets the date when the version was published
+
+            Returns:
+                (datetime): The date when the version was published
+            """
+            return util.format_time(self.model.date_published)
+
+        def get_downloads(self) -> int:
+            """Gets the number of downloads for the version
+
+            Returns:
+                (int): The number of downloads of the version
+            """
+            return self.model.downloads  # type: ignore
+
+        def get_name(self) -> str:
+            """Gets the name of the version
+
+            Returns:
+                (str): The name of the version
+            """
+            return self.model.name
+
+        def get_version_number(self) -> str:
+            """Gets the version number of the version
+
+            Returns:
+                (str): The version number of the version
+            """
+            return self.model.version_number
+
+        def __repr__(self) -> str:
+            return f"Version: {self.model.name}"
+
+    class GalleryImage:
+        """
+        Represents an image in a gallery
+
+        Attributes:
+            file_path (str): The path to the image
+            ext (str): Image extension
+            featured (str): Whether an image is featured
+            title (str): Title of the image
+            description (str): Description of the image
+            ordering (int): Ordering of the image
+
+        """
+
+        def __init__(
+            self,
+            file_path: str,
+            featured: bool,
+            title: str,
+            description: str,
+            ordering: int = 0,
+        ) -> None:
+            """
+            Initializes a GalleryImage object
+
+            Args:
+                file_path (str): The path to the image
+                featured (str): Whether an image is featured
+                title (str): Title of the image
+                description (str): Description of the image
+                ordering (int): Ordering of the image
+            """
+            self.file_path = file_path
+            self.ext = file_path.split(".")[-1]
+            self.featured = str(featured).lower()
+            self.title = title
+            self.description = description
+            self.ordering = ordering
+
+        @staticmethod
+        def _from_json(json_: dict) -> "Project.GalleryImage":
+            return Project.GalleryImage(
+                json_.get("url"),  # type: ignore
+                json_.get("featured"),  # type: ignore
+                json_.get("title"),  # type: ignore
+                json_.get("description"),  # type: ignore
+                json_.get("ordering"),  # type: ignore
+            )
+
+        def _to_json(self) -> dict:
+            return util.remove_null_values(self.__dict__)
+
+    class File:
+        """
+        Represents a file with various attributes and methods
+
+        Attributes:
+            hashes (dict[str, str]): A dictionary of hash algorithms and their corresponding hash values for the file
+            url (str): The URL where the file can be downloaded
+            name (str): The name of the file
+            primary (str): The primary hash algorithm used to verify the file's integrity
+            size (int): The size of the file in bytes
+            file_type (str): The type of the file
+            extension (str): The file extension
+
+        """
+
+        def __init__(
+            self,
+            hashes: dict[str, str],
+            url: str,
+            filename: str,
+            primary: str,
+            size: int,
+            file_type: str,
+        ) -> None:
+            """
+            Initializes a File object
+
+            Args:
+                hashes (dict[str, str]): A dictionary of hash algorithms and their corresponding hash values for the file
+                url (str): The URL where the file can be downloaded
+                filename (str): The name of the file
+                primary (str): The primary hash algorithm used to verify the file's integrity
+                size (int): The size of the file in bytes
+                file_type (str): The type of the file
+            """
+            self.hashes = hashes
+            self.url = url
+            self.name = filename
+            self.primary = primary
+            self.size = size
+            self.file_type = file_type
+            self.extension = filename.split(".")[-1]
+
+        def is_resourcepack(self) -> bool:
+            """
+            Checks if a file is a resourcepack
+
+            Returns:
+                (bool): If the file is a resourcepack
+            """
+            if self.file_type is None:
+                return False
+            return True
+
+        @staticmethod
+        def _from_json(json_: dict) -> "Project.File":
+            result = Project.File(
+                json_.get("hashes"),  # type: ignore
+                json_.get("url"),  # type: ignore
+                json_.get("filename"),  # type: ignore
+                json_.get("primary"),  # type: ignore
+                json_.get("size"),  # type: ignore
+                json_.get("file_type"),  # type: ignore
+            )
+            return result
+
+        def __repr__(self) -> str:
+            return f"File: {self.name}"
+
+    class License:
+        """
+        Represents a license
+
+        Attributes:
+            id (str): The SPDX license ID of a project
+            name (str): The long name of a license
+            url (str): The URL to this license
+
+        """
+
+        def __init__(self, id_: str, name: str, url: str | None = None) -> None:
+            """
+            Initializes a License object
+
+            Args:
+                id_ (str): The SPDX license ID of a project
+                name (str): The long name of a license
+                url (str): The URL to this license
+            """
+            self.id = id_
+            self.name = name
+            self.url = url
+
+        @staticmethod
+        def _from_json(json_: dict) -> "Project.License":
+            result = Project.License(
+                json_.get("id"),  # type: ignore
+                json_.get("name"),  # type: ignore
+                json_.get("url"),  # type: ignore
+            )
+
+            return result
+
+        def _to_json(self) -> dict:
+            return self.__dict__
+
+        def __repr__(self) -> str:
+            return f"License: {self.name if self.name else self.id}"
+
+    class Donation:
+        """
+        Represents a donation
+
+        Attributes:
+            id (str): The ID of the donation platform
+            platform (str): The donation platform this link is to
+            url (str): The URL of the donation platform and user
+
+        """
+
+        def __init__(self, id_: str, platform: str, url: str) -> None:
+            """
+            Initializes a Donation object
+
+            Args:
+                id_ (str): The ID of the donation
+                platform (str): The platform used for the donation
+                url (str): The URL to the donation page
+            """
+            self.id = id_
+            self.platform = platform
+            self.url = url
+
+        @staticmethod
+        def _from_json(json_: dict) -> "Project.Donation":
+            result = Project.Donation(
+                json_.get("id"),  # type: ignore
+                json_.get("platform"),  # type: ignore
+                json_.get("url"),  # type: ignore
+            )
+
+            return result
+
+        def __repr__(self) -> str:
+            return f"Donation: {self.platform}"
+
+    class Dependency:
+        """
+        Represents a dependency
+
+        Attributes:
+            dependency_type (str): The type of the dependency
+            id (str): The ID of the dependency
+            dependency_option (str): The option for the dependency
+        """
+
+        def __init__(self) -> None:
+            self.dependency_option: str | None = None
+            self.file_name: str | None = None
+            self.version_id: str | None = None
+            self.project_id: str | None = None
+
+        def _to_json(self) -> dict:
+            return self.__dict__
+
+        @staticmethod
+        def _from_json(json_: dict) -> "Project.Dependency":
+            result = Project.Dependency()
+            result.version_id = json_.get("version_id")
+            result.project_id = json_.get("project_id")
+            result.dependency_option = json_.get("dependency_option")
+            result.file_name = json_.get("file_name")
+            return result
+
+        def get_version(self) -> "Project.Version":
+            id_ = self.project_id
+            if self.version_id:
+                id_ = self.version_id
+            return Project.Version.get(id_)  # type: ignore
+
+        def is_required(self) -> bool:
+            """
+            Checks if the dependency is required
+
+            Returns:
+                (bool): True if the dependency is required, False otherwise
+            """
+            return True if self.dependency_option == "required" else False
+
+        def is_optional(self) -> bool:
+            """
+            Checks if the dependency is optional
+
+            Returns:
+                (bool): True if the dependency is optional, False otherwise
+            """
+            return True if self.dependency_option == "optional" else False
+
+        def is_incompatible(self) -> bool:
+            """
+            Checks if the dependency is incompatible
+
+            Returns:
+                (bool): True if the dependency is incompatible, False otherwise
+            """
+            return True if self.dependency_option == "incompatible" else False
+
+    class SearchResult:
+        """
+        Represents a search result
+
+        Attributes:
+            model (SearchResultModel): The search result model
+
+        """
+
+        def __init__(self, search_result_model: "models.SearchResultModel") -> None:
+            """
+            Initializes a SearchResult object
+
+            Args:
+                search_result_model (SearchResultModel): The search result model or a dictionary representing the search result model
+            """
+            self.model = search_result_model
+
+        def __repr__(self) -> str:
+            return f"Search Result: {self.model.title}"
```

### Comparing `python-modrinth-1.2.0/src/pyrinth/tags.py` & `python-modrinth-1.2.1/src/pyrinth/tags.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,286 +1,286 @@
-import requests as r
-
-import pyrinth.exceptions as exceptions
-
-
-class Tag:
-    @staticmethod
-    def get_categories() -> list["Tag.Category"]:
-        """
-        Gets a list of tag categories
-
-        Returns:
-            (list[Tag.Category]): A list of tag categories
-
-        Raises:
-            exceptions.InvalidRequestError: If the request to the API fails
-        """
-        raw_response = r.get("https://api.modrinth.com/v2/tag/category", timeout=60)
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        response = raw_response.json()
-        return [
-            Tag.Category(
-                json.get("icon"),
-                json.get("name"),
-                json.get("project_type"),
-                json.get("header"),
-            )
-            for json in response
-        ]
-
-    @staticmethod
-    def get_loaders() -> list["Tag.Loader"]:
-        """
-        Gets a list of tag loaders
-
-        Returns:
-            (list[Tag.Loader]): A list of tag loaders
-
-        Raises:
-            exceptions.InvalidRequestError: If the request to the API fails
-        """
-        raw_response = r.get("https://api.modrinth.com/v2/tag/loader", timeout=60)
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        response = raw_response.json()
-        return [
-            Tag.Loader(
-                json.get("icon"), json.get("name"), json.get("supported_project_types")
-            )
-            for json in response
-        ]
-
-    @staticmethod
-    def get_game_versions() -> list["Tag.GameVersion"]:
-        """
-        Gets a list of tag game versions
-
-        Returns:
-            (list[Tag.GameVersion]): A list of tag game versions
-
-        Raises:
-            (InvalidRequestError): If the request to the API fails
-        """
-        raw_response = r.get("https://api.modrinth.com/v2/tag/game_version", timeout=60)
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        response = raw_response.json()
-        return [
-            Tag.GameVersion(
-                json.get("version"),
-                json.get("version_type"),
-                json.get("date"),
-                json.get("major"),
-            )
-            for json in response
-        ]
-
-    @staticmethod
-    def get_licenses() -> list["Tag.License"]:
-        """
-        Gets a list of tag licenses
-
-        Returns:
-            (list[Tag.License]): A list of tag licenses
-
-        Raises:
-            exceptions.InvalidRequestError: If the request to the API fails
-        """
-        raw_response = r.get("https://api.modrinth.com/v2/tag/license", timeout=60)
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        response = raw_response.json()
-        return [Tag.License(json.get("short"), json.get("name")) for json in response]
-
-    @staticmethod
-    def get_donation_platforms() -> list["Tag.DonationPlatform"]:
-        """
-        Gets a list of tag donation platforms
-
-        Returns:
-            (list[Tag.DonationPlatform]): A list of tag donation platforms
-
-        Raises:
-            exceptions.InvalidRequestError: If the request to the API fails
-        """
-        raw_response = r.get(
-            "https://api.modrinth.com/v2/tag/donation_platform", timeout=60
-        )
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        response = raw_response.json()
-        return [
-            Tag.DonationPlatform(json.get("short"), json.get("name"))
-            for json in response
-        ]
-
-    @staticmethod
-    def get_report_types() -> list[str]:
-        """
-        Gets a list of tag report types
-
-        Returns:
-            (list[str]): A list of tag report types
-
-        Raises:
-            exceptions.InvalidRequestError: If the request to the API fails
-        """
-        raw_response = r.get("https://api.modrinth.com/v2/tag/report_type", timeout=60)
-
-        if not raw_response.ok:
-            raise exceptions.InvalidRequestError(raw_response.text)
-
-        response = raw_response.json()
-        return response
-
-    class Category:
-        """
-        Represents a tag category
-
-        Attributes:
-            icon (str): The icon for the category
-            name (str): The name of the category
-            project_type (str): The project type for the category
-            header (str): The header for the category
-
-        """
-
-        def __init__(
-            self, icon: str, name: str, project_type: str, header: str
-        ) -> None:
-            """
-            Initializes a Category object
-
-            Args:
-                icon (str): The icon for the category
-                name (str): The name of the category
-                project_type (str): The project type for the category
-                header (str): The header for the category
-            """
-            self.icon = icon
-            self.name = name
-            self.project_type = project_type
-            self.header = header
-
-        def __repr__(self) -> str:
-            return f"Category: {self.name}"
-
-    class Loader:
-        """
-        Represents a tag loader
-
-        Attributes:
-            icon (str): The icon for the loader
-            name (str): The name of the loader
-            supported_project_types (list[str]): A list of supported project types for the loader
-
-        """
-
-        def __init__(
-            self, icon: str, name: str, supported_project_types: list[str]
-        ) -> None:
-            """
-            Initializes a Loader object
-
-            Args:
-                icon (str): The icon for the loader
-                name (str): The name of the loader
-                supported_project_types (list[str]): A list of supported project types for the loader
-            """
-            self.icon = icon
-            self.name = name
-            self.supported_project_types = supported_project_types
-
-        def __repr__(self) -> str:
-            return f"Loader: {self.name}"
-
-    class GameVersion:
-        """
-        Represents a tag game version
-
-        Attributes:
-            version (str): The version of the game
-            version_type (str): The type of the version
-            date (str): The date of the version
-            major (bool): Whether the version is a major version or not
-
-        """
-
-        def __init__(
-            self, version: str, version_type: str, date: str, major: bool
-        ) -> None:
-            """
-            Initializes a GameVersion object
-
-            Args:
-                version (str): The version of the game
-                version_type (str): The type of the version
-                date (str): The date of the version
-                major (bool): Whether the version is a major version or not
-            """
-            self.version = version
-            self.version_type = version_type
-            self.date = date
-            self.major = major
-
-        def __repr__(self) -> str:
-            return f"Game Version: {self.version}"
-
-    class License:
-        """
-        Represents a tag license
-
-        Attributes:
-            short (str): The short name of the license
-            name (str): The name of the license
-
-        """
-
-        def __init__(self, short: str, name: str) -> None:
-            """
-            Initializes a License object
-
-            Args:
-                short (str): The short name of the license
-                name (str): The name of the license
-            """
-            self.short = short
-            self.name = name
-
-        def __repr__(self) -> str:
-            return f"License: {self.name}"
-
-    class DonationPlatform:
-        """
-        Represents a tag donation platform
-
-        Attributes:
-            short (str): The short name of the donation platform
-            name (str): The name of the donation platform
-
-        """
-
-        def __init__(self, short: str, name: str) -> None:
-            """
-            Initializes a DonationPlatform object
-
-            Args:
-                short (str): The short name of the donation platform
-                name (str): The name of the donation platform
-            """
-            self.short = short
-            self.name = name
-
-        def __repr__(self) -> str:
-            return f"Donation Platform: {self.name}"
+import requests as r
+
+import pyrinth.exceptions as exceptions
+
+
+class Tag:
+    @staticmethod
+    def get_categories() -> list["Tag.Category"]:
+        """
+        Gets a list of tag categories
+
+        Returns:
+            (list[Tag.Category]): A list of tag categories
+
+        Raises:
+            exceptions.InvalidRequestError: If the request to the API fails
+        """
+        raw_response = r.get("https://api.modrinth.com/v2/tag/category", timeout=60)
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        response = raw_response.json()
+        return [
+            Tag.Category(
+                json.get("icon"),
+                json.get("name"),
+                json.get("project_type"),
+                json.get("header"),
+            )
+            for json in response
+        ]
+
+    @staticmethod
+    def get_loaders() -> list["Tag.Loader"]:
+        """
+        Gets a list of tag loaders
+
+        Returns:
+            (list[Tag.Loader]): A list of tag loaders
+
+        Raises:
+            exceptions.InvalidRequestError: If the request to the API fails
+        """
+        raw_response = r.get("https://api.modrinth.com/v2/tag/loader", timeout=60)
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        response = raw_response.json()
+        return [
+            Tag.Loader(
+                json.get("icon"), json.get("name"), json.get("supported_project_types")
+            )
+            for json in response
+        ]
+
+    @staticmethod
+    def get_game_versions() -> list["Tag.GameVersion"]:
+        """
+        Gets a list of tag game versions
+
+        Returns:
+            (list[Tag.GameVersion]): A list of tag game versions
+
+        Raises:
+            (InvalidRequestError): If the request to the API fails
+        """
+        raw_response = r.get("https://api.modrinth.com/v2/tag/game_version", timeout=60)
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        response = raw_response.json()
+        return [
+            Tag.GameVersion(
+                json.get("version"),
+                json.get("version_type"),
+                json.get("date"),
+                json.get("major"),
+            )
+            for json in response
+        ]
+
+    @staticmethod
+    def get_licenses() -> list["Tag.License"]:
+        """
+        Gets a list of tag licenses
+
+        Returns:
+            (list[Tag.License]): A list of tag licenses
+
+        Raises:
+            exceptions.InvalidRequestError: If the request to the API fails
+        """
+        raw_response = r.get("https://api.modrinth.com/v2/tag/license", timeout=60)
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        response = raw_response.json()
+        return [Tag.License(json.get("short"), json.get("name")) for json in response]
+
+    @staticmethod
+    def get_donation_platforms() -> list["Tag.DonationPlatform"]:
+        """
+        Gets a list of tag donation platforms
+
+        Returns:
+            (list[Tag.DonationPlatform]): A list of tag donation platforms
+
+        Raises:
+            exceptions.InvalidRequestError: If the request to the API fails
+        """
+        raw_response = r.get(
+            "https://api.modrinth.com/v2/tag/donation_platform", timeout=60
+        )
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        response = raw_response.json()
+        return [
+            Tag.DonationPlatform(json.get("short"), json.get("name"))
+            for json in response
+        ]
+
+    @staticmethod
+    def get_report_types() -> list[str]:
+        """
+        Gets a list of tag report types
+
+        Returns:
+            (list[str]): A list of tag report types
+
+        Raises:
+            exceptions.InvalidRequestError: If the request to the API fails
+        """
+        raw_response = r.get("https://api.modrinth.com/v2/tag/report_type", timeout=60)
+
+        if not raw_response.ok:
+            raise exceptions.InvalidRequestError(raw_response.text)
+
+        response = raw_response.json()
+        return response
+
+    class Category:
+        """
+        Represents a tag category
+
+        Attributes:
+            icon (str): The icon for the category
+            name (str): The name of the category
+            project_type (str): The project type for the category
+            header (str): The header for the category
+
+        """
+
+        def __init__(
+            self, icon: str, name: str, project_type: str, header: str
+        ) -> None:
+            """
+            Initializes a Category object
+
+            Args:
+                icon (str): The icon for the category
+                name (str): The name of the category
+                project_type (str): The project type for the category
+                header (str): The header for the category
+            """
+            self.icon = icon
+            self.name = name
+            self.project_type = project_type
+            self.header = header
+
+        def __repr__(self) -> str:
+            return f"Category: {self.name}"
+
+    class Loader:
+        """
+        Represents a tag loader
+
+        Attributes:
+            icon (str): The icon for the loader
+            name (str): The name of the loader
+            supported_project_types (list[str]): A list of supported project types for the loader
+
+        """
+
+        def __init__(
+            self, icon: str, name: str, supported_project_types: list[str]
+        ) -> None:
+            """
+            Initializes a Loader object
+
+            Args:
+                icon (str): The icon for the loader
+                name (str): The name of the loader
+                supported_project_types (list[str]): A list of supported project types for the loader
+            """
+            self.icon = icon
+            self.name = name
+            self.supported_project_types = supported_project_types
+
+        def __repr__(self) -> str:
+            return f"Loader: {self.name}"
+
+    class GameVersion:
+        """
+        Represents a tag game version
+
+        Attributes:
+            version (str): The version of the game
+            version_type (str): The type of the version
+            date (str): The date of the version
+            major (bool): Whether the version is a major version or not
+
+        """
+
+        def __init__(
+            self, version: str, version_type: str, date: str, major: bool
+        ) -> None:
+            """
+            Initializes a GameVersion object
+
+            Args:
+                version (str): The version of the game
+                version_type (str): The type of the version
+                date (str): The date of the version
+                major (bool): Whether the version is a major version or not
+            """
+            self.version = version
+            self.version_type = version_type
+            self.date = date
+            self.major = major
+
+        def __repr__(self) -> str:
+            return f"Game Version: {self.version}"
+
+    class License:
+        """
+        Represents a tag license
+
+        Attributes:
+            short (str): The short name of the license
+            name (str): The name of the license
+
+        """
+
+        def __init__(self, short: str, name: str) -> None:
+            """
+            Initializes a License object
+
+            Args:
+                short (str): The short name of the license
+                name (str): The name of the license
+            """
+            self.short = short
+            self.name = name
+
+        def __repr__(self) -> str:
+            return f"License: {self.name}"
+
+    class DonationPlatform:
+        """
+        Represents a tag donation platform
+
+        Attributes:
+            short (str): The short name of the donation platform
+            name (str): The name of the donation platform
+
+        """
+
+        def __init__(self, short: str, name: str) -> None:
+            """
+            Initializes a DonationPlatform object
+
+            Args:
+                short (str): The short name of the donation platform
+                name (str): The name of the donation platform
+            """
+            self.short = short
+            self.name = name
+
+        def __repr__(self) -> str:
+            return f"Donation Platform: {self.name}"
```

### Comparing `python-modrinth-1.2.0/src/python_modrinth.egg-info/PKG-INFO` & `python-modrinth-1.2.1/src/python_modrinth.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-Metadata-Version: 2.1
-Name: python-modrinth
-Version: 1.2.0
-Summary: A Python library that interacts with the Modrinth API
-Home-page: https://github.com/RevolvingMadness/Pyrinth
-Author: RevolvingMadness
-Author-email: revolvingmad@gmail.com
-Project-URL: Bug Tracker, https://github.com/RevolvingMadness/Pyrinth/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<div align="center">
-
-<div id="user-content-toc">
-  <ul>
-    <img src="pyrinth.png" width="64" height="64"/>
-    <summary><h1>Pyrinth</h1></summary>
-  </ul>
-</div>
-
-  <p>
-    Interacts with the Modrinth API
-    <br />
-    <a href="https://github.com/RevolvingMadness/Pyrinth"><strong>Explore the docs »</strong></a>
-    <br />
-    <br />
-    <a href="https://github.com/RevolvingMadness/Pyrinth/issues">Report Bug</a>
-    ·
-    <a href="https://github.com/RevolvingMadness/Pyrinth/issues">Request Feature</a>
-  </p>
-
-[![Contributors][contributors-shield]][contributors-url]
-[![Forks][forks-shield]][forks-url]
-[![Stargazers][stars-shield]][stars-url]
-[![Issues][issues-shield]][issues-url]
-[![Apache License][license-shield]][license-url]
-</div>
-<br />
-
-
-## Getting Started
-
-### Prerequisites
-
-To use Pyrinth you need the following:
-- [Python](https://www.python.org/downloads)
-- pip (Comes with Python)
-
-### Installation
-
-#### Automatic Installation
-
-To automatically install the latest version of Pyrinth, run this command in the terminal:
-```sh
-pip install python-modrinth
-```
----
-
-#### Manual Installation
-If you want to get the latest beta or pre-releases, follow the steps below:
-1. Go to the [releases page](https://github.com/RevolvingMadness/Pyrinth/releases/) and download one of the `.whl` files.
-2. Open a terminal and go to the downloads directory.
-3. Type this: `pip install pyrinth`, then press tab and it should autocomplete.
-
-## Issues
-
-If you find a bug, please check if the issue already exists, otherwise open an issue through [this](https://github.com/RevolvingMadness/Pyrinth/issues) link.
-
-
-
-## Contributing
-
-### Creating A Fork And Pull Request
-Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
-
-If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".  
-Don't forget to give the project a star! Thanks again!
-
-1. Fork the Project
-2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
-3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
-4. Push to the Branch (`git push origin feature/AmazingFeature`)
-5. Open a Pull Request
-
-## Using Pyrinth Source Code
-When you're using the Pyrinth source code, navigate to the `src` directory and create your main Python file.
-
-
-
-
-
-## License
-
-This project is distributed under the MIT License. See `LICENSE` for more information.
-
-## Contact
-
-Project Link: https://github.com/RevolvingMadness/Pyrinth 
-Discord Server: Coming Soon!
-
-## To-Do
-- Projects
-  - [x] Search Projects
-  - [x] Get a project
-  - [x] Modify a project
-  - [x] Delete a project
-  - [x] Get multiple projects
-  - [x] Edit multiple projects
-  - [x] Get a list of random projects
-  - [x] Create a project
-  - [x] Change project's icon
-  - [x] Delete projcet's icon
-  - [x] Check project slug/ID validity
-  - [x] Add a gallery image
-  - [x] Modify a gallery image
-  - [x] Delete a gallery image
-  - [x] Get all of a project's dependencies
-  - [x] Follow a project
-  - [x] Unfollow a project
-  - [ ] Schedule a project
-- Versions
-  - [x] List project's versions
-  - [x] Get a version
-  - [x] Modify a version
-  - [x] Delete a version
-  - [x] Create a version
-  - [ ] Schedule a version
-  - [x] Get multipe versions
-  - [ ] Add files to version
-- Version Files
-  - [x] Get version from hash
-  - [x] Delete a file from its hash
-  - [ ] Latest version of a project from a has, loader(s), and game version(s)
-  - [ ] Get versions from hashes
-  - [ ] Latest versions multiple project from hashes, loader(s), and game version(s)
-- Users - Complete
-  - [x] Get a user
-  - [x] Modify a user
-  - [x] Delete a user
-  - [x] Get user from authorization header
-  - [x] Get multiple users
-  - [x] Change user's avatar
-  - [x] Get user's projects
-  - [x] Get user's notifications
-  - [x] Get user's followed projects
-  - [x] Get user's payout history
-  - [x] Withdraw payout balance to PayPal or Venmo
-- Teams
-  - [x] Get a project's team members
-  - [x] Get a team's members
-  - [ ] Add a user to a team
-  - [x] Get the members of multiple teams
-  - [ ] Join a team
-  - [ ] Modify a team member's information
-  - [ ] Remove a team member from a team
-  - [ ] Transfer team's ownership to another user
-- Tags - Complete
-  - [x] Get a list of categories
-  - [x] Get a list of loaders
-  - [x] Get a list of game versions
-  - [x] Get a list of licenses
-  - [x] Get a list of donation platforms
-  - [x] Get a list of report types
-- Miscellaneous
-  - [ ] Report a project, user, or version
-  - [x] Various statistics about this Modrinth instance
-
-## Documentation
-You can find the documentation [here](https://revolvingmadness.github.io/Pyrinth)
-
-
-[contributors-shield]: https://img.shields.io/github/contributors/RevolvingMadness/Pyrinth.svg?style=for-the-badge
-[contributors-url]: https://github.com/RevolvingMadness/Pyrinth/graphs/contributors
-[forks-shield]: https://img.shields.io/github/forks/RevolvingMadness/Pyrinth.svg?style=for-the-badge
-[forks-url]: https://github.com/RevolvingMadness/Pyrinth/network/members
-[stars-shield]: https://img.shields.io/github/stars/RevolvingMadness/Pyrinth.svg?style=for-the-badge
-[stars-url]: https://github.com/RevolvingMadness/Pyrinth/stargazers
-[issues-shield]: https://img.shields.io/github/issues/RevolvingMadness/Pyrinth.svg?style=for-the-badge
-[issues-url]: https://github.com/RevolvingMadness/Pyrinth/issues
-[license-shield]: https://img.shields.io/github/license/RevolvingMadness/Pyrinth.svg?style=for-the-badge
-[license-url]: https://github.com/RevolvingMadness/Pyrinth/LICENSE.txt
+Metadata-Version: 2.1
+Name: python-modrinth
+Version: 1.2.1
+Summary: A Python library that interacts with the Modrinth API
+Home-page: https://github.com/RevolvingMadness/Pyrinth
+Author: RevolvingMadness
+Author-email: revolvingmad@gmail.com
+Project-URL: Bug Tracker, https://github.com/RevolvingMadness/Pyrinth/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+
+<div id="user-content-toc">
+  <ul>
+    <img src="pyrinth.png" width="64" height="64"/>
+    <summary><h1>Pyrinth</h1></summary>
+  </ul>
+</div>
+
+  <p>
+    Interacts with the Modrinth API
+    <br />
+    <a href="https://github.com/RevolvingMadness/Pyrinth"><strong>Explore the docs »</strong></a>
+    <br />
+    <br />
+    <a href="https://github.com/RevolvingMadness/Pyrinth/issues">Report Bug</a>
+    ·
+    <a href="https://github.com/RevolvingMadness/Pyrinth/issues">Request Feature</a>
+  </p>
+
+[![Contributors][contributors-shield]][contributors-url]
+[![Forks][forks-shield]][forks-url]
+[![Stargazers][stars-shield]][stars-url]
+[![Issues][issues-shield]][issues-url]
+[![Apache License][license-shield]][license-url]
+</div>
+<br />
+
+
+## Getting Started
+
+### Prerequisites
+
+To use Pyrinth you need the following:
+- [Python](https://www.python.org/downloads)
+- pip (Comes with Python)
+
+### Installation
+
+#### Automatic Installation
+
+To automatically install the latest version of Pyrinth, run this command in the terminal:
+```sh
+pip install python-modrinth
+```
+---
+
+#### Manual Installation
+If you want to get the latest beta or pre-releases, follow the steps below:
+1. Go to the [releases page](https://github.com/RevolvingMadness/Pyrinth/releases/) and download one of the `.whl` files.
+2. Open a terminal and go to the downloads directory.
+3. Type this: `pip install pyrinth`, then press tab and it should autocomplete.
+
+## Issues
+
+If you find a bug, please check if the issue already exists, otherwise open an issue through [this](https://github.com/RevolvingMadness/Pyrinth/issues) link.
+
+
+
+## Contributing
+
+### Creating A Fork And Pull Request
+Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.
+
+If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".  
+Don't forget to give the project a star! Thanks again!
+
+1. Fork the Project
+2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
+3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
+4. Push to the Branch (`git push origin feature/AmazingFeature`)
+5. Open a Pull Request
+
+## Using Pyrinth Source Code
+When you're using the Pyrinth source code, navigate to the `src` directory and create your main Python file.
+
+
+
+
+
+## License
+
+This project is distributed under the MIT License. See `LICENSE` for more information.
+
+## Contact
+
+Project Link: https://github.com/RevolvingMadness/Pyrinth 
+Discord Server: Coming Soon!
+
+## To-Do
+- Projects
+  - [x] Search Projects
+  - [x] Get a project
+  - [x] Modify a project
+  - [x] Delete a project
+  - [x] Get multiple projects
+  - [x] Edit multiple projects
+  - [x] Get a list of random projects
+  - [x] Create a project
+  - [x] Change project's icon
+  - [x] Delete projcet's icon
+  - [x] Check project slug/ID validity
+  - [x] Add a gallery image
+  - [x] Modify a gallery image
+  - [x] Delete a gallery image
+  - [x] Get all of a project's dependencies
+  - [x] Follow a project
+  - [x] Unfollow a project
+  - [ ] Schedule a project
+- Versions
+  - [x] List project's versions
+  - [x] Get a version
+  - [x] Modify a version
+  - [x] Delete a version
+  - [x] Create a version
+  - [ ] Schedule a version
+  - [x] Get multipe versions
+  - [ ] Add files to version
+- Version Files
+  - [x] Get version from hash
+  - [x] Delete a file from its hash
+  - [ ] Latest version of a project from a has, loader(s), and game version(s)
+  - [ ] Get versions from hashes
+  - [ ] Latest versions multiple project from hashes, loader(s), and game version(s)
+- Users - Complete
+  - [x] Get a user
+  - [x] Modify a user
+  - [x] Delete a user
+  - [x] Get user from authorization header
+  - [x] Get multiple users
+  - [x] Change user's avatar
+  - [x] Get user's projects
+  - [x] Get user's notifications
+  - [x] Get user's followed projects
+  - [x] Get user's payout history
+  - [x] Withdraw payout balance to PayPal or Venmo
+- Teams
+  - [x] Get a project's team members
+  - [x] Get a team's members
+  - [ ] Add a user to a team
+  - [x] Get the members of multiple teams
+  - [ ] Join a team
+  - [ ] Modify a team member's information
+  - [ ] Remove a team member from a team
+  - [ ] Transfer team's ownership to another user
+- Tags - Complete
+  - [x] Get a list of categories
+  - [x] Get a list of loaders
+  - [x] Get a list of game versions
+  - [x] Get a list of licenses
+  - [x] Get a list of donation platforms
+  - [x] Get a list of report types
+- Miscellaneous
+  - [ ] Report a project, user, or version
+  - [x] Various statistics about this Modrinth instance
+
+## Documentation
+You can find the documentation [here](https://revolvingmadness.github.io/Pyrinth)
+
+
+[contributors-shield]: https://img.shields.io/github/contributors/RevolvingMadness/Pyrinth.svg?style=for-the-badge
+[contributors-url]: https://github.com/RevolvingMadness/Pyrinth/graphs/contributors
+[forks-shield]: https://img.shields.io/github/forks/RevolvingMadness/Pyrinth.svg?style=for-the-badge
+[forks-url]: https://github.com/RevolvingMadness/Pyrinth/network/members
+[stars-shield]: https://img.shields.io/github/stars/RevolvingMadness/Pyrinth.svg?style=for-the-badge
+[stars-url]: https://github.com/RevolvingMadness/Pyrinth/stargazers
+[issues-shield]: https://img.shields.io/github/issues/RevolvingMadness/Pyrinth.svg?style=for-the-badge
+[issues-url]: https://github.com/RevolvingMadness/Pyrinth/issues
+[license-shield]: https://img.shields.io/github/license/RevolvingMadness/Pyrinth.svg?style=for-the-badge
+[license-url]: https://github.com/RevolvingMadness/Pyrinth/LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-modrinth Version: 1.2.0 Summary: A Python
+Metadata-Version: 2.1 Name: python-modrinth Version: 1.2.1 Summary: A Python
 library that interacts with the Modrinth API Home-page: https://github.com/
 RevolvingMadness/Pyrinth Author: RevolvingMadness Author-email:
 revolvingmad@gmail.com Project-URL: Bug Tracker, https://github.com/
 RevolvingMadness/Pyrinth/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.11 Description-Content-Type: text/
 markdown License-File: LICENSE
```

