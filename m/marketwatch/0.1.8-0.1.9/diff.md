# Comparing `tmp/marketwatch-0.1.8.tar.gz` & `tmp/marketwatch-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marketwatch-0.1.8.tar", max compression
+gzip compressed data, was "marketwatch-0.1.9.tar", max compression
```

## Comparing `marketwatch-0.1.8.tar` & `marketwatch-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11358 2023-03-29 01:59:06.943941 marketwatch-0.1.8/LICENSE
--rw-r--r--   0        0        0     2957 2023-03-29 01:59:06.943941 marketwatch-0.1.8/README.md
--rw-r--r--   0        0        0    43488 2023-03-29 01:59:06.947941 marketwatch-0.1.8/marketwatch/__init__.py
--rw-r--r--   0        0        0      266 2023-03-29 01:59:06.947941 marketwatch-0.1.8/marketwatch/exceptions.py
--rw-r--r--   0        0        0     1170 2023-03-29 01:59:06.947941 marketwatch-0.1.8/marketwatch/game.py
--rw-r--r--   0        0        0     5242 2023-03-29 01:59:06.947941 marketwatch-0.1.8/marketwatch/schemas.py
--rw-r--r--   0        0        0      722 2023-03-29 01:59:06.947941 marketwatch-0.1.8/marketwatch/watchlist.py
--rw-r--r--   0        0        0     1181 2023-03-29 01:59:06.947941 marketwatch-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4178 1970-01-01 00:00:00.000000 marketwatch-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-04-03 17:17:47.713564 marketwatch-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2957 2023-04-03 17:17:47.713564 marketwatch-0.1.9/README.md
+-rw-r--r--   0        0        0    46034 2023-04-03 17:17:47.713564 marketwatch-0.1.9/marketwatch/__init__.py
+-rw-r--r--   0        0        0      643 2023-04-03 17:17:47.713564 marketwatch-0.1.9/marketwatch/exceptions.py
+-rw-r--r--   0        0        0     2798 2023-04-03 17:17:47.713564 marketwatch-0.1.9/marketwatch/game.py
+-rw-r--r--   0        0        0     5328 2023-04-03 17:17:47.713564 marketwatch-0.1.9/marketwatch/schemas.py
+-rw-r--r--   0        0        0     2147 2023-04-03 17:17:47.713564 marketwatch-0.1.9/marketwatch/watchlist.py
+-rw-r--r--   0        0        0     1181 2023-04-03 17:17:47.717564 marketwatch-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4178 1970-01-01 00:00:00.000000 marketwatch-0.1.9/PKG-INFO
```

### Comparing `marketwatch-0.1.8/LICENSE` & `marketwatch-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `marketwatch-0.1.8/README.md` & `marketwatch-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `marketwatch-0.1.8/marketwatch/__init__.py` & `marketwatch-0.1.9/marketwatch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     """
     MarketWatch API
 
     :param email: Email
     :param password: Password
     """
 
