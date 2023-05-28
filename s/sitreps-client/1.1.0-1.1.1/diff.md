# Comparing `tmp/sitreps_client-1.1.0-py2.py3-none-any.whl.zip` & `tmp/sitreps_client-1.1.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 21028 bytes, number of entries: 18
+Zip file size: 21305 bytes, number of entries: 18
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 sitreps_client/__init__.py
 -rw-r--r--  2.0 unx     5495 b- defN 20-Feb-02 00:00 sitreps_client/cloc.py
 -rw-r--r--  2.0 unx     4921 b- defN 20-Feb-02 00:00 sitreps_client/code_coverage.py
 -rw-r--r--  2.0 unx      425 b- defN 20-Feb-02 00:00 sitreps_client/exceptions.py
 -rw-r--r--  2.0 unx     3719 b- defN 20-Feb-02 00:00 sitreps_client/issues.py
 -rw-r--r--  2.0 unx     7634 b- defN 20-Feb-02 00:00 sitreps_client/project.py
--rw-r--r--  2.0 unx     2232 b- defN 20-Feb-02 00:00 sitreps_client/sonarqube.py
+-rw-r--r--  2.0 unx     3233 b- defN 20-Feb-02 00:00 sitreps_client/sonarqube.py
 -rw-r--r--  2.0 unx    17351 b- defN 20-Feb-02 00:00 sitreps_client/unit_tests.py
 -rw-r--r--  2.0 unx     2632 b- defN 20-Feb-02 00:00 sitreps_client/conf/config.py
 -rw-r--r--  2.0 unx     1712 b- defN 20-Feb-02 00:00 sitreps_client/conf/default_settings.yaml
 -rw-r--r--  2.0 unx     1525 b- defN 20-Feb-02 00:00 sitreps_client/utils/ci_downloader.py
 -rw-r--r--  2.0 unx     2576 b- defN 20-Feb-02 00:00 sitreps_client/utils/helpers.py
 -rw-r--r--  2.0 unx      162 b- defN 20-Feb-02 00:00 sitreps_client/utils/path.py
 -rw-r--r--  2.0 unx     3531 b- defN 20-Feb-02 00:00 sitreps_client/utils/repository.py
-?rw-r--r--  2.0 unx     1371 b- defN 20-Feb-02 00:00 sitreps_client-1.1.0.dist-info/METADATA
-?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 sitreps_client-1.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1071 b- defN 20-Feb-02 00:00 sitreps_client-1.1.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1537 b- defN 20-Feb-02 00:00 sitreps_client-1.1.0.dist-info/RECORD
-18 files, 57999 bytes uncompressed, 18498 bytes compressed:  68.1%
+?rw-r--r--  2.0 unx     1371 b- defN 20-Feb-02 00:00 sitreps_client-1.1.1.dist-info/METADATA
+?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 sitreps_client-1.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1071 b- defN 20-Feb-02 00:00 sitreps_client-1.1.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1537 b- defN 20-Feb-02 00:00 sitreps_client-1.1.1.dist-info/RECORD
+18 files, 59000 bytes uncompressed, 18775 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: sitreps_client/utils/path.py
 Comment: 
 
 Filename: sitreps_client/utils/repository.py
 Comment: 
 
-Filename: sitreps_client-1.1.0.dist-info/METADATA
+Filename: sitreps_client-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: sitreps_client-1.1.0.dist-info/WHEEL
+Filename: sitreps_client-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: sitreps_client-1.1.0.dist-info/licenses/LICENSE
+Filename: sitreps_client-1.1.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: sitreps_client-1.1.0.dist-info/RECORD
+Filename: sitreps_client-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sitreps_client/sonarqube.py

```diff
@@ -1,11 +1,12 @@
 import logging
 
 from cached_property import cached_property
 from sonarqube import SonarQubeClient
+from sonarqube.utils.exceptions import NotFoundError
 
 
 LOGGER = logging.getLogger(__name__)
 
 METRIC_KEYS = ["code_smells", "bugs", "vulnerabilities", "security_hotspots"]
 
 
@@ -57,16 +58,38 @@
         return {m["metric"]: int(m["value"]) for m in measures}
 
     def get_quality_gates_status(self):
         """Quality gate status."""
         data = self.client.qualitygates.get_project_qualitygates_status(projectKey=self.project_key)
         return data["projectStatus"]
 
+    def get_last_update_time(self):
+        """Collect last analysis time."""
+        try:
+            data = self.client.project_analyses.search_project_analyses_and_events(
+                project=self.project_key, branch=self.branch, ps=2
+            )
+        except NotFoundError as e:
+            msg = f"branch '{self.branch}' not found"
+            if msg in str(e):
+                LOGGER.warning(f"[SonarQube] {msg}. Collecting global event.")
+                data = self.client.project_analyses.search_project_analyses_and_events(
+                    project=self.project_key, ps=2
+                )
+        if data["analyses"]:
+            date = data["analyses"][0]["date"]
+            LOGGER.info(f"Last analysis {data['analyses'][0]['key']} time: {date}")
+            return date
+
 
 def get_sonar_metrics(project_key, host, token, branch):
     LOGGER.info(f"[SonarQube] Collecting metrics for {project_key}")
     sonar = SonarQubeProject(project_key=project_key, host=host, token=token, branch=branch)
-    return sonar.get_measures()
+    measures = sonar.get_measures()
+    last_update_time = sonar.get_last_update_time()
+    if measures:
+        measures["sonar_last_analysis"] = last_update_time
+    return measures
 
 
 if __name__ == "__main__":
     pass
```

