# Comparing `tmp/les-louisdelatech-0.2.2.tar.gz` & `tmp/les_louisdelatech-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "les-louisdelatech-0.2.2.tar", max compression
+gzip compressed data, was "les_louisdelatech-0.3.0.tar", max compression
```

## Comparing `les-louisdelatech-0.2.2.tar` & `les_louisdelatech-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0    22294 2022-10-02 23:33:52.474428 les-louisdelatech-0.2.2/LICENSE
--rw-r--r--   0        0        0    23504 2022-10-02 23:33:52.474428 les-louisdelatech-0.2.2/LICENSE.fr
--rw-r--r--   0        0        0     2331 2022-10-02 23:33:52.474428 les-louisdelatech-0.2.2/README.md
--rw-r--r--   0        0        0        0 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/__init__.py
--rw-r--r--   0        0        0     2564 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/bot.py
--rw-r--r--   0        0        0      813 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/extensions/cats.py
--rw-r--r--   0        0        0      469 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/extensions/config.py
--rw-r--r--   0        0        0     2718 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/extensions/management.py
--rw-r--r--   0        0        0     4200 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/extensions/otp.py
--rw-r--r--   0        0        0      671 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/extensions/task.py
--rw-r--r--   0        0        0    14325 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/extensions/user.py
--rw-r--r--   0        0        0     1526 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/main.py
--rw-r--r--   0        0        0       45 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/models/__init__.py
--rw-r--r--   0        0        0      481 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/models/otp.py
--rw-r--r--   0        0        0     1094 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/templates/discord/base.j2
--rw-r--r--   0        0        0        0 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/templates/discord/ca.j2
--rw-r--r--   0        0        0        0 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/templates/discord/logistique.j2
--rw-r--r--   0        0        0        0 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/templates/discord/marketing.j2
--rw-r--r--   0        0        0      459 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/templates/discord/reset_password.j2
--rw-r--r--   0        0        0        0 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/templates/discord/scene.j2
--rw-r--r--   0        0        0        0 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/templates/discord/technique.j2
--rw-r--r--   0        0        0        0 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/templates/discord/tournoi.j2
--rw-r--r--   0        0        0     2705 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/templates/google/gmail_signature.j2
--rw-r--r--   0        0        0       48 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/utils/LouisDeLaTechError.py
--rw-r--r--   0        0        0     2958 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/utils/User.py
--rw-r--r--   0        0        0      753 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/utils/discord.py
--rw-r--r--   0        0        0     6169 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/utils/gsuite.py
--rw-r--r--   0        0        0      380 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/les_louisdelatech/utils/password.py
--rw-r--r--   0        0        0     1473 2022-10-02 23:33:52.478428 les-louisdelatech-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3514 1970-01-01 00:00:00.000000 les-louisdelatech-0.2.2/setup.py
--rw-r--r--   0        0        0     3787 1970-01-01 00:00:00.000000 les-louisdelatech-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    22294 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/LICENSE
+-rw-r--r--   0        0        0    23504 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/LICENSE.fr
+-rw-r--r--   0        0        0     2307 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/__init__.py
+-rw-r--r--   0        0        0     3330 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/bot.py
+-rw-r--r--   0        0        0      824 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/extensions/cats.py
+-rw-r--r--   0        0        0      492 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/extensions/config.py
+-rw-r--r--   0        0        0     2902 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/extensions/management.py
+-rw-r--r--   0        0        0     4632 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/extensions/otp.py
+-rw-r--r--   0        0        0      683 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/extensions/task.py
+-rw-r--r--   0        0        0    15315 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/extensions/user.py
+-rw-r--r--   0        0        0     1366 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/main.py
+-rw-r--r--   0        0        0       45 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/models/__init__.py
+-rw-r--r--   0        0        0      481 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/models/otp.py
+-rw-r--r--   0        0        0     1094 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/base.j2
+-rw-r--r--   0        0        0        0 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/ca.j2
+-rw-r--r--   0        0        0        0 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/logistique.j2
+-rw-r--r--   0        0        0        0 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/marketing.j2
+-rw-r--r--   0        0        0      459 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/reset_password.j2
+-rw-r--r--   0        0        0        0 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/scene.j2
+-rw-r--r--   0        0        0        0 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/technique.j2
+-rw-r--r--   0        0        0        0 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/tournoi.j2
+-rw-r--r--   0        0        0     2705 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/templates/google/gmail_signature.j2
+-rw-r--r--   0        0        0       48 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/utils/LouisDeLaTechError.py
+-rw-r--r--   0        0        0     2958 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/utils/User.py
+-rw-r--r--   0        0        0      753 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/utils/discord.py
+-rw-r--r--   0        0        0     6169 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/utils/gsuite.py
+-rw-r--r--   0        0        0      380 2023-05-08 22:04:22.325832 les_louisdelatech-0.3.0/les_louisdelatech/utils/password.py
+-rw-r--r--   0        0        0     1474 2023-05-08 22:04:47.821780 les_louisdelatech-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3861 1970-01-01 00:00:00.000000 les_louisdelatech-0.3.0/PKG-INFO
```

### Comparing `les-louisdelatech-0.2.2/LICENSE` & `les_louisdelatech-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `les-louisdelatech-0.2.2/LICENSE.fr` & `les_louisdelatech-0.3.0/LICENSE.fr`

 * *Files identical despite different names*

