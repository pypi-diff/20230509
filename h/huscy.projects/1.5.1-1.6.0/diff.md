# Comparing `tmp/huscy.projects-1.5.1.tar.gz` & `tmp/huscy.projects-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.projects-1.5.1.tar", last modified: Mon Apr 17 12:33:44 2023, max compression
+gzip compressed data, was "huscy.projects-1.6.0.tar", last modified: Tue May  9 15:40:45 2023, max compression
```

## Comparing `huscy.projects-1.5.1.tar` & `huscy.projects-1.6.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 12:33:44.916421 huscy.projects-1.5.1/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3769 2023-04-17 12:33:44.916421 huscy.projects-1.5.1/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1991 2023-04-13 10:10:55.000000 huscy.projects-1.5.1/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 12:33:44.916421 huscy.projects-1.5.1/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 12:33:44.916421 huscy.projects-1.5.1/huscy/projects/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      154 2023-04-13 10:10:55.000000 huscy.projects-1.5.1/huscy/projects/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1727 2021-10-29 14:50:52.000000 huscy.projects-1.5.1/huscy/projects/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      527 2022-12-09 10:03:27.000000 huscy.projects-1.5.1/huscy/projects/api_urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      186 2022-06-23 09:54:31.000000 huscy.projects-1.5.1/huscy/projects/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 12:33:44.916421 huscy.projects-1.5.1/huscy/projects/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3042 2021-10-28 10:46:34.000000 huscy.projects-1.5.1/huscy/projects/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      369 2021-11-01 07:26:46.000000 huscy.projects-1.5.1/huscy/projects/migrations/0002_alter_membership_options.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-03-17 12:30:45.000000 huscy.projects-1.5.1/huscy/projects/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2823 2021-10-28 10:46:34.000000 huscy.projects-1.5.1/huscy/projects/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1764 2022-12-01 10:43:26.000000 huscy.projects-1.5.1/huscy/projects/permissions.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     4101 2022-03-15 12:22:45.000000 huscy.projects-1.5.1/huscy/projects/serializers.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3193 2023-04-13 10:10:55.000000 huscy.projects-1.5.1/huscy/projects/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      702 2022-12-09 10:03:27.000000 huscy.projects-1.5.1/huscy/projects/urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     5085 2022-12-01 10:43:26.000000 huscy.projects-1.5.1/huscy/projects/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-04-17 12:33:44.916421 huscy.projects-1.5.1/huscy.projects.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3769 2023-04-17 12:33:44.000000 huscy.projects-1.5.1/huscy.projects.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      606 2023-04-17 12:33:44.000000 huscy.projects-1.5.1/huscy.projects.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-04-17 12:33:44.000000 huscy.projects-1.5.1/huscy.projects.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)      164 2023-04-17 12:33:44.000000 huscy.projects-1.5.1/huscy.projects.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-04-17 12:33:44.000000 huscy.projects-1.5.1/huscy.projects.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-04-17 12:33:44.916421 huscy.projects-1.5.1/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1751 2023-04-17 11:26:50.000000 huscy.projects-1.5.1/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-09 15:40:45.082633 huscy.projects-1.6.0/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3769 2023-05-09 15:40:45.082633 huscy.projects-1.6.0/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1991 2023-04-13 10:10:55.000000 huscy.projects-1.6.0/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-09 15:40:45.078633 huscy.projects-1.6.0/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-09 15:40:45.082633 huscy.projects-1.6.0/huscy/projects/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      154 2023-05-09 14:31:59.000000 huscy.projects-1.6.0/huscy/projects/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1727 2021-10-29 14:50:52.000000 huscy.projects-1.6.0/huscy/projects/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      527 2022-12-09 10:03:27.000000 huscy.projects-1.6.0/huscy/projects/api_urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      186 2022-06-23 09:54:31.000000 huscy.projects-1.6.0/huscy/projects/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-09 15:40:45.082633 huscy.projects-1.6.0/huscy/projects/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3042 2021-10-28 10:46:34.000000 huscy.projects-1.6.0/huscy/projects/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      369 2021-11-01 07:26:46.000000 huscy.projects-1.6.0/huscy/projects/migrations/0002_alter_membership_options.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      893 2023-05-09 14:31:59.000000 huscy.projects-1.6.0/huscy/projects/migrations/0003_project_project_manager_and_more.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2020-03-17 12:30:45.000000 huscy.projects-1.6.0/huscy/projects/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3124 2023-05-09 14:31:59.000000 huscy.projects-1.6.0/huscy/projects/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1764 2022-12-01 10:43:26.000000 huscy.projects-1.6.0/huscy/projects/permissions.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     4756 2023-05-09 14:31:59.000000 huscy.projects-1.6.0/huscy/projects/serializers.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3537 2023-05-09 14:31:59.000000 huscy.projects-1.6.0/huscy/projects/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      702 2022-12-09 10:03:27.000000 huscy.projects-1.6.0/huscy/projects/urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     5633 2023-05-09 14:31:59.000000 huscy.projects-1.6.0/huscy/projects/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2023-05-09 15:40:45.082633 huscy.projects-1.6.0/huscy.projects.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3769 2023-05-09 15:40:44.000000 huscy.projects-1.6.0/huscy.projects.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      673 2023-05-09 15:40:44.000000 huscy.projects-1.6.0/huscy.projects.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2023-05-09 15:40:44.000000 huscy.projects-1.6.0/huscy.projects.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      164 2023-05-09 15:40:44.000000 huscy.projects-1.6.0/huscy.projects.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2023-05-09 15:40:44.000000 huscy.projects-1.6.0/huscy.projects.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2023-05-09 15:40:45.082633 huscy.projects-1.6.0/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1751 2023-04-17 11:26:50.000000 huscy.projects-1.6.0/setup.py
```

### Comparing `huscy.projects-1.5.1/PKG-INFO` & `huscy.projects-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.projects
-Version: 1.5.1
+Version: 1.6.0
 Summary: Managing projects in a research context.
 Home-page: https://bitbucket.org/huscy/projects/
 Author: Mathias Goldau, Stefan Bunde
 Author-email: goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.projects
