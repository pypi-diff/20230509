# Comparing `tmp/magyar-2.9.9.tar.gz` & `tmp/magyar-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-2.9.9.tar", last modified: Wed May  3 19:34:15 2023, max compression
+gzip compressed data, was "magyar-3.0.0.tar", last modified: Tue May  9 20:26:21 2023, max compression
```

## Comparing `magyar-2.9.9.tar` & `magyar-3.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-03 19:34:15.241380 magyar-2.9.9/
--rw-rw-r--   0 bela      (1000) bela      (1000)     5398 2023-05-03 19:34:15.237380 magyar-2.9.9/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     5000 2023-05-03 19:14:22.000000 magyar-2.9.9/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-03 19:34:15.237380 magyar-2.9.9/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     5398 2023-05-03 19:34:15.000000 magyar-2.9.9/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-03 19:34:15.000000 magyar-2.9.9/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-03 19:34:15.000000 magyar-2.9.9/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-03 19:34:15.000000 magyar-2.9.9/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)    36183 2023-05-03 19:14:22.000000 magyar-2.9.9/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-03 19:34:15.241380 magyar-2.9.9/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      615 2023-05-03 19:14:22.000000 magyar-2.9.9/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-09 20:26:21.121485 magyar-3.0.0/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     5855 2023-05-09 20:26:21.121485 magyar-3.0.0/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     5445 2023-05-09 20:24:54.000000 magyar-3.0.0/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-09 20:26:21.121485 magyar-3.0.0/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     5855 2023-05-09 20:26:21.000000 magyar-3.0.0/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-09 20:26:21.000000 magyar-3.0.0/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-09 20:26:21.000000 magyar-3.0.0/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-09 20:26:21.000000 magyar-3.0.0/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    38473 2023-05-09 20:11:06.000000 magyar-3.0.0/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-09 20:26:21.121485 magyar-3.0.0/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-09 20:12:58.000000 magyar-3.0.0/setup.py
```

### Comparing `magyar-2.9.9/PKG-INFO` & `magyar-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.9.9
-Summary: Hungarian names,animals,food, fruit, river ..
+Version: 3.0.0
+Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -33,44 +33,50 @@
 15. Magyarország halai = magyar.**hal**
 16. Magyarország madarai = magyar.**madar**
 17. A naprendszer bolygóinak magyar neve = magyar.**bolygo**
 18. Magyar leves nevek =  magyar.**leves**
 19. Magyar főételek = magyar.**foetel**
 20. Magyar köretek = magyar.**koret**
 21. Magyar egytál ételek = magyar.**egytal**
+22. Magyar desszertek = magyar.**desszert**
+23. Magyar borok = magyar.**bor**
+24. Magyar üdítők= magyar.**utito**
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
 
 ## Description
-1. last names =  magyar.**vezeteknev**
-2. female first names = magyar.**keresztnev_n**
-3. male first names  = magyar.**keresztnev_f**
-4. street names = magyar.**utca**
-5. city names = magyar.**telepules**
-6. names of counties = magyar.**megye**
-7. names of rivers = magyar.**folyo**
+1. Last names =  magyar.**vezeteknev**
+2. Female first names = magyar.**keresztnev_n**
+3. Male first names  = magyar.**keresztnev_f**
+4. Street names = magyar.**utca**
+5. City names = magyar.**telepules**
+6. Names of counties = magyar.**megye**
+7. Names of rivers = magyar.**folyo**
 8. The days of the week = magyar.**nap**
-9. the months of the year = magyar.**honap**
-10. fruits = magyar.**gyumolcs**
-11. vegetables = magyar.**zoldseg**
-12. domesticated animals = magyar.**haszonallat**
-13. hungarian wildlife  = magyar.**vad**
+9. The months of the year = magyar.**honap**
+10. Fruits = magyar.**gyumolcs**
+11. Vegetables = magyar.**zoldseg**
+12. Domesticated animals = magyar.**haszonallat**
+13. Hungarian wildlife  = magyar.**vad**
 14. Fishes of Hungary = magyar.**hal**
 15. Birds of Hungary = magyar.**madar**
 16. Hungarian names of planets = magyar.**bolygo**
 17. Hungarian soup names = magyar.**leves**