-    def __init__(self, email, password):
+    def __init__(self, email: str, password: str):
         """
         Initialize the MarketWatch API
 
         :param email: Email
         :param password: Password
 
         :return: None
@@ -54,24 +54,24 @@
         self.client_id = self.get_client_id()
         self.login()
 
         self.user_id = self.get_user_id()
         self.ledger_id = None
         self.games = None
 
-    def generate_csrf_token(self):
+    def generate_csrf_token(self) -> str:
         """
         Get the csrf token from the login page
 
         :return: CSRF Token
         """
         client = self.session.get("https://sso.accounts.dowjones.com/login-page")
         return client.cookies["csrf"]
 
-    def get_client_id(self):
+    def get_client_id(self) -> str:
         """
         Generate a client id
 
         :return: Client ID
         """
         return "5hssEAdMy0mJTICnJNvC9TXEw3Va7jfO"
 
@@ -83,15 +83,15 @@
                 "csrf": self.generate_csrf_token(),
             },
         )
 
         if user.status_code == 200:
             return user.json()["id"]
 
-    def get_ledger_id(self, game_id):
+    def get_ledger_id(self, game_id) -> str:
         """
         Get the ledger id
 
         :param game_id: Game ID
         """
         game_page = self.session.get(f"https://www.marketwatch.com/games/{game_id}")
 
@@ -257,22 +257,92 @@
                     "rank": game_rank,
                     "end": game_end,
                     "players": game_players,
                 }
             )
         return games_data
 
+    def create_game(self, name: str, start_date: int, end_date: int, **kwargs) -> dict:
+        """
+        Create a game on MarketWatch.
+
+        Args:
+            name (str): Name of the game to create.
+            start_date (int): Start date of the game in epoch time.
+            end_date (int): End date of the game in epoch time.
+            **kwargs: Additional optional parameters to configure the game.
+
+        Returns:
+            dict: A dictionary containing information about the created game.
+
+        Raises:
+            MarketWatchException: If game creation fails.
+        """
+        url = 'https://vse-api.marketwatch.com/v1/games'
+        headers = {'Content-Type': 'application/json'}
+
+        # Construct payload with default and optional parameters
+        payload = {
+            "name": name,
+            "uri": kwargs.get('uri', name),
+            "startDateUtc": start_date,
+            "endDateUtc": end_date,
+            "allowJoinAfterStart": kwargs.get('allowJoinAfterStart', True),
+            "privacyPortfolios": kwargs.get('privacyPortfolios', 'public'),
+            "privacyGame": kwargs.get('privacyGame', 'public'),
+            "allowComment": kwargs.get('allowComment', True),
+            "description": kwargs.get('description', ''),
+            "startingAmount": kwargs.get('startingAmount', 100000),
+            "commissionPerTrade": kwargs.get('commissionPerTrade', 10),
+            "creditInterestRate": kwargs.get('creditInterestRate', 0),
+            "debitInterestRate": kwargs.get('debitInterestRate', 0),
+            "minimumTradePrice": kwargs.get('minimumTradePrice', 2),
+            "maximumTradePrice": kwargs.get('maximumTradePrice', 500000),
+            "allowShortSelling": kwargs.get('allowShortSelling', True),
+            "marginEnabled": kwargs.get('marginEnabled', True),
+            "allowLimitOrders": kwargs.get('allowLimitOrders', False),
+            "allowStopOrders": kwargs.get('allowStopOrders', False),
+            "allowPartialShares": kwargs.get('allowPartialShares', False),
+        }
+
+        # Make request to create game
+        response = self.session.post(
+            url,
+            headers=headers,
+            json=payload,
+        )
+
+        # Raise exception if game creation fails
+        if response.status_code != 200:
+            raise MarketWatchException('Failed to create game')
+
+        # Return information about created game
+        return self.get_game(name)
+
+
     @auth
     def get_game(self, game_id: str) -> list:
         """
         Get a game
-        {'name': 'algoets-h2023', 'title': 'ALGOETS-H2023', 'time': 'Game ends in 4 days', 'url': 'https://www.marketwatch.com/games/algoets-h2023', 'start_date': 'Mar 20, 2023', 'end_date': 'Mar 31, 2023', 'players': '27', 'creator': 'Mohamed Ilias',
-                        'rank': '15', 'portfolio_value': '$996,289.15', 'gain_percentage': '0.00%', 'gain': '-$3,710.85', 'return': '-0.37%', 'cash_remaining': '$249,845.55', 'buying_power': '$143,734.12', 'shorts_reserve': '$0.00', 'cash_borrowed': '$0.00'}
+        {
+        'name': 'algoets-h2023',
+        'title': 'ALGOETS-H2023',
+        'time': 'Game ends in 4 days',
+        'url': 'https://www.marketwatch.com/games/algoets-h2023',
+        'start_date': 'Mar 20, 2023', 'end_date': 'Mar 31, 2023',
+        'players': '27', 'creator': 'Mohamed Ilias',
+        'rank': '15', 'portfolio_value': '$996,289.15',
+        'gain_percentage': '0.00%', 'gain': '-$3,710.85',
+        'return': '-0.37%', 'cash_remaining': '$249,845.55',
+        'buying_power': '$143,734.12',
+        'shorts_reserve': '$0.00',
+        'cash_borrowed': '$0.00'
+        }
 
