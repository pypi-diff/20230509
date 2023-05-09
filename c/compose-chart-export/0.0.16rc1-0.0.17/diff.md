# Comparing `tmp/compose_chart_export-0.0.16rc1-py3-none-any.whl.zip` & `tmp/compose_chart_export-0.0.17-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
 Zip file size: 13247 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-May-08 16:57 compose_chart_export/__init__.py
--rw-r--r--  2.0 unx     2534 b- defN 23-May-08 16:57 compose_chart_export/chart_export.py
--rw-r--r--  2.0 unx    14200 b- defN 23-May-08 16:57 compose_chart_export/chart_file_templates.py
--rw-r--r--  2.0 unx     4967 b- defN 23-May-08 16:57 compose_chart_export/chart_mods.py
--rw-r--r--  2.0 unx     2211 b- defN 23-May-08 16:57 compose_chart_export/chart_read.py
--rw-r--r--  2.0 unx     9543 b- defN 23-May-08 16:57 compose_chart_export/compose_export.py
--rw-r--r--  2.0 unx     2359 b- defN 23-May-08 16:57 compose_chart_export/ports.py
--rw-r--r--  2.0 unx      191 b- defN 23-May-08 16:57 compose_chart_export/settings.py
--rw-r--r--  2.0 unx      586 b- defN 23-May-08 16:57 compose_chart_export-0.0.16rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-08 16:57 compose_chart_export-0.0.16rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-08 16:57 compose_chart_export-0.0.16rc1.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       21 b- defN 23-May-08 16:57 compose_chart_export-0.0.16rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1214 b- defN 23-May-08 16:57 compose_chart_export-0.0.16rc1.dist-info/RECORD
-13 files, 37919 bytes uncompressed, 11161 bytes compressed:  70.6%
+-rw-r--r--  2.0 unx        0 b- defN 23-May-09 17:50 compose_chart_export/__init__.py
+-rw-r--r--  2.0 unx     2534 b- defN 23-May-09 17:50 compose_chart_export/chart_export.py
+-rw-r--r--  2.0 unx    14342 b- defN 23-May-09 17:50 compose_chart_export/chart_file_templates.py
+-rw-r--r--  2.0 unx     4967 b- defN 23-May-09 17:50 compose_chart_export/chart_mods.py
+-rw-r--r--  2.0 unx     2211 b- defN 23-May-09 17:50 compose_chart_export/chart_read.py
+-rw-r--r--  2.0 unx     9544 b- defN 23-May-09 17:50 compose_chart_export/compose_export.py
+-rw-r--r--  2.0 unx     2359 b- defN 23-May-09 17:50 compose_chart_export/ports.py
+-rw-r--r--  2.0 unx      191 b- defN 23-May-09 17:50 compose_chart_export/settings.py
+-rw-r--r--  2.0 unx      583 b- defN 23-May-09 17:50 compose_chart_export-0.0.17.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-09 17:50 compose_chart_export-0.0.17.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-09 17:50 compose_chart_export-0.0.17.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-May-09 17:50 compose_chart_export-0.0.17.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1199 b- defN 23-May-09 17:50 compose_chart_export-0.0.17.dist-info/RECORD
+13 files, 38044 bytes uncompressed, 11191 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: compose_chart_export/ports.py
 Comment: 
 
 Filename: compose_chart_export/settings.py
 Comment: 
 
-Filename: compose_chart_export-0.0.16rc1.dist-info/METADATA
+Filename: compose_chart_export-0.0.17.dist-info/METADATA
 Comment: 
 
-Filename: compose_chart_export-0.0.16rc1.dist-info/WHEEL
+Filename: compose_chart_export-0.0.17.dist-info/WHEEL
 Comment: 
 
-Filename: compose_chart_export-0.0.16rc1.dist-info/namespace_packages.txt
+Filename: compose_chart_export-0.0.17.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.16rc1.dist-info/top_level.txt
+Filename: compose_chart_export-0.0.17.dist-info/top_level.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.16rc1.dist-info/RECORD
+Filename: compose_chart_export-0.0.17.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## compose_chart_export/chart_file_templates.py