-18. Hugarian given names M+F  magyar.**keresztnev_v**
+18. Hungarian given names M+F  magyar.**keresztnev_v**
 19. Hungarian main foods = magyar.**foetel**
 20. Hungarian side dishes  = magyar.**koret**
 21. Hungarian one-pot meals = magyar.**egytal**
+22. Hungarian sweet treats = magyar.**desszert**
+23. Hungarian wines =magyar.**bor**
+24. Hungarian soft drinks= magyar.**udito**
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
 4. Hungarian tram lines = magyar.villamos
 5. Hunngarian names of Europian capitals, states = magyar.orszag
@@ -122,19 +128,23 @@
 Gulyásleves, Halászlé, Hideg meggyleves, Zöldborsóleves, 
 Jókai bableves, Csontleves, Marhahúsleves, Zellerkrémleves, 
 Sárgaborsóleves, Babgulyásleves, Karalábéleves, Zöldségleves, 
 Kukoricaleves, Karfiolleves, Hideg gyümölcsleves, Korhelyleves, 
 Tyúkhúsleves, Pirított tarhonyaleves, Gombaleves, Lencseleves, 
 Gulyáskrémleves, Csülökleves, Paradicsomleves, Borleves, 
 
-3. Listák ABC sorrendbe rendezése  </br>
+3. Listák ABC sorrendbe rendezése, ékezet érzékeny </br>
 
 
-    magyar.abc(lista):
+         magyar.abc(lista):
 
+Használat : </br> </br>
+gyumolcs =['Áfonya', 'Eper', 'Alma', 'Meggy','Őszibarack',]
+sorban =magyar.abc(gyumolcs) </br>
+['Alma', 'Áfonya', 'Eper', 'Meggy', 'Őszibarack']
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-2.9.9/README.md` & `magyar-3.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,44 +21,50 @@
 15. Magyarország halai = magyar.**hal**
 16. Magyarország madarai = magyar.**madar**
 17. A naprendszer bolygóinak magyar neve = magyar.**bolygo**
 18. Magyar leves nevek =  magyar.**leves**
 19. Magyar főételek = magyar.**foetel**
 20. Magyar köretek = magyar.**koret**
 21. Magyar egytál ételek = magyar.**egytal**
+22. Magyar desszertek = magyar.**desszert**
+23. Magyar borok = magyar.**bor**
+24. Magyar üdítők= magyar.**utito**
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
 
 ## Description
-1. last names =  magyar.**vezeteknev**
-2. female first names = magyar.**keresztnev_n**
-3. male first names  = magyar.**keresztnev_f**
-4. street names = magyar.**utca**
-5. city names = magyar.**telepules**
-6. names of counties = magyar.**megye**
-7. names of rivers = magyar.**folyo**
+1. Last names =  magyar.**vezeteknev**
+2. Female first names = magyar.**keresztnev_n**
+3. Male first names  = magyar.**keresztnev_f**
+4. Street names = magyar.**utca**
+5. City names = magyar.**telepules**
+6. Names of counties = magyar.**megye**
+7. Names of rivers = magyar.**folyo**
 8. The days of the week = magyar.**nap**
-9. the months of the year = magyar.**honap**
-10. fruits = magyar.**gyumolcs**
-11. vegetables = magyar.**zoldseg**
-12. domesticated animals = magyar.**haszonallat**
-13. hungarian wildlife  = magyar.**vad**
+9. The months of the year = magyar.**honap**
+10. Fruits = magyar.**gyumolcs**
+11. Vegetables = magyar.**zoldseg**
+12. Domesticated animals = magyar.**haszonallat**
+13. Hungarian wildlife  = magyar.**vad**
 14. Fishes of Hungary = magyar.**hal**
 15. Birds of Hungary = magyar.**madar**
 16. Hungarian names of planets = magyar.**bolygo**
 17. Hungarian soup names = magyar.**leves**