### Comparing `les-louisdelatech-0.2.2/README.md` & `les_louisdelatech-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 ```bash
 python3 -m les_louisdelatech.main -c config.toml -g google.json
 ```
 
 # Dev
 
-Install [Poetry](https://python-poetry.org/docs/master/#installing-with-the-official-installer) with version >= 1.2.0a1
+Install [Poetry](https://python-poetry.org/docs/master/#installing-with-the-official-installer)
 
 ```bash
 poetry install
 poetry shell
 pre-commit install
 ```
```

### Comparing `les-louisdelatech-0.2.2/les_louisdelatech/bot.py` & `les_louisdelatech-0.3.0/les_louisdelatech/bot.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,38 +6,50 @@
 import discord
 from cryptography.fernet import Fernet
 from discord.ext import commands
 from google.oauth2.service_account import Credentials
 from googleapiclient import discovery
 from tortoise import Tortoise, connections
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger()
 
 
 class LouisDeLaTech(commands.Bot):
     def __init__(self, config, google_path):
         super().__init__(
             command_prefix=config["discord"]["command_prefix"],
             description="LouisDeLaTech is a discord bot manager for Lyon e-Sport",
+            intents=discord.Intents(
+                messages=True,
+                message_content=True,
+                guilds=True,
+                voice_states=True,
+                members=True,
+            ),
         )
+        # added to make sure that the command tree will be synced only once
+        self.synced = False
 
         self.root_dir = os.path.dirname(os.path.abspath(__file__))
 
         self.config = config
         self.google_path = google_path
 
         self.fernet = Fernet(self.config["db"]["secret_key"])
 
     def encrypt(self, s):
         return self.fernet.encrypt(s.encode("ascii"))
 
     def decrypt(self, s):
         return self.fernet.decrypt(s).decode("ascii")
 
-    async def init_tortoise(self):
+    async def setup_hook(self):
+        for extension in self.config["discord"]["initial_cogs"]:
+            await self.load_extension(extension)
+
         await Tortoise.init(
             db_url=f"sqlite://{self.config['db']['filename']}",
             modules={"models": ["les_louisdelatech.models"]},
         )
         await Tortoise.generate_schemas()
 
     def admin_sdk(self):
@@ -59,20 +71,27 @@
         )
 
         return discovery.build("gmail", "v1", credentials=creds, cache_discovery=False)
 
     async def on_ready(self):
         logger.info(f"Logged in as: {self.user.name} - {self.user.id}")
         logger.info("Successfully logged in and booted...!")
+        if not self.synced:  # check if slash commands have been synced
+            await self.tree.sync()
+            logger.info("Slash commands synced")
 
     async def on_command_error(self, ctx, error):
         if isinstance(error, discord.ext.commands.errors.CommandNotFound):
             await ctx.send("Command not found")
+        elif isinstance(ctx, discord.Interaction):
+            await ctx.response.send_message(
+                f"Error while executing command => {error.__cause__}"
+            )
         else:
             await ctx.send(f"Error while executing command => {error.__cause__}")
-            traceback.print_exception(
-                type(error), error, error.__traceback__, file=sys.stderr
-            )
+        traceback.print_exception(
+            type(error), error, error.__traceback__, file=sys.stderr
+        )
 
     async def close(self):
         await connections.close_all()
         super()
