# Comparing `tmp/com.castsoftware.uc.arg-1.5.4.tar.gz` & `tmp/com.castsoftware.uc.arg-1.5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.arg-1.5.4.tar", last modified: Thu Mar  9 18:54:03 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.arg-1.5.4.1.tar", last modified: Tue May  9 19:56:33 2023, max compression
```

## Comparing `com.castsoftware.uc.arg-1.5.4.tar` & `com.castsoftware.uc.arg-1.5.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 18:54:03.372586 com.castsoftware.uc.arg-1.5.4/
--rw-rw-rw-   0        0        0      589 2023-03-09 18:54:03.358871 com.castsoftware.uc.arg-1.5.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-09 18:54:03.257409 com.castsoftware.uc.arg-1.5.4/cast_arg/
--rw-rw-rw-   0        0        0     1429 2021-09-15 15:25:49.000000 com.castsoftware.uc.arg-1.5.4/cast_arg/Effort.csv
--rw-rw-rw-   0        0        0        0 2023-01-25 18:38:49.000000 com.castsoftware.uc.arg-1.5.4/cast_arg/__init__.py
--rw-rw-rw-   0        0        0     7714 2023-01-26 16:57:48.000000 com.castsoftware.uc.arg-1.5.4/cast_arg/actionPlan.py
--rw-rw-rw-   0        0        0     1004 2022-12-28 17:17:44.000000 com.castsoftware.uc.arg-1.5.4/cast_arg/cause.json
--rw-rw-rw-   0        0        0     6237 2023-01-25 16:41:12.000000 com.castsoftware.uc.arg-1.5.4/cast_arg/config.py
--rw-rw-rw-   0        0        0    32923 2023-03-07 15:35:56.000000 com.castsoftware.uc.arg-1.5.4/cast_arg/convert.py
--rw-rw-rw-   0        0        0      745 2023-02-14 14:23:07.000000 com.castsoftware.uc.arg-1.5.4/cast_arg/main.py
-drwxrwxrwx   0        0        0        0 2023-03-09 18:54:03.285667 com.castsoftware.uc.arg-1.5.4/cast_arg/pages/
--rw-rw-rw-   0        0        0        0 2023-03-07 13:55:37.000000 com.castsoftware.uc.arg-1.5.4/cast_arg/pages/__init__.py
--rw-rw-rw-   0        0        0       30 2023-03-07 15:35:56.000000 com.castsoftware.uc.arg-1.5.4/cast_arg/pages/aip.py
--rw-rw-rw-   0        0        0     1478 2023-03-07 15:35:56.000000 com.castsoftware.uc.arg-1.5.4/cast_arg/pages/green_it.py
--rw-rw-rw-   0        0        0    28453 2023-01-25 23:20:11.000000 com.castsoftware.uc.arg-1.5.4/cast_arg/powerpoint.py
--rw-rw-rw-   0        0        0    32985 2023-03-09 18:53:15.000000 com.castsoftware.uc.arg-1.5.4/cast_arg/restCall.py
--rw-rw-rw-   0        0        0     7182 2023-01-25 18:55:23.000000 com.castsoftware.uc.arg-1.5.4/cast_arg/stats.py
-drwxrwxrwx   0        0        0        0 2023-03-09 18:54:03.348795 com.castsoftware.uc.arg-1.5.4/com.castsoftware.uc.arg.egg-info/
--rw-rw-rw-   0        0        0      589 2023-03-09 18:54:03.000000 com.castsoftware.uc.arg-1.5.4/com.castsoftware.uc.arg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-03-09 18:54:03.000000 com.castsoftware.uc.arg-1.5.4/com.castsoftware.uc.arg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 18:54:03.000000 com.castsoftware.uc.arg-1.5.4/com.castsoftware.uc.arg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-03-09 18:54:03.000000 com.castsoftware.uc.arg-1.5.4/com.castsoftware.uc.arg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-09 18:54:03.000000 com.castsoftware.uc.arg-1.5.4/com.castsoftware.uc.arg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      645 2023-03-09 18:53:49.000000 com.castsoftware.uc.arg-1.5.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-09 18:54:03.372586 com.castsoftware.uc.arg-1.5.4/setup.cfg
--rw-rw-rw-   0        0        0      422 2023-01-26 17:04:17.000000 com.castsoftware.uc.arg-1.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:56:33.140768 com.castsoftware.uc.arg-1.5.4.1/
+-rw-rw-rw-   0        0        0      591 2023-05-09 19:56:33.126202 com.castsoftware.uc.arg-1.5.4.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-09 19:56:33.006492 com.castsoftware.uc.arg-1.5.4.1/cast_arg/
+-rw-rw-rw-   0        0        0     1429 2021-09-15 15:25:49.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/Effort.csv
+-rw-rw-rw-   0        0        0        0 2023-01-25 18:38:49.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/__init__.py
+-rw-rw-rw-   0        0        0     7714 2023-04-18 19:43:06.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/actionPlan.py
+-rw-rw-rw-   0        0        0     1004 2022-12-28 17:17:44.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/cause.json
+-rw-rw-rw-   0        0        0     6237 2023-01-25 16:41:12.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/config.py
+-rw-rw-rw-   0        0        0    33344 2023-04-19 15:23:24.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/convert.py
+-rw-rw-rw-   0        0        0      809 2023-04-19 12:46:04.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/main.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:56:33.040675 com.castsoftware.uc.arg-1.5.4.1/cast_arg/pages/
+-rw-rw-rw-   0        0        0        0 2023-03-07 13:55:37.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/pages/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-03-07 15:35:56.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/pages/aip.py
+-rw-rw-rw-   0        0        0     1478 2023-03-07 15:35:56.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/pages/green_it.py
+-rw-rw-rw-   0        0        0    28453 2023-01-25 23:20:11.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/powerpoint.py
+-rw-rw-rw-   0        0        0    33059 2023-04-19 19:19:12.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/restCall.py
+-rw-rw-rw-   0        0        0     7182 2023-01-25 18:55:23.000000 com.castsoftware.uc.arg-1.5.4.1/cast_arg/stats.py
+drwxrwxrwx   0        0        0        0 2023-05-09 19:56:33.111985 com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/
+-rw-rw-rw-   0        0        0      591 2023-05-09 19:56:32.000000 com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-05-09 19:56:32.000000 com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 19:56:32.000000 com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-05-09 19:56:32.000000 com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-09 19:56:32.000000 com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      647 2023-05-09 19:55:50.000000 com.castsoftware.uc.arg-1.5.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-09 19:56:33.140768 com.castsoftware.uc.arg-1.5.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      422 2023-01-26 17:04:17.000000 com.castsoftware.uc.arg-1.5.4.1/setup.py
```

### Comparing `com.castsoftware.uc.arg-1.5.4/PKG-INFO` & `com.castsoftware.uc.arg-1.5.4.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.arg
-Version: 1.5.4
+Version: 1.5.4.1
 Summary: Assessment Report Generator (ARG)
 Home-page: https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `com.castsoftware.uc.arg-1.5.4/cast_arg/Effort.csv` & `com.castsoftware.uc.arg-1.5.4.1/cast_arg/Effort.csv`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4/cast_arg/actionPlan.py` & `com.castsoftware.uc.arg-1.5.4.1/cast_arg/actionPlan.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,30 +71,30 @@
             col_widths=[50,40,10,10,10,50,10,10,10]
             summary_tab = format_table(writer,ap_summary_df[['Quality Rule','Business Criteria','No. of Actions','comment']],'Summary',col_widths)
             col_widths=[10,50,50,30,30,30,30,30,30,30,30,30,30]
             format_table(writer,ap_df,'Action Plan',col_widths)
             writer.close()
 
             #fill action plan related tags
