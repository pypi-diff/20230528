# Comparing `tmp/lndb_storage-0.3.1.tar.gz` & `tmp/lndb_storage-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb_storage-0.3.1.tar", last modified: Sat May 27 16:11:15 2023, max compression
+gzip compressed data, was "lndb_storage-0.3.2.tar", last modified: Sun May 28 14:43:27 2023, max compression
```

## Comparing `lndb_storage-0.3.1.tar` & `lndb_storage-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     3181 2023-04-10 13:55:12.337864 lndb_storage-0.3.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-03-29 20:45:21.388328 lndb_storage-0.3.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-03-29 20:45:21.388401 lndb_storage-0.3.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2023-03-29 20:45:21.388463 lndb_storage-0.3.1/.gitignore
--rw-r--r--   0        0        0     1765 2023-04-24 16:53:24.500304 lndb_storage-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-03-29 20:45:21.388633 lndb_storage-0.3.1/LICENSE
--rw-r--r--   0        0        0      124 2023-03-29 20:45:21.388936 lndb_storage-0.3.1/README.md
--rw-r--r--   0        0        0     3430 2023-05-27 16:10:58.877632 lndb_storage-0.3.1/docs/changelog.md
--rw-r--r--   0        0        0     9684 2023-04-23 22:03:51.292643 lndb_storage-0.3.1/docs/guide/add-replace-stage.ipynb
--rw-r--r--   0        0        0       88 2023-04-09 22:14:23.875135 lndb_storage-0.3.1/docs/guide/index.md
--rw-r--r--   0        0        0     3976 2023-04-08 09:43:17.308905 lndb_storage-0.3.1/docs/guide/iris.csv
--rw-r--r--   0        0        0     4550 2023-04-08 09:43:17.309082 lndb_storage-0.3.1/docs/guide/iris.data
--rw-r--r--   0        0        0     4349 2023-04-23 22:03:51.292792 lndb_storage-0.3.1/docs/guide/new_iris.csv
--rw-r--r--   0        0        0     4615 2023-04-10 12:49:18.628116 lndb_storage-0.3.1/docs/guide/serialize-cache.ipynb
--rw-r--r--   0        0        0     5600 2023-05-27 16:08:47.046588 lndb_storage-0.3.1/docs/guide/stream.ipynb
--rw-r--r--   0        0        0     7566 2023-04-10 10:36:19.544617 lndb_storage-0.3.1/docs/guide/upload.ipynb
--rw-r--r--   0        0        0      122 2023-04-10 13:20:18.123402 lndb_storage-0.3.1/docs/index.md
--rw-r--r--   0        0        0       60 2023-04-09 20:42:44.949390 lndb_storage-0.3.1/docs/reference.md
--rw-r--r--   0        0        0      160 2023-03-29 20:45:21.390164 lndb_storage-0.3.1/lamin-project.yaml
--rw-r--r--   0        0        0      579 2023-05-27 16:10:40.280665 lndb_storage-0.3.1/lndb_storage/__init__.py
--rw-r--r--   0        0        0     3337 2023-04-18 11:35:08.919567 lndb_storage-0.3.1/lndb_storage/_file.py
--rw-r--r--   0        0        0      492 2023-04-16 20:58:33.198299 lndb_storage-0.3.1/lndb_storage/_h5ad.py
--rw-r--r--   0        0        0      204 2023-03-29 20:45:21.390606 lndb_storage-0.3.1/lndb_storage/_images.py
--rw-r--r--   0        0        0     2307 2023-03-29 20:45:21.390671 lndb_storage-0.3.1/lndb_storage/_subset.py
--rw-r--r--   0        0        0     2764 2023-04-09 20:42:44.950408 lndb_storage-0.3.1/lndb_storage/_zarr.py
--rw-r--r--   0        0        0      317 2023-03-29 20:45:21.390956 lndb_storage-0.3.1/lndb_storage/object/__init__.py
--rw-r--r--   0        0        0      945 2023-04-16 20:58:33.198732 lndb_storage-0.3.1/lndb_storage/object/_anndata.py
--rw-r--r--   0        0        0    11730 2023-05-27 16:08:47.046772 lndb_storage-0.3.1/lndb_storage/object/_anndata_accessor.py
--rw-r--r--   0        0        0      730 2023-03-29 20:45:21.391077 lndb_storage-0.3.1/lndb_storage/object/_anndata_sizes.py
--rw-r--r--   0        0        0      900 2023-03-29 20:45:21.391132 lndb_storage-0.3.1/lndb_storage/object/_core.py
--rw-r--r--   0        0        0     4116 2023-03-29 20:45:21.391201 lndb_storage-0.3.1/lndb_storage/object/_lazy_field.py
--rw-r--r--   0        0        0     3991 2023-05-27 16:08:47.047268 lndb_storage-0.3.1/lndb_storage/object/_subset_anndata.py
--rw-r--r--   0        0        0      933 2023-05-27 16:08:47.047494 lndb_storage-0.3.1/noxfile.py
--rw-r--r--   0        0        0     1108 2023-05-23 14:40:16.493381 lndb_storage-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      484 2023-05-23 14:40:16.493813 lndb_storage-0.3.1/tests/test_notebooks.py
--rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 lndb_storage-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3285 2023-05-28 10:46:30.904356 lndb_storage-0.3.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      135 2022-11-13 16:42:34.073467 lndb_storage-0.3.2/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      622 2022-11-13 16:42:34.079466 lndb_storage-0.3.2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1307 2022-11-13 16:42:34.087464 lndb_storage-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1829 2023-04-27 12:28:45.977838 lndb_storage-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11525 2022-11-13 16:42:34.107465 lndb_storage-0.3.2/LICENSE
+-rw-r--r--   0        0        0      127 2023-04-04 17:37:51.923635 lndb_storage-0.3.2/README.md
+-rw-r--r--   0        0        0     3759 2023-05-28 14:42:45.235025 lndb_storage-0.3.2/docs/changelog.md
+-rw-r--r--   0        0        0    10222 2023-04-23 18:25:59.426479 lndb_storage-0.3.2/docs/guide/add-replace-stage.ipynb
+-rw-r--r--   0        0        0       98 2023-04-10 13:07:42.667859 lndb_storage-0.3.2/docs/guide/index.md
+-rw-r--r--   0        0        0     4127 2023-04-04 17:37:51.986149 lndb_storage-0.3.2/docs/guide/iris.csv
+-rw-r--r--   0        0        0     4700 2023-04-04 17:37:52.017398 lndb_storage-0.3.2/docs/guide/iris.data
+-rw-r--r--   0        0        0     4500 2023-04-23 18:25:59.447479 lndb_storage-0.3.2/docs/guide/new_iris.csv
+-rw-r--r--   0        0        0     4853 2023-04-10 13:07:42.667859 lndb_storage-0.3.2/docs/guide/serialize-cache.ipynb
+-rw-r--r--   0        0        0     5889 2023-05-27 13:51:12.723290 lndb_storage-0.3.2/docs/guide/stream.ipynb
+-rw-r--r--   0        0        0     9234 2023-05-28 14:38:51.236000 lndb_storage-0.3.2/docs/guide/upload.ipynb
+-rw-r--r--   0        0        0      134 2023-04-10 13:07:42.721318 lndb_storage-0.3.2/docs/index.md
+-rw-r--r--   0        0        0       65 2023-04-10 13:07:42.721318 lndb_storage-0.3.2/docs/reference.md
+-rw-r--r--   0        0        0      165 2022-11-13 16:42:34.193462 lndb_storage-0.3.2/lamin-project.yaml
+-rw-r--r--   0        0        0      579 2023-05-28 14:42:45.955147 lndb_storage-0.3.2/lndb_storage/__init__.py
+-rw-r--r--   0        0        0     3450 2023-04-18 13:49:41.034991 lndb_storage-0.3.2/lndb_storage/_file.py
+-rw-r--r--   0        0        0      509 2023-04-16 14:26:59.906685 lndb_storage-0.3.2/lndb_storage/_h5ad.py
+-rw-r--r--   0        0        0      212 2023-03-13 18:04:48.685214 lndb_storage-0.3.2/lndb_storage/_images.py
+-rw-r--r--   0        0        0     2374 2023-03-26 12:52:12.411859 lndb_storage-0.3.2/lndb_storage/_subset.py
+-rw-r--r--   0        0        0     2851 2023-04-10 13:07:42.783828 lndb_storage-0.3.2/lndb_storage/_zarr.py
+-rw-r--r--   0        0        0      332 2023-03-26 12:52:12.411859 lndb_storage-0.3.2/lndb_storage/object/__init__.py
+-rw-r--r--   0        0        0      972 2023-04-16 14:26:59.906685 lndb_storage-0.3.2/lndb_storage/object/_anndata.py
+-rw-r--r--   0        0        0    12088 2023-05-27 13:51:12.746289 lndb_storage-0.3.2/lndb_storage/object/_anndata_accessor.py
+-rw-r--r--   0        0        0      761 2023-03-13 18:04:48.716390 lndb_storage-0.3.2/lndb_storage/object/_anndata_sizes.py
+-rw-r--r--   0        0        0      931 2023-03-14 18:15:14.187412 lndb_storage-0.3.2/lndb_storage/object/_core.py
+-rw-r--r--   0        0        0     4274 2023-03-13 18:04:48.716390 lndb_storage-0.3.2/lndb_storage/object/_lazy_field.py
+-rw-r--r--   0        0        0     4100 2023-05-27 13:51:12.758291 lndb_storage-0.3.2/lndb_storage/object/_subset_anndata.py
+-rw-r--r--   0        0        0      959 2023-05-27 13:51:12.769318 lndb_storage-0.3.2/noxfile.py
+-rw-r--r--   0        0        0     1140 2023-05-28 14:38:51.251649 lndb_storage-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      500 2023-05-07 12:55:11.415073 lndb_storage-0.3.2/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 lndb_storage-0.3.2/PKG-INFO
```

### Comparing `lndb_storage-0.3.1/LICENSE` & `lndb_storage-0.3.2/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `lndb_storage-0.3.1/docs/changelog.md` & `lndb_storage-0.3.2/docs/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+➖ Update fsspec and move s3 and gs dependencies to extras  | [38](https://github.com/laminlabs/lndb-storage/pull/38) | [Koncopd](https://github.com/Koncopd) | 2023-05-28 | 0.3.2
+:memo: Add content from lamindb | [36](https://github.com/laminlabs/lndb-storage/pull/36) | [falexwolf](https://github.com/falexwolf) | 2023-05-28 |
 ✨ `AnnDataAccessor` for access to cloud AnnData attributes | [32](https://github.com/laminlabs/lndb-storage/pull/32) | [Koncopd](https://github.com/Koncopd) | 2023-05-27 | 0.3.1
 ✅ Use nbproject-test directly in test_notebooks.py | [31](https://github.com/laminlabs/lndb-storage/pull/31) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 | 0.3.0
 ♻️ Refactor CloudAnnData | [29](https://github.com/laminlabs/lndb-storage/pull/29) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 |
 🦺 Check that obs and var are dataframes in subset | [28](https://github.com/laminlabs/lndb-storage/pull/28) | [Koncopd](https://github.com/Koncopd) | 2023-05-04 |
 ✨ Add `CloudAnnData` | [26](https://github.com/laminlabs/lndb-storage/pull/26) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 | 0.2rc6
 📝 Drastically simplify streaming guide | [25](https://github.com/laminlabs/lndb-storage/pull/25) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 |
 ✅ Add additional tests for replace | [24](https://github.com/laminlabs/lndb-storage/pull/24) | [Koncopd](https://github.com/Koncopd) | 2023-04-23 |
```