```

### Comparing `les-louisdelatech-0.2.2/les_louisdelatech/extensions/cats.py` & `les_louisdelatech-0.3.0/les_louisdelatech/extensions/cats.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
 
 import discord
 import httpx
 from discord.ext import commands
 from discord.ext.commands import Context
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger()
 
 
 class CatCog(commands.Cog):
     def __init__(self, bot):
         self.bot = bot
 
-    @commands.command(name="cat", help="Get cat")
+    @commands.hybrid_command(name="cat", help="Get cat")
     async def get_cat(self, ctx: Context):
         async with httpx.AsyncClient() as client:
             cat_data = await client.get("https://api.thecatapi.com/v1/images/search")
 
         payload = cat_data.json()
         if not payload:
             return
@@ -24,9 +24,9 @@
         embed = discord.Embed(
             colour=discord.Colour.random(),
             title="Here is your kitty",
         ).set_image(url=cat_url)
         await ctx.send(embed=embed)
 
 
-def setup(bot):
-    bot.add_cog(CatCog(bot))
+async def setup(bot):
+    await bot.add_cog(CatCog(bot))
```

### Comparing `les-louisdelatech-0.2.2/les_louisdelatech/extensions/management.py` & `les_louisdelatech-0.3.0/les_louisdelatech/extensions/management.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,79 @@
-from itertools import count
-
 from discord.ext import commands
 
 from les_louisdelatech.utils.discord import is_team_allowed
 
 
-class TaskCog(commands.Cog):
+class ManagementCog(commands.Cog):
     def __init__(self, bot):
         self.bot = bot
 
-    @commands.command(help="Change channel topic")
+    @commands.hybrid_command(help="Change channel topic")
     @is_team_allowed
-    async def topic(self, ctx, description):
+    async def topic(
+        self,
+        ctx,
+        description: str = commands.parameter(description="Topic description"),
+    ):
         await ctx.channel.edit(topic=description)
         await ctx.send("Channel topic updated")
 
     # Meeting voice channel creation & deletion listener
     @commands.Cog.listener()
     async def on_voice_state_update(self, member, before, after):
         # Create voice channel block
         if (
             after.channel
             and after.channel.name
-            == self.bot.config["voice_channel_creation"]["trigger_channel_name"]
+            == self.bot.config["discord"]["voice_channel_creation"][
+                "trigger_channel_name"
+            ]
             and not member.bot
         ):
             # List meeting channels already existing in the user's category and order it
             list_channels_name = []
 
             def predicate(channel):
                 return channel.name.startswith(
-                    self.bot.config["voice_channel_creation"]["new_channel_name"]
+                    self.bot.config["discord"]["voice_channel_creation"][
+                        "new_channel_name"
+                    ]
                 )
 
             for channel in filter(predicate, after.channel.category.voice_channels):
                 list_channels_name.append(channel.name)
 
             # Iterate through the existing channels (if they exist) to create an non-existing one
             new_channel_name = None
             channel_number = 1
 
             while new_channel_name is None:
-                channel_name_check = f'{self.bot.config["voice_channel_creation"]["new_channel_name"]} #{channel_number}'
+                channel_name_check = f'{self.bot.config["discord"]["voice_channel_creation"]["new_channel_name"]} #{channel_number}'
                 if (
-                    not channel_name_check in list_channels_name
+                    channel_name_check not in list_channels_name
                     or not list_channels_name
                 ):
                     new_channel_name = channel_name_check
                 channel_number = channel_number + 1
 
             # Create the channel and move member
             new_channel = await member.guild.create_voice_channel(
                 new_channel_name,
-                overwrites=None,
                 category=after.channel.category,
                 bitrate=self.bot.config["voice_channel_creation"]["bitrate"],
             )
             await member.move_to(new_channel)
 
         # Delete voice channel block
         if (
             before.channel
             and before.channel.name.startswith(
-                self.bot.config["voice_channel_creation"]["new_channel_name"]
+                self.bot.config["discord"]["voice_channel_creation"]["new_channel_name"]
             )
             and not member.bot
             and not before.channel.members
         ):
             await before.channel.delete(reason="Channel is empty")
 
 