-            self._fix_now = self.calc_action_plan_effort(ap_summary_df,app_no,'Extreme','security')
-            self._high = self.calc_action_plan_effort(ap_summary_df,app_no,'High')
-            self._med = self.calc_action_plan_effort(ap_summary_df,app_no,'Moderate')
-            self._low = self.calc_action_plan_effort(ap_summary_df,app_no,'Low')
+            self._fix_now = self.calc_action_plan_effort(ap_summary_df,app_no,'extreme','security')
+            self._high = self.calc_action_plan_effort(ap_summary_df,app_no,'high')
+            self._med = self.calc_action_plan_effort(ap_summary_df,app_no,'moderate')
+            self._low = self.calc_action_plan_effort(ap_summary_df,app_no,'low')
             
 
             #configure action plan table background colors 
-            ap_summary_df.loc[ap_summary_df['tag']=='Extreme','RGB']='244,212,212'
-            ap_summary_df.loc[ap_summary_df['tag']=='High','RGB']='255,229,194'
-            ap_summary_df.loc[ap_summary_df['tag']=='Moderate','RGB']='203,225,238'
-            ap_summary_df.loc[ap_summary_df['tag']=='Low','RGB']='254,254,255'
-
-            ap_table = pd.concat([ap_summary_df[ap_summary_df['tag']=='Extreme'],
-                                  ap_summary_df[ap_summary_df['tag']=='High'],
-                                  ap_summary_df[ap_summary_df['tag']=='Moderate'],
-                                  ap_summary_df[ap_summary_df['tag']=='Low']])
+            ap_summary_df.loc[ap_summary_df['tag']=='extreme','RGB']='244,212,212'
+            ap_summary_df.loc[ap_summary_df['tag']=='high','RGB']='255,229,194'
+            ap_summary_df.loc[ap_summary_df['tag']=='moderate','RGB']='203,225,238'
+            ap_summary_df.loc[ap_summary_df['tag']=='low','RGB']='254,254,255'
+
+            ap_table = pd.concat([ap_summary_df[ap_summary_df['tag']=='extreme'],
+                                  ap_summary_df[ap_summary_df['tag']=='high'],
+                                  ap_summary_df[ap_summary_df['tag']=='moderate'],
+                                  ap_summary_df[ap_summary_df['tag']=='low']])
 
             ap_table = ap_table.drop(columns=['comment','tag','Technical Criteria','Days Effort','Cost Est.','Eff Hours'])
 
             self._ppt.update_table(f'app{app_no}_action_plan',ap_table.head(29),include_index=False,background='RGB')
 
             sum = ap_summary_df['No. of Actions'].sum()
             self._ppt.replace_text(f"{{app{app_no}_total_violations}}",str(sum))