### Comparing `lndb_storage-0.3.1/docs/guide/iris.data` & `lndb_storage-0.3.2/docs/guide/iris.data`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-5.1,3.5,1.4,0.2,Iris-setosa
-4.9,3.0,1.4,0.2,Iris-setosa
-4.7,3.2,1.3,0.2,Iris-setosa
-4.6,3.1,1.5,0.2,Iris-setosa
-5.0,3.6,1.4,0.2,Iris-setosa
-5.4,3.9,1.7,0.4,Iris-setosa
-4.6,3.4,1.4,0.3,Iris-setosa
-5.0,3.4,1.5,0.2,Iris-setosa
-4.4,2.9,1.4,0.2,Iris-setosa
-4.9,3.1,1.5,0.1,Iris-setosa
-5.4,3.7,1.5,0.2,Iris-setosa
-4.8,3.4,1.6,0.2,Iris-setosa
-4.8,3.0,1.4,0.1,Iris-setosa
-4.3,3.0,1.1,0.1,Iris-setosa
-5.8,4.0,1.2,0.2,Iris-setosa
-5.7,4.4,1.5,0.4,Iris-setosa
-5.4,3.9,1.3,0.4,Iris-setosa
-5.1,3.5,1.4,0.3,Iris-setosa
-5.7,3.8,1.7,0.3,Iris-setosa
-5.1,3.8,1.5,0.3,Iris-setosa
-5.4,3.4,1.7,0.2,Iris-setosa
-5.1,3.7,1.5,0.4,Iris-setosa
-4.6,3.6,1.0,0.2,Iris-setosa
-5.1,3.3,1.7,0.5,Iris-setosa
-4.8,3.4,1.9,0.2,Iris-setosa
-5.0,3.0,1.6,0.2,Iris-setosa
-5.0,3.4,1.6,0.4,Iris-setosa
-5.2,3.5,1.5,0.2,Iris-setosa
-5.2,3.4,1.4,0.2,Iris-setosa
-4.7,3.2,1.6,0.2,Iris-setosa
-4.8,3.1,1.6,0.2,Iris-setosa
-5.4,3.4,1.5,0.4,Iris-setosa
-5.2,4.1,1.5,0.1,Iris-setosa
-5.5,4.2,1.4,0.2,Iris-setosa
-4.9,3.1,1.5,0.1,Iris-setosa
-5.0,3.2,1.2,0.2,Iris-setosa
-5.5,3.5,1.3,0.2,Iris-setosa
-4.9,3.1,1.5,0.1,Iris-setosa
-4.4,3.0,1.3,0.2,Iris-setosa
-5.1,3.4,1.5,0.2,Iris-setosa
-5.0,3.5,1.3,0.3,Iris-setosa
-4.5,2.3,1.3,0.3,Iris-setosa
-4.4,3.2,1.3,0.2,Iris-setosa
-5.0,3.5,1.6,0.6,Iris-setosa
-5.1,3.8,1.9,0.4,Iris-setosa
-4.8,3.0,1.4,0.3,Iris-setosa
-5.1,3.8,1.6,0.2,Iris-setosa
-4.6,3.2,1.4,0.2,Iris-setosa
-5.3,3.7,1.5,0.2,Iris-setosa
-5.0,3.3,1.4,0.2,Iris-setosa
-7.0,3.2,4.7,1.4,Iris-versicolor
-6.4,3.2,4.5,1.5,Iris-versicolor
-6.9,3.1,4.9,1.5,Iris-versicolor
-5.5,2.3,4.0,1.3,Iris-versicolor
-6.5,2.8,4.6,1.5,Iris-versicolor
-5.7,2.8,4.5,1.3,Iris-versicolor
-6.3,3.3,4.7,1.6,Iris-versicolor
-4.9,2.4,3.3,1.0,Iris-versicolor
-6.6,2.9,4.6,1.3,Iris-versicolor
-5.2,2.7,3.9,1.4,Iris-versicolor
-5.0,2.0,3.5,1.0,Iris-versicolor
-5.9,3.0,4.2,1.5,Iris-versicolor
-6.0,2.2,4.0,1.0,Iris-versicolor
-6.1,2.9,4.7,1.4,Iris-versicolor
-5.6,2.9,3.6,1.3,Iris-versicolor
-6.7,3.1,4.4,1.4,Iris-versicolor
-5.6,3.0,4.5,1.5,Iris-versicolor
-5.8,2.7,4.1,1.0,Iris-versicolor
-6.2,2.2,4.5,1.5,Iris-versicolor
-5.6,2.5,3.9,1.1,Iris-versicolor
-5.9,3.2,4.8,1.8,Iris-versicolor
-6.1,2.8,4.0,1.3,Iris-versicolor
-6.3,2.5,4.9,1.5,Iris-versicolor
-6.1,2.8,4.7,1.2,Iris-versicolor
-6.4,2.9,4.3,1.3,Iris-versicolor
-6.6,3.0,4.4,1.4,Iris-versicolor
-6.8,2.8,4.8,1.4,Iris-versicolor
-6.7,3.0,5.0,1.7,Iris-versicolor
-6.0,2.9,4.5,1.5,Iris-versicolor
-5.7,2.6,3.5,1.0,Iris-versicolor
-5.5,2.4,3.8,1.1,Iris-versicolor
-5.5,2.4,3.7,1.0,Iris-versicolor
-5.8,2.7,3.9,1.2,Iris-versicolor
-6.0,2.7,5.1,1.6,Iris-versicolor
-5.4,3.0,4.5,1.5,Iris-versicolor
-6.0,3.4,4.5,1.6,Iris-versicolor
-6.7,3.1,4.7,1.5,Iris-versicolor
-6.3,2.3,4.4,1.3,Iris-versicolor
-5.6,3.0,4.1,1.3,Iris-versicolor
-5.5,2.5,4.0,1.3,Iris-versicolor
-5.5,2.6,4.4,1.2,Iris-versicolor
-6.1,3.0,4.6,1.4,Iris-versicolor
-5.8,2.6,4.0,1.2,Iris-versicolor
-5.0,2.3,3.3,1.0,Iris-versicolor
-5.6,2.7,4.2,1.3,Iris-versicolor
-5.7,3.0,4.2,1.2,Iris-versicolor
-5.7,2.9,4.2,1.3,Iris-versicolor
-6.2,2.9,4.3,1.3,Iris-versicolor
-5.1,2.5,3.0,1.1,Iris-versicolor
-5.7,2.8,4.1,1.3,Iris-versicolor
-6.3,3.3,6.0,2.5,Iris-virginica
-5.8,2.7,5.1,1.9,Iris-virginica
-7.1,3.0,5.9,2.1,Iris-virginica
-6.3,2.9,5.6,1.8,Iris-virginica
-6.5,3.0,5.8,2.2,Iris-virginica
-7.6,3.0,6.6,2.1,Iris-virginica
-4.9,2.5,4.5,1.7,Iris-virginica
-7.3,2.9,6.3,1.8,Iris-virginica
-6.7,2.5,5.8,1.8,Iris-virginica
-7.2,3.6,6.1,2.5,Iris-virginica
-6.5,3.2,5.1,2.0,Iris-virginica
-6.4,2.7,5.3,1.9,Iris-virginica
-6.8,3.0,5.5,2.1,Iris-virginica
-5.7,2.5,5.0,2.0,Iris-virginica
-5.8,2.8,5.1,2.4,Iris-virginica
-6.4,3.2,5.3,2.3,Iris-virginica
-6.5,3.0,5.5,1.8,Iris-virginica
-7.7,3.8,6.7,2.2,Iris-virginica
-7.7,2.6,6.9,2.3,Iris-virginica
-6.0,2.2,5.0,1.5,Iris-virginica
-6.9,3.2,5.7,2.3,Iris-virginica
-5.6,2.8,4.9,2.0,Iris-virginica
-7.7,2.8,6.7,2.0,Iris-virginica
-6.3,2.7,4.9,1.8,Iris-virginica
-6.7,3.3,5.7,2.1,Iris-virginica
-7.2,3.2,6.0,1.8,Iris-virginica
-6.2,2.8,4.8,1.8,Iris-virginica
-6.1,3.0,4.9,1.8,Iris-virginica
-6.4,2.8,5.6,2.1,Iris-virginica
-7.2,3.0,5.8,1.6,Iris-virginica
-7.4,2.8,6.1,1.9,Iris-virginica
-7.9,3.8,6.4,2.0,Iris-virginica
-6.4,2.8,5.6,2.2,Iris-virginica
-6.3,2.8,5.1,1.5,Iris-virginica
-6.1,2.6,5.6,1.4,Iris-virginica
-7.7,3.0,6.1,2.3,Iris-virginica
-6.3,3.4,5.6,2.4,Iris-virginica
-6.4,3.1,5.5,1.8,Iris-virginica
-6.0,3.0,4.8,1.8,Iris-virginica
-6.9,3.1,5.4,2.1,Iris-virginica
-6.7,3.1,5.6,2.4,Iris-virginica
-6.9,3.1,5.1,2.3,Iris-virginica
-5.8,2.7,5.1,1.9,Iris-virginica
-6.8,3.2,5.9,2.3,Iris-virginica
-6.7,3.3,5.7,2.5,Iris-virginica
-6.7,3.0,5.2,2.3,Iris-virginica
-6.3,2.5,5.0,1.9,Iris-virginica
-6.5,3.0,5.2,2.0,Iris-virginica
-6.2,3.4,5.4,2.3,Iris-virginica
-5.9,3.0,5.1,1.8,Iris-virginica
+5.1,3.5,1.4,0.2,Iris-setosa
+4.9,3.0,1.4,0.2,Iris-setosa
+4.7,3.2,1.3,0.2,Iris-setosa
+4.6,3.1,1.5,0.2,Iris-setosa
+5.0,3.6,1.4,0.2,Iris-setosa
+5.4,3.9,1.7,0.4,Iris-setosa
+4.6,3.4,1.4,0.3,Iris-setosa
+5.0,3.4,1.5,0.2,Iris-setosa
+4.4,2.9,1.4,0.2,Iris-setosa
+4.9,3.1,1.5,0.1,Iris-setosa
+5.4,3.7,1.5,0.2,Iris-setosa
+4.8,3.4,1.6,0.2,Iris-setosa
+4.8,3.0,1.4,0.1,Iris-setosa
+4.3,3.0,1.1,0.1,Iris-setosa
+5.8,4.0,1.2,0.2,Iris-setosa
+5.7,4.4,1.5,0.4,Iris-setosa
+5.4,3.9,1.3,0.4,Iris-setosa
+5.1,3.5,1.4,0.3,Iris-setosa
+5.7,3.8,1.7,0.3,Iris-setosa
+5.1,3.8,1.5,0.3,Iris-setosa
+5.4,3.4,1.7,0.2,Iris-setosa
+5.1,3.7,1.5,0.4,Iris-setosa
+4.6,3.6,1.0,0.2,Iris-setosa
+5.1,3.3,1.7,0.5,Iris-setosa
+4.8,3.4,1.9,0.2,Iris-setosa
+5.0,3.0,1.6,0.2,Iris-setosa
+5.0,3.4,1.6,0.4,Iris-setosa
+5.2,3.5,1.5,0.2,Iris-setosa
+5.2,3.4,1.4,0.2,Iris-setosa
+4.7,3.2,1.6,0.2,Iris-setosa
+4.8,3.1,1.6,0.2,Iris-setosa
+5.4,3.4,1.5,0.4,Iris-setosa
+5.2,4.1,1.5,0.1,Iris-setosa
+5.5,4.2,1.4,0.2,Iris-setosa
+4.9,3.1,1.5,0.1,Iris-setosa
+5.0,3.2,1.2,0.2,Iris-setosa
+5.5,3.5,1.3,0.2,Iris-setosa
+4.9,3.1,1.5,0.1,Iris-setosa
+4.4,3.0,1.3,0.2,Iris-setosa
+5.1,3.4,1.5,0.2,Iris-setosa
+5.0,3.5,1.3,0.3,Iris-setosa
+4.5,2.3,1.3,0.3,Iris-setosa
+4.4,3.2,1.3,0.2,Iris-setosa
+5.0,3.5,1.6,0.6,Iris-setosa
+5.1,3.8,1.9,0.4,Iris-setosa
+4.8,3.0,1.4,0.3,Iris-setosa
+5.1,3.8,1.6,0.2,Iris-setosa
+4.6,3.2,1.4,0.2,Iris-setosa
+5.3,3.7,1.5,0.2,Iris-setosa
+5.0,3.3,1.4,0.2,Iris-setosa
+7.0,3.2,4.7,1.4,Iris-versicolor
+6.4,3.2,4.5,1.5,Iris-versicolor
+6.9,3.1,4.9,1.5,Iris-versicolor
+5.5,2.3,4.0,1.3,Iris-versicolor
+6.5,2.8,4.6,1.5,Iris-versicolor
+5.7,2.8,4.5,1.3,Iris-versicolor
+6.3,3.3,4.7,1.6,Iris-versicolor
+4.9,2.4,3.3,1.0,Iris-versicolor
+6.6,2.9,4.6,1.3,Iris-versicolor
+5.2,2.7,3.9,1.4,Iris-versicolor
+5.0,2.0,3.5,1.0,Iris-versicolor
+5.9,3.0,4.2,1.5,Iris-versicolor
+6.0,2.2,4.0,1.0,Iris-versicolor
+6.1,2.9,4.7,1.4,Iris-versicolor
+5.6,2.9,3.6,1.3,Iris-versicolor
+6.7,3.1,4.4,1.4,Iris-versicolor
+5.6,3.0,4.5,1.5,Iris-versicolor
+5.8,2.7,4.1,1.0,Iris-versicolor
+6.2,2.2,4.5,1.5,Iris-versicolor
+5.6,2.5,3.9,1.1,Iris-versicolor
+5.9,3.2,4.8,1.8,Iris-versicolor
+6.1,2.8,4.0,1.3,Iris-versicolor
+6.3,2.5,4.9,1.5,Iris-versicolor
+6.1,2.8,4.7,1.2,Iris-versicolor
+6.4,2.9,4.3,1.3,Iris-versicolor
+6.6,3.0,4.4,1.4,Iris-versicolor
+6.8,2.8,4.8,1.4,Iris-versicolor
+6.7,3.0,5.0,1.7,Iris-versicolor
+6.0,2.9,4.5,1.5,Iris-versicolor
+5.7,2.6,3.5,1.0,Iris-versicolor
+5.5,2.4,3.8,1.1,Iris-versicolor
+5.5,2.4,3.7,1.0,Iris-versicolor
+5.8,2.7,3.9,1.2,Iris-versicolor
+6.0,2.7,5.1,1.6,Iris-versicolor
+5.4,3.0,4.5,1.5,Iris-versicolor
+6.0,3.4,4.5,1.6,Iris-versicolor
+6.7,3.1,4.7,1.5,Iris-versicolor
+6.3,2.3,4.4,1.3,Iris-versicolor
+5.6,3.0,4.1,1.3,Iris-versicolor
+5.5,2.5,4.0,1.3,Iris-versicolor
+5.5,2.6,4.4,1.2,Iris-versicolor
+6.1,3.0,4.6,1.4,Iris-versicolor
+5.8,2.6,4.0,1.2,Iris-versicolor
+5.0,2.3,3.3,1.0,Iris-versicolor
+5.6,2.7,4.2,1.3,Iris-versicolor
+5.7,3.0,4.2,1.2,Iris-versicolor
+5.7,2.9,4.2,1.3,Iris-versicolor
+6.2,2.9,4.3,1.3,Iris-versicolor
+5.1,2.5,3.0,1.1,Iris-versicolor
+5.7,2.8,4.1,1.3,Iris-versicolor
+6.3,3.3,6.0,2.5,Iris-virginica
+5.8,2.7,5.1,1.9,Iris-virginica
+7.1,3.0,5.9,2.1,Iris-virginica
+6.3,2.9,5.6,1.8,Iris-virginica
+6.5,3.0,5.8,2.2,Iris-virginica
+7.6,3.0,6.6,2.1,Iris-virginica
+4.9,2.5,4.5,1.7,Iris-virginica
+7.3,2.9,6.3,1.8,Iris-virginica
+6.7,2.5,5.8,1.8,Iris-virginica
+7.2,3.6,6.1,2.5,Iris-virginica
+6.5,3.2,5.1,2.0,Iris-virginica
+6.4,2.7,5.3,1.9,Iris-virginica
+6.8,3.0,5.5,2.1,Iris-virginica
+5.7,2.5,5.0,2.0,Iris-virginica
+5.8,2.8,5.1,2.4,Iris-virginica
+6.4,3.2,5.3,2.3,Iris-virginica
+6.5,3.0,5.5,1.8,Iris-virginica
+7.7,3.8,6.7,2.2,Iris-virginica
+7.7,2.6,6.9,2.3,Iris-virginica
+6.0,2.2,5.0,1.5,Iris-virginica
+6.9,3.2,5.7,2.3,Iris-virginica
+5.6,2.8,4.9,2.0,Iris-virginica
+7.7,2.8,6.7,2.0,Iris-virginica
+6.3,2.7,4.9,1.8,Iris-virginica
+6.7,3.3,5.7,2.1,Iris-virginica
+7.2,3.2,6.0,1.8,Iris-virginica
+6.2,2.8,4.8,1.8,Iris-virginica
+6.1,3.0,4.9,1.8,Iris-virginica
+6.4,2.8,5.6,2.1,Iris-virginica
+7.2,3.0,5.8,1.6,Iris-virginica
+7.4,2.8,6.1,1.9,Iris-virginica
+7.9,3.8,6.4,2.0,Iris-virginica
+6.4,2.8,5.6,2.2,Iris-virginica
+6.3,2.8,5.1,1.5,Iris-virginica
+6.1,2.6,5.6,1.4,Iris-virginica
+7.7,3.0,6.1,2.3,Iris-virginica
+6.3,3.4,5.6,2.4,Iris-virginica
+6.4,3.1,5.5,1.8,Iris-virginica
+6.0,3.0,4.8,1.8,Iris-virginica
+6.9,3.1,5.4,2.1,Iris-virginica
+6.7,3.1,5.6,2.4,Iris-virginica
+6.9,3.1,5.1,2.3,Iris-virginica
+5.8,2.7,5.1,1.9,Iris-virginica
+6.8,3.2,5.9,2.3,Iris-virginica
+6.7,3.3,5.7,2.5,Iris-virginica
+6.7,3.0,5.2,2.3,Iris-virginica
+6.3,2.5,5.0,1.9,Iris-virginica
+6.5,3.0,5.2,2.0,Iris-virginica
+6.2,3.4,5.4,2.3,Iris-virginica
+5.9,3.0,5.1,1.8,Iris-virginica
```

### Comparing `lndb_storage-0.3.1/docs/guide/new_iris.csv` & `lndb_storage-0.3.2/docs/guide/new_iris.csv`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-;sepal.length;sepal.width;petal.length;petal.width;variety
-0;5.1;3.5;1.4;0.2;Setosa
-1;4.9;3.0;1.4;0.2;Setosa
-2;4.7;3.2;1.3;0.2;Setosa
-3;4.6;3.1;1.5;0.2;Setosa
-4;5.0;3.6;1.4;0.2;Setosa
-5;5.4;3.9;1.7;0.4;Setosa
-6;4.6;3.4;1.4;0.3;Setosa
-7;5.0;3.4;1.5;0.2;Setosa
-8;4.4;2.9;1.4;0.2;Setosa
-9;4.9;3.1;1.5;0.1;Setosa
-10;5.4;3.7;1.5;0.2;Setosa
-11;4.8;3.4;1.6;0.2;Setosa
-12;4.8;3.0;1.4;0.1;Setosa
-13;4.3;3.0;1.1;0.1;Setosa
-14;5.8;4.0;1.2;0.2;Setosa
-15;5.7;4.4;1.5;0.4;Setosa
-16;5.4;3.9;1.3;0.4;Setosa
-17;5.1;3.5;1.4;0.3;Setosa
-18;5.7;3.8;1.7;0.3;Setosa
-19;5.1;3.8;1.5;0.3;Setosa
-20;5.4;3.4;1.7;0.2;Setosa
-21;5.1;3.7;1.5;0.4;Setosa
-22;4.6;3.6;1.0;0.2;Setosa
-23;5.1;3.3;1.7;0.5;Setosa
-24;4.8;3.4;1.9;0.2;Setosa
-25;5.0;3.0;1.6;0.2;Setosa
-26;5.0;3.4;1.6;0.4;Setosa
-27;5.2;3.5;1.5;0.2;Setosa
-28;5.2;3.4;1.4;0.2;Setosa
-29;4.7;3.2;1.6;0.2;Setosa
-30;4.8;3.1;1.6;0.2;Setosa
-31;5.4;3.4;1.5;0.4;Setosa
-32;5.2;4.1;1.5;0.1;Setosa
-33;5.5;4.2;1.4;0.2;Setosa
-34;4.9;3.1;1.5;0.2;Setosa
-35;5.0;3.2;1.2;0.2;Setosa
-36;5.5;3.5;1.3;0.2;Setosa
-37;4.9;3.6;1.4;0.1;Setosa
-38;4.4;3.0;1.3;0.2;Setosa
-39;5.1;3.4;1.5;0.2;Setosa
-40;5.0;3.5;1.3;0.3;Setosa
-41;4.5;2.3;1.3;0.3;Setosa
-42;4.4;3.2;1.3;0.2;Setosa
-43;5.0;3.5;1.6;0.6;Setosa
-44;5.1;3.8;1.9;0.4;Setosa
-45;4.8;3.0;1.4;0.3;Setosa
-46;5.1;3.8;1.6;0.2;Setosa
-47;4.6;3.2;1.4;0.2;Setosa
-48;5.3;3.7;1.5;0.2;Setosa
-49;5.0;3.3;1.4;0.2;Setosa
-50;7.0;3.2;4.7;1.4;Versicolor
-51;6.4;3.2;4.5;1.5;Versicolor
-52;6.9;3.1;4.9;1.5;Versicolor
-53;5.5;2.3;4.0;1.3;Versicolor
-54;6.5;2.8;4.6;1.5;Versicolor
-55;5.7;2.8;4.5;1.3;Versicolor
-56;6.3;3.3;4.7;1.6;Versicolor
-57;4.9;2.4;3.3;1.0;Versicolor
-58;6.6;2.9;4.6;1.3;Versicolor
-59;5.2;2.7;3.9;1.4;Versicolor
-60;5.0;2.0;3.5;1.0;Versicolor
-61;5.9;3.0;4.2;1.5;Versicolor
-62;6.0;2.2;4.0;1.0;Versicolor
-63;6.1;2.9;4.7;1.4;Versicolor
-64;5.6;2.9;3.6;1.3;Versicolor
-65;6.7;3.1;4.4;1.4;Versicolor
-66;5.6;3.0;4.5;1.5;Versicolor
-67;5.8;2.7;4.1;1.0;Versicolor
-68;6.2;2.2;4.5;1.5;Versicolor
-69;5.6;2.5;3.9;1.1;Versicolor
-70;5.9;3.2;4.8;1.8;Versicolor
-71;6.1;2.8;4.0;1.3;Versicolor
-72;6.3;2.5;4.9;1.5;Versicolor
-73;6.1;2.8;4.7;1.2;Versicolor
-74;6.4;2.9;4.3;1.3;Versicolor
-75;6.6;3.0;4.4;1.4;Versicolor
-76;6.8;2.8;4.8;1.4;Versicolor
-77;6.7;3.0;5.0;1.7;Versicolor
-78;6.0;2.9;4.5;1.5;Versicolor
-79;5.7;2.6;3.5;1.0;Versicolor
-80;5.5;2.4;3.8;1.1;Versicolor
-81;5.5;2.4;3.7;1.0;Versicolor
-82;5.8;2.7;3.9;1.2;Versicolor
-83;6.0;2.7;5.1;1.6;Versicolor
-84;5.4;3.0;4.5;1.5;Versicolor
-85;6.0;3.4;4.5;1.6;Versicolor
-86;6.7;3.1;4.7;1.5;Versicolor
-87;6.3;2.3;4.4;1.3;Versicolor
-88;5.6;3.0;4.1;1.3;Versicolor
-89;5.5;2.5;4.0;1.3;Versicolor
-90;5.5;2.6;4.4;1.2;Versicolor
-91;6.1;3.0;4.6;1.4;Versicolor
-92;5.8;2.6;4.0;1.2;Versicolor
-93;5.0;2.3;3.3;1.0;Versicolor
-94;5.6;2.7;4.2;1.3;Versicolor
-95;5.7;3.0;4.2;1.2;Versicolor
-96;5.7;2.9;4.2;1.3;Versicolor
-97;6.2;2.9;4.3;1.3;Versicolor
-98;5.1;2.5;3.0;1.1;Versicolor
-99;5.7;2.8;4.1;1.3;Versicolor
-100;6.3;3.3;6.0;2.5;Virginica
-101;5.8;2.7;5.1;1.9;Virginica
-102;7.1;3.0;5.9;2.1;Virginica
-103;6.3;2.9;5.6;1.8;Virginica
-104;6.5;3.0;5.8;2.2;Virginica
-105;7.6;3.0;6.6;2.1;Virginica
-106;4.9;2.5;4.5;1.7;Virginica
-107;7.3;2.9;6.3;1.8;Virginica
-108;6.7;2.5;5.8;1.8;Virginica
-109;7.2;3.6;6.1;2.5;Virginica
-110;6.5;3.2;5.1;2.0;Virginica
-111;6.4;2.7;5.3;1.9;Virginica
-112;6.8;3.0;5.5;2.1;Virginica
-113;5.7;2.5;5.0;2.0;Virginica
-114;5.8;2.8;5.1;2.4;Virginica
-115;6.4;3.2;5.3;2.3;Virginica
-116;6.5;3.0;5.5;1.8;Virginica
-117;7.7;3.8;6.7;2.2;Virginica
-118;7.7;2.6;6.9;2.3;Virginica
-119;6.0;2.2;5.0;1.5;Virginica
-120;6.9;3.2;5.7;2.3;Virginica
-121;5.6;2.8;4.9;2.0;Virginica
-122;7.7;2.8;6.7;2.0;Virginica
-123;6.3;2.7;4.9;1.8;Virginica
-124;6.7;3.3;5.7;2.1;Virginica
-125;7.2;3.2;6.0;1.8;Virginica
-126;6.2;2.8;4.8;1.8;Virginica
-127;6.1;3.0;4.9;1.8;Virginica
-128;6.4;2.8;5.6;2.1;Virginica
-129;7.2;3.0;5.8;1.6;Virginica
-130;7.4;2.8;6.1;1.9;Virginica
-131;7.9;3.8;6.4;2.0;Virginica
-132;6.4;2.8;5.6;2.2;Virginica
-133;6.3;2.8;5.1;1.5;Virginica
-134;6.1;2.6;5.6;1.4;Virginica
-135;7.7;3.0;6.1;2.3;Virginica
-136;6.3;3.4;5.6;2.4;Virginica
-137;6.4;3.1;5.5;1.8;Virginica
-138;6.0;3.0;4.8;1.8;Virginica
-139;6.9;3.1;5.4;2.1;Virginica
-140;6.7;3.1;5.6;2.4;Virginica
-141;6.9;3.1;5.1;2.3;Virginica
-142;5.8;2.7;5.1;1.9;Virginica
-143;6.8;3.2;5.9;2.3;Virginica
-144;6.7;3.3;5.7;2.5;Virginica
-145;6.7;3.0;5.2;2.3;Virginica
-146;6.3;2.5;5.0;1.9;Virginica
-147;6.5;3.0;5.2;2.0;Virginica
-148;6.2;3.4;5.4;2.3;Virginica
-149;5.9;3.0;5.1;1.8;Virginica
+;sepal.length;sepal.width;petal.length;petal.width;variety
+0;5.1;3.5;1.4;0.2;Setosa
+1;4.9;3.0;1.4;0.2;Setosa
+2;4.7;3.2;1.3;0.2;Setosa
+3;4.6;3.1;1.5;0.2;Setosa
+4;5.0;3.6;1.4;0.2;Setosa
+5;5.4;3.9;1.7;0.4;Setosa
+6;4.6;3.4;1.4;0.3;Setosa
+7;5.0;3.4;1.5;0.2;Setosa
+8;4.4;2.9;1.4;0.2;Setosa
+9;4.9;3.1;1.5;0.1;Setosa
+10;5.4;3.7;1.5;0.2;Setosa
+11;4.8;3.4;1.6;0.2;Setosa
+12;4.8;3.0;1.4;0.1;Setosa
+13;4.3;3.0;1.1;0.1;Setosa
+14;5.8;4.0;1.2;0.2;Setosa
+15;5.7;4.4;1.5;0.4;Setosa
+16;5.4;3.9;1.3;0.4;Setosa
+17;5.1;3.5;1.4;0.3;Setosa
+18;5.7;3.8;1.7;0.3;Setosa
+19;5.1;3.8;1.5;0.3;Setosa
+20;5.4;3.4;1.7;0.2;Setosa
+21;5.1;3.7;1.5;0.4;Setosa
+22;4.6;3.6;1.0;0.2;Setosa
+23;5.1;3.3;1.7;0.5;Setosa
+24;4.8;3.4;1.9;0.2;Setosa
+25;5.0;3.0;1.6;0.2;Setosa
+26;5.0;3.4;1.6;0.4;Setosa
+27;5.2;3.5;1.5;0.2;Setosa
+28;5.2;3.4;1.4;0.2;Setosa
+29;4.7;3.2;1.6;0.2;Setosa
+30;4.8;3.1;1.6;0.2;Setosa
+31;5.4;3.4;1.5;0.4;Setosa
+32;5.2;4.1;1.5;0.1;Setosa
+33;5.5;4.2;1.4;0.2;Setosa
+34;4.9;3.1;1.5;0.2;Setosa
+35;5.0;3.2;1.2;0.2;Setosa
+36;5.5;3.5;1.3;0.2;Setosa
+37;4.9;3.6;1.4;0.1;Setosa
+38;4.4;3.0;1.3;0.2;Setosa
+39;5.1;3.4;1.5;0.2;Setosa
+40;5.0;3.5;1.3;0.3;Setosa
+41;4.5;2.3;1.3;0.3;Setosa
+42;4.4;3.2;1.3;0.2;Setosa
+43;5.0;3.5;1.6;0.6;Setosa
+44;5.1;3.8;1.9;0.4;Setosa
+45;4.8;3.0;1.4;0.3;Setosa
+46;5.1;3.8;1.6;0.2;Setosa
+47;4.6;3.2;1.4;0.2;Setosa
+48;5.3;3.7;1.5;0.2;Setosa
+49;5.0;3.3;1.4;0.2;Setosa
+50;7.0;3.2;4.7;1.4;Versicolor
+51;6.4;3.2;4.5;1.5;Versicolor
+52;6.9;3.1;4.9;1.5;Versicolor
+53;5.5;2.3;4.0;1.3;Versicolor
+54;6.5;2.8;4.6;1.5;Versicolor
+55;5.7;2.8;4.5;1.3;Versicolor
+56;6.3;3.3;4.7;1.6;Versicolor
+57;4.9;2.4;3.3;1.0;Versicolor
+58;6.6;2.9;4.6;1.3;Versicolor
+59;5.2;2.7;3.9;1.4;Versicolor
+60;5.0;2.0;3.5;1.0;Versicolor
+61;5.9;3.0;4.2;1.5;Versicolor
+62;6.0;2.2;4.0;1.0;Versicolor
+63;6.1;2.9;4.7;1.4;Versicolor
+64;5.6;2.9;3.6;1.3;Versicolor
+65;6.7;3.1;4.4;1.4;Versicolor
+66;5.6;3.0;4.5;1.5;Versicolor
+67;5.8;2.7;4.1;1.0;Versicolor
+68;6.2;2.2;4.5;1.5;Versicolor
+69;5.6;2.5;3.9;1.1;Versicolor
+70;5.9;3.2;4.8;1.8;Versicolor
+71;6.1;2.8;4.0;1.3;Versicolor
+72;6.3;2.5;4.9;1.5;Versicolor
+73;6.1;2.8;4.7;1.2;Versicolor
+74;6.4;2.9;4.3;1.3;Versicolor
+75;6.6;3.0;4.4;1.4;Versicolor
+76;6.8;2.8;4.8;1.4;Versicolor
+77;6.7;3.0;5.0;1.7;Versicolor
+78;6.0;2.9;4.5;1.5;Versicolor
+79;5.7;2.6;3.5;1.0;Versicolor
+80;5.5;2.4;3.8;1.1;Versicolor
+81;5.5;2.4;3.7;1.0;Versicolor
+82;5.8;2.7;3.9;1.2;Versicolor
+83;6.0;2.7;5.1;1.6;Versicolor
+84;5.4;3.0;4.5;1.5;Versicolor
+85;6.0;3.4;4.5;1.6;Versicolor
+86;6.7;3.1;4.7;1.5;Versicolor
+87;6.3;2.3;4.4;1.3;Versicolor
+88;5.6;3.0;4.1;1.3;Versicolor
+89;5.5;2.5;4.0;1.3;Versicolor
+90;5.5;2.6;4.4;1.2;Versicolor
+91;6.1;3.0;4.6;1.4;Versicolor
+92;5.8;2.6;4.0;1.2;Versicolor
+93;5.0;2.3;3.3;1.0;Versicolor
+94;5.6;2.7;4.2;1.3;Versicolor
+95;5.7;3.0;4.2;1.2;Versicolor
+96;5.7;2.9;4.2;1.3;Versicolor
+97;6.2;2.9;4.3;1.3;Versicolor
+98;5.1;2.5;3.0;1.1;Versicolor
+99;5.7;2.8;4.1;1.3;Versicolor
+100;6.3;3.3;6.0;2.5;Virginica
+101;5.8;2.7;5.1;1.9;Virginica
+102;7.1;3.0;5.9;2.1;Virginica
+103;6.3;2.9;5.6;1.8;Virginica
+104;6.5;3.0;5.8;2.2;Virginica
+105;7.6;3.0;6.6;2.1;Virginica
+106;4.9;2.5;4.5;1.7;Virginica
+107;7.3;2.9;6.3;1.8;Virginica
+108;6.7;2.5;5.8;1.8;Virginica
+109;7.2;3.6;6.1;2.5;Virginica
+110;6.5;3.2;5.1;2.0;Virginica
+111;6.4;2.7;5.3;1.9;Virginica
+112;6.8;3.0;5.5;2.1;Virginica
+113;5.7;2.5;5.0;2.0;Virginica
+114;5.8;2.8;5.1;2.4;Virginica
+115;6.4;3.2;5.3;2.3;Virginica
+116;6.5;3.0;5.5;1.8;Virginica
+117;7.7;3.8;6.7;2.2;Virginica
+118;7.7;2.6;6.9;2.3;Virginica
+119;6.0;2.2;5.0;1.5;Virginica
+120;6.9;3.2;5.7;2.3;Virginica
+121;5.6;2.8;4.9;2.0;Virginica
+122;7.7;2.8;6.7;2.0;Virginica
+123;6.3;2.7;4.9;1.8;Virginica
+124;6.7;3.3;5.7;2.1;Virginica
+125;7.2;3.2;6.0;1.8;Virginica
+126;6.2;2.8;4.8;1.8;Virginica
+127;6.1;3.0;4.9;1.8;Virginica
+128;6.4;2.8;5.6;2.1;Virginica
+129;7.2;3.0;5.8;1.6;Virginica
+130;7.4;2.8;6.1;1.9;Virginica
+131;7.9;3.8;6.4;2.0;Virginica
+132;6.4;2.8;5.6;2.2;Virginica
+133;6.3;2.8;5.1;1.5;Virginica
+134;6.1;2.6;5.6;1.4;Virginica
+135;7.7;3.0;6.1;2.3;Virginica
+136;6.3;3.4;5.6;2.4;Virginica
+137;6.4;3.1;5.5;1.8;Virginica
+138;6.0;3.0;4.8;1.8;Virginica
+139;6.9;3.1;5.4;2.1;Virginica
+140;6.7;3.1;5.6;2.4;Virginica
+141;6.9;3.1;5.1;2.3;Virginica
+142;5.8;2.7;5.1;1.9;Virginica
+143;6.8;3.2;5.9;2.3;Virginica
+144;6.7;3.3;5.7;2.5;Virginica
+145;6.7;3.0;5.2;2.3;Virginica
+146;6.3;2.5;5.0;1.9;Virginica
+147;6.5;3.0;5.2;2.0;Virginica
+148;6.2;3.4;5.4;2.3;Virginica
+149;5.9;3.0;5.1;1.8;Virginica
```