-18. Hugarian given names M+F  magyar.**keresztnev_v**
+18. Hungarian given names M+F  magyar.**keresztnev_v**
 19. Hungarian main foods = magyar.**foetel**
 20. Hungarian side dishes  = magyar.**koret**
 21. Hungarian one-pot meals = magyar.**egytal**
+22. Hungarian sweet treats = magyar.**desszert**
+23. Hungarian wines =magyar.**bor**
+24. Hungarian soft drinks= magyar.**udito**
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
 4. Hungarian tram lines = magyar.villamos
 5. Hunngarian names of Europian capitals, states = magyar.orszag
@@ -110,19 +116,23 @@
 Gulyásleves, Halászlé, Hideg meggyleves, Zöldborsóleves, 
 Jókai bableves, Csontleves, Marhahúsleves, Zellerkrémleves, 
 Sárgaborsóleves, Babgulyásleves, Karalábéleves, Zöldségleves, 
 Kukoricaleves, Karfiolleves, Hideg gyümölcsleves, Korhelyleves, 
 Tyúkhúsleves, Pirított tarhonyaleves, Gombaleves, Lencseleves, 
 Gulyáskrémleves, Csülökleves, Paradicsomleves, Borleves, 
 
-3. Listák ABC sorrendbe rendezése  </br>
+3. Listák ABC sorrendbe rendezése, ékezet érzékeny </br>
 
 
-    magyar.abc(lista):
+         magyar.abc(lista):
 
+Használat : </br> </br>
+gyumolcs =['Áfonya', 'Eper', 'Alma', 'Meggy','Őszibarack',]
+sorban =magyar.abc(gyumolcs) </br>
+['Alma', 'Áfonya', 'Eper', 'Meggy', 'Őszibarack']
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-2.9.9/magyar.egg-info/PKG-INFO` & `magyar-3.0.0/magyar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.9.9
-Summary: Hungarian names,animals,food, fruit, river ..
+Version: 3.0.0
+Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -33,44 +33,50 @@
 15. Magyarország halai = magyar.**hal**
 16. Magyarország madarai = magyar.**madar**
 17. A naprendszer bolygóinak magyar neve = magyar.**bolygo**
 18. Magyar leves nevek =  magyar.**leves**
 19. Magyar főételek = magyar.**foetel**
 20. Magyar köretek = magyar.**koret**
 21. Magyar egytál ételek = magyar.**egytal**
+22. Magyar desszertek = magyar.**desszert**
+23. Magyar borok = magyar.**bor**
+24. Magyar üdítők= magyar.**utito**
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
 
 ## Description
-1. last names =  magyar.**vezeteknev**
-2. female first names = magyar.**keresztnev_n**
-3. male first names  = magyar.**keresztnev_f**
-4. street names = magyar.**utca**
-5. city names = magyar.**telepules**
-6. names of counties = magyar.**megye**
-7. names of rivers = magyar.**folyo**
+1. Last names =  magyar.**vezeteknev**
+2. Female first names = magyar.**keresztnev_n**
+3. Male first names  = magyar.**keresztnev_f**
+4. Street names = magyar.**utca**
+5. City names = magyar.**telepules**
+6. Names of counties = magyar.**megye**
+7. Names of rivers = magyar.**folyo**
 8. The days of the week = magyar.**nap**
-9. the months of the year = magyar.**honap**
-10. fruits = magyar.**gyumolcs**
-11. vegetables = magyar.**zoldseg**
-12. domesticated animals = magyar.**haszonallat**
-13. hungarian wildlife  = magyar.**vad**
+9. The months of the year = magyar.**honap**
+10. Fruits = magyar.**gyumolcs**
+11. Vegetables = magyar.**zoldseg**
+12. Domesticated animals = magyar.**haszonallat**
+13. Hungarian wildlife  = magyar.**vad**
 14. Fishes of Hungary = magyar.**hal**
 15. Birds of Hungary = magyar.**madar**
 16. Hungarian names of planets = magyar.**bolygo**
 17. Hungarian soup names = magyar.**leves**
-18. Hugarian given names M+F  magyar.**keresztnev_v**
+18. Hungarian given names M+F  magyar.**keresztnev_v**
 19. Hungarian main foods = magyar.**foetel**
 20. Hungarian side dishes  = magyar.**koret**
 21. Hungarian one-pot meals = magyar.**egytal**
