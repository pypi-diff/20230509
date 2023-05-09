# Comparing `tmp/django-districts-2023.1.tar.gz` & `tmp/django-districts-2023.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-districts-2023.1.tar", last modified: Fri Apr 28 20:46:38 2023, max compression
+gzip compressed data, was "django-districts-2023.2.tar", last modified: Tue May  9 22:31:33 2023, max compression
```

## Comparing `django-districts-2023.1.tar` & `django-districts-2023.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 daniel    (1002) daniel    (1002)        0 2023-04-28 20:46:38.207898 django-districts-2023.1/
--rw-rw-r--   0 daniel    (1002) daniel    (1002)     1089 2023-04-28 18:25:41.000000 django-districts-2023.1/LICENSE
--rw-rw-r--   0 daniel    (1002) daniel    (1002)       77 2023-04-28 18:40:13.000000 django-districts-2023.1/MANIFEST.in
--rw-rw-r--   0 daniel    (1002) daniel    (1002)     1938 2023-04-28 20:46:38.207898 django-districts-2023.1/PKG-INFO
--rw-rw-r--   0 daniel    (1002) daniel    (1002)      933 2023-04-28 19:56:51.000000 django-districts-2023.1/README.md
--rw-rw-r--   0 daniel    (1002) daniel    (1002)     1033 2023-04-28 19:59:03.000000 django-districts-2023.1/README.rst
--rw-rw-r--   0 daniel    (1002) daniel    (1002)   112035 2023-04-28 16:35:03.000000 django-districts-2023.1/data.json
-drwxrwxr-x   0 daniel    (1002) daniel    (1002)        0 2023-04-28 20:46:38.203898 django-districts-2023.1/districts/
--rw-rw-r--   0 daniel    (1002) daniel    (1002)        0 2023-04-28 16:35:03.000000 django-districts-2023.1/districts/__init__.py
--rw-rw-r--   0 daniel    (1002) daniel    (1002)     1646 2023-04-28 16:35:03.000000 django-districts-2023.1/districts/admin.py
--rw-rw-r--   0 daniel    (1002) daniel    (1002)      150 2023-04-28 16:35:03.000000 django-districts-2023.1/districts/apps.py
-drwxrwxr-x   0 daniel    (1002) daniel    (1002)        0 2023-04-28 20:46:38.203898 django-districts-2023.1/districts/management/
--rw-rw-r--   0 daniel    (1002) daniel    (1002)        0 2023-04-28 16:35:03.000000 django-districts-2023.1/districts/management/__init__.py
-drwxrwxr-x   0 daniel    (1002) daniel    (1002)        0 2023-04-28 20:46:38.203898 django-districts-2023.1/districts/management/commands/
--rw-rw-r--   0 daniel    (1002) daniel    (1002)        0 2023-04-28 16:35:03.000000 django-districts-2023.1/districts/management/commands/__init__.py
--rw-rw-r--   0 daniel    (1002) daniel    (1002)      338 2023-04-28 16:35:03.000000 django-districts-2023.1/districts/management/commands/load_district_data.py
-drwxrwxr-x   0 daniel    (1002) daniel    (1002)        0 2023-04-28 20:46:38.203898 django-districts-2023.1/districts/migrations/
--rw-rw-r--   0 daniel    (1002) daniel    (1002)     4410 2023-04-28 16:35:03.000000 django-districts-2023.1/districts/migrations/0001_initial.py
--rw-rw-r--   0 daniel    (1002) daniel    (1002)        0 2023-04-28 16:35:03.000000 django-districts-2023.1/districts/migrations/__init__.py
--rw-rw-r--   0 daniel    (1002) daniel    (1002)     2653 2023-04-28 16:35:03.000000 django-districts-2023.1/districts/models.py
--rw-rw-r--   0 daniel    (1002) daniel    (1002)      987 2023-04-28 16:35:03.000000 django-districts-2023.1/districts/serializers.py
--rw-rw-r--   0 daniel    (1002) daniel    (1002)       60 2023-04-28 16:35:03.000000 django-districts-2023.1/districts/tests.py
--rw-rw-r--   0 daniel    (1002) daniel    (1002)      643 2023-04-28 16:35:03.000000 django-districts-2023.1/districts/urls.py
--rw-rw-r--   0 daniel    (1002) daniel    (1002)     7321 2023-04-28 16:35:03.000000 django-districts-2023.1/districts/views.py
-drwxrwxr-x   0 daniel    (1002) daniel    (1002)        0 2023-04-28 20:46:38.207898 django-districts-2023.1/django_districts.egg-info/
--rw-rw-r--   0 daniel    (1002) daniel    (1002)     1938 2023-04-28 20:46:38.000000 django-districts-2023.1/django_districts.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1002) daniel    (1002)      640 2023-04-28 20:46:38.000000 django-districts-2023.1/django_districts.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1002) daniel    (1002)        1 2023-04-28 20:46:38.000000 django-districts-2023.1/django_districts.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1002) daniel    (1002)       68 2023-04-28 20:46:38.000000 django-districts-2023.1/django_districts.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1002) daniel    (1002)       10 2023-04-28 20:46:38.000000 django-districts-2023.1/django_districts.egg-info/top_level.txt
--rw-rw-r--   0 daniel    (1002) daniel    (1002)       88 2023-04-28 20:43:37.000000 django-districts-2023.1/pyproject.toml
--rw-rw-r--   0 daniel    (1002) daniel    (1002)     1073 2023-04-28 20:46:38.207898 django-districts-2023.1/setup.cfg
--rw-rw-r--   0 daniel    (1002) daniel    (1002)       37 2023-04-28 18:30:23.000000 django-districts-2023.1/setup.py
+drwxrwxr-x   0 daniel    (1002) daniel    (1002)        0 2023-05-09 22:31:33.312095 django-districts-2023.2/
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)     1089 2023-04-28 18:25:41.000000 django-districts-2023.2/LICENSE
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)       77 2023-04-28 18:40:13.000000 django-districts-2023.2/MANIFEST.in
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)     1938 2023-05-09 22:31:33.312095 django-districts-2023.2/PKG-INFO
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)      933 2023-04-28 19:56:51.000000 django-districts-2023.2/README.md
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)     1033 2023-04-28 19:59:03.000000 django-districts-2023.2/README.rst
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)   112581 2023-05-09 22:26:39.000000 django-districts-2023.2/data.json
+drwxrwxr-x   0 daniel    (1002) daniel    (1002)        0 2023-05-09 22:31:33.312095 django-districts-2023.2/districts/
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)        0 2023-05-09 22:26:39.000000 django-districts-2023.2/districts/__init__.py
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)     1646 2023-05-09 22:26:39.000000 django-districts-2023.2/districts/admin.py
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)      150 2023-05-09 22:26:39.000000 django-districts-2023.2/districts/apps.py
+drwxrwxr-x   0 daniel    (1002) daniel    (1002)        0 2023-05-09 22:31:33.312095 django-districts-2023.2/districts/management/
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)        0 2023-05-09 22:26:39.000000 django-districts-2023.2/districts/management/__init__.py
+drwxrwxr-x   0 daniel    (1002) daniel    (1002)        0 2023-05-09 22:31:33.312095 django-districts-2023.2/districts/management/commands/
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)        0 2023-05-09 22:26:39.000000 django-districts-2023.2/districts/management/commands/__init__.py
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)      338 2023-05-09 22:26:39.000000 django-districts-2023.2/districts/management/commands/load_districts_data.py
+drwxrwxr-x   0 daniel    (1002) daniel    (1002)        0 2023-05-09 22:31:33.312095 django-districts-2023.2/districts/migrations/
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)     4465 2023-05-09 22:26:39.000000 django-districts-2023.2/districts/migrations/0001_initial.py
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)        0 2023-05-09 22:26:39.000000 django-districts-2023.2/districts/migrations/__init__.py
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)     2692 2023-05-09 22:26:39.000000 django-districts-2023.2/districts/models.py
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)     1964 2023-05-09 22:26:39.000000 django-districts-2023.2/districts/serializers.py
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)       60 2023-05-09 22:26:39.000000 django-districts-2023.2/districts/tests.py
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)      643 2023-05-09 22:26:39.000000 django-districts-2023.2/districts/urls.py
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)     9117 2023-05-09 22:26:39.000000 django-districts-2023.2/districts/views.py
+drwxrwxr-x   0 daniel    (1002) daniel    (1002)        0 2023-05-09 22:31:33.312095 django-districts-2023.2/django_districts.egg-info/
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)     1938 2023-05-09 22:31:33.000000 django-districts-2023.2/django_districts.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)      641 2023-05-09 22:31:33.000000 django-districts-2023.2/django_districts.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)        1 2023-05-09 22:31:33.000000 django-districts-2023.2/django_districts.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)       68 2023-05-09 22:31:33.000000 django-districts-2023.2/django_districts.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)       10 2023-05-09 22:31:33.000000 django-districts-2023.2/django_districts.egg-info/top_level.txt
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)       88 2023-04-28 20:43:37.000000 django-districts-2023.2/pyproject.toml
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)     1073 2023-05-09 22:31:33.312095 django-districts-2023.2/setup.cfg
+-rw-rw-r--   0 daniel    (1002) daniel    (1002)       37 2023-04-28 18:30:23.000000 django-districts-2023.2/setup.py
```

### Comparing `django-districts-2023.1/LICENSE` & `django-districts-2023.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-districts-2023.1/PKG-INFO` & `django-districts-2023.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-districts
-Version: 2023.1
+Version: 2023.2
 Summary: A Django app for managing districts in Africa.
 Home-page: https://www.example.com/
 Author: Ongom Daniel
 Author-email: ongomdaniel9@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-districts-2023.1/README.md` & `django-districts-2023.2/README.md`

 * *Files identical despite different names*

### Comparing `django-districts-2023.1/README.rst` & `django-districts-2023.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-districts-2023.1/data.json` & `django-districts-2023.2/data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986798679867988%*

 * *Differences: {'10': "{'fields': {'population': 241800}}",*

 * * '11': "{'fields': {'population': 2107500}}",*

 * * '12': "{'fields': {'population': 1529400}}",*

 * * '13': "{'fields': {'population': 610200}}",*

 * * '14': "{'fields': {'population': 465500}}",*

 * * '15': "{'fields': {'population': 186100}}",*

 * * '16': "{'fields': {'population': 202200}}",*

 * * '17': "{'fields': {'population': 429300}}",*

 * * '18': "{'fields': {'population': 373200}}",*

 * * '19': "{'fields': {'population': 333300}}",*

 * * '20': "{'fields': {'population': 225200}}",*

 * * '5': "{'fields […]*

```diff
@@ -44,164 +44,180 @@
         "model": "districts.regions",
         "pk": 4
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Jinja",
+            "population": 226800,
             "region": 1,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 1
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Mayuge",
+            "population": 484900,
             "region": 1,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 2
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Buyende",
+            "population": 334500,
             "region": 1,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 3
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Iganga",
+            "population": 347400,
             "region": 1,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 4
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Kamuli",
+            "population": 495600,
             "region": 1,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 5
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Luuka",
+            "population": 241800,
             "region": 1,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 6
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Kampala",
+            "population": 2107500,
             "region": 2,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 7
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Wakiso",
+            "population": 1529400,
             "region": 2,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 8
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Mukono",
+            "population": 610200,
             "region": 2,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 9
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Luwero",
+            "population": 465500,
             "region": 2,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 10
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Nakasongola",
+            "population": 186100,
             "region": 2,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 11
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Nakaseke",
+            "population": 202200,
             "region": 2,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 12
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Buikwe",
+            "population": 429300,
             "region": 2,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 13
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Kayunga",
+            "population": 373200,
             "region": 2,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 14
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Mityana",
+            "population": 333300,
             "region": 2,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 15
     },
     {
         "fields": {
             "created_at": "2023-04-26T13:13:00.000000Z",
             "district": "Mpigi",
+            "population": 225200,
             "region": 2,
             "updated_at": "2023-04-26T13:13:00.000000Z"
         },
         "model": "districts.districts",
         "pk": 16
     },
     {
```

### Comparing `django-districts-2023.1/districts/admin.py` & `django-districts-2023.2/districts/admin.py`

 * *Files identical despite different names*

### Comparing `django-districts-2023.1/districts/migrations/0001_initial.py` & `django-districts-2023.2/districts/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2 on 2023-04-28 16:21
+# Generated by Django 4.2 on 2023-05-09 22:20
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
@@ -83,14 +83,15 @@
         ),
         migrations.CreateModel(
             name='Districts',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created_at', models.DateTimeField(auto_now_add=True)),
                 ('district', models.CharField(max_length=50)),
+                ('population', models.IntegerField()),
                 ('updated_at', models.DateTimeField(auto_now=True)),
                 ('region', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='districts.regions')),
             ],
             options={
                 'verbose_name': 'District/City',
                 'verbose_name_plural': 'District/City',
             },