```

### Comparing `com.castsoftware.uc.arg-1.5.4/cast_arg/cause.json` & `com.castsoftware.uc.arg-1.5.4.1/cast_arg/cause.json`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4/cast_arg/config.py` & `com.castsoftware.uc.arg-1.5.4.1/cast_arg/config.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4/cast_arg/convert.py` & `com.castsoftware.uc.arg-1.5.4.1/cast_arg/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,21 +167,22 @@
                     self.info('Filling Technical details TABLE')
                     # Technical Overview - Technical details TABLE
                     grade_all = self._aip_data.get_app_grades(app_id)
                     #self._ppt.replace_risk_factor(grade_all,app_no)
                     grade_by_tech_df = self._aip_data.get_grade_by_tech(app_id)
                     grades = grade_by_tech_df.drop(['Documentation',"ISO","ISO_EFF","ISO_MAINT","ISO_REL","ISO_SEC"],axis=1)
                     self._ppt.update_table(f'app{app_no}_grade_by_tech_table',grades)
-                    
-                    #add appmarq technology
-                    self._ppt.replace_text(f'{{app{app_no}_largest_tech}}',grade_by_tech_df.index[0])
 
-                    self.info('Filling Technical Overview')
-                    # Technical Overview - Lines of code by technology GRAPH
-                    self._ppt.update_chart(f'app{app_no}_sizing_pie_chart',grade_by_tech_df['LOC'])
+                    if not grade_by_tech_df.empty:
+                        #add appmarq technology
+                        self._ppt.replace_text(f'{{app{app_no}_largest_tech}}',grade_by_tech_df.index[0])
+
+                        self.info('Filling Technical Overview')
+                        # Technical Overview - Lines of code by technology GRAPH
+                        self._ppt.update_chart(f'app{app_no}_sizing_pie_chart',grade_by_tech_df['LOC'])
 
                     snapshot = self._aip_data.snapshot(app=app_id)
                     # app_name = snapshot['name']
                     # self._ppt.replace_text(f'{{app{app_no}_name}}',app_name)
                     self._ppt.replace_text(f'{{app{app_no}_all_technogies}}',list_to_text(snapshot['technology']))
 
                     #calculate high and medium risk factors
@@ -209,46 +210,48 @@
                     doc_df.Score = doc_df.Score.map('{:.2f}'.format)
                     self._ppt.update_table(f'app{app_no}_doc_table',doc_df,include_index=False,background='RGB')
                     
 
 
                    
                     loc_df = self._aip_data.get_loc_sizing(app_id)
-                    loc = loc_df['Number of Code Lines']
-                    self._ppt.replace_loc(loc,app_no)
-
-                    loc_tbl = pd.DataFrame.from_dict(data=self._aip_data.get_loc_sizing(app_id),orient='index').drop('Critical Violations')
-                    loc_tbl = loc_tbl.rename(columns={0:'loc'})
-                    loc_tbl['percent'] = round((loc_tbl['loc'] / loc_tbl['loc'].sum()) * 100,2)
-                    loc_tbl['loc']=pd.Series(["{0:,.0f}".format(val) for val in loc_tbl['loc']], index = loc_tbl.index)
-
-                    percent_comment = loc_tbl.loc['Number of Comment Lines','percent']
-                    percent_comment_out = loc_tbl.loc['Number of Commented-out Code Lines','percent']
-
-                    if percent_comment < 15:
-                        comment_level='low'
-                    elif percent_comment > 15 and percent_comment <= 20:
-                        comment_level='good'
-                    else:
-                        comment_level='high'
-                    
-                    self._ppt.replace_text(f'{{app{app_no}_comment_hl}}',comment_level)
-                    self._ppt.replace_text(f'{{app{app_no}_comment_level}}',comment_level)
-                    self._ppt.replace_text(f'{{app{app_no}_comment_pct}}',percent_comment)
-                    self._ppt.replace_text(f'{{app{app_no}_comment_out_pct}}',percent_comment_out)
-
-                    loc_tbl['percent']=pd.Series(["{0:.2f}%".format(val) for val in loc_tbl['percent']], index = loc_tbl.index)
-                    self._ppt.update_table(f'app{app_no}_loc_table',loc_tbl,has_header=False)
-                    self._ppt.update_chart(f'app{app_no}_loc_pie_chart',loc_tbl['loc'])
-
-                    # self._ppt.replace_grade(grade_all,app_no)
-
-                    self.fill_sizing(app_id,app_no)
+                    if len(loc_df) > 0:
+                        loc = loc_df['Number of Code Lines']
+                        self._ppt.replace_loc(loc,app_no)
+
+                        loc_tbl = pd.DataFrame.from_dict(data=self._aip_data.get_loc_sizing(app_id),orient='index').drop('Critical Violations')
+                        loc_tbl = loc_tbl.rename(columns={0:'loc'})
+                        loc_tbl['percent'] = round((loc_tbl['loc'] / loc_tbl['loc'].sum()) * 100,2)
+                        loc_tbl['loc']=pd.Series(["{0:,.0f}".format(val) for val in loc_tbl['loc']], index = loc_tbl.index)
+
+                        percent_comment = loc_tbl.loc['Number of Comment Lines','percent']
+                        percent_comment_out = loc_tbl.loc['Number of Commented-out Code Lines','percent']
+
+                        if percent_comment < 15:
+                            comment_level='low'
+                        elif percent_comment > 15 and percent_comment <= 20:
+                            comment_level='good'
+                        else:
+                            comment_level='high'
+                    
+                        self._ppt.replace_text(f'{{app{app_no}_comment_hl}}',comment_level)
+                        self._ppt.replace_text(f'{{app{app_no}_comment_level}}',comment_level)
+                        self._ppt.replace_text(f'{{app{app_no}_comment_pct}}',percent_comment)
+                        self._ppt.replace_text(f'{{app{app_no}_comment_out_pct}}',percent_comment_out)
+
+                        loc_tbl['percent']=pd.Series(["{0:.2f}%".format(val) for val in loc_tbl['percent']], index = loc_tbl.index)
+                        self._ppt.update_table(f'app{app_no}_loc_table',loc_tbl,has_header=False)
+                        self._ppt.update_chart(f'app{app_no}_loc_pie_chart',loc_tbl['loc'])
+
+                        # self._ppt.replace_grade(grade_all,app_no)
+
+                        self.fill_sizing(app_id,app_no)
+                        self.fill_violations(app_id,app_no)
+    
                     self.fill_critical_rules(app_id,app_no)
-                    self.fill_violations(app_id,app_no)
 
                     """
                         Get Action Plan data and combine it for the various slide combinations
 
                         Executive Summary uses a combination of extreme and high violation data
                         Action Plan midigation slice is divided into three sections
                             1. Fix before sigining contains only extreme violation data
@@ -284,47 +287,49 @@
                     iso_df = self._aip_data.iso_rules(app_id)
                     if not iso_df.empty:
                         iso_df.loc[iso_df['violation']=='','background']='205,218,226'
                         iso_df.loc[iso_df['violation']!='','background']='255,255,255'
                         self._ppt.update_table(f'app{app_no}_iso5055',iso_df,
                                             include_index=False,background='background')
                                        
-                    pourcentage_iso5055 = iso_df["count"].sum()
-                    
-                    iso_Maintainaility = iso_df[iso_df.category == 'Maintainability' ]
-                    iso_MaintainailityCall = iso_Maintainaility["count"].sum()
-                    self._ppt.replace_text(f'{{app{app_no}_ISO_5055}}', round((iso_MaintainailityCall/(pourcentage_iso5055/2))*100,1))
+                        pourcentage_iso5055 = iso_df["count"].sum()
+                        
+                        iso_Maintainaility = iso_df[iso_df.category == 'Maintainability' ]
+                        iso_MaintainailityCall = iso_Maintainaility["count"].sum()
+                        self._ppt.replace_text(f'{{app{app_no}_ISO_5055}}', round((iso_MaintainailityCall/(pourcentage_iso5055/2))*100,1))
                     
             #replaceHighlight application specific data
             if self._config.hl_active and self._hl_data.has_data(hl_id):
-                (oss_crit,oss_high,oss_med,lic,components) = self.oss_risk_assessment(hl_id,app_no,day_rate)
-                fix_now_total.add_effort(oss_crit.effort)
-                fix_now_total.add_violations(oss_crit.violations)
-
-                near_term_total.add_effort(oss_high.effort)
-                near_term_total.add_effort(oss_med.effort)
-
-                hl_near_term_total.add_effort(oss_high.effort)
-                hl_near_term_total.add_effort(oss_med.effort)
-                hl_near_term_total.add_violations(oss_high.violations)
-                hl_near_term_total.add_violations(oss_med.violations)
-                hl_near_term_total.replace_text(self._ppt,app_no,'hl_near_term_total')
-
-                hl_summary_critical.add_components(oss_crit.components)
-                hl_summary_critical.add_violations(oss_crit.violations)
-
-                hl_summary_high_near.add_components(oss_high.components)
-                hl_summary_high_near.add_components(oss_med.components)
-
-                hl_summary.add_components(components)
-
-                lic_summary.add_high(lic.high)
-                lic_summary.add_medium(lic.medium)
-                lic_summary.add_low(lic.low)
-
+                try:
+                    (oss_crit,oss_high,oss_med,lic,components) = self.oss_risk_assessment(hl_id,app_no,day_rate)
+                    fix_now_total.add_effort(oss_crit.effort)
+                    fix_now_total.add_violations(oss_crit.violations)
+
+                    near_term_total.add_effort(oss_high.effort)
+                    near_term_total.add_effort(oss_med.effort)
+
+                    hl_near_term_total.add_effort(oss_high.effort)
+                    hl_near_term_total.add_effort(oss_med.effort)
+                    hl_near_term_total.add_violations(oss_high.violations)
+                    hl_near_term_total.add_violations(oss_med.violations)
+                    hl_near_term_total.replace_text(self._ppt,app_no,'hl_near_term_total')
+
+                    hl_summary_critical.add_components(oss_crit.components)
+                    hl_summary_critical.add_violations(oss_crit.violations)
+
+                    hl_summary_high_near.add_components(oss_high.components)
+                    hl_summary_high_near.add_components(oss_med.components)
+
+                    hl_summary.add_components(components)
+
+                    lic_summary.add_high(lic.high)
+                    lic_summary.add_medium(lic.medium)
+                    lic_summary.add_low(lic.low)
+                except KeyError as ex:
+                    self.warning(f'OSS information not found {str(ex)}')
                 """
                     Cloud ready excel sheet generation
                 """
                 try:
                     cloud = self._hl_data.get_cloud_info(hl_id)
                     cloud = cloud[['cloudRequirement.display','Technology','cloudRequirement.ruleType','cloudRequirement.criticality','contributionScore','roadblocks']]
                     file_name = f'{self._config.output}/cloud-{self._config.title_list[idx]}.xlsx'
```