## Comparing `sitreps_client-1.1.0.dist-info/METADATA` & `sitreps_client-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitreps-client
-Version: 1.1.0
+Version: 1.1.1
 Summary: A client help to collect different metrics.
 Project-URL: Source, https://github.com/digitronik/sitreps-client
 Maintainer-email: Nikhil Dhandare <ndhandre@redhat.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `sitreps_client-1.1.0.dist-info/licenses/LICENSE` & `sitreps_client-1.1.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `sitreps_client-1.1.0.dist-info/RECORD` & `sitreps_client-1.1.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 sitreps_client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sitreps_client/cloc.py,sha256=iN_4lw6q7py3oKvsxIS45l__wGBtsVnAAOdvVPnmByU,5495
 sitreps_client/code_coverage.py,sha256=kB3I1rgBwZqvQffJs8E3JlipXZWx50G5bLfM_oyEJns,4921
 sitreps_client/exceptions.py,sha256=ey9fBW9t8sckaWM6vFeU1sxQpVj4ohJFgQg3vI6rR58,425
 sitreps_client/issues.py,sha256=S6k_n82QWpIN0der5kpHYqFrZhTpgqk3a08dVG1DKQI,3719
 sitreps_client/project.py,sha256=5UupPEDBFNZFumRsZMD_JmTitY3BtPELHqSbzkC9J4Q,7634
-sitreps_client/sonarqube.py,sha256=_IG3lHnoEs94lTvxt28mMb1YORW_DKj7fjtDspJNAsc,2232
+sitreps_client/sonarqube.py,sha256=-iJTdu6tBNlOdULyOStk0XwUOxTkNZzz5JOgASXt9h0,3233
 sitreps_client/unit_tests.py,sha256=bqf9v6xi9tq7D6WuzBjNiS5AC9jryR0FlqEA6C8OHvc,17351
 sitreps_client/conf/config.py,sha256=NatSvY0sxWKdM1gOKJTblwQ964MTkI1thXbdznNWCr0,2632
 sitreps_client/conf/default_settings.yaml,sha256=AlRHe5awZRANMFBhePYtIC75u1ClYz2jnt-Y-rW0onc,1712
 sitreps_client/utils/ci_downloader.py,sha256=atzPrA-coOLrDvCyq9Ot4tbFbsdEB8FnMt5BlTrQ-Js,1525
 sitreps_client/utils/helpers.py,sha256=ayjxyyFFNI2tyKzsq1SlElyvsAZsZfstI10fqzfpyFk,2576
 sitreps_client/utils/path.py,sha256=eOwe26HwN_WYaw28Kae-ZYtHT5reb0l4nEfK5K6LVbk,162
 sitreps_client/utils/repository.py,sha256=E7XblcUkEN0X-WO0NOa9WAHxodqYpqGnG3NinQJ1H7Q,3531
-sitreps_client-1.1.0.dist-info/METADATA,sha256=MBPreFbvDp6hYAO5OF45c0BmaUwWsRqXKm5Hn9RhinM,1371
-sitreps_client-1.1.0.dist-info/WHEEL,sha256=nYNlZuHZ28ui1K118WE5qpb9yEZSMQ3u8pC2H4PftME,105
-sitreps_client-1.1.0.dist-info/licenses/LICENSE,sha256=O5tfZlESkbOf5s8Fbq8KW3MHGZgX5XCS6FT2ZQuOUbI,1071
-sitreps_client-1.1.0.dist-info/RECORD,,
+sitreps_client-1.1.1.dist-info/METADATA,sha256=115RDbrnhr1iPN_ZyKa940VQ9KoczXMtPLDZjZ4_QL4,1371
+sitreps_client-1.1.1.dist-info/WHEEL,sha256=BnTM96A0yHS39SE-waRX_LK6xllJtQJhpP4G4cCnPIA,105
+sitreps_client-1.1.1.dist-info/licenses/LICENSE,sha256=O5tfZlESkbOf5s8Fbq8KW3MHGZgX5XCS6FT2ZQuOUbI,1071
+sitreps_client-1.1.1.dist-info/RECORD,,
```

