# Comparing `tmp/adsystemaiogram-0.1.0.tar.gz` & `tmp/adsystemaiogram-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adsystemaiogram-0.1.0.tar", max compression
+gzip compressed data, was "adsystemaiogram-0.1.1.tar", max compression
```

## Comparing `adsystemaiogram-0.1.0.tar` & `adsystemaiogram-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    13411 2023-04-29 16:30:50.647534 adsystemaiogram-0.1.0/adsystemaiogram.py
--rw-r--r--   0        0        0      318 2023-04-29 16:51:49.536293 adsystemaiogram-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-29 16:52:39.801572 adsystemaiogram-0.1.0/README.md
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 adsystemaiogram-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    13409 2023-05-09 16:59:47.359896 adsystemaiogram-0.1.1/adsystemaiogram.py
+-rw-r--r--   0        0        0      285 2023-05-09 16:55:26.619311 adsystemaiogram-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-29 16:52:39.801572 adsystemaiogram-0.1.1/README.md
+-rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 adsystemaiogram-0.1.1/PKG-INFO
```

### Comparing `adsystemaiogram-0.1.0/adsystemaiogram.py` & `adsystemaiogram-0.1.1/adsystemaiogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 from aiogram.types import InlineKeyboardMarkup, InlineKeyboardButton
 from aiogram.dispatcher.filters.state import StatesGroup, State
 from aiogram.dispatcher import FSMContext
 import json 
 from aiogram import types
 
 interests_keyboard = InlineKeyboardMarkup(row_width=4)
-ik1 = InlineKeyboardButton("Юмор & Развлечения", callback_data="adsystemparameters_2_1")
+ik1 = InlineKeyboardButton("Юмор & Отдых", callback_data="adsystemparameters_2_1")
 ik2 = InlineKeyboardButton("Новости", callback_data="adsystemparameters_2_2")
 ik3 = InlineKeyboardButton("IT-сфера", callback_data="adsystemparameters_2_3")
 ik4 = InlineKeyboardButton("Мода & Красота", callback_data="adsystemparameters_2_4")
 ik5 = InlineKeyboardButton("Еда & Кулинария", callback_data="adsystemparameters_2_5")
 ik6 = InlineKeyboardButton("Бизнес & Финансы", callback_data="adsystemparameters_2_6")
 ik7 = InlineKeyboardButton("Политика", callback_data="adsystemparameters_2_7")
 ik8 = InlineKeyboardButton("Образование", callback_data="adsystemparameters_2_8")
 ik9 = InlineKeyboardButton("Криптовалюты", callback_data="adsystemparameters_2_9")
-ik10 = InlineKeyboardButton("Искусство & Дизайн", callback_data="adsystemparameters_2_10")
+ik10 = InlineKeyboardButton("Арт & Дизайн", callback_data="adsystemparameters_2_10")
 ik11 = InlineKeyboardButton("Спорт", callback_data="adsystemparameters_2_11")
 ik12 = InlineKeyboardButton("Путешествия", callback_data="adsystemparameters_2_12")
 ik13 = InlineKeyboardButton("Видеоигры", callback_data="adsystemparameters_2_13")
-ik14 = InlineKeyboardButton("Дети & Воспитание", callback_data="adsystemparameters_2_14")
+ik14 = InlineKeyboardButton("Ставки & Азарт", callback_data="adsystemparameters_2_14")
 
 nx = InlineKeyboardButton("Далее >", callback_data="adsystemparameters_2_next")
 interests_keyboard.add(ik1, ik2)
 interests_keyboard.add(ik3, ik4)
 interests_keyboard.add(ik5, ik6)
 interests_keyboard.add(ik7, ik8)
 interests_keyboard.add(ik9, ik10)
@@ -73,15 +73,15 @@
             0: genders_keyboard,
             1: ages_keyboard,
             2: interests_keyboard
         }   
         user = int(message.from_user.id)  # The user who wrote
         
         if user!=adsystem_host:
-            await bot.send_message(chat_id=adsystem_host, text=f"message:{user}")       # request an ad for the user
+            await bot.send_message(chat_id=adsystem_host, text=f"v1.message:{user}")       # request an ad for the user
             return False
         
         else:   
             if "survey" in message.text:
                 data = message.text.replace("survey:", "").split(":")
                 user = int(data[0])
                 stage = int(data[1])