```

### Comparing `django-districts-2023.1/districts/models.py` & `django-districts-2023.2/districts/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 
 # Districts/City Model.
 class Districts(models.Model):
     created_at = models.DateTimeField(auto_now_add=True)
     region = models.ForeignKey(Regions, on_delete=models.CASCADE)
     district = models.CharField(max_length=50)
+    population = models.IntegerField()
     updated_at = models.DateTimeField(auto_now=True)
 
     def __str__(self):
         return self.district
     
     class Meta:
         verbose_name = "District/City"
```

### Comparing `django-districts-2023.1/districts/serializers.py` & `django-districts-2023.2/districts/serializers.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,34 +13,69 @@
 
 # Districts Serializer Class
 class Districts_Serializer(serializers.ModelSerializer):
     class Meta:
         model = Districts
         fields = '__all__'
 
+# Districts ListSerializer Class
+class Districts_ListSerializer(serializers.ModelSerializer):
+    region = serializers.SlugRelatedField(read_only=True, slug_field="region")
+    
+    class Meta:
+        model = Districts
+        fields = '__all__'
+
 
 # County Serializer Class
 class County_Serializer(serializers.ModelSerializer):
     class Meta:
         model = County
         fields = '__all__'
 
 
+# County ListSerializer Class
+class County_ListSerializer(serializers.ModelSerializer):
+    district = serializers.SlugRelatedField(read_only=True, slug_field="district")
+
+    class Meta:
+        model = County
+        fields = '__all__'
+
+
 # SubCounty Serializer Class
 class SubCounty_Serializer(serializers.ModelSerializer):
     class Meta:
         model = SubCounty
         fields = '__all__'
 
 