### Comparing `lndb_storage-0.3.1/lndb_storage/__init__.py` & `lndb_storage-0.3.2/lndb_storage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
    :toctree: .
 
    store_object
    store_png
    delete_storage
 """
 
-__version__ = "0.3.1"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.3.2"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 from lndb.dev.upath import UPath
 from lndb.dev.upath import infer_filesystem as _infer_filesystem
 
 from ._file import delete_storage, load_to_memory, store_object
 from ._h5ad import h5ad_to_anndata
 from ._images import store_png
```

### Comparing `lndb_storage-0.3.1/lndb_storage/_file.py` & `lndb_storage-0.3.2/lndb_storage/_file.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-import os
-import shutil
-from pathlib import Path
-from typing import Union
-
-import fsspec
-import pandas as pd
-import readfcs
-from lndb import settings
-from lndb.dev.upath import UPath
-
-from ._h5ad import read_adata_h5ad
-from ._zarr import read_adata_zarr
-
-READER_FUNCS = {
-    ".csv": pd.read_csv,
-    ".h5ad": read_adata_h5ad,
-    ".parquet": pd.read_parquet,
-    ".fcs": readfcs.read,
-    ".zarr": read_adata_zarr,
-}
-
-
-def print_hook(size, value, **kwargs):
-    progress = value / size
-    out = f"... uploading {Path(kwargs['filepath']).name}: {min(progress, 1.):4.2f}"
-    if progress >= 1:
-        out += "\n"
-    if "NBPRJ_TEST_NBPATH" not in os.environ:
-        print(out, end="\r")
-
-
-class ProgressCallback(fsspec.callbacks.Callback):
-    def branch(self, path_1, path_2, kwargs):
-        kwargs["callback"] = fsspec.callbacks.Callback(
-            hooks=dict(print_hook=print_hook), filepath=path_1
-        )
-
-    def call(self, *args, **kwargs):
-        return None
-
-
-def store_object(localpath: Union[str, Path], storagekey: str) -> float:
-    """Store arbitrary file to configured storage location.
-
-    Returns size in bytes.
-    """
-    storagepath = settings.instance.storage.key_to_filepath(storagekey)
-    localpath = Path(localpath)
-
-    if localpath.is_file():
-        size = localpath.stat().st_size
-    else:
-        size = sum(f.stat().st_size for f in localpath.rglob("*") if f.is_file())
-
-    if isinstance(storagepath, UPath):
-        if localpath.suffix != ".zarr":
-            cb = ProgressCallback()
-        else:
-            # todo: make proper progress bar for zarr
-            cb = fsspec.callbacks.NoOpCallback()
-        storagepath.upload_from(localpath, recursive=True, callback=cb)
-    else:  # storage path is local
-        storagepath.parent.mkdir(parents=True, exist_ok=True)
-        if localpath.is_file():
-            try:
-                shutil.copyfile(localpath, storagepath)
-            except shutil.SameFileError:
-                pass
-        else:
-            if storagepath.exists():
-                shutil.rmtree(storagepath)
-            shutil.copytree(localpath, storagepath)
-    return float(size)  # because this is how we store in the db
-
-
-def delete_storage(storagekey: str):
-    """Delete arbitrary file."""
-    storagepath = settings.instance.storage.key_to_filepath(storagekey)
-    if storagepath.is_file():
-        storagepath.unlink()
-    elif storagepath.is_dir():
-        if isinstance(storagepath, UPath):
-            storagepath.rmdir()
-        else:
-            shutil.rmtree(storagepath)
-    else:
-        raise FileNotFoundError(f"{storagepath} is not an existing path!")
-
-
-def load_to_memory(filepath: Union[str, Path, UPath], stream: bool = False):
-    """Load a file into memory.
-
-    Returns the filepath if no in-memory form is found.
-    """
-    if isinstance(filepath, str):
-        filepath = Path(filepath)
-
-    if filepath.suffix == ".zarr":
-        stream = True
-    elif filepath.suffix != ".h5ad":
-        stream = False
-
-    if not stream:
-        # caching happens here if filename is a UPath
-        # todo: make it safe when filepath is just Path
-        filepath = settings.instance.storage.cloud_to_local(filepath)
-
-    reader = READER_FUNCS.get(filepath.suffix)
-    if reader is None:
-        return filepath
-    else:
-        return reader(filepath)
+import os
+import shutil
+from pathlib import Path
+from typing import Union
+
+import fsspec
+import pandas as pd
+import readfcs
+from lndb import settings
+from lndb.dev.upath import UPath
+
+from ._h5ad import read_adata_h5ad
+from ._zarr import read_adata_zarr
+
+READER_FUNCS = {
+    ".csv": pd.read_csv,
+    ".h5ad": read_adata_h5ad,
+    ".parquet": pd.read_parquet,
+    ".fcs": readfcs.read,
+    ".zarr": read_adata_zarr,
+}
+
+
+def print_hook(size, value, **kwargs):
+    progress = value / size
+    out = f"... uploading {Path(kwargs['filepath']).name}: {min(progress, 1.):4.2f}"
+    if progress >= 1:
+        out += "\n"
+    if "NBPRJ_TEST_NBPATH" not in os.environ:
+        print(out, end="\r")
+
+
+class ProgressCallback(fsspec.callbacks.Callback):
+    def branch(self, path_1, path_2, kwargs):
+        kwargs["callback"] = fsspec.callbacks.Callback(
+            hooks=dict(print_hook=print_hook), filepath=path_1
+        )
+
+    def call(self, *args, **kwargs):
+        return None
+
+
+def store_object(localpath: Union[str, Path], storagekey: str) -> float:
+    """Store arbitrary file to configured storage location.
+
+    Returns size in bytes.
+    """
+    storagepath = settings.instance.storage.key_to_filepath(storagekey)
+    localpath = Path(localpath)
+
+    if localpath.is_file():
+        size = localpath.stat().st_size
+    else:
+        size = sum(f.stat().st_size for f in localpath.rglob("*") if f.is_file())
+
+    if isinstance(storagepath, UPath):
+        if localpath.suffix != ".zarr":
+            cb = ProgressCallback()
+        else:
+            # todo: make proper progress bar for zarr
+            cb = fsspec.callbacks.NoOpCallback()
+        storagepath.upload_from(localpath, recursive=True, callback=cb)
+    else:  # storage path is local
+        storagepath.parent.mkdir(parents=True, exist_ok=True)
+        if localpath.is_file():
+            try:
+                shutil.copyfile(localpath, storagepath)
+            except shutil.SameFileError:
+                pass
+        else:
+            if storagepath.exists():
+                shutil.rmtree(storagepath)
+            shutil.copytree(localpath, storagepath)
+    return float(size)  # because this is how we store in the db
+
+
+def delete_storage(storagekey: str):
+    """Delete arbitrary file."""
+    storagepath = settings.instance.storage.key_to_filepath(storagekey)
+    if storagepath.is_file():
+        storagepath.unlink()
+    elif storagepath.is_dir():
+        if isinstance(storagepath, UPath):
+            storagepath.rmdir()
+        else:
+            shutil.rmtree(storagepath)
+    else:
+        raise FileNotFoundError(f"{storagepath} is not an existing path!")
+
+
+def load_to_memory(filepath: Union[str, Path, UPath], stream: bool = False):
+    """Load a file into memory.
+
+    Returns the filepath if no in-memory form is found.
+    """
+    if isinstance(filepath, str):
+        filepath = Path(filepath)
+
+    if filepath.suffix == ".zarr":
+        stream = True
+    elif filepath.suffix != ".h5ad":
+        stream = False
+
+    if not stream:
+        # caching happens here if filename is a UPath
+        # todo: make it safe when filepath is just Path
+        filepath = settings.instance.storage.cloud_to_local(filepath)
+
+    reader = READER_FUNCS.get(filepath.suffix)
+    if reader is None:
+        return filepath
+    else:
+        return reader(filepath)
```

### Comparing `lndb_storage-0.3.1/lndb_storage/_subset.py` & `lndb_storage-0.3.2/lndb_storage/_subset.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from typing import List, Optional, Union
-
-from anndata import AnnData, concat
-from lamin_logger import logger
-from lnschema_core import File
-
-from .object import LazySelector, _subset_anndata_file
-
-SUFFIXES = (".h5ad", ".zarr")
-
-
-def subset(
-    files: Union[List[File], File],
-    query_obs: Optional[Union[List[str], str, LazySelector]] = None,
-    query_var: Optional[Union[List[str], str, LazySelector]] = None,
-    use_concat: bool = False,
-    concat_args: Optional[dict] = None,
-) -> Union[List[AnnData], AnnData, None]:
-    """Subset AnnData files and stream results into memory.
-
-    Args:
-        files: A `File` or a list of `Files` containing `AnnData` objects
-        to subset and load into memory.
-        query_obs: The pandas query string to evaluate on `.obs` of each
-        underlying `AnnData` object.
-        query_var: The pandas query string to evaluate on `.var` of each
-        underlying `AnnData` object.
-        use_concat: If `True`, applies `anndata.concat` on
-        the returned `AnnData` objects.
-        concat_args: Arguments for concatenation.
-    """
-    if isinstance(files, File):
-        files = [files]
-
-    n_files = len(files)
-    if isinstance(query_obs, list):
-        if len(query_obs) != n_files:
-            raise ValueError("query_obs list should be the same length as files.")
-    else:
-        query_obs = [query_obs] * n_files  # type: ignore
-    if isinstance(query_var, list):
-        if len(query_var) != n_files:
-            raise ValueError("query_var list should be the same length as files.")
-    else:
-        query_var = [query_var] * n_files  # type: ignore
-
-    adatas = []
-    # todo: implement parallel processing
-    for i, file in enumerate(files):
-        if file.suffix not in SUFFIXES:
-            logger.warning(f"File {file.id} is not an AnnData object, ignoring.")
-            continue
-        result = _subset_anndata_file(file, query_obs[i], query_var[i])
-        if result is not None:
-            adatas.append(result)
-
-    if not use_concat:
-        return adatas
-    # concat branch here
-    n_adatas = len(adatas)
-    if n_adatas == 0:
-        return None
-    elif n_adatas == 1:
-        return adatas[0]
-    else:
-        concat_args = {} if concat_args is None else concat_args
-        return concat(adatas, **concat_args)
+from typing import List, Optional, Union
+
+from anndata import AnnData, concat
+from lamin_logger import logger
+from lnschema_core import File
+
+from .object import LazySelector, _subset_anndata_file
+
+SUFFIXES = (".h5ad", ".zarr")
+
+
+def subset(
+    files: Union[List[File], File],
+    query_obs: Optional[Union[List[str], str, LazySelector]] = None,
+    query_var: Optional[Union[List[str], str, LazySelector]] = None,
+    use_concat: bool = False,
+    concat_args: Optional[dict] = None,
+) -> Union[List[AnnData], AnnData, None]:
+    """Subset AnnData files and stream results into memory.
+
+    Args:
+        files: A `File` or a list of `Files` containing `AnnData` objects
+        to subset and load into memory.
+        query_obs: The pandas query string to evaluate on `.obs` of each
+        underlying `AnnData` object.
+        query_var: The pandas query string to evaluate on `.var` of each
+        underlying `AnnData` object.
+        use_concat: If `True`, applies `anndata.concat` on
+        the returned `AnnData` objects.
+        concat_args: Arguments for concatenation.
+    """
+    if isinstance(files, File):
+        files = [files]
+
+    n_files = len(files)
+    if isinstance(query_obs, list):
+        if len(query_obs) != n_files:
+            raise ValueError("query_obs list should be the same length as files.")
+    else:
+        query_obs = [query_obs] * n_files  # type: ignore
+    if isinstance(query_var, list):
+        if len(query_var) != n_files:
+            raise ValueError("query_var list should be the same length as files.")
+    else:
+        query_var = [query_var] * n_files  # type: ignore
+
+    adatas = []
+    # todo: implement parallel processing
+    for i, file in enumerate(files):
+        if file.suffix not in SUFFIXES:
+            logger.warning(f"File {file.id} is not an AnnData object, ignoring.")
+            continue
+        result = _subset_anndata_file(file, query_obs[i], query_var[i])
+        if result is not None:
+            adatas.append(result)
+
+    if not use_concat:
+        return adatas
+    # concat branch here
+    n_adatas = len(adatas)
+    if n_adatas == 0:
+        return None
+    elif n_adatas == 1:
+        return adatas[0]
+    else:
+        concat_args = {} if concat_args is None else concat_args
+        return concat(adatas, **concat_args)
```

### Comparing `lndb_storage-0.3.1/lndb_storage/_zarr.py` & `lndb_storage-0.3.2/lndb_storage/_zarr.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-import warnings
-from typing import Optional
-
-import scipy.sparse as sparse
-import zarr
-from anndata import AnnData
-from anndata._io import read_zarr
-from anndata._io.specs import write_elem
-from lndb.dev.upath import infer_filesystem
-
-from .object._anndata_sizes import _size_elem, _size_raw, size_adata
-
-
-def read_adata_zarr(storepath) -> AnnData:
-    fs, storepath = infer_filesystem(storepath)
-
-    store = fs.get_mapper(storepath, check=True)
-    adata = read_zarr(store)
-
-    return adata
-
-
-def write_adata_zarr(
-    adata: AnnData, storepath, callback=None, chunks=None, **dataset_kwargs
-):
-    fs, storepath = infer_filesystem(storepath)
-
-    store = fs.get_mapper(storepath, create=True)
-    f = zarr.open(store, mode="w")
-
-    adata.strings_to_categoricals()
-    if adata.raw is not None:
-        adata.strings_to_categoricals(adata.raw.var)
-
-    f.attrs.setdefault("encoding-type", "anndata")
-    f.attrs.setdefault("encoding-version", "0.1.0")
-
-    adata_size = None
-    cumulative_val = 0
-
-    def _cb(key_write: Optional[str] = None):
-        nonlocal adata_size
-        nonlocal cumulative_val
-
-        if callback is None:
-            return None
-        if adata_size is None:
-            adata_size = size_adata(adata)
-        if key_write is None:
-            # begin or finish
-            if cumulative_val < adata_size:
-                callback(adata_size, adata_size if cumulative_val > 0 else 0)
-            return None
-
-        elem = getattr(adata, key_write, None)
-        if elem is None:
-            return None
-        elem_size = _size_raw(elem) if key_write == "raw" else _size_elem(elem)
-        if elem_size == 0:
-            return None
-
-        cumulative_val += elem_size
-        callback(adata_size, cumulative_val)
-
-    def _write_elem_cb(f, k, elem, dataset_kwargs):
-        write_elem(f, k, elem, dataset_kwargs=dataset_kwargs)
-        _cb(k)
-
-    _cb(None)
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", category=UserWarning, module="zarr")
-
-        if chunks is not None and not isinstance(adata.X, sparse.spmatrix):
-            _write_elem_cb(
-                f, "X", adata.X, dataset_kwargs=dict(chunks=chunks, **dataset_kwargs)
-            )
-        else:
-            _write_elem_cb(f, "X", adata.X, dataset_kwargs=dataset_kwargs)
-        for elem in ("obs", "var"):
-            _write_elem_cb(f, elem, getattr(adata, elem), dataset_kwargs=dataset_kwargs)
-        for elem in ("obsm", "varm", "obsp", "varp", "layers", "uns"):
-            _write_elem_cb(
-                f, elem, dict(getattr(adata, elem)), dataset_kwargs=dataset_kwargs
-            )
-        _write_elem_cb(f, "raw", adata.raw, dataset_kwargs=dataset_kwargs)
-    # todo: fix size less than total at the end
-    _cb(None)
+import warnings
+from typing import Optional
+
+import scipy.sparse as sparse
+import zarr
+from anndata import AnnData
+from anndata._io import read_zarr
+from anndata._io.specs import write_elem
+from lndb.dev.upath import infer_filesystem
+
+from .object._anndata_sizes import _size_elem, _size_raw, size_adata
+
+
+def read_adata_zarr(storepath) -> AnnData:
+    fs, storepath = infer_filesystem(storepath)
+
+    store = fs.get_mapper(storepath, check=True)
+    adata = read_zarr(store)
+
+    return adata
+
+
+def write_adata_zarr(
+    adata: AnnData, storepath, callback=None, chunks=None, **dataset_kwargs
+):
+    fs, storepath = infer_filesystem(storepath)
+
+    store = fs.get_mapper(storepath, create=True)
+    f = zarr.open(store, mode="w")
+
+    adata.strings_to_categoricals()
+    if adata.raw is not None:
+        adata.strings_to_categoricals(adata.raw.var)
+
+    f.attrs.setdefault("encoding-type", "anndata")
+    f.attrs.setdefault("encoding-version", "0.1.0")
+
+    adata_size = None
+    cumulative_val = 0
+
+    def _cb(key_write: Optional[str] = None):
+        nonlocal adata_size
+        nonlocal cumulative_val
+
+        if callback is None:
+            return None
+        if adata_size is None:
+            adata_size = size_adata(adata)
+        if key_write is None:
+            # begin or finish
+            if cumulative_val < adata_size:
+                callback(adata_size, adata_size if cumulative_val > 0 else 0)
+            return None
+
+        elem = getattr(adata, key_write, None)
+        if elem is None:
+            return None
+        elem_size = _size_raw(elem) if key_write == "raw" else _size_elem(elem)
+        if elem_size == 0:
+            return None
+
+        cumulative_val += elem_size
+        callback(adata_size, cumulative_val)
+
+    def _write_elem_cb(f, k, elem, dataset_kwargs):
+        write_elem(f, k, elem, dataset_kwargs=dataset_kwargs)
+        _cb(k)
+
+    _cb(None)
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", category=UserWarning, module="zarr")
+
+        if chunks is not None and not isinstance(adata.X, sparse.spmatrix):
+            _write_elem_cb(
+                f, "X", adata.X, dataset_kwargs=dict(chunks=chunks, **dataset_kwargs)
+            )
+        else:
+            _write_elem_cb(f, "X", adata.X, dataset_kwargs=dataset_kwargs)
+        for elem in ("obs", "var"):
+            _write_elem_cb(f, elem, getattr(adata, elem), dataset_kwargs=dataset_kwargs)
+        for elem in ("obsm", "varm", "obsp", "varp", "layers", "uns"):
+            _write_elem_cb(
+                f, elem, dict(getattr(adata, elem)), dataset_kwargs=dataset_kwargs
+            )
+        _write_elem_cb(f, "raw", adata.raw, dataset_kwargs=dataset_kwargs)
+    # todo: fix size less than total at the end
+    _cb(None)
```

### Comparing `lndb_storage-0.3.1/lndb_storage/object/_anndata_accessor.py` & `lndb_storage-0.3.2/lndb_storage/object/_anndata_accessor.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,358 +1,358 @@
-from functools import cached_property
-from typing import Dict, Mapping, Union
-
-import h5py
-import pandas as pd
-import zarr
-from anndata._core.index import Index, _normalize_indices
-from anndata._core.sparse_dataset import SparseDataset
-from anndata._core.views import _resolve_idx
-from anndata._io.specs.methods import read_indices
-from anndata._io.specs.registry import get_spec, read_elem, read_elem_partial
-from anndata.compat import _read_attr
-from lndb.dev.upath import infer_filesystem as _infer_filesystem
-from lnschema_core import File
-from lnschema_core._core import filepath_from_file_or_folder
-
-from ._subset_anndata import _read_dataframe
-
-
-def _try_backed_full(elem):
-    # think what to do for compatibility with old var and obs
-    if isinstance(elem, (h5py.Dataset, zarr.Array)):
-        return elem
-
-    if isinstance(elem, (h5py.Group, zarr.Group)):
-        encoding_type = get_spec(elem)
-        if encoding_type in ("csr_matrix", "csc_matrix"):
-            return SparseDataset(elem)
-        if "h5sparse_format" in elem.attrs:
-            return SparseDataset(elem)
-
-    return read_elem(elem)
-
-
-class _MapAccessor:
-    def __init__(self, elem, name, indices=None):
-        self.elem = elem
-        self.indices = indices
-        self.name = name
-
-    def __getitem__(self, key):
-        if self.indices is None:
-            return _try_backed_full(self.elem[key])
-        else:
-            return read_elem_partial(self.elem[key], indices=self.indices)
-
-    def keys(self):
-        return list(self.elem.keys())
-
-    def __repr__(self):
-        """Description of the _MapAccessor object."""
-        descr = f"Accessor for the AnnData attribute {self.name}"
-        descr += f"\n  with keys: {self.keys()}"
-        return descr
-
-
-class _AnnDataAttrsMixin:
-    storage: Union[h5py.File, zarr.Group]
-    _attrs_keys: Mapping[str, list]
-
-    @cached_property
-    def obs(self) -> pd.DataFrame:
-        if "obs" not in self._attrs_keys:
-            return None
-        indices = getattr(self, "indices", None)
-        if indices is not None:
-            indices = (indices[0], slice(None))
-            return read_elem_partial(self.storage["obs"], indices=indices)
-        else:
-            return _read_dataframe(self.storage["obs"])
-
-    @cached_property
-    def var(self) -> pd.DataFrame:
-        if "var" not in self._attrs_keys:
-            return None
-        indices = getattr(self, "indices", None)
-        if indices is not None:
-            indices = (indices[1], slice(None))
-            return read_elem_partial(self.storage["var"], indices=indices)
-        else:
-            return _read_dataframe(self.storage["var"])
-
-    @cached_property
-    def uns(self):
-        if "uns" not in self._attrs_keys:
-            return None
-        return read_elem(self.storage["uns"])
-
-    @cached_property
-    def X(self):
-        indices = getattr(self, "indices", None)
-        if indices is not None:
-            return read_elem_partial(self.storage["X"], indices=indices)
-        else:
-            return _try_backed_full(self.storage["X"])
-
-    @cached_property
-    def obsm(self):
-        if "obsm" not in self._attrs_keys:
-            return None
-        indices = getattr(self, "indices", None)
-        if indices is not None:
-            indices = (indices[0], slice(None))
-        return _MapAccessor(self.storage["obsm"], "obsm", indices)
-
-    @cached_property
-    def varm(self):
-        if "varm" not in self._attrs_keys:
-            return None
-        indices = getattr(self, "indices", None)
-        if indices is not None:
-            indices = (indices[1], slice(None))
-        return _MapAccessor(self.storage["varm"], "varm", indices)
-
-    @cached_property
-    def obsp(self):
-        if "obsp" not in self._attrs_keys:
-            return None
-        indices = getattr(self, "indices", None)
-        if indices is not None:
-            indices = (indices[0], indices[0])
-        return _MapAccessor(self.storage["obsp"], "obsp", indices)
-
-    @cached_property
-    def varp(self):
-        if "varp" not in self._attrs_keys:
-            return None
-        indices = getattr(self, "indices", None)
-        if indices is not None:
-            indices = (indices[1], indices[1])
-        return _MapAccessor(self.storage["varp"], "varp", indices)
-
-    @cached_property
-    def layers(self):
-        if "layers" not in self._attrs_keys:
-            return None
-        indices = getattr(self, "indices", None)
-        return _MapAccessor(self.storage["layers"], "layers", indices)
-
-    @property
-    def obs_names(self):
-        return self._obs_names
-
-    @property
-    def var_names(self):
-        return self._var_names
-
-    @cached_property
-    def shape(self):
-        return len(self._obs_names), len(self._var_names)
-
-
-class AnnDataAccessorSubset(_AnnDataAttrsMixin):
-    def __init__(self, storage, indices, attrs_keys, obs_names, var_names, ref_shape):
-        self.storage = storage
-        self.indices = indices
-
-        self._attrs_keys = attrs_keys
-        self._obs_names, self._var_names = obs_names, var_names
-
-        self._ref_shape = ref_shape
-
-    def __getitem__(self, index: Index):
-        """Access a subset of the underlying AnnData object."""
-        oidx, vidx = _normalize_indices(index, self._obs_names, self._var_names)
-        new_obs_names, new_var_names = self._obs_names[oidx], self._var_names[vidx]
-        if self.indices is not None:
-            oidx = _resolve_idx(self.indices[0], oidx, self._ref_shape[0])
-            vidx = _resolve_idx(self.indices[1], vidx, self._ref_shape[1])
-        return type(self)(
-            self.storage,
-            (oidx, vidx),
-            self._attrs_keys,
-            new_obs_names,
-            new_var_names,
-            self._ref_shape,
-        )
-
-    def __repr__(self):
-        """Description of the object."""
-        n_obs, n_vars = self.shape
-        descr = f"{type(self).__name__} object with n_obs × n_vars = {n_obs} × {n_vars}"
-        for attr, keys in self._attrs_keys.items():
-            descr += f"\n  {attr}: {keys}"
-        return descr
-
-    @cached_property
-    def raw(self):
-        if "raw" not in self._attrs_keys:
-            return None
-        prepare_indices = None
-        if self.indices is not None:
-            oidx = self.indices[0]
-            if oidx != slice(None):
-                prepare_indices = oidx, slice(None)
-        return AnnDataRawAccessor(
-            self.storage["raw"],
-            prepare_indices,
-            None,
-            self._obs_names,
-            None,
-            self._ref_shape[0],
-        )
-
-
-class AnnDataRawAccessor(AnnDataAccessorSubset):
-    def __init__(
-        self, storage_raw, indices, attrs_keys, obs_names, var_names, ref_shape
-    ):
-        var_raw = storage_raw["var"]
-
-        if var_names is None:
-            var_names = read_elem(var_raw[_read_attr(var_raw.attrs, "_index")])
-
-        if isinstance(ref_shape, int):
-            ref_shape = ref_shape, len(var_names)
-        elif isinstance(ref_shape, tuple) and len(ref_shape) < 2:
-            ref_shape = ref_shape[0], len(var_names)
-
-        if attrs_keys is None:
-            attrs_keys = {}
-            if isinstance(var_raw, (h5py.Dataset, zarr.Array)):
-                attrs_keys["var"] = list(var_raw.dtype.fields.keys())
-            else:
-                # for some reason list(var_raw.keys()) is very slow for zarr
-                # maybe also directly get keys from the underlying mapper
-                attrs_keys["var"] = [key for key in var_raw]
-            if "varm" in storage_raw:
-                varm_keys_raw = [key for key in storage_raw["varm"]]
-                if len(varm_keys_raw) > 0:
-                    attrs_keys["varm"] = varm_keys_raw
-
-        super().__init__(
-            storage_raw, indices, attrs_keys, obs_names, var_names, ref_shape
-        )
-
-    @property
-    def raw(self):
-        raise AttributeError
-
-
-class AnnDataAccessor(_AnnDataAttrsMixin):
-    def __init__(self, file: File):
-        fs, file_path_str = _infer_filesystem(filepath_from_file_or_folder(file))
-
-        if file.suffix == ".h5ad":
-            self._conn = fs.open(file_path_str, mode="rb")
-            try:
-                self.storage = h5py.File(self._conn, mode="r")
-            except Exception as e:
-                self._conn.close()
-                raise e
-            self._attrs_keys = _keys_h5(self.storage)
-        elif file.suffix in (".zarr", ".zrad"):
-            self._conn = None
-            mapper = fs.get_mapper(file_path_str, check=True)
-            self.storage = zarr.open(mapper, mode="r")
-            self._attrs_keys = _keys_zarr(self.storage)
-        else:
-            raise ValueError(
-                f"file should have .h5ad, .zarr or .zrad suffix, not {file.suffix}."
-            )
-
-        self._name = file.name
-
-        self._obs_names, self._var_names = read_indices(self.storage)
-
-    def __del__(self):
-        """Closes the connection."""
-        if self._conn is not None:
-            self.storage.close()
-            self._conn.close()
-
-    def __getitem__(self, index: Index) -> AnnDataAccessorSubset:
-        """Access a subset of the underlying AnnData object."""
-        oidx, vidx = _normalize_indices(index, self._obs_names, self._var_names)
-        new_obs_names, new_var_names = self._obs_names[oidx], self._var_names[vidx]
-        return AnnDataAccessorSubset(
-            self.storage,
-            (oidx, vidx),
-            self._attrs_keys,
-            new_obs_names,
-            new_var_names,
-            self.shape,
-        )
-
-    def __repr__(self):
-        """Description of the AnnDataAccessor object."""
-        n_obs, n_vars = self.shape
-        descr = f"AnnDataAccessor object with n_obs × n_vars = {n_obs} × {n_vars}"
-        descr += f"\n  constructed for the AnnData object {self._name}"
-        for attr, keys in self._attrs_keys.items():
-            descr += f"\n    {attr}: {keys}"
-        return descr
-
-    @cached_property
-    def raw(self):
-        if "raw" not in self._attrs_keys:
-            return None
-        return AnnDataRawAccessor(
-            self.storage["raw"], None, None, self._obs_names, None, self.shape[0]
-        )
-
-
-# this is needed because accessing zarr.Group.keys() directly is very slow
-def _keys_zarr(storage: zarr.Group):
-    paths = storage._store.keys()
-
-    attrs_keys: Dict[str, list] = {}
-    obs_var_arrays = []
-
-    for path in paths:
-        if path in (".zattrs", ".zgroup"):
-            continue
-        parts = path.split("/")
-        if len(parts) < 2:
-            continue
-        attr = parts[0]
-        key = parts[1]
-
-        if attr == "X":
-            continue
-
-        if attr in ("obs", "var"):
-            if attr in obs_var_arrays:
-                continue
-            if key == ".zarray":
-                attrs_keys.pop(attr, None)
-                obs_var_arrays.append(attr)
-
-        if attr not in attrs_keys:
-            attrs_keys[attr] = []
-
-        if key in (".zattrs", ".zgroup", ".zarray"):
-            continue
-        attr_keys = attrs_keys[attr]
-        if key not in attr_keys:
-            attr_keys.append(key)
-
-    for attr in obs_var_arrays:
-        attrs_keys[attr] = list(storage[attr].dtype.fields.keys())
-
-    return {attr: keys for attr, keys in attrs_keys.items() if len(keys) > 0}
-
-
-def _keys_h5(storage: h5py.File):
-    attrs_keys: Dict[str, list] = {}
-    for attr in storage.keys():
-        if attr == "X":
-            continue
-        attr_obj = storage[attr]
-        if attr in ("obs", "var") and isinstance(attr_obj, h5py.Dataset):
-            keys = list(attr_obj.dtype.fields.keys())
-        else:
-            keys = list(attr_obj.keys())
-        if len(keys) > 0:
-            attrs_keys[attr] = keys
-    return attrs_keys
+from functools import cached_property
+from typing import Dict, Mapping, Union
+
+import h5py
+import pandas as pd
+import zarr
+from anndata._core.index import Index, _normalize_indices
+from anndata._core.sparse_dataset import SparseDataset
+from anndata._core.views import _resolve_idx
+from anndata._io.specs.methods import read_indices
+from anndata._io.specs.registry import get_spec, read_elem, read_elem_partial
+from anndata.compat import _read_attr
+from lndb.dev.upath import infer_filesystem as _infer_filesystem
+from lnschema_core import File
+from lnschema_core._core import filepath_from_file_or_folder
+
+from ._subset_anndata import _read_dataframe
+
+
+def _try_backed_full(elem):
+    # think what to do for compatibility with old var and obs
+    if isinstance(elem, (h5py.Dataset, zarr.Array)):
+        return elem
+
+    if isinstance(elem, (h5py.Group, zarr.Group)):
+        encoding_type = get_spec(elem)
+        if encoding_type in ("csr_matrix", "csc_matrix"):
+            return SparseDataset(elem)
+        if "h5sparse_format" in elem.attrs:
+            return SparseDataset(elem)
+
+    return read_elem(elem)
+
+
+class _MapAccessor:
+    def __init__(self, elem, name, indices=None):
+        self.elem = elem
+        self.indices = indices
+        self.name = name
+
+    def __getitem__(self, key):
+        if self.indices is None:
+            return _try_backed_full(self.elem[key])
+        else:
+            return read_elem_partial(self.elem[key], indices=self.indices)
+
+    def keys(self):
+        return list(self.elem.keys())
+
+    def __repr__(self):
+        """Description of the _MapAccessor object."""
+        descr = f"Accessor for the AnnData attribute {self.name}"
+        descr += f"\n  with keys: {self.keys()}"
+        return descr
+
+
+class _AnnDataAttrsMixin:
+    storage: Union[h5py.File, zarr.Group]
+    _attrs_keys: Mapping[str, list]
+
+    @cached_property
+    def obs(self) -> pd.DataFrame:
+        if "obs" not in self._attrs_keys:
+            return None
+        indices = getattr(self, "indices", None)
+        if indices is not None:
+            indices = (indices[0], slice(None))
+            return read_elem_partial(self.storage["obs"], indices=indices)
+        else:
+            return _read_dataframe(self.storage["obs"])
+
+    @cached_property
+    def var(self) -> pd.DataFrame:
+        if "var" not in self._attrs_keys:
+            return None
+        indices = getattr(self, "indices", None)
+        if indices is not None:
+            indices = (indices[1], slice(None))
+            return read_elem_partial(self.storage["var"], indices=indices)
+        else:
+            return _read_dataframe(self.storage["var"])
+
+    @cached_property
+    def uns(self):
+        if "uns" not in self._attrs_keys:
+            return None
+        return read_elem(self.storage["uns"])
+
+    @cached_property
+    def X(self):
+        indices = getattr(self, "indices", None)
+        if indices is not None:
+            return read_elem_partial(self.storage["X"], indices=indices)
+        else:
+            return _try_backed_full(self.storage["X"])
+
+    @cached_property
+    def obsm(self):
+        if "obsm" not in self._attrs_keys:
+            return None
+        indices = getattr(self, "indices", None)
+        if indices is not None:
+            indices = (indices[0], slice(None))
+        return _MapAccessor(self.storage["obsm"], "obsm", indices)
+
+    @cached_property
+    def varm(self):
+        if "varm" not in self._attrs_keys:
+            return None
+        indices = getattr(self, "indices", None)
+        if indices is not None:
+            indices = (indices[1], slice(None))
+        return _MapAccessor(self.storage["varm"], "varm", indices)
+
+    @cached_property
+    def obsp(self):
+        if "obsp" not in self._attrs_keys:
+            return None
+        indices = getattr(self, "indices", None)
+        if indices is not None:
+            indices = (indices[0], indices[0])
+        return _MapAccessor(self.storage["obsp"], "obsp", indices)
+
+    @cached_property
+    def varp(self):
+        if "varp" not in self._attrs_keys:
+            return None
+        indices = getattr(self, "indices", None)
+        if indices is not None:
+            indices = (indices[1], indices[1])
+        return _MapAccessor(self.storage["varp"], "varp", indices)
+
+    @cached_property
+    def layers(self):
+        if "layers" not in self._attrs_keys:
+            return None
+        indices = getattr(self, "indices", None)
+        return _MapAccessor(self.storage["layers"], "layers", indices)
+
+    @property
+    def obs_names(self):
+        return self._obs_names
+
+    @property
+    def var_names(self):
+        return self._var_names
+
+    @cached_property
+    def shape(self):
+        return len(self._obs_names), len(self._var_names)
+
+
+class AnnDataAccessorSubset(_AnnDataAttrsMixin):
+    def __init__(self, storage, indices, attrs_keys, obs_names, var_names, ref_shape):
+        self.storage = storage
+        self.indices = indices
+
+        self._attrs_keys = attrs_keys
+        self._obs_names, self._var_names = obs_names, var_names
+
+        self._ref_shape = ref_shape
+
+    def __getitem__(self, index: Index):
+        """Access a subset of the underlying AnnData object."""
+        oidx, vidx = _normalize_indices(index, self._obs_names, self._var_names)
+        new_obs_names, new_var_names = self._obs_names[oidx], self._var_names[vidx]
+        if self.indices is not None:
+            oidx = _resolve_idx(self.indices[0], oidx, self._ref_shape[0])
+            vidx = _resolve_idx(self.indices[1], vidx, self._ref_shape[1])
+        return type(self)(
+            self.storage,
+            (oidx, vidx),
+            self._attrs_keys,
+            new_obs_names,
+            new_var_names,
+            self._ref_shape,
+        )
+
+    def __repr__(self):
+        """Description of the object."""
+        n_obs, n_vars = self.shape
+        descr = f"{type(self).__name__} object with n_obs × n_vars = {n_obs} × {n_vars}"
+        for attr, keys in self._attrs_keys.items():
+            descr += f"\n  {attr}: {keys}"
+        return descr
+
+    @cached_property
+    def raw(self):
+        if "raw" not in self._attrs_keys:
+            return None
+        prepare_indices = None
+        if self.indices is not None:
+            oidx = self.indices[0]
+            if oidx != slice(None):
+                prepare_indices = oidx, slice(None)
+        return AnnDataRawAccessor(
+            self.storage["raw"],
+            prepare_indices,
+            None,
+            self._obs_names,
+            None,
+            self._ref_shape[0],
+        )
+
+
+class AnnDataRawAccessor(AnnDataAccessorSubset):
+    def __init__(
+        self, storage_raw, indices, attrs_keys, obs_names, var_names, ref_shape
+    ):
+        var_raw = storage_raw["var"]
+
+        if var_names is None:
+            var_names = read_elem(var_raw[_read_attr(var_raw.attrs, "_index")])
+
+        if isinstance(ref_shape, int):
+            ref_shape = ref_shape, len(var_names)
+        elif isinstance(ref_shape, tuple) and len(ref_shape) < 2:
+            ref_shape = ref_shape[0], len(var_names)
+
+        if attrs_keys is None:
+            attrs_keys = {}
+            if isinstance(var_raw, (h5py.Dataset, zarr.Array)):
+                attrs_keys["var"] = list(var_raw.dtype.fields.keys())
+            else:
+                # for some reason list(var_raw.keys()) is very slow for zarr
+                # maybe also directly get keys from the underlying mapper
+                attrs_keys["var"] = [key for key in var_raw]
+            if "varm" in storage_raw:
+                varm_keys_raw = [key for key in storage_raw["varm"]]
+                if len(varm_keys_raw) > 0:
+                    attrs_keys["varm"] = varm_keys_raw
+
+        super().__init__(
+            storage_raw, indices, attrs_keys, obs_names, var_names, ref_shape
+        )
+
+    @property
+    def raw(self):
+        raise AttributeError
+
+
+class AnnDataAccessor(_AnnDataAttrsMixin):
+    def __init__(self, file: File):
+        fs, file_path_str = _infer_filesystem(filepath_from_file_or_folder(file))
+
+        if file.suffix == ".h5ad":
+            self._conn = fs.open(file_path_str, mode="rb")
+            try:
+                self.storage = h5py.File(self._conn, mode="r")
+            except Exception as e:
+                self._conn.close()
+                raise e
+            self._attrs_keys = _keys_h5(self.storage)
+        elif file.suffix in (".zarr", ".zrad"):
+            self._conn = None
+            mapper = fs.get_mapper(file_path_str, check=True)
+            self.storage = zarr.open(mapper, mode="r")
+            self._attrs_keys = _keys_zarr(self.storage)
+        else:
+            raise ValueError(
+                f"file should have .h5ad, .zarr or .zrad suffix, not {file.suffix}."
+            )
+
+        self._name = file.name
+
+        self._obs_names, self._var_names = read_indices(self.storage)
+
+    def __del__(self):
+        """Closes the connection."""
+        if self._conn is not None:
+            self.storage.close()
+            self._conn.close()
+
+    def __getitem__(self, index: Index) -> AnnDataAccessorSubset:
+        """Access a subset of the underlying AnnData object."""
+        oidx, vidx = _normalize_indices(index, self._obs_names, self._var_names)
+        new_obs_names, new_var_names = self._obs_names[oidx], self._var_names[vidx]
+        return AnnDataAccessorSubset(
+            self.storage,
+            (oidx, vidx),
+            self._attrs_keys,
+            new_obs_names,
+            new_var_names,
+            self.shape,
+        )
+
+    def __repr__(self):
+        """Description of the AnnDataAccessor object."""
+        n_obs, n_vars = self.shape
+        descr = f"AnnDataAccessor object with n_obs × n_vars = {n_obs} × {n_vars}"
+        descr += f"\n  constructed for the AnnData object {self._name}"
+        for attr, keys in self._attrs_keys.items():
+            descr += f"\n    {attr}: {keys}"
+        return descr
+
+    @cached_property
+    def raw(self):
+        if "raw" not in self._attrs_keys:
+            return None
+        return AnnDataRawAccessor(
+            self.storage["raw"], None, None, self._obs_names, None, self.shape[0]
+        )
+
+
+# this is needed because accessing zarr.Group.keys() directly is very slow
+def _keys_zarr(storage: zarr.Group):
+    paths = storage._store.keys()
+
+    attrs_keys: Dict[str, list] = {}
+    obs_var_arrays = []
+
+    for path in paths:
+        if path in (".zattrs", ".zgroup"):
+            continue
+        parts = path.split("/")
+        if len(parts) < 2:
+            continue
+        attr = parts[0]
+        key = parts[1]
+
+        if attr == "X":
+            continue
+
+        if attr in ("obs", "var"):
+            if attr in obs_var_arrays:
+                continue
+            if key == ".zarray":
+                attrs_keys.pop(attr, None)
+                obs_var_arrays.append(attr)
+
+        if attr not in attrs_keys:
+            attrs_keys[attr] = []
+
+        if key in (".zattrs", ".zgroup", ".zarray"):
+            continue
+        attr_keys = attrs_keys[attr]
+        if key not in attr_keys:
+            attr_keys.append(key)
+
+    for attr in obs_var_arrays:
+        attrs_keys[attr] = list(storage[attr].dtype.fields.keys())
+
+    return {attr: keys for attr, keys in attrs_keys.items() if len(keys) > 0}
+
+
+def _keys_h5(storage: h5py.File):
+    attrs_keys: Dict[str, list] = {}
+    for attr in storage.keys():
+        if attr == "X":
+            continue
+        attr_obj = storage[attr]
+        if attr in ("obs", "var") and isinstance(attr_obj, h5py.Dataset):
+            keys = list(attr_obj.dtype.fields.keys())
+        else:
+            keys = list(attr_obj.keys())
+        if len(keys) > 0:
+            attrs_keys[attr] = keys
+    return attrs_keys
```

### Comparing `lndb_storage-0.3.1/lndb_storage/object/_subset_anndata.py` & `lndb_storage-0.3.2/lndb_storage/object/_subset_anndata.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-from typing import Optional, Union
-
-import h5py
-import zarr
-from anndata import AnnData
-from anndata._io.h5ad import read_dataframe_legacy as read_dataframe_legacy_h5
-from anndata._io.specs.methods import _read_partial
-from anndata._io.specs.registry import read_elem, read_elem_partial
-from anndata._io.zarr import read_dataframe_legacy as read_dataframe_legacy_zarr
-from lndb.dev.upath import infer_filesystem as _infer_filesystem
-from lnschema_core import File
-from lnschema_core._core import filepath_from_file_or_folder
-
-from ._lazy_field import LazySelector
-
-
-def _read_dataframe(elem: Union[zarr.Array, h5py.Dataset, zarr.Group, h5py.Group]):
-    if isinstance(elem, zarr.Array):
-        return read_dataframe_legacy_zarr(elem)
-    elif isinstance(elem, h5py.Dataset):
-        return read_dataframe_legacy_h5(elem)
-    else:
-        return read_elem(elem)
-
-
-def _indices(base_indices, select_indices):
-    if len(base_indices) == len(select_indices):
-        return slice(None)
-    else:
-        return list(base_indices.get_indexer(select_indices))
-
-
-def _subset_adata_storage(
-    storage: Union[zarr.Group, h5py.File],
-    query_obs: Optional[Union[str, LazySelector]] = None,
-    query_var: Optional[Union[str, LazySelector]] = None,
-) -> Union[AnnData, None]:
-    with storage as access:
-        obs = _read_dataframe(access["obs"])
-        var = _read_dataframe(access["var"])
-
-        if query_obs is not None:
-            if hasattr(query_obs, "evaluate"):
-                obs_result = obs[query_obs.evaluate(obj=obs)]  # type: ignore
-            else:
-                obs_result = obs.query(query_obs)
-        else:
-            obs_result = obs
-
-        if query_var is not None:
-            if hasattr(query_var, "evaluate"):
-                var_result = var[query_var.evaluate(obj=var)]  # type: ignore
-            else:
-                var_result = var.query(query_var)
-        else:
-            var_result = var
-
-        if obs_result.index.empty or var_result.index.empty:
-            return None
-
-        obs_idx = _indices(obs.index, obs_result.index)
-        var_idx = _indices(var.index, var_result.index)
-
-        prepare_adata = {}
-        prepare_adata["obs"] = obs_result
-        prepare_adata["var"] = var_result
-        X = read_elem_partial(access["X"], indices=(obs_idx, var_idx))
-        prepare_adata["X"] = X
-        if "obsm" in access:
-            obsm = _read_partial(access["obsm"], indices=(obs_idx, slice(None)))
-            prepare_adata["obsm"] = obsm
-        if "varm" in access:
-            varm = _read_partial(access["varm"], indices=(var_idx, slice(None)))
-            prepare_adata["varm"] = varm
-        if "obsp" in access:
-            obsp = _read_partial(access["obsp"], indices=(obs_idx, obs_idx))
-            prepare_adata["obsp"] = obsp
-        if "varp" in access:
-            varp = _read_partial(access["varp"], indices=(var_idx, var_idx))
-            prepare_adata["varp"] = varp
-        if "layers" in access:
-            layers = _read_partial(access["layers"], indices=(obs_idx, var_idx))
-            prepare_adata["layers"] = layers
-        if "uns" in access:
-            prepare_adata["uns"] = read_elem(access["uns"])
-
-        return AnnData(**prepare_adata)
-
-
-def _subset_anndata_file(
-    file: File,
-    query_obs: Optional[Union[str, LazySelector]] = None,
-    query_var: Optional[Union[str, LazySelector]] = None,
-) -> Union[AnnData, None]:
-    file_path = filepath_from_file_or_folder(file)
-    fs, file_path_str = _infer_filesystem(file_path)
-
-    adata: Union[AnnData, None] = None
-
-    if file.suffix == ".h5ad":
-        with fs.open(file_path_str, mode="rb") as file:
-            storage = h5py.File(file, mode="r")
-            adata = _subset_adata_storage(storage, query_obs, query_var)
-    elif file.suffix == ".zarr":
-        mapper = fs.get_mapper(file_path_str, check=True)
-        storage = zarr.open(mapper, mode="r")
-        adata = _subset_adata_storage(storage, query_obs, query_var)
-
-    return adata
+from typing import Optional, Union
+
+import h5py
+import zarr
+from anndata import AnnData
+from anndata._io.h5ad import read_dataframe_legacy as read_dataframe_legacy_h5
+from anndata._io.specs.methods import _read_partial
+from anndata._io.specs.registry import read_elem, read_elem_partial
+from anndata._io.zarr import read_dataframe_legacy as read_dataframe_legacy_zarr
+from lndb.dev.upath import infer_filesystem as _infer_filesystem
+from lnschema_core import File
+from lnschema_core._core import filepath_from_file_or_folder
+
+from ._lazy_field import LazySelector
+
+
+def _read_dataframe(elem: Union[zarr.Array, h5py.Dataset, zarr.Group, h5py.Group]):
+    if isinstance(elem, zarr.Array):
+        return read_dataframe_legacy_zarr(elem)
+    elif isinstance(elem, h5py.Dataset):
+        return read_dataframe_legacy_h5(elem)
+    else:
+        return read_elem(elem)
+
+
+def _indices(base_indices, select_indices):
+    if len(base_indices) == len(select_indices):
+        return slice(None)
+    else:
+        return list(base_indices.get_indexer(select_indices))
+
+
+def _subset_adata_storage(
+    storage: Union[zarr.Group, h5py.File],
+    query_obs: Optional[Union[str, LazySelector]] = None,
+    query_var: Optional[Union[str, LazySelector]] = None,
+) -> Union[AnnData, None]:
+    with storage as access:
+        obs = _read_dataframe(access["obs"])
+        var = _read_dataframe(access["var"])
+
+        if query_obs is not None:
+            if hasattr(query_obs, "evaluate"):
+                obs_result = obs[query_obs.evaluate(obj=obs)]  # type: ignore
+            else:
+                obs_result = obs.query(query_obs)
+        else:
+            obs_result = obs
+
+        if query_var is not None:
+            if hasattr(query_var, "evaluate"):
+                var_result = var[query_var.evaluate(obj=var)]  # type: ignore
+            else:
+                var_result = var.query(query_var)
+        else:
+            var_result = var
+
+        if obs_result.index.empty or var_result.index.empty:
+            return None
+
+        obs_idx = _indices(obs.index, obs_result.index)
+        var_idx = _indices(var.index, var_result.index)
+
+        prepare_adata = {}
+        prepare_adata["obs"] = obs_result
+        prepare_adata["var"] = var_result
+        X = read_elem_partial(access["X"], indices=(obs_idx, var_idx))
+        prepare_adata["X"] = X
+        if "obsm" in access:
+            obsm = _read_partial(access["obsm"], indices=(obs_idx, slice(None)))
+            prepare_adata["obsm"] = obsm
+        if "varm" in access:
+            varm = _read_partial(access["varm"], indices=(var_idx, slice(None)))
+            prepare_adata["varm"] = varm
+        if "obsp" in access:
+            obsp = _read_partial(access["obsp"], indices=(obs_idx, obs_idx))
+            prepare_adata["obsp"] = obsp
+        if "varp" in access:
+            varp = _read_partial(access["varp"], indices=(var_idx, var_idx))
+            prepare_adata["varp"] = varp
+        if "layers" in access:
+            layers = _read_partial(access["layers"], indices=(obs_idx, var_idx))
+            prepare_adata["layers"] = layers
+        if "uns" in access:
+            prepare_adata["uns"] = read_elem(access["uns"])
+
+        return AnnData(**prepare_adata)
+
+
+def _subset_anndata_file(
+    file: File,
+    query_obs: Optional[Union[str, LazySelector]] = None,
+    query_var: Optional[Union[str, LazySelector]] = None,
+) -> Union[AnnData, None]:
+    file_path = filepath_from_file_or_folder(file)
+    fs, file_path_str = _infer_filesystem(file_path)
+
+    adata: Union[AnnData, None] = None
+
+    if file.suffix == ".h5ad":
+        with fs.open(file_path_str, mode="rb") as file:
+            storage = h5py.File(file, mode="r")
+            adata = _subset_adata_storage(storage, query_obs, query_var)
+    elif file.suffix == ".zarr":
+        mapper = fs.get_mapper(file_path_str, check=True)
+        storage = zarr.open(mapper, mode="r")
+        adata = _subset_adata_storage(storage, query_obs, query_var)
+
+    return adata
```

### Comparing `lndb_storage-0.3.1/noxfile.py` & `lndb_storage-0.3.2/noxfile.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import nox
-import requests  # type: ignore
-from laminci import move_built_docs_to_docs_slash_project_slug, upload_docs_artifact
-from laminci.nox import build_docs, login_testuser1, run_pre_commit, run_pytest
-
-nox.options.reuse_existing_virtualenvs = True
-
-
-@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
-def lint(session: nox.Session) -> None:
-    run_pre_commit(session)
-
-
-@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
-def build(session):
-    login_testuser1(session)
-    session.install(".[dev,test]")
-    response = requests.get("https://github.com/laminlabs/lamindb/tree/adata_access")
-    if response.status_code < 400:
-        session.install("git+https://github.com/laminlabs/lamindb@adata_access")
-    else:
-        session.install("git+https://github.com/laminlabs/lamindb")
-    run_pytest(session)
-    build_docs(session)
-    upload_docs_artifact()
-    move_built_docs_to_docs_slash_project_slug()
+import nox
+import requests  # type: ignore
+from laminci import move_built_docs_to_docs_slash_project_slug, upload_docs_artifact
+from laminci.nox import build_docs, login_testuser1, run_pre_commit, run_pytest
+
+nox.options.reuse_existing_virtualenvs = True
+
+
+@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
+def lint(session: nox.Session) -> None:
+    run_pre_commit(session)
+
+
+@nox.session(python=["3.7", "3.8", "3.9", "3.10", "3.11"])
+def build(session):
+    login_testuser1(session)
+    session.install(".[dev,test]")
+    response = requests.get("https://github.com/laminlabs/lamindb/tree/adata_access")
+    if response.status_code < 400:
+        session.install("git+https://github.com/laminlabs/lamindb@adata_access")
+    else:
+        session.install("git+https://github.com/laminlabs/lamindb")
+    run_pytest(session)
+    build_docs(session)
+    upload_docs_artifact()
+    move_built_docs_to_docs_slash_project_slug()
```