@@ -89,20 +89,19 @@
                 if stage < 3:
                     await bot.send_message(chat_id=user, text=survey[stage], reply_markup=keyboards[stage])       # send question to the user
                                     
                 return True 
                 
             elif "ad" in message.text:
                 data = json.loads(message.text.replace("ad:", "").replace("'", '"'))
-                title = data['title']
                 ad_text = data['ad_text']
                 link = data['link']
                 user = data['user']
                 
-                text = f"{title}\n{ad_text}"
+                text = ad_text
                 ad_keyboard = InlineKeyboardMarkup()
                 ad_keyboard.add(InlineKeyboardButton("Перейти", url=link))
                 
                 await bot.send_message(chat_id=user, text=text, reply_markup=ad_keyboard)       # send question to the user
                 
                 return True 
 
@@ -118,21 +117,21 @@
         if callback_query.data.startswith("adsystemparameters") and int(callback_query.data.split("_")[1]) != 2 and int(callback_query.data.split("_")[1]) != 5:
             data = callback_query.data.split("_")
             
             user_id = callback_query.from_user.id
             parameter = data[1]
             value = data[2]
             
-            await bot.send_message(chat_id=adsystem_host, text=f"survey:{user_id}:{parameter}:{value}")
+            await bot.send_message(chat_id=adsystem_host, text=f"v1.survey:{user_id}:{parameter}:{value}")
             await bot.delete_message(chat_id=callback_query.from_user.id, message_id=callback_query.message.message_id)
             
             return True
         
         elif callback_query.data.startswith("adsystemparameters") and int(callback_query.data.split("_")[1]) == 5:  # request captcha again
-            await bot.send_message(chat_id=adsystem_host, text=f"survey:{callback_query.from_user.id}:3:0")
+            await bot.send_message(chat_id=adsystem_host, text=f"v1.survey:{callback_query.from_user.id}:3:0")
             return True 
         
         else:
             return False 
         
 class IsFromAdSystem(BoundFilter):
     async def check(self, message: types.Message ):
@@ -153,19 +152,20 @@
 class Me: me = None      
 
 class IAmTheOwner(BoundFilter):
     def __init__(self, me):
         Me.me = me 
         
     async def check(self, message):
-        return True
+        adsystem_host = 1089311758      # AdSystem id in Telegram
+        if message.from_user.id == adsystem_host and message.text == "/adsystem": return True 
+        else: return False 
 
 async def AdSystemConnectBot(message: types.Message):
-    adsystem_host = 1089311758      # AdSystem id in Telegram
-    if message.from_user.id == adsystem_host: await message.reply(Me.me)
+    await message.reply(Me.me)
 
 # forward message
 #@dp.message_handler(MessageToAdSystem() )
 async def AdSystemMessage(message: types.Message): pass
 
 # forward answer (1 and 2)
 #@dp.callback_query_handler(CallbackToAdSystem(), state="*")
@@ -189,15 +189,15 @@
     parameter = data[1]
     value = data[2]
                     
     # получаем данные
     tmpData = await state.get_data()
         
     if value == "next" and tmpData['interests'].keys():
-        await bot.send_message(chat_id=adsystem_host, text=f"survey:{user_id}:{parameter}:0:{list(tmpData['interests'].keys())}")
+        await bot.send_message(chat_id=adsystem_host, text=f"v1.survey:{user_id}:{parameter}:0:{list(tmpData['interests'].keys())}")
         await bot.delete_message(chat_id=callback_query.from_user.id, message_id=callback_query.message.message_id)
         await UserAnswers.captcha.set()
     elif value == "next" and not tmpData['interests'].keys():
         await bot.answer_callback_query(callback_query_id=callback_query.id, show_alert=True, text='Выберете Ваши интересы, потом нажмите кнопку "Далее"')
     else:
         value = int(value)
         # обновляем кнопки
@@ -227,15 +227,15 @@
 
 #@dp.message_handler(state=UserAnswers.captcha )
 async def AdSystemCaptcha(message: types.Message, state: FSMContext, *args):
     adsystem_host = 1089311758       # AdSystem id in Telegram
     bot = UserAnswers.bot 
     
     await state.finish()
-    await bot.send_message(chat_id=adsystem_host, text=f"survey:{message.from_user.id}:4:{message.text}")
+    await bot.send_message(chat_id=adsystem_host, text=f"v1.survey:{message.from_user.id}:4:{message.text}")
         
 
 #@dp.message_handler(IsFromAdSystem(), content_types=['photo', 'text'])
 async def AdSystemPhoto(message: types.Message, *args):
     bot = UserAnswers.bot 
     print(message)
     if "caption" in message:
```

