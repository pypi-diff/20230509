# Comparing `tmp/nsdotpy-1.2.2.tar.gz` & `tmp/nsdotpy-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdotpy-1.2.2.tar", max compression
+gzip compressed data, was "nsdotpy-1.2.3.tar", max compression
```

## Comparing `nsdotpy-1.2.2.tar` & `nsdotpy-1.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34354 2023-05-08 23:33:15.715624 nsdotpy-1.2.2/LICENSE.md
--rw-r--r--   0        0        0     2406 2023-05-08 23:33:15.715624 nsdotpy-1.2.2/README.md
--rw-r--r--   0        0        0      790 2023-05-08 23:33:15.723624 nsdotpy-1.2.2/nsdotpy/__init__.py
--rw-r--r--   0        0        0    36877 2023-05-08 23:33:44.295974 nsdotpy-1.2.2/nsdotpy/session.py
--rw-r--r--   0        0        0     2302 2023-05-08 23:33:15.723624 nsdotpy-1.2.2/nsdotpy/valid_tags.py
--rw-r--r--   0        0        0      703 2023-05-08 23:33:15.723624 nsdotpy-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3283 1970-01-01 00:00:00.000000 nsdotpy-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    34354 2023-05-09 19:49:15.673584 nsdotpy-1.2.3/LICENSE.md
+-rw-r--r--   0        0        0     2436 2023-05-09 19:49:15.673584 nsdotpy-1.2.3/README.md
+-rw-r--r--   0        0        0      790 2023-05-09 19:49:15.681584 nsdotpy-1.2.3/nsdotpy/__init__.py
+-rw-r--r--   0        0        0    40012 2023-05-09 19:49:15.685584 nsdotpy-1.2.3/nsdotpy/session.py
+-rw-r--r--   0        0        0     2302 2023-05-09 19:49:15.685584 nsdotpy-1.2.3/nsdotpy/valid_tags.py
+-rw-r--r--   0        0        0      703 2023-05-09 19:49:15.685584 nsdotpy-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3313 1970-01-01 00:00:00.000000 nsdotpy-1.2.3/PKG-INFO
```

### Comparing `nsdotpy-1.2.2/LICENSE.md` & `nsdotpy-1.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.2/README.md` & `nsdotpy-1.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,29 @@
 ## Installation
 
 `pip install nsdotpy`
 
 ## Simple Example
 
 ```python
-from nsdotpy.session import NSClient
-session = NSClient("NSDotPy Example," "1.0.0", "Script Author's nation", "Script User's nation")
+
+from nsdotpy.session import NSSession
+session = NSSession("NSDotPy Example," "1.0.0", "Script Author's nation", "Script User's nation")
+
 if session.login("User Nation", "Password"):  # logs in and checks if login was successful
     session.move_to_region("Lily")  # only moves if you successfully logged in
 ```
 
 ## TODO:
 
 - ~~Region Admin Controls~~
 - Dossier and reports handling
 - More fleshed out API Client
-- Cards support
-- Migrate automatic docs generation, code formatting, and PyPI uploading to GitHub Actions for better CI
+- ~~Cards support~~ Shoutouts to 9003
+- ~~Migrate automatic docs generation, code formatting, and PyPI uploading to GitHub Actions for better CI~~
 
 ## Docs
 
 https://sw33ze.github.io/NSDotPy/nsdotpy/session.html#NSSession
 
 ## Generating Docs
```

### Comparing `nsdotpy-1.2.2/nsdotpy/__init__.py` & `nsdotpy-1.2.3/nsdotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.2/nsdotpy/session.py` & `nsdotpy-1.2.3/nsdotpy/session.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             script_version (str): Version number of your script
             script_author (str): Author of your script
             script_user (str): Nation name of the user running your script
             keybind (str, optional): Keybind to count as a user click. Defaults to "space".
             link_to_src (str, optional): Link to the source code of your script.
             logger (logging.Logger | None, optional): Logger to use. Will create its own with name "NSDotPy" if none is specified. Defaults to None.
         """
-        self.VERSION = "1.2.2"
+        self.VERSION = "1.2.3"
         # Initialize logger
         if not logger:
             self._init_logger()
         else:
             self.logger = logger
         # Attach the tendo singleton to the session object so it can
         # only be run once at a time, avoiding simultaneity issues
@@ -881,15 +881,15 @@
             card_id (str): ID of the card
             season (str): Season of the card
 
         Returns:
             bool: Whether the ask was successfully lodged or not
         """
         self.logger.info(f"Asking for {price} on {card_id} season {season}")