```diff
@@ -137,15 +137,18 @@
         return list(zip(self.containers, self.containers_values_names))
 
 
 def chart_yaml(spec: ChartTemplateSpec) -> str:
     return spec.replacements.replace(_CHART_YAML)
 
 
-_VALUES_YAML = """podLabels: {}
+_VALUES_YAML = """\
+app_kubernetes_io_name: ''
+app_kubernetes_io_instance: ''
+podLabels: {}
 podAnnotations: {}
 nodeSelector: {}
 replicas: 1"""
 
 _RESOURCES_YAML = """\
 resources:
   limits:
@@ -219,16 +222,16 @@
 app.kubernetes.io/name: {{ .Chart.Name }}
 app.kubernetes.io/version: {{ .Chart.AppVersion }}
 helm.sh/chart: {{ printf "%s-%s" .Chart.Name .Chart.Version | replace "+" "_" | trunc 63 | trimSuffix "-" }}
 EXTRA_LABELS
 {{- end -}}
 
 {{- define "common.labels.matchLabels" -}}
-app.kubernetes.io/name: {{ .Chart.Name }}
-app.kubernetes.io/instance: {{ .Release.Name }}
+app.kubernetes.io/name: {{ default .Chart.Name .Values.app_kubernetes_io_name }}
+app.kubernetes.io/instance: {{ default .Release.Name .Values.app_kubernetes_io_instance }}
 {{- end -}}
 """
 _service_account_tpl = """
 # Template from
 # https://github.com/influxdata/helm-charts/blob/master/charts/telegraf-ds/templates/_helpers.tpl#L400
 {{- define "APP_NAME.serviceAccountName" -}}
 {{- if .Values.serviceAccount.create -}}
```

## compose_chart_export/compose_export.py

```diff
@@ -75,14 +75,15 @@
 def parse_service_account_name(labels: dict[str, str]):
     return labels.get("chart_service_account_name", "")
 
 
 def parse_chart_name(labels: dict[str, str]) -> str:
     return labels.get("chart_name", "")
 
+
 class ExtraContainer(BaseModel):
     name: kubernetes_label_regex
     env: dict[str, str]
     command: list[str]
 
 
 def parse_service_name_extra_containers(
```

## Comparing `compose_chart_export-0.0.16rc1.dist-info/METADATA` & `compose_chart_export-0.0.17.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: compose-chart-export
-Version: 0.0.16rc1
+Version: 0.0.17
 Summary: compose_agent_export for docker-compose -> helm chart
 Author: Espen
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
-Requires-Dist: docker-compose-parser (==0.0.16)
-Requires-Dist: model-lib (==0.0.16)
+Requires-Dist: docker-compose-parser (==0.0.17)
+Requires-Dist: model-lib (==0.0.17)
 Requires-Dist: pydantic (>=1.10.2)
 Requires-Dist: semver (==2.13.0)
-Requires-Dist: zero-3rdparty (==0.0.16)
+Requires-Dist: zero-3rdparty (==0.0.17)
 
 # Compose Chart Export
 - Uses `docker-compose.yaml` to generate a helm chart
 - Supports various customizations using labels
```

## Comparing `compose_chart_export-0.0.16rc1.dist-info/RECORD` & `compose_chart_export-0.0.17.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 compose_chart_export/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 compose_chart_export/chart_export.py,sha256=oDgolV_QNeF12D2xh2D9xhn45IQSbKDMmj2WRZ2UTaI,2534
-compose_chart_export/chart_file_templates.py,sha256=bG35ma5Un9_18GpPiB5MYdKtvbZOQ-4zzEn7oCv0rSs,14200
+compose_chart_export/chart_file_templates.py,sha256=wTWip-U9Sy0EIy12b1A-c_wWJ7eRAwjXFPH8krLs__8,14342
 compose_chart_export/chart_mods.py,sha256=Zn-NSYhv7jJfUtGs6V--fquIolVqFT3bwL8mSWrwgOI,4967
 compose_chart_export/chart_read.py,sha256=chwkPcucA6dLWStADbP2kpAGNbhYVMms9zmPjNIQrLs,2211
-compose_chart_export/compose_export.py,sha256=w7MblSmri-sPAJd6yNjghJQw7WhAbCZJe0w1P2XM4G0,9543
+compose_chart_export/compose_export.py,sha256=bExlBsswEkLbbt21NGC0B5QEzPPX-VjN6L92gdmDnPM,9544
 compose_chart_export/ports.py,sha256=06WBSFYTUEPUYh9x4U5BjjUeE-EPNCs1Pot6MO7zxD4,2359
 compose_chart_export/settings.py,sha256=-vo5OY1ttQUeGQwihuX2YTD-qHRgvBdMuRwP_BelWQY,191
-compose_chart_export-0.0.16rc1.dist-info/METADATA,sha256=s4jS3b-jskSAUvfGfcpmagdMdiEkx4m7Y6FVfro1EhY,586
-compose_chart_export-0.0.16rc1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-compose_chart_export-0.0.16rc1.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-compose_chart_export-0.0.16rc1.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
-compose_chart_export-0.0.16rc1.dist-info/RECORD,,
+compose_chart_export-0.0.17.dist-info/METADATA,sha256=UYDPpYbLTOG6c-B6mdJVPh-nH0d9KDc8XVW4RjHGK-o,583
+compose_chart_export-0.0.17.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+compose_chart_export-0.0.17.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+compose_chart_export-0.0.17.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
+compose_chart_export-0.0.17.dist-info/RECORD,,
```