+22. Hungarian sweet treats = magyar.**desszert**
+23. Hungarian wines =magyar.**bor**
+24. Hungarian soft drinks= magyar.**udito**
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
 4. Hungarian tram lines = magyar.villamos
 5. Hunngarian names of Europian capitals, states = magyar.orszag
@@ -122,19 +128,23 @@
 Gulyásleves, Halászlé, Hideg meggyleves, Zöldborsóleves, 
 Jókai bableves, Csontleves, Marhahúsleves, Zellerkrémleves, 
 Sárgaborsóleves, Babgulyásleves, Karalábéleves, Zöldségleves, 
 Kukoricaleves, Karfiolleves, Hideg gyümölcsleves, Korhelyleves, 
 Tyúkhúsleves, Pirított tarhonyaleves, Gombaleves, Lencseleves, 
 Gulyáskrémleves, Csülökleves, Paradicsomleves, Borleves, 
 
-3. Listák ABC sorrendbe rendezése  </br>
+3. Listák ABC sorrendbe rendezése, ékezet érzékeny </br>
 
 
-    magyar.abc(lista):
+         magyar.abc(lista):
 
+Használat : </br> </br>
+gyumolcs =['Áfonya', 'Eper', 'Alma', 'Meggy','Őszibarack',]
+sorban =magyar.abc(gyumolcs) </br>
+['Alma', 'Áfonya', 'Eper', 'Meggy', 'Őszibarack']
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
```

### Comparing `magyar-2.9.9/magyar.py` & `magyar-3.0.0/magyar.py`

 * *Files 6% similar despite different names*

```diff
@@ -154,37 +154,66 @@
            "Tarkabableves", "Hideg szilvaleves", "Fokhagymaleves", "Májgombócleves", "Brokkolileves",
            "Savanyú káposztaleves", "Erőleves", "Tejfölös gombaleves",  "Húsos káposztaleves", "Zöldspárga krémleves",
            "Sóska krémleves", "Burgonyapüréleves", "Laskaleves",  "Paradicsomleves húsgombóccal", "Csirkemájleves",
            "Ribizlileves", "Cukkinikrémleves", "Fokhagymás zöldbableves", "Zöldségleves tojással"]
 
 foetel= ['Vadörkölt', 'Sült csirke',
          'Sertésszelet', 'Rántott hús', 'Paprikás csirke', 'Sült kolbász', 'Rántott sajt', 'Rántott karfiol',
-         'Kacsacomb rántva', 'Kakaspörkölt',  'Sült hal', 'Túrós csusza', 'Gombapaprikás',
-         'Székelykáposzta', 'Marhapörkölt', 'Pacalpörkölt', 'Paprikás krumpli', 'Roston sült csirke',
-         'Rántott gomba', 'Rántott karaj', 'Rántott csirkemell', 'Rakott padlizsán', 'Halpaprikás', 'Libamáj',
+         'Kacsacomb rántva', 'Kakaspörkölt',  'Sült hal',  'Gombapaprikás',
+         'Marhapörkölt', 'Pacalpörkölt', 'Roston sült csirke',
+         'Rántott gomba', 'Rántott karaj', 'Rántott csirkemell', 'Halpaprikás', 'Libamáj',
          'Sült sertés', 'Halpaprikás', 'Csülök Pékné módra', 'Borjúpörkölt ',
-        'Párizsi csirkemell', 'Rántott karaj', 'Kacsapörkölt', 'Csirkepaprikás',  'Rántott csirkeszárny', 'Pacalpörkölt',
+         'Párizsi csirkemell', 'Rántott karaj', 'Kacsapörkölt', 'Csirkepaprikás',  'Rántott csirkeszárny', 'Pacalpörkölt',
          'Rántott jércemell', 'Sertéspörkölt','Mátrai borzaska',
-       'Grillezett csirkecomb', 'Lecsós csirke', 'Rántott gomba tartármártással', 'Rántott ponty', 'Lazacsteak', 'Roston sült hal',
-       'Rántott camembert', 'Sült kacsacomb', 'Sült libacomb', 'Sült pulykamell', 'Sült tarja', 'Báránytokány',
-       'Szűzérmék',  'Cordon bleu', 'Sült Kacsamáj',
-       'Kapros-túrós csusza', 'Lecsós tarja', 'Stefánia vagdalt']
+         'Grillezett csirkecomb', 'Lecsós csirke', 'Rántott gomba ', 'Rántott ponty', 'Lazacsteak', 'Roston sült hal',
+         'Rántott camembert', 'Sült kacsacomb', 'Sült libacomb', 'Sült pulykamell', 'Sült tarja', 'Báránytokány',
+         'Szűzérmék',  'Cordon bleu', 'Sült Kacsamáj',
+         'Lecsós tarja', 'Stefánia vagdalt']
 