-        url = f"https://www.nationstates.net/page=deck/card={card_id}/season={season}"
+        url = f"https://www.nationstates.net/template-overall=none/page=deck/card={card_id}/season={season}"
 
         data = {"auction_ask": price, "auction_submit": "ask"}
         response = self.request(url, data)
         return f"Your ask of {price} has been lodged." in response.text
 
     def bid(self, price: str, card_id: str, season: str) -> bool:
         """Places a bid on a card in a season
@@ -899,15 +899,15 @@
             card_id (str): ID of the card
             season (str): Season of the card
 
         Returns:
             bool: Whether the bid was successfully lodged or not
         """
         self.logger.info(f"Putting a bid for {price} on {card_id} season {season}")
-        url = f"https://www.nationstates.net/page=deck/card={card_id}/season={season}"
+        url = f"https://www.nationstates.net/template-overall=none/page=deck/card={card_id}/season={season}"
 
         data = {"auction_bid": price, "auction_submit": "bid"}
         response = self.request(url, data)
 
         return f"Your bid of {price} has been lodged." in response.text
 
     def remove_ask(self, price: str, card_id: str, season: str) -> bool:
@@ -919,32 +919,32 @@
             season (str): Season of the card
 
         Returns:
             bool: Whether the ask was successfully removed or not
         """
 
         self.logger.info(f"removing an ask for {price} on {card_id} season {season}")
-        url = f"https://www.nationstates.net/page=deck/card={card_id}/season={season}"
+        url = f"https://www.nationstates.net/template-overall=none/page=deck/card={card_id}/season={season}"
 
         data = {"new_price": price, "remove_ask_price": price}
         response = self.request(url, data)
         return f"Removed your ask for {price}" in response.text
 
     def remove_bid(self, price: str, card_id: str, season: str) -> bool:
-        """Removes a big on a card
+        """Removes a bid on a card
         Args:
             price (str): Price of the bid to remove
             card_id (str): ID of the card
             season (str): Season of the card
         Returns:
             bool: Whether the bid was successfully removed or not
         """
 
         self.logger.info(f"Removing a bid for {price} on {card_id} season {season}")
-        url = f"https://www.nationstates.net/page=deck/card={card_id}/season={season}"
+        url = f"https://www.nationstates.net/template-overall=none/page=deck/card={card_id}/season={season}"
 
         data = {"new_price": price, "remove_bid_price": price}
         response = self.request(url, data)
 
         return f"Removed your bid for {price}" in response.text
 
     def expand_deck(self, price: str) -> bool:
@@ -952,17 +952,96 @@
         Args:
             price (str): Price of the Upgrade
         Returns:
             bool: Whether the upgrade was successfully removed or not
         """
 
         self.logger.info(f"Upgrading your deck at a cost of {price}")
-        url = "https://www.nationstates.net/page=deck"
+        url = "https://www.nationstates.net/template-overall=none/page=deck"
 
         data = {"embiggen_deck": price}
         response = self.request(url, data)
 
-        return f"Increased deck capacity from" in response.text
+        return "Increased deck capacity from" in response.text
+
+    def add_to_collection(self, card_id: str, card_season: str, collection_id: str):
+        """Adds a card to collection_id
+        Args:
+            card_id (str): Card ID
+            card_season (str): Cards season
+            collection_id (str): The ID of the collection you want to add to
+        Returns:
+            bool: Whether the adding was successfully added or not
+        """
+        self.logger.info(f"Adding {card_id} of season {card_season} to {collection_id}")
+        url = f"https://www.nationstates.net/template-overall=none/page=deck/card={card_id}/season={card_season}"
+
+        data = {
+            "manage_collections": "1",
+            "modify_card_in_collection": "1",
+            f"collection_{collection_id}": "1",
+            "save_collection": "1",
+        }
+        response = self.request(url, data)
+
+        return "Updated collections." in response.text
+
+    def remove_from_collection(
+        self, card_id: str, card_season: str, collection_id: str
+    ):
+        """Removes a card from collection_id
+        Args:
+            card_id (str): Card ID
+            card_season (str): Cards season
+            collection_id (str): The ID of the collection you want to remove from
+        Returns:
+            bool: Whether the removal was successfully added or not
+        """
+        self.logger.info(
+            f"Removing {card_id} of season {card_season} from {collection_id}"
+        )
+        url = f"https://www.nationstates.net/template-overall=none/page=deck/card={card_id}/season={card_season}"
+
+        data = {
+            "manage_collections": "1",
+            "modify_card_in_collection": "1",
+            "start": "0",
+            f"collection_{collection_id}": "0",
+            "save_collection": "1",
+        }
+        response = self.request(url, data)
+
+        return "Updated collections." in response.text
+
+    def create_collection(self, name: str):
+        """Creates a collection named name
+        Args:
+            name (str): The name of the collection you want to create
+        Returns:
+            bool: Whether the creating was successfully added or not
+        """
+        self.logger.info(f"Creating {name} collection")
+        url = "https://www.nationstates.net/template-overall=none/page=deck"
+
+        data = {"edit": "1", "collection_name": name, "save_collection": "1"}
+        response = self.request(url, data)
+
+        return "Created collection!" in response.text
+
+    def delete_collection(self, name: str):
+        """Deletes a collection named name
+        Args:
+            name (str): The name of the collection you want to delete
+        Returns:
+            bool: Whether the deleting was successfully added or not
+        """
+        self.logger.info(f"Deleting {name} collection")
+        url = "https://www.nationstates.net/template-overall=none/page=deck"
+
+        data = {"edit": "1", "collection_name": name, "delete_collection": "1"}
+        response = self.request(url, data)
+
+        return "Created collection!" in response.text
 
 
 if __name__ == "__main__":
     print("this is a module/library, not a script")
```

### Comparing `nsdotpy-1.2.2/nsdotpy/valid_tags.py` & `nsdotpy-1.2.3/nsdotpy/valid_tags.py`

 * *Files identical despite different names*

### Comparing `nsdotpy-1.2.2/pyproject.toml` & `nsdotpy-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdotpy"
-version = "1.2.2"
+version = "1.2.3"
 description = "A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use."
 authors = ["audrey <audreyreal@proton.me>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/sw33ze/NSDotPy"
 
 [tool.poetry.dependencies]
```

### Comparing `nsdotpy-1.2.2/PKG-INFO` & `nsdotpy-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdotpy
-Version: 1.2.2
+Version: 1.2.3
 Summary: A wrapper around httpx that abstracts away interacting with the HTML nationstates.net site. Focused on legality, correctness, and ease of use.
 Home-page: https://github.com/sw33ze/NSDotPy
 License: AGPL-3.0-or-later
 Author: audrey
 Author-email: audreyreal@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -25,27 +25,29 @@
 ## Installation
 
 `pip install nsdotpy`
 
 ## Simple Example
 
 ```python
-from nsdotpy.session import NSClient
-session = NSClient("NSDotPy Example," "1.0.0", "Script Author's nation", "Script User's nation")
+
+from nsdotpy.session import NSSession
+session = NSSession("NSDotPy Example," "1.0.0", "Script Author's nation", "Script User's nation")
+
 if session.login("User Nation", "Password"):  # logs in and checks if login was successful
     session.move_to_region("Lily")  # only moves if you successfully logged in
 ```
 
 ## TODO:
 
 - ~~Region Admin Controls~~
 - Dossier and reports handling
 - More fleshed out API Client
-- Cards support
-- Migrate automatic docs generation, code formatting, and PyPI uploading to GitHub Actions for better CI
+- ~~Cards support~~ Shoutouts to 9003
+- ~~Migrate automatic docs generation, code formatting, and PyPI uploading to GitHub Actions for better CI~~
 
 ## Docs
 
 https://sw33ze.github.io/NSDotPy/nsdotpy/session.html#NSSession
 
 ## Generating Docs
```