-def setup(bot):
-    bot.add_cog(TaskCog(bot))
+async def setup(bot):
+    await bot.add_cog(ManagementCog(bot))
```

### Comparing `les-louisdelatech-0.2.2/les_louisdelatech/extensions/otp.py` & `les_louisdelatech-0.3.0/les_louisdelatech/extensions/otp.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 from les_louisdelatech.models.otp import Otp
 from les_louisdelatech.utils.discord import is_team_allowed
 from les_louisdelatech.utils.gsuite import format_google_api_error, search_user
 from les_louisdelatech.utils.LouisDeLaTechError import LouisDeLaTechError
 from les_louisdelatech.utils.User import User
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger()
 
 
 class OtpCog(commands.Cog):
     def __init__(self, bot):
         self.bot = bot
 
-    @commands.command(name="lotp", help="List otp code")
+    @commands.hybrid_command(name="lotp", help="List otp code")
     @commands.guild_only()
     @is_team_allowed
     async def list_otp(self, ctx):
         try:
             user = User(
                 search_user(self.bot.admin_sdk(), ctx.author.name, ctx.author.id)
             )
@@ -40,18 +40,20 @@
                 message += f"\n{o.name}"
         else:
             message += "No Otp code available"
         message += "```"
 
         await ctx.send(message)
 
-    @commands.command(name="gotp", help="Get otp code")
+    @commands.hybrid_command(name="gotp", help="Get otp code")
     @commands.guild_only()
     @is_team_allowed
-    async def get_otp(self, ctx, name):
+    async def get_otp(
+        self, ctx, name: str = commands.parameter(description="Otp name")
+    ):
         try:
             user = User(
                 search_user(self.bot.admin_sdk(), ctx.author.name, ctx.author.id)
             )
         except LouisDeLaTechError as e:
             await ctx.send(f"{ctx.author} => {e.args[0]}")
             return
@@ -70,18 +72,25 @@
         await ctx.author.send(f"Otp code for {name} is {totp.now()}")
 
         logger.info(f"Otp code {name} of team {user.team} send in DM to {ctx.author}")
         await ctx.send(
             f"Otp code {name} of team {user.team} send in DM to {ctx.author}"
         )
 
-    @commands.command(name="cotp", help="Create otp code")
+    @commands.hybrid_command(name="cotp", help="Create otp code")
     @commands.guild_only()
     @is_team_allowed
-    async def create_otp(self, ctx, name, digest, digits, secret):
+    async def create_otp(
+        self,
+        ctx,
+        name: str = commands.parameter(description="Otp name"),
+        digest: str = commands.parameter(description="Otp digest"),
+        digits: str = commands.parameter(description="Otp digits"),
+        secret: str = commands.parameter(description="Otp secret"),
+    ):
         await ctx.message.delete()
 
         try:
             user = User(
                 search_user(self.bot.admin_sdk(), ctx.author.name, ctx.author.id)
             )
         except LouisDeLaTechError as e:
@@ -98,18 +107,20 @@
             digits=digits,
             secret=self.bot.encrypt(secret),
         )
 
         logger.info(f"Otp code {name} of team {user.team} created by {ctx.author}")
         await ctx.send(f"Otp code {name} of team {user.team} created by {ctx.author}")
 
-    @commands.command(name="dotp", help="Delete otp code")
+    @commands.hybrid_command(name="dotp", help="Delete otp code")
     @commands.guild_only()
     @is_team_allowed
-    async def delete_otp(self, ctx, name):
+    async def delete_otp(
+        self, ctx, name: str = commands.parameter(description="Otp name")
+    ):
         try:
             user = User(
                 search_user(self.bot.admin_sdk(), ctx.author.name, ctx.author.id)
             )
         except LouisDeLaTechError as e:
             await ctx.send(f"{ctx.author} => {e.args[0]}")
             return
@@ -119,9 +130,9 @@
 
         await Otp.filter(name=name, team=user.team).delete()
 
         logger.info(f"Otp code {name} of team {user.team} deleted by {ctx.author}")
         await ctx.send(f"Otp code {name} of team {user.team} deleted by {ctx.author}")
 
 
-def setup(bot):
-    bot.add_cog(OtpCog(bot))
+async def setup(bot):
+    await bot.add_cog(OtpCog(bot))
```

### Comparing `les-louisdelatech-0.2.2/les_louisdelatech/extensions/task.py` & `les_louisdelatech-0.3.0/les_louisdelatech/extensions/task.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,9 +19,9 @@
     @change_bot_activity.before_loop
     async def before_send(self):
         await self.bot.wait_until_ready()
 
         return
 
 