-koret = ['Párolt rizs', 'Hagymás tört burgonya', 'Burgonyapüré', 'Tócsni', 'Párolt zöldségek', 'Hasábburgonya',
+koret = ['Párolt rizs', 'Hagymás tört burgonya', 'Burgonyapüré', 'Párolt zöldségek', 'Hasábburgonya',
            'Grillezett zöldségek', 'Köleskása', 'Galuska', 'Zöldségköret', 'Kukoricás rizs', 'Sárgarépa püré',
-            'Zöldségpüré',  'Burgonyakrokett', 'Kuszkusz', 'Brokkolipüré', 'Párolt sárgarépa', 'Zellerpüré',
-           'Tarhonya',  'Zöldborsós rizs', 'Sajtos tócsni', 'Gombás rizs', 'Gersli',  'Sült édesburgonya',
-           'Édesburgonya püré',  'Hercegnő burgonya', 'Csónak burgonya', 'Tepsis burgonya']
+            'Tarhonya',  'Burgonyakrokett', 'Kuszkusz', 'Brokkolipüré', 'Párolt sárgarépa',
+           'Tarhonya',  'Zöldborsós rizs', 'Gombás rizs', 'Gersli',  'Sült édesburgonya hasáb',
+           'Édesburgonya püré',  'Hercegnő burgonya', 'Csónak burgonya', 'Tepsis sült burgonya']
 
 egytal = ['Rakott krumpli', 'Töltött káposzta', 'Lecsó','Töltött paprika','Lencsefőzelék sültkolbásszal','Hortobágyi húsos palacsinta',
           'Sztrapacska szalonna pörccel','Burgonyás tészta','Csirkés rizottó','Rakott kelkáposzta csőben sütve',
-           'Rakott zöldbab', 'Disznótoros káposzta', 'Bácskai rizseshús', 'Brassói aprópecsenye','Tarhonyás hús',
-          'Székelykáposzta','Paradicsomos töltött káposzta','Rakott cukkini', 'Pásztortarhonya','Húsos-szaftos tészta',
+           'Rakott zöldbab', 'Disznótoros káposzta friss kenyérrel', 'Bácskai rizseshús', 'Brassói aprópecsenye','Tarhonyás hús',
+          'Székelykáposzta kenyérrel','Paradicsomos töltött káposzta','Rakott cukkini', 'Pásztortarhonya','Húsos-szaftos tészta',
           'Lecsó Mezőcsáti módra', 'Sonkás-paradicsomos tészta', 'Sajtos-sonkás rakott tészta', 'Kolozsvári rakott káposzta',
-          'Sonkás tészta csőben sütve']
+          'Sonkás tészta csőben sütve','Túrós csusza','Kapros-túrós csusza', 'Székelykáposzta','Paprikás krumpli', 'Rakott padlizsán' ]
+
+desszert = [
+    'Almás pite', 'Aranygaluska','Bejgli','Bodri torta','Boszorkányszigeti torta','Budapest roló', 'Császármorzsa',
+    'Csokoládé torta','Dobostorta','Diótorta', 'Esterházy torta','Fekete-erdő torta','Flódni','Gesztenyepüré torta',
+    'János vitéz tortája', 'Joghurt torta', 'Kakaós-meggyes pite', 'Képviselőfánk', 'Két színű torta',
+    'Kókuszos szelet', 'Krémes', 'Linzer', 'Mákos guba', 'Mákos kalács', 'Napóleon torta', 'Orosz krémtorta',
+    'Francia krémes', 'Puncsgolyó','Rakott palacsinta','Rákóczi túrós','Rigó Jancsi', 'Somlói galuska',
+    'Tiramisu','Répatorta']
+
+bor = ['Tokaji Furmint', 'Villányi Franc', 'Eger Bikavér', 'Szekszárdi Bikavér', 'Balatonboglári Kékfrankos',
+       'Badacsonyi Olaszrizling', 'Villányi Portugieser', 'Villányi Cabernet Franc', 'Egri Kékfrankos',
+       'Villányi Merlot', 'Etyeki Chardonnay', 'Somlói Juhfark', 'Tokaji Aszú', 'Mátrai Irsai Olivér',
+       'Villányi Cabernet Sauvignon', 'Balatonfüredi Szürkebarát', 'Soproni Kékfrankos', 'Szekszárdi Kadarka',
+       'Szekszárdi Merlot', 'Balatonlellei Olaszrizling', 'Badacsonyi Kéknyelű', 'Villányi Syrah',
+       'Somlói Furmint', 'Tokaji Szamorodni', 'Villányi Cuvée', 'Villányi Pinot Noir', 'Badacsonyi Kékfrankos',
+       'Mátrai Pinot Noir', 'Tokaji Hárslevelű', 'Villányi Kékfrankos', 'Somlói Traminer',
+       'Badacsonyi Muscat Ottonel', 'Villányi Kadarka', 'Mátrai Cabernet Sauvignon', 'Soproni Pinot Noir',
+       'Balatonfüredi Olaszrizling', 'Badacsonyi Szürkebarát', 'Tokaji Szamorodni Édes', 'Egri Leányka',
+       'Szekszárdi Cuvée', 'Villányi Kéknyelű', 'Egri Merlot', 'Somlói Olaszrizling',
+       'Badacsonyi Rizlingszilváni', 'Villányi Portugieser Rosé', 'Balatonboglári Zenit',
+       'Balatonlellei Riesling', 'Tokaji Szamorodni Száraz', 'Soproni Rosé']
+
+udito = ['Narancslé', 'Almalé', 'Tonik', 'Ásványvíz', 'Gyümölcslé', 'Szőlőlé',
+        'Bodza szörp', 'Cseresznyeszörp', 'Málnaszörp', 'Eper szörp',  'Zöld teás üdítő',
+        'Narancs ízű ásványvíz','Coca Cola', 'Fanta', 'Sprite', 'Jeges tea', 'Gyömbér',
+        'Bambi', 'Róna', 'Márka','Traubisoda','Olympos','Málna-gyöngye','Meggy-gyöngye',
+        'Sió gyümölcs nektár','Limonádé']
+
+
 
 kiraly = {'Árpád': (895, 907), 'Zoltán': (907, 947), 'Fajsz': (947, 955), 'Taksony': (955, 972), 'Géza': (972, 997),
     'I.István': (997, 1038),'I. Péter': (1038, 1041), 'Sámuel': (1041, 1044), 'Péter-2': (1044, 1045), 'I.András': (1041, 1060),
     'I. Béla': (1060, 1063), 'Salamon': (1063, 1074), 'I. Géza': (1074, 1077), 'I. László': (1077, 1095),
     'Kálmán': (1095, 1116),'II. István': (1116, 1131), 'II. Béla': (1131, 1141), 'II. Géza': (1141,1162),
     'III. István': (1162, 1172), 'III. Béla': (1172, 1196), 'Imre':(1196, 1204), 'III. László': (1204, 1205),
     'II. András': (1205, 1235),'IV. Béla': (1235, 1270), 'V. István': (1270, 1272), 'IV. László': (1272, 1290),
```

### Comparing `magyar-2.9.9/setup.py` & `magyar-3.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="2.9.9",
+    version="3.0.0",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
-    description="Hungarian names,animals,food, fruit, river ..",
+    description="Hungarian lists of names,animals,foods, fruits, rivers ..",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