```

### Comparing `huscy.projects-1.5.1/README.md` & `huscy.projects-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `huscy.projects-1.5.1/huscy/projects/admin.py` & `huscy.projects-1.6.0/huscy/projects/admin.py`

 * *Files identical despite different names*

### Comparing `huscy.projects-1.5.1/huscy/projects/api_urls.py` & `huscy.projects-1.6.0/huscy/projects/api_urls.py`

 * *Files identical despite different names*

### Comparing `huscy.projects-1.5.1/huscy/projects/migrations/0001_initial.py` & `huscy.projects-1.6.0/huscy/projects/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.projects-1.5.1/huscy/projects/models.py` & `huscy.projects-1.6.0/huscy/projects/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,15 +37,19 @@
                                       verbose_name=_('Research unit'))
     local_id = models.PositiveIntegerField(_('Local ID'))
 
     title = models.CharField(_('Title'), max_length=255)
     description = models.TextField(_('Description'), blank=True, default='')
 
     principal_investigator = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.PROTECT,
+                                               related_name='+',
                                                verbose_name=_('Principal investigator'))
+    project_manager = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.PROTECT,
+                                        related_name='+', null=True,
+                                        verbose_name=_('Project manager'))
 
     objects = ProjectManager()
 
     @property
     def local_id_name(self):
         return f'{self.research_unit.code}-{self.local_id}'
```

### Comparing `huscy.projects-1.5.1/huscy/projects/permissions.py` & `huscy.projects-1.6.0/huscy/projects/permissions.py`

 * *Files identical despite different names*

### Comparing `huscy.projects-1.5.1/huscy/projects/serializers.py` & `huscy.projects-1.6.0/huscy/projects/serializers.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from rest_framework.exceptions import ValidationError
 
 from huscy.projects.models import Membership, Project, ResearchUnit
 from huscy.projects.services import (
     create_membership,
     create_project,
     set_principal_investigator,
+    set_project_manager,
     update_membership,
     update_project,
 )
 
 
 class ResearchUnitSerializer(serializers.ModelSerializer):
     class Meta:
@@ -32,40 +33,58 @@
         principal_investigator = validated_data.get('principal_investigator')
         try:
             return set_principal_investigator(project=project, user=principal_investigator)
         except ValueError as e:
             raise ValidationError({'detail': e})
 
 
+class ProjectManagerSerializer(serializers.ModelSerializer):
+    class Meta:
+        model = Project
+        fields = 'project_manager',
+
+    def update(self, project, validated_data):
+        project_manager = validated_data.get('project_manager')
+        try:
+            return set_project_manager(project=project, user=project_manager)
+        except ValueError as e:
+            raise ValidationError({'detail': e})
+
+
 class ProjectSerializer(serializers.ModelSerializer):
 
     class Meta:
         model = Project
         fields = (
             'id',
             'description',
             'local_id',
             'local_id_name',
             'participating',
             'principal_investigator',
             'principal_investigator_name',
+            'project_manager',
+            'project_manager_name',
             'research_unit',
             'research_unit_name',
             'title',
         )
         extra_args = {
             'description': {'required': False},
             'local_id': {'required': False},
             'title': {'required': False},
         }