-                        :param game_id: Game id
+        :param game_id: Game id
         :return: Game data
         """
         game_page = self.session.get(f"https://www.marketwatch.com/games/{game_id}")
 
         if game_page.status_code != 200:
             raise MarketWatchException("Game not found")
         soup = BeautifulSoup(game_page.text, "html.parser")
@@ -505,20 +575,18 @@
             response = self.session.get(next_page_url)
 
         if response.status_code != 200:
             raise MarketWatchException("Game not found")
 
         soup = BeautifulSoup(response.text, "html.parser")
 
-        # ledger_id = self.get_ledger_id(game_id=game_id)
-        ledger_id = soup.find(
-            "div", {"class": "element element--table portfolio-performance"}
-        )["pub"]
+        ledger_id = self.get_ledger_id(game_id=game_id)
         table = (
-            soup.find("div", {"class": "element element--table portfolio-performance"})
+            soup.find("div", {"class": "portfolio-performance"})
+            .find("table", {"class": "table--primary"})
             .find("tbody")
             .find_all("tr")
         )
 
         if download:
             print("Downloaded")
             return self.session.get(
@@ -1040,14 +1108,15 @@
         response = self.session.get(url)
         soup = BeautifulSoup(response.text, "html.parser")
         option_tables = soup.find_all("table", {"class": "portfolio-options"})
 
         def clean_text(text):
             return text.replace("$", "").replace(",", "").replace("%", "")
 
+        # Extract the game settings from the option tables
         settings = {
             "game_public": option_tables[0]
             .find_all("td", {"class": "table__cell"})[1]
             .text.strip()
             == "Public",
             "portfolios_public": option_tables[1]
             .find_all("td", {"class": "table__cell"})[1]
@@ -1105,14 +1174,16 @@
             .find_all("td", {"class": "table__cell"})[9]
             .text.strip()
             == "Enabled",
         }
 
         return settings
 
+        return settings
+
     def _clean_text(self, text):
         """
         Clean text
 
         :param text: Text to clean
         :return: Cleaned text
         """
```

### Comparing `marketwatch-0.1.8/marketwatch/schemas.py` & `marketwatch-0.1.9/marketwatch/schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""
+MarketWatch Schemas
+
+This file contains the schemas for the MarketWatch API.
+"""
+
 from enum import Enum
 
 
 # Order Types and Enums
 class Term(Enum):
     """
     Order Term
```

### Comparing `marketwatch-0.1.8/pyproject.toml` & `marketwatch-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "marketwatch"
-version = "0.1.8"
+version = "0.1.9"
 description = "MarketWatch's API"
 authors = ["Antoine Boucher <antoine.boucher012@gmail.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "http://github.com/antoineboucher/marketwatch"
 documentation = "http://github.com/antoineboucher/marketwatch/wiki"
 keywords = ["marketwatch", "api", "stock", "finance", "market", "game"]
@@ -29,13 +29,13 @@
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 sphinx = "^6.1.3"
 pre-commit = "^3.0.0"
 black = "^23.1.0"
 genbadge = "^1.0.0"
 mkdocs = "^1.4.2"
-mkdocs-material = "^9.1.4"
+mkdocs-material = "^9.1.5"
 mkdocstrings = "^0.20.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `marketwatch-0.1.8/PKG-INFO` & `marketwatch-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marketwatch
-Version: 0.1.8
+Version: 0.1.9
 Summary: MarketWatch's API
 Home-page: http://github.com/antoineboucher/marketwatch
 License: Apache-2.0
 Keywords: marketwatch,api,stock,finance,market,game
 Author: Antoine Boucher
 Author-email: antoine.boucher012@gmail.com
 Requires-Python: >=3.10,<4.0
```