-def setup(bot):
-    bot.add_cog(TaskCog(bot))
+async def setup(bot):
+    await bot.add_cog(TaskCog(bot))
```

### Comparing `les-louisdelatech-0.2.2/les_louisdelatech/extensions/user.py` & `les_louisdelatech-0.3.0/les_louisdelatech/extensions/user.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,23 +24,29 @@
     update_user_recovery,
     update_user_signature,
 )
 from les_louisdelatech.utils.LouisDeLaTechError import LouisDeLaTechError
 from les_louisdelatech.utils.password import generate_password
 from les_louisdelatech.utils.User import User
 
-logger = logging.getLogger(__name__)
+logger = logging.getLogger()
 
 
 class UserCog(commands.Cog):
-    @commands.command(help="Provision an user")
+    @commands.hybrid_command(help="Provision an user")
     @commands.guild_only()
     @is_gsuite_admin
     async def provision(
-        self, ctx, member: discord.Member, firstname, lastname, pseudo, role_name
+        self,
+        ctx,
+        member: discord.Member = commands.parameter(description="Discord user"),
+        firstname: str = commands.parameter(description="User firstname"),
+        lastname: str = commands.parameter(description="User lastname"),
+        pseudo: str = commands.parameter(description="User pseudo"),
+        role_name: str = commands.parameter(description="User role"),
     ):
         """
         Provision an user
         [Discord]
             => User will be added to default group
             => User will be added to team group
         [Google]
@@ -141,18 +147,22 @@
         team_message = template.render()
         if team_message:
             await member.send(team_message)
 
     def __init__(self, bot):
         self.bot = bot
 
-    @commands.command(help="Deprovision an user")
+    @commands.hybrid_command(help="Deprovision an user")
     @commands.guild_only()
     @is_gsuite_admin
-    async def deprovision(self, ctx, member: discord.Member):
+    async def deprovision(
+        self,
+        ctx,
+        member: discord.Member = commands.parameter(description="Discord user"),
+    ):
         """
         [Discord]
             => User will be removed from all groups
         [Google]
             => User will be suspended
         """
         try:
@@ -173,18 +183,23 @@
             await ctx.send(format_google_api_error(e))
             raise
 
         await member.edit(roles=[])
 
         await ctx.send(f"User {member.name} deprovisionned")
 
-    @commands.command(name="uteam", help="Update user team")
+    @commands.hybrid_command(name="uteam", help="Update user team")
     @commands.guild_only()
     @is_gsuite_admin
-    async def update_team(self, ctx, member: discord.Member, new_team_name):
+    async def update_team(
+        self,
+        ctx,
+        member: discord.Member = commands.parameter(description="Discord user"),
+        new_team_name: str = commands.parameter(description="New team name"),
+    ):
         """
         [Discord]
             => User will be removed from all team groups
             => User will be added to this new team
         [Google]
             => User will be removed from all team groups
             => User will be added to this new team
@@ -258,18 +273,23 @@
             await member.add_roles(role)
         else:
             await ctx.send(f"Discord role {user.team} does not exist")
             return
 
         await ctx.send(f"User {member.name} is now member of team: {user.team}")
 
-    @commands.command(name="upseudo", help="Update user pseudo")
+    @commands.hybrid_command(name="upseudo", help="Update user pseudo")
     @commands.guild_only()
     @is_gsuite_admin
-    async def update_pseudo(self, ctx, member: discord.Member, new_pseudo):
+    async def update_pseudo(
+        self,
+        ctx,
+        member: discord.Member = commands.parameter(description="Discord user"),
+        new_pseudo: str = commands.parameter(description="New user pseudo"),
+    ):
         """
         [Discord]
             => User will be renamed
         [Google]
             => User pseudo will be renamed
         """
         try:
@@ -299,15 +319,15 @@
 
         await member.edit(
             nick=User.discord_name(user.firstname, user.pseudo, user.lastname)
         )
 
         await ctx.send(f"User {old_nick} you now shall be called {member.nick} !")
 