### Comparing `com.castsoftware.uc.arg-1.5.4/cast_arg/main.py` & `com.castsoftware.uc.arg-1.5.4.1/cast_arg/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from argparse import ArgumentParser
 from cast_arg.convert import GeneratePPT
 from cast_arg.config import Config
+# from convert import GeneratePPT
+# from config import Config
 
 __author__ = "Nevin Kaplan"
 __email__ = "n.kaplan@castsoftware.com"
 __copyright__ = "Copyright 2023, CAST Software"
 
 if __name__ == '__main__':
     print('\nCAST Assessment Deck Generation Tool')
```

### Comparing `com.castsoftware.uc.arg-1.5.4/cast_arg/pages/green_it.py` & `com.castsoftware.uc.arg-1.5.4.1/cast_arg/pages/green_it.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4/cast_arg/powerpoint.py` & `com.castsoftware.uc.arg-1.5.4.1/cast_arg/powerpoint.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4/cast_arg/restCall.py` & `com.castsoftware.uc.arg-1.5.4.1/cast_arg/restCall.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,25 +354,26 @@
         grade_df = self.grades(app).round(2).applymap('{:,.2f}'.format)
         grade_df = self.grades(app).round(2)
         grade_df = grade_df[grade_df.index.isin(['All'])==False]
 
         sizing_df = DataFrame(self.sizing(app))
         sizing_df = sizing_df[sizing_df.index.isin(['All'])==False]
         sizing_df = DataFrame(sizing_df["Number of Code Lines"].rename("LOC")).dropna()