+# SubCounty ListSerializer Class
+class SubCounty_ListSerializer(serializers.ModelSerializer):
+    county = serializers.SlugRelatedField(read_only=True, slug_field="county")
+
+    class Meta:
+        model = SubCounty
+        fields = '__all__'
+
+
 # Parish Serializer Class
 class Parish_Serializer(serializers.ModelSerializer):
     class Meta:
         model = Parish
         fields = '__all__'
 
 
+# Parish ListSerializer Class
+class Parish_ListSerializer(serializers.ModelSerializer):
+    sub_county = serializers.SlugRelatedField(read_only=True, slug_field="sub_county")
+
+    class Meta:
+        model = Parish
+        fields = '__all__'
+
+
 # Location Serializer Class
 class Location_Serializer(serializers.ModelSerializer):
     class Meta:
         model = Location
         fields = '__all__'
```

### Comparing `django-districts-2023.1/districts/urls.py` & `django-districts-2023.2/districts/urls.py`

 * *Files identical despite different names*

### Comparing `django-districts-2023.1/django_districts.egg-info/PKG-INFO` & `django-districts-2023.2/django_districts.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-districts
-Version: 2023.1
+Version: 2023.2
 Summary: A Django app for managing districts in Africa.
 Home-page: https://www.example.com/
 Author: Ongom Daniel
 Author-email: ongomdaniel9@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-districts-2023.1/django_districts.egg-info/SOURCES.txt` & `django-districts-2023.2/django_districts.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 districts/models.py
 districts/serializers.py
 districts/tests.py
 districts/urls.py
 districts/views.py
 districts/management/__init__.py
 districts/management/commands/__init__.py
-districts/management/commands/load_district_data.py
+districts/management/commands/load_districts_data.py
 districts/migrations/0001_initial.py
 districts/migrations/__init__.py
 django_districts.egg-info/PKG-INFO
 django_districts.egg-info/SOURCES.txt
 django_districts.egg-info/dependency_links.txt
 django_districts.egg-info/requires.txt
 django_districts.egg-info/top_level.txt
```

### Comparing `django-districts-2023.1/setup.cfg` & `django-districts-2023.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-districts
-version = 2023.1
+version = 2023.2
 description = A Django app for managing districts in Africa.
 long_description = file: README.md
 long_description_content_type = text/markdown  # text/markdown | text/x-rst
 url = https://www.example.com/
 author = Ongom Daniel
 author_email = ongomdaniel9@gmail.com
 license = MIT License
```