-    @commands.command(
+    @commands.hybrid_command(
         name="usignatures", help="Update the signature of all users on gmail"
     )
     @commands.guild_only()
     @is_gsuite_admin
     async def update_signatures(self, ctx):
         user_updated = 0
         try:
@@ -349,18 +369,23 @@
                 continue
             except HttpError as e:
                 await ctx.send(format_google_api_error(e))
                 return
 
         await ctx.send(f"Updated signatures for {user_updated}/{len(users)} users")
 
-    @commands.command(help="Update recovery email of an user")
+    @commands.hybrid_command(help="Update recovery email of an user")
     @commands.guild_only()
     @is_gsuite_admin
-    async def urecovery(self, ctx, member: discord.Member, backup_email):
+    async def urecovery(
+        self,
+        ctx,
+        member: discord.Member = commands.parameter(description="Discord user"),
+        backup_email: str = commands.parameter(description="User backup email"),
+    ):
         try:
             user = User(search_user(self.bot.admin_sdk(), member.name, member.id))
             is_user_managed(
                 self.bot.admin_sdk(), user.email, self.bot.config["teams_to_skip"]
             )
         except LouisDeLaTechError as e:
             await ctx.send(f"{member} => {e.args[0]}")
@@ -372,18 +397,22 @@
             update_user_recovery(self.bot.admin_sdk(), user.email, backup_email)
         except HttpError as e:
             await ctx.send(format_google_api_error(e))
             raise
 
         await ctx.send(f"Updated recovery information for user {member.name}")
 
-    @commands.command(help="Reset password of an user")
+    @commands.hybrid_command(help="Reset password of an user")
     @commands.guild_only()
     @is_gsuite_admin
-    async def rpassword(self, ctx, member: discord.Member):
+    async def rpassword(
+        self,
+        ctx,
+        member: discord.Member = commands.parameter(description="Discord user"),
+    ):
         try:
             user = User(search_user(self.bot.admin_sdk(), member.name, member.id))
             is_user_managed(
                 self.bot.admin_sdk(), user.email, self.bot.config["teams_to_skip"]
             )
         except LouisDeLaTechError as e:
             await ctx.send(f"{member} => {e.args[0]}")
@@ -413,9 +442,9 @@
             template.render(
                 {"email": user.email, "password": escape_markdown(temp_pass)}
             )
         )
         await ctx.send(f"Sent a new password to {member.name} in PM")
 
 
-def setup(bot):
-    bot.add_cog(UserCog(bot))
+async def setup(bot):
+    await bot.add_cog(UserCog(bot))
```

### Comparing `les-louisdelatech-0.2.2/les_louisdelatech/main.py` & `les_louisdelatech-0.3.0/les_louisdelatech/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import sentry_sdk
 import tomli
 
 from les_louisdelatech.bot import LouisDeLaTech
 
 logging.basicConfig(level=logging.INFO, format="%(asctime)s %(levelname)s:%(message)s")
-logger = logging.getLogger(__name__)
+logger = logging.getLogger()
 
 parser = ArgumentParser()
 parser.add_argument(
     "-c",
     "--config",
     action="store",
     dest="config",
@@ -24,19 +24,19 @@
     action="store",
     dest="google",
     default="/etc/LouisDeLaTech/google.json",
     help="Path to google secrets json",
 )
 args = parser.parse_args()
 
-logger.info(f"Bot started")
+logger.info("Bot started")
 
 with open(args.config, "rb") as f:
     config = tomli.load(f)
-logger.info(f"Config loaded")
+logger.info("Config loaded")
 
 log_level = logging.getLevelName(config["log_level"])
 logger.setLevel(log_level)
 logger.info(f"Started bot with log level {logging.getLevelName(logger.level)}")
 
 if len(config["sentry_dsn"]) > 0:
     sentry_sdk.init(
@@ -44,13 +44,9 @@
         # Set traces_sample_rate to 1.0 to capture 100%
         # of transactions for performance monitoring.
         # We recommend adjusting this value in production.
         traces_sample_rate=0.5,
     )
 
 bot = LouisDeLaTech(config, args.google)
-bot.loop.run_until_complete(bot.init_tortoise())
 