+        sizing_df.sort_values(by=['LOC'], ascending=False,inplace=True)
         sizing_df = sizing_df.applymap('{:,.0f}'.format)
         
         tech = sizing_df.join(grade_df) 
 
         sizing_df = DataFrame(self.sizing(app)) 
         sizing_df = sizing_df[sizing_df.index.isin(['All'])==False]
         sizing_df = DataFrame(sizing_df["Critical Violations"]).dropna()
         sizing_df = sizing_df.applymap('{:,.0f}'.format)
 
         tech = tech.join(sizing_df)
-        tech.sort_values(by='LOC',ascending=False,inplace=True)
+#        tech.sort_values(by='LOC',ascending=False,inplace=True)
 #        tech = tech.applymap('{:,.2f}'.format)
 
         
         return tech
 
     def get_high_risk_grade_text(self, grades):
         grade_at_risk=self.calc_health_grades_high_risk(grades)
```

### Comparing `com.castsoftware.uc.arg-1.5.4/cast_arg/stats.py` & `com.castsoftware.uc.arg-1.5.4.1/cast_arg/stats.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4/com.castsoftware.uc.arg.egg-info/PKG-INFO` & `com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.arg
-Version: 1.5.4
+Version: 1.5.4.1
 Summary: Assessment Report Generator (ARG)
 Home-page: https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `com.castsoftware.uc.arg-1.5.4/com.castsoftware.uc.arg.egg-info/SOURCES.txt` & `com.castsoftware.uc.arg-1.5.4.1/com.castsoftware.uc.arg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4/pyproject.toml` & `com.castsoftware.uc.arg-1.5.4.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name='com.castsoftware.uc.arg'
 description="Assessment Report Generator (ARG)"
-version='1.5.4' #prod version
+version='1.5.4.1' #prod version
 dependencies = ['pandas', 'python-pptx==0.6.18', 'com.castsoftware.uc.python.common>=0.1.6', 'IPython', 'requests', 'Jinja2']
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.6"
```