-        read_only_fields = 'principal_investigator', 'research_unit'
+        read_only_fields = 'principal_investigator', 'project_manager', 'research_unit'
 
     participating = serializers.SerializerMethodField()
     principal_investigator_name = serializers.CharField(
-        source='principal_investigator.get_full_name', read_only=True
+        source='principal_investigator.get_full_name', read_only=True,
+    )
+    project_manager_name = serializers.CharField(
+        source='project_manager.get_full_name', read_only=True,
     )
     research_unit_name = serializers.CharField(source='research_unit.name', read_only=True)
 
     # default=None is used as required=False does not work together with the unique_together
     # constraint, however this defaut=None is a workaround, see:
     # https://github.com/encode/django-rest-framework/issues/4456
     local_id = serializers.IntegerField(min_value=1, default=None)
```

### Comparing `huscy.projects-1.5.1/huscy/projects/services.py` & `huscy.projects-1.6.0/huscy/projects/services.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,23 @@
                          'principal investigators.')
 
     project.principal_investigator = user
     project.save(update_fields=['principal_investigator'])
     return project
 
 
+def set_project_manager(project, user):
+    if not Membership.objects.filter(project=project, user=user, is_coordinator=True).exists():
+        raise ValueError('Only project members who are coordinators can become project managers.')
+
+    project.project_manager = user
+    project.save(update_fields=['project_manager'])
+    return project
+
+
 def update_membership(membership, is_coordinator, has_write_permission):
     if is_coordinator or has_write_permission:
         assign_perm('change_project', membership.user, membership.project)
     else:
         remove_perm('change_project', membership.user, membership.project)
     membership.is_coordinator = is_coordinator
     membership.save()
```

### Comparing `huscy.projects-1.5.1/huscy/projects/urls.py` & `huscy.projects-1.6.0/huscy/projects/urls.py`

 * *Files identical despite different names*

### Comparing `huscy.projects-1.5.1/huscy/projects/views.py` & `huscy.projects-1.6.0/huscy/projects/views.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                     membership.user.get_full_name())
 
 
 class ProjectViewSet(RevisionMixin, viewsets.ModelViewSet):
     permission_classes = (IsAuthenticated, ProjectPermission)
 
     def initial(self, request, *args, **kwargs):
-        if self.action == 'principalinvestigator':
+        if self.action in ['principalinvestigator', 'projectmanager']:
             self.project = self.get_object()  # required for permission check in extra action
         super().initial(request, *args, **kwargs)
 
     def get_queryset(self):
         return services.get_projects()
 
     def get_serializer_class(self):
@@ -97,14 +97,24 @@
                                                                  data=request.data)
         serializer.is_valid(raise_exception=True)
         project = serializer.save()
 
         set_comment(f'Changed principal investigator for project <ID-{self.project.id}>')
         return Response(serializers.ProjectSerializer(project, context=dict(request=request)).data)
 
+    @action(detail=True, methods=['PUT'],
+            permission_classes=[UpdatePrincipalInvestigatorPermission])
+    def projectmanager(self, request, pk):
+        serializer = serializers.ProjectManagerSerializer(instance=self.project, data=request.data)
+        serializer.is_valid(raise_exception=True)
+        project = serializer.save()
+
+        set_comment(f'Changed project manager for project <ID-{self.project.id}>')
+        return Response(serializers.ProjectSerializer(project, context=dict(request=request)).data)
+
 
 class ResearchUnitViewSet(RevisionMixin, viewsets.ModelViewSet):
     permission_classes = (DjangoModelPermissions, )
     queryset = services.get_research_units()
     serializer_class = serializers.ResearchUnitSerializer
 
     def perform_create(self, serializer):
```

### Comparing `huscy.projects-1.5.1/huscy.projects.egg-info/PKG-INFO` & `huscy.projects-1.6.0/huscy.projects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.projects
-Version: 1.5.1
+Version: 1.6.0
 Summary: Managing projects in a research context.
 Home-page: https://bitbucket.org/huscy/projects/
 Author: Mathias Goldau, Stefan Bunde
 Author-email: goldau@cbs.mpg.de, stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.projects
```

### Comparing `huscy.projects-1.5.1/huscy.projects.egg-info/SOURCES.txt` & `huscy.projects-1.6.0/huscy.projects.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 huscy/projects/permissions.py
 huscy/projects/serializers.py
 huscy/projects/services.py
 huscy/projects/urls.py
 huscy/projects/views.py
 huscy/projects/migrations/0001_initial.py
 huscy/projects/migrations/0002_alter_membership_options.py
+huscy/projects/migrations/0003_project_project_manager_and_more.py
 huscy/projects/migrations/__init__.py
```

### Comparing `huscy.projects-1.5.1/setup.py` & `huscy.projects-1.6.0/setup.py`

 * *Files identical despite different names*