-for extension in config["discord"]["initial_cogs"]:
-    bot.load_extension(extension)
-
-bot.run(config["discord"]["token"], bot=True, reconnect=True)
+bot.run(config["discord"]["token"], reconnect=True)
```

### Comparing `les-louisdelatech-0.2.2/les_louisdelatech/templates/discord/base.j2` & `les_louisdelatech-0.3.0/les_louisdelatech/templates/discord/base.j2`

 * *Files identical despite different names*

### Comparing `les-louisdelatech-0.2.2/les_louisdelatech/templates/google/gmail_signature.j2` & `les_louisdelatech-0.3.0/les_louisdelatech/templates/google/gmail_signature.j2`

 * *Files identical despite different names*

### Comparing `les-louisdelatech-0.2.2/les_louisdelatech/utils/User.py` & `les_louisdelatech-0.3.0/les_louisdelatech/utils/User.py`

 * *Files identical despite different names*

### Comparing `les-louisdelatech-0.2.2/les_louisdelatech/utils/discord.py` & `les_louisdelatech-0.3.0/les_louisdelatech/utils/discord.py`

 * *Files identical despite different names*

### Comparing `les-louisdelatech-0.2.2/les_louisdelatech/utils/gsuite.py` & `les_louisdelatech-0.3.0/les_louisdelatech/utils/gsuite.py`

 * *Files identical despite different names*

### Comparing `les-louisdelatech-0.2.2/pyproject.toml` & `les_louisdelatech-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "les-louisdelatech"
-version = "0"
+version = "0.3.0"
 description = "LouisDeLaTech is a discord bot manager for Lyon e-Sport"
 authors = [
     "Ludovic Ortega <ludovic.ortega@lyon-esport.fr>",
     "Etienne 'PoPs' G. <etienne.guilluy@lyon-esport.fr>",
     "Pierre 'DrumSlayer' Sarret <pierre.sarret@lyon-esport.fr>",
 
 ]
@@ -14,39 +14,37 @@
 repository = "https://github.com/lyon-esport/LouisDeLaTech"
 keywords = ["google", "discord"]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)",
     "Topic :: Utilities",
 ]
 include = [
     "LICENSE",
     "LICENSE.fr",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-"discord.py" = "^1.7.3"
+discord-py = "^2.2.3"
 Jinja2 = "^3.1.2"
 google-api-python-client = "^2.52.0"
 google-auth-httplib2 = "^0.1.0"
 pyotp = "^2.6.0"
 tortoise-orm = "^0.19.1"
 aiosqlite = "^0.17.0"
-cryptography = ">=37.0.4,<39.0.0"
+cryptography = ">=37.0.4,<41.0.0"
 sentry-sdk = "^1.6.0"
-httpx = "^0.23.0"
+httpx = ">=0.23,<0.25"
 tomli = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
-pre-commit = "^2.20.0"
+pre-commit = "^3.3.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
-
-[tool.poetry-version-plugin]
-source = "git-tag"
```

### Comparing `les-louisdelatech-0.2.2/PKG-INFO` & `les_louisdelatech-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: les-louisdelatech
-Version: 0.2.2
+Version: 0.3.0
 Summary: LouisDeLaTech is a discord bot manager for Lyon e-Sport
 Home-page: https://github.com/lyon-esport/LouisDeLaTech
 License: CeCILL
 Keywords: google,discord
 Author: Ludovic Ortega
 Author-email: ludovic.ortega@lyon-esport.fr
 Requires-Python: >=3.8,<4.0
@@ -12,25 +12,27 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: aiosqlite (>=0.17.0,<0.18.0)
-Requires-Dist: cryptography (>=37.0.4,<39.0.0)
-Requires-Dist: discord.py (>=1.7.3,<2.0.0)
+Requires-Dist: cryptography (>=37.0.4,<41.0.0)
+Requires-Dist: discord-py (>=2.2.3,<3.0.0)
 Requires-Dist: google-api-python-client (>=2.52.0,<3.0.0)
 Requires-Dist: google-auth-httplib2 (>=0.1.0,<0.2.0)
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: httpx (>=0.23,<0.25)
 Requires-Dist: pyotp (>=2.6.0,<3.0.0)
 Requires-Dist: sentry-sdk (>=1.6.0,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tortoise-orm (>=0.19.1,<0.20.0)
 Project-URL: Repository, https://github.com/lyon-esport/LouisDeLaTech
 Description-Content-Type: text/markdown
 
@@ -89,15 +91,15 @@
 
 ```bash
 python3 -m les_louisdelatech.main -c config.toml -g google.json
 ```
 
 # Dev
 
-Install [Poetry](https://python-poetry.org/docs/master/#installing-with-the-official-installer) with version >= 1.2.0a1
+Install [Poetry](https://python-poetry.org/docs/master/#installing-with-the-official-installer)
 
 ```bash
 poetry install
 poetry shell
 pre-commit install
 ```
```

